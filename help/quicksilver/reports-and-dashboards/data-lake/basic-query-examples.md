---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Beispiele für Data Connect-Abfragen
description: Beispielabfragen Sie können verwenden, um sich mit der Syntax und Struktur bestimmter Arten von Abfragen vertraut zu machen.
author: Nolan
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: c8a25bcc8c9b56a649ca7764918c86f9cdd5b3e2
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 0%

---

# Beispiele für Workfront Data Connect-Abfragen

Damit Sie Ihre Workfront Data Connect-Daten besser nutzen können, enthält diese Seite einfache Beispielabfragen, mit denen Sie sich mit der Syntax und Struktur bestimmter Arten von Abfragen vertraut machen können.

## Benutzerdefinierte Datenabfrage

Dieses Beispiel zeigt, wie Sie eine Abfrage erstellen können, um Ihre benutzerdefinierten Daten in Workfront zurückzugeben, z. B. benutzerdefinierte Formulare und benutzerdefinierte Felder.

### Szenario

Ihr Unternehmen verwendet ein benutzerdefiniertes Formular namens Finanzintegration. Das Formular ist an jedes Projekt angehängt und enthält die folgenden Felder:

* **Geschäftseinheit**: Ein benutzerdefiniertes Feld, das eine Zeichenfolge enthält.
* **ProjectID**: Ein benutzerdefiniertes Feld, das eine numerische Zeichenfolge enthält.
* **Erweiterter Projektname**: Ein berechnetes benutzerdefiniertes Datenfeld, das die Werte von Geschäftseinheit, Projekt-ID und dem nativen Workfront-Projektnamen in einer einzigen Zeichenfolge verkettet.

Sie müssen diese Informationen in die Antwort für eine Abfrage bezüglich Data Connect aufnehmen. Benutzerdefinierte Datenwerte für einen Datensatz im Data Lake sind in einer Spalte mit dem Titel `parametervalues` enthalten. Diese Spalte wird als JSON-Objekt gespeichert.

### Abfrage

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

### Antwort

Die obige Abfrage gibt die folgenden Daten zurück:

* `projectid`: Die native Workfront-Projekt-ID.
* `parametervalues`: Eine Spalte, die ein JSON-Objekt speichert.
* `name`: Der native Workfront-Projektname.
* `Business Unit`: Ein benutzerdefinierter Datenwert, der im `parametervalues` enthalten ist.
* `Project ID`: Ein benutzerdefinierter Datenwert, der im `parametervalues` enthalten ist.
* `Expanded Project Name`: Ein benutzerdefinierter Datenwert, der im `parametervalues` enthalten ist.

### Erklärung

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

## Zeit in der Statusabfrage

Dieses Beispiel zeigt, wie Sie die Zeit messen, die ein Projekt in zuvor zugewiesenen Status verbracht hat. Sie kann einfach angepasst werden, um die Aufgaben- oder Problemzeit in einem Status zu messen, oder sie kann angepasst werden, um zu messen, wie lange einem Objekt ein anderes Attribut (einschließlich benutzerdefinierter Datenwerte) zugewiesen wurde.

### Szenario

Ihre Unternehmensführung ist der Ansicht, dass Sie in jeder Phase Ihres Arbeitszyklus zu viel Zeit investieren. Bevor Sie Empfehlungen zur Verbesserung des Prozesses abgeben, sollten Sie eine allgemeine Messung erstellen, um festzustellen, wie oft sich ein Projektstatus im Laufe der Zeit ändert und wie viele Tage ein Projekt in einem bestimmten Status verbleibt.

Sie verwenden die Datenansicht PROJECTS_EVENT, um eine Liste jeder Statusänderung für das Projektobjekt abzurufen. Sie vergleichen den neuen Status mit dem vorherigen Status, erfassen den effektiven Zeitraum für den zuvor zugewiesenen Status und berechnen dann die in diesem Status verbrachten Tage.

Mithilfe dieser Rohausgabe der in jedem Status pro Projekt verbrachten Zeit können Sie mit dem Erstellen von Visualisierungen beginnen oder die Daten weiter aggregieren, um Statusdauermittelwerte nach Status, Projekttyp oder Jahreszeit zu erstellen. Anhand dieser Grundlinie können Sie dann einen Maßstab festlegen, an dem Sie messen können, um die Erwartungen Ihrer Führung zu erfüllen.

