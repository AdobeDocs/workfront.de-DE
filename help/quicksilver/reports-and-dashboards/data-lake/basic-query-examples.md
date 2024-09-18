---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Beispiele für Data Connect-Abfragen
description: Beispielabfragen, mit denen Sie sich mit der Syntax und Struktur bestimmter Abfragen vertraut machen können.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: 364b668f23f5437e5cca0c4cc4793b17d444fb56
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Workfront Data Connect-Abfragebeispiele

Damit Sie Ihre Workfront Data Connect-Daten besser nutzen können, enthält diese Seite grundlegende Beispielabfragen, mit denen Sie sich mit der Syntax und Struktur bestimmter Abfragen vertraut machen können.

## Benutzerdefinierte Datenabfrage

In diesem Beispiel wird gezeigt, wie Sie eine Abfrage erstellen können, um Ihre benutzerdefinierten Daten in Workfront zurückzugeben, z. B. benutzerdefinierte Formulare und benutzerdefinierte Felder.

### Szenario:

Ihr Unternehmen verwendet ein benutzerdefiniertes Formular namens Finanzintegration. Das Formular wird an jedes Projekt angehängt und enthält die folgenden Felder:

* **Business Unit** - Ein benutzerdefiniertes Feld, das eine Zeichenfolge enthält.
* **ProjectID** - Ein benutzerdefiniertes Feld, das eine numerische Zeichenfolge enthält.
* **Erweiterter Projektname** - Ein berechnetes benutzerdefiniertes Datenfeld, das die Werte der Geschäftseinheit, der Projekt-ID und des nativen Workfront-Projektnamen in einer einzigen Zeichenfolge verkettet.

Sie müssen diese Informationen in die Antwort für eine Abfrage gegen Data Connect aufnehmen. Benutzerdefinierte Datenwerte für einen Datensatz im Data Lake sind in einer Spalte mit dem Titel `parametervalues` enthalten. Diese Spalte wird als JSON-Objekt gespeichert.

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
* `name` - der native Workfront-Projektname
* `Business Unit` - ein benutzerdefinierter Datenwert, der im `parametervalues` -Objekt enthalten ist
* `Project ID` - ein benutzerdefinierter Datenwert, der im `parametervalues` -Objekt enthalten ist
* `Expanded Project Name` - ein benutzerdefinierter Datenwert, der im `parametervalues` -Objekt enthalten ist

### Erklärung:

Beim Abfragen des JSON-Objekts `parametervalues` kann auf jedes benutzerdefinierte Datenfeld wie folgt in Form einer Spalte zugegriffen werden:

`<field_name>:"<parameter_name>"::<data_type> as <column_name>`

* `<field_name>` ist der Name des JSON-Objekts in der Tabelle, die abgefragt wird. Bei benutzerdefinierten Daten ist dies immer `parametervalues`.
* `<parameter_name>` ist die im Formular-Konfigurations-Tool gefundene `parametername` Zeichenfolge, die möglicherweise nicht immer mit diesem Wert übereinstimmt.

>[!NOTE]
>
>Wenn der Name des Parameters im Workfront-Formularkonfigurationstool geändert wird, wird er im JSON-Objekt als neue Spalte dargestellt. Daher wird empfohlen, den Namen einer Spalte nicht zu ändern, nachdem sie im Formular-Konfigurations-Tool erstellt wurde. Die Beschriftung kann jedoch geändert werden, ohne dass sich dies auf das JSON-Objekt auswirkt.
>
>Wenn die Textzeichenfolge für den Parameternamen falsch ist, gibt die Spalte einen NULL-Wert und keinen Fehler zurück.

* `<data_type>` konvertiert den vom JSON-Objekt zurückgegebenen Wert in einen für das Feld geeigneten Datentyp. Wenn Sie einen inkompatiblen Datentyp für den zurückgegebenen Wert auswählen, tritt ein Fehler wegen der unterschiedlichen Datentypen auf. Mögliche Datentypen sind:

   * `text`
   * `varchar`
   * `int`
   * `float`
   * `number(len,precision)` (z. B. würde `Number(32,4)` 1234.0987 zurückgeben)
   * `date`
   * `timestamp`

* `<column_name>` ist die Bezeichnung, die Sie für jede benutzerdefinierte Datenspalte erstellen.

>[!NOTE]
>
>Nur Parameter, denen im Formular Werte zugewiesen sind, werden in das JSON-Objekt aufgenommen. Wenn ein benutzerdefiniertes Datenfeld im Formular leer ist, wird es nicht angezeigt.

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
