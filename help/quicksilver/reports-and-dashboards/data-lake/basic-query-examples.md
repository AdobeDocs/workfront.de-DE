---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Beispiele für Data Connect-Abfragen
description: Beispielabfragen Sie können verwenden, um sich mit der Syntax und Struktur bestimmter Arten von Abfragen vertraut zu machen.
author: Nolan
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: 4c8b7e7f33ec593b2942725eb9160f7fbe2962e3
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Beispiele für Workfront Data Connect-Abfragen

Damit Sie Ihre Workfront Data Connect-Daten besser nutzen können, enthält diese Seite einfache Beispielabfragen, mit denen Sie sich mit der Syntax und Struktur bestimmter Arten von Abfragen vertraut machen können.

## Benutzerdefinierte Datenabfrage

Dieses Beispiel zeigt, wie Sie eine Abfrage erstellen können, um Ihre benutzerdefinierten Daten in Workfront zurückzugeben, z. B. benutzerdefinierte Formulare und benutzerdefinierte Felder.

### Szenario:

Ihr Unternehmen verwendet ein benutzerdefiniertes Formular namens Finanzintegration. Das Formular ist an jedes Projekt angehängt und enthält die folgenden Felder:

* **Geschäftseinheit** - Ein benutzerdefiniertes Feld, das eine Zeichenfolge enthält.
* **ProjectID** - Ein benutzerdefiniertes Feld, das eine numerische Zeichenfolge enthält.
* **Erweiterter Projektname**: Ein berechnetes benutzerdefiniertes Datenfeld, das die Werte von Geschäftseinheit, Projekt-ID und dem nativen Workfront-Projektnamen in einer einzigen Zeichenfolge verkettet.

Sie müssen diese Informationen in die Antwort für eine Abfrage bezüglich Data Connect aufnehmen. Benutzerdefinierte Datenwerte für einen Datensatz im Data Lake sind in einer Spalte mit dem Titel `parametervalues` enthalten. Diese Spalte wird als JSON-Objekt gespeichert.

### Abfrage:

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:Business Unit"::int as BusinessUnit,
    parametervalues:"DE:Project ID"::int as ProjectID,
    parametervalues:"DE:Expanded Project Name"::text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### Antwort:

Die obige Abfrage gibt die folgenden Daten zurück:

* `projectid` - die native Workfront-Projekt-ID
* `parametervalues` - eine Spalte, die ein JSON-Objekt speichert
* `name` - Der native Workfront-Projektname
* `Business Unit` - Ein benutzerdefinierter Datenwert, der im `parametervalues` enthalten ist
* `Project ID` - Ein benutzerdefinierter Datenwert, der im `parametervalues` enthalten ist
* `Expanded Project Name` - Ein benutzerdefinierter Datenwert, der im `parametervalues` enthalten ist

### Erklärung:

Bei der Abfrage des `parametervalues` JSON-Objekts kann jedes benutzerdefinierte Datenfeld wie folgt als Spalte aufgerufen werden:

`<field_name>:"<parameter_name>"::<data_type> as <column_name>`

* `<field_name>` ist der Name des JSON-Objekts in der Tabelle, die abgefragt wird. Bei benutzerdefinierten Daten ist dies immer `parametervalues`.
* `<parameter_name>` ist die `parametername` Zeichenfolge, die im Formular-Konfigurations-Tool gefunden wird, auch wenn sie möglicherweise nicht immer mit diesem Wert übereinstimmt.

>[!NOTE]
>
>Wenn der Name des Parameters im Workfront-Formular-Konfigurations-Tool geändert wird, wird er im JSON-Objekt als neue Spalte dargestellt. Daher wird empfohlen, den Namen einer Spalte nach ihrer Erstellung im Formular-Konfigurations-Tool nicht zu ändern. Die Beschriftung kann jedoch geändert werden, ohne dass sich dies auf das JSON-Objekt auswirkt.
>
>Wenn die Textzeichenfolge für den Parameternamen falsch ist, gibt die Spalte einen NULL-Wert und keinen Fehler zurück.

* `<data_type>` konvertiert den vom JSON-Objekt zurückgegebenen Wert in einen für das Feld geeigneten Datentyp. Die Auswahl eines inkompatiblen Datentyps für den zurückgegebenen Wert führt zu einem Fehler wegen nicht übereinstimmender Datentypen. Zu den möglichen Datentypen gehören:

   * `text`
   * `varchar`
   * `int`
   * `float`
   * `number(len,precision)` (z. B. `Number(32,4)` würde 1234,0987 zurückgeben)
   * `date`
   * `timestamp`

* `<column_name>` ist die Beschriftung, die Sie für jede benutzerdefinierte Datenspalte erstellen.

>[!NOTE]
>
>Nur Parameter, denen Werte im Formular zugewiesen sind, werden in das JSON-Objekt aufgenommen. Wenn ein benutzerdefiniertes Datenfeld im Formular leer ist, wird es nicht angezeigt.

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