Die folgende Abfrage verwendet die Datenansicht Data Connect PROJECTS_EVENTS , um jedes Projektstatusänderungsereignis zu vergleichen und die Zeit im Status anzuzeigen.

### Abfrage

```
-- Calculate the begin/end effective timestamp and duration in days 

SELECT 

    projectid, 
    name as project_name, 
    prev_status as previous_status, 
    status, 
    status_change_date as status_begin_effective_timestamp, 
    case 
        when status_change_date is null then NULL
        else
            nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp) 
    end as status_end_effective_timestamp, 
    datediff('DAYS',status_change_date, nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp)) as status_duration_days 

FROM 
    ( -- Filter to just the records that have changed 
     SELECT projectid, 
        name, 
        prev_status, 
        status, 
        begin_effective_timestamp as status_change_date    
     FROM 
        (  -- Calculate records where previous status is different 
          SELECT DISTINCT  
           pe.projectid, 
           pe.name AS name, 
           pe.STATUS, 
           nvl(lag(pe.STATUS) over (partition by pe.projectid order by pe.BEGIN_EFFECTIVE_TIMESTAMP), status) prev_status, 
           begin_effective_timestamp 

          FROM projects_event pe 
         -- Set any WHERE conditions to limit the results as needed 
         --WHERE 
            -- pe.PROJECTID = '5ebe…c1e1' 
        ) 
        WHERE prev_status != status 
    ) 
    order by status_change_date; 
```

### Antwort

Die obige Abfrage gibt die folgenden Daten zurück:

* `PROJECTID`: Die mit dem Statusänderungsereignis verknüpfte Workfront-Projekt-ID.
* `PROJECT_NAME`: Der Workfront-Projektname.
* `PREVIOUS_STATUS`: Der Projektstatus unmittelbar vor der Änderung.
* `STATUS`: Der Projektstatus nach der Änderung.
* `STATUS_BEGIN_EFFECTIVE_TIMESTAMP`: Der Zeitstempel des Änderungsereignisses, an dem der vorherige Status festgelegt wurde.
* `STATUS_END_EFFECTIVE_TIMESTAMP`: Der Zeitstempel des Änderungsereignisses, an dem der aktualisierte Statuswert festgelegt wurde.
* `STATUS_DURATION_DAYS`: Die Differenz (in Tagen) zwischen dem effektiven Endzeitstempel und dem effektiven Anfangszeitstempel.

### Erklärung

Die Abfrage verwendet die Tracking-Funktionen für Änderungsereignisse von Data Connect.  Sie bestimmt das Datum, an dem ein Ereignis ausgelöst wurde, das einen neuen Statuswert hatte, der sich vom vorherigen Ereignis unterschied. 

Überprüfen der Abfrage von innen nach außen: 

1. Datensätze berechnen, deren vorheriger Status unterschiedlich ist: 
   * Verwenden Sie für jedes Änderungsereignis die Funktion lag() , um den vorherigen Statuswert zu identifizieren. 

2. Filtern Sie nur nach den geänderten Datensätzen: 

   * Wählen Sie Datensätze aus der Berechnung in Schritt 1, bei denen der vorherige Status != Aktueller Status. 

3. Berechnen Sie den effektiven Zeitstempel und die Dauer des Beginns/Endes in Tagen: 

   * `<status_begin_effective_timestamp>`: In Schritt 2 berechnet. 

   * `<status_end_effective_timestamp>`: Wird anhand des nächsten (Lead()) berechnet. `<status_begin_effective_timestamp>`: Zeigt den Status nur an, wenn `<status_begin_effective_timestamp>` NICHT NULL ist. 
   * `<status_duration_days>`: Datendifferenz zwischen `<status_begin_effective_timestamp>` und `<status_end_effective_timestamp>`. 

>[!NOTE]
>
>Es wird empfohlen, diese Abfrage als eigene „Ansicht“ in Power BI oder Tableau zu verwenden.  Wenn Sie andere Felder aus dem `<object>_event view` einbringen möchten, verbinden Sie die Ausgabe aus dieser Abfrage wieder mit dem `<object>_event view`.  Die Verknüpfungsfelder lauten wie folgt: <br>
>&#x200B;>Für projects_event: 
>&#x200B;>`From projects_event p`
>&#x200B;>`Join <above query> c on c.projectid = p.projectid  `
>&#x200B;>`and c. status_begin_effective_timestamp = p begin_effective_timestamp`



<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
