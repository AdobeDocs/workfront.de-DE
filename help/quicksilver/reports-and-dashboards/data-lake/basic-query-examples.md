---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Beispiele für Data Connect-Abfragen
description: Beispielabfragen Sie können verwenden, um sich mit der Syntax und Struktur bestimmter Arten von Abfragen vertraut zu machen.
author: Courtney
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/flDonZVaLR3bTF2aZcY9iy2ZnWbfrdhctL7J8esvxng
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: edee967a5c19d86fd471c4571a0b458f72bf370e
workflow-type: tm+mt
source-wordcount: 2201
ht-degree: 1%

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

Die Abfrage verwendet die Tracking-Funktionen für Änderungsereignisse von Data Connect. Sie ermittelt das Datum, an dem ein Ereignis ausgelöst wurde, das einen neuen Statuswert hatte, der sich vom vorherigen Ereignis unterschied. 

Überprüfen der Abfrage von innen nach außen: 

1. Datensätze berechnen, deren vorheriger Status unterschiedlich ist: 
   * Verwenden Sie für jedes Änderungsereignis die Funktion lag() , um den vorherigen Statuswert zu identifizieren. 

2. Filtern Sie nur nach den geänderten Datensätzen: 

   * Wählen Sie Datensätze aus der Berechnung in Schritt 1, bei denen der vorherige Status den aktuellen Status !=. 

3. Berechnen Sie den effektiven Zeitstempel und die Dauer des Beginns/Endes in Tagen: 

   * `<status_begin_effective_timestamp>`: In Schritt 2 berechnet. 

   * `<status_end_effective_timestamp>`: Wird anhand des nächsten (Lead()) berechnet. `<status_begin_effective_timestamp>`: Zeigt den Status nur an, wenn `<status_begin_effective_timestamp>` NICHT NULL ist. 
   * `<status_duration_days>`: Datendifferenz zwischen `<status_begin_effective_timestamp>` und `<status_end_effective_timestamp>`. 

>[!NOTE]
>
>Es wird empfohlen, diese Abfrage als eigene „Ansicht“ in Power BI oder Tableau zu verwenden. Wenn Sie andere Felder aus dem `<object>_event view` einbringen möchten, verbinden Sie die Ausgabe aus dieser Abfrage wieder mit dem `<object>_event view`. Die Verknüpfungsfelder lauten wie folgt: <br>
>Für projects_event: 
>`From projects_event p`>`Join <above query> c on c.projectid = p.projectid  `>`and c. status_begin_effective_timestamp = p begin_effective_timestamp`

## Planung: Abfrage vom Typ Einzel-Datensatz

Dieses Beispiel zeigt, wie Workfront Planning-Daten für einen einzelnen Datensatztyp abgefragt werden, der im Data Connect Data Lake gespeichert ist.

### Szenario

Ihr Unternehmen verwendet Workfront Planning zur Verfolgung von Kampagnen. Jeder Kampagnendatensatz enthält einen Namen, einen Status, ein Startdatum, ein Enddatum und einen Besitzer. Sie möchten eine Liste aller aktiven Kampagnen und ihrer wichtigsten Details zur Verwendung in einem Dashboard abrufen.

* Daten vom Typ Planungsdatensatz werden in der Ansicht PLANNINGRECORD_CURRENT gespeichert.
* Jede Zeile stellt einen einzelnen Datensatz dar, und alle Feldwerte werden in einer JSON-Spalte mit dem Namen FIELD_VALUES gespeichert.
* Der Datensatztyp wird durch die Spalte RECORDTYPEID identifiziert.
* Der Arbeitsbereich des Datensatzes wird durch die Spalte WORKSPACEID (oder die Spalte WORKSPACENAME für einen menschenlesbaren Filter) identifiziert.

### Abfrage

```sql
SELECT
  recordid,
  FIELD_VALUES:"Name"::text AS campaign_name,
  FIELD_VALUES:"Status"::text AS campaign_status,
  FIELD_VALUES:"Start Date"::date AS start_date,
  FIELD_VALUES:"End Date"::date AS end_date,
  FIELD_VALUES:"Owner"::text AS owner
FROM PLANNINGRECORD_CURRENT
WHERE WORKSPACEID = '<your_campaign_workspace_id>'
AND RECORDTYPEID = '<your_campaign_record_type_id>'
AND FIELD_VALUES:"Status"::text = 'Active'
ORDER BY start_date ASC
```

### Antwort

Die obige Abfrage gibt die folgenden Daten zurück:

* **recordId**: Die eindeutige Planungsdatensatz-ID für die Kampagne.
* **campaign_name**: Der Name der Kampagne, extrahiert aus dem JSON-Objekt „FIELD_VALUES“.
* **campaign_status**: Der aktuelle Status der Kampagne.
* **start_date**: Das Startdatum der Kampagne, umgewandelt in einen Datumsdatentyp.
* **end_date**: Das Enddatum der Kampagne, umgewandelt in einen Datumsdatentyp.
* **Inhaber**: Der Name des Benutzers oder Teams, der/das als Kampagnenverantwortlicher zugewiesen wurde.

### Erklärung

Die Planung von Datensätzen in Data Connect verwendet unabhängig vom Datensatztyp eine einzige Tabellenstruktur. Die Spalte RECORDTYPEID wird verwendet, um die Abfrage auf einen bestimmten Datensatztyp zu beschränken - in diesem Fall Kampagnen. Ersetzen Sie `<your_campaign_record_type_id>` durch die ID des Datensatztyps, den Sie abfragen möchten. Diese finden Sie in den Einstellungen für den Workfront Planning-Datensatztyp oder durch Abfragen von RECORDTYPE_CURRENT.

Feldwerte werden als JSON-Objekt in der Spalte FIELD_VALUES gespeichert und über dieselbe Doppelpunktsyntax aufgerufen, die auch für benutzerdefinierte Formulardaten verwendet wird:

```
<field_column>:"<field_name>"::<data_type> AS <alias>
```

Feldnamenverweise müssen genau mit dem Feldnamen übereinstimmen, der in der Feldkonfiguration für den Planungs-Datensatztyp definiert ist, einschließlich Groß- und Kleinschreibung, Leerzeichen und Emoji.

>[!NOTE]
>
>Die IDs für den Planungs-Datensatztyp finden Sie in der URL, wenn Sie einen Datensatztyp in Workfront Planning anzeigen. Es ist der Pfad der URL, die mit „Rt…“ beginnt. Datensatztypen finden Sie auch mit dem folgenden SQL-Aufruf in Data Connect:
>
>
>```sql
>SELECT
>ID AS recordtypeid,
>DISPLAYNAME AS record_type_name,
>WORKSPACEID
>FROM RECORDTYPE_CURRENT
>ORDER BY record_type_name ASC
>```

## Planung: Abfrage für verbundene Datensatztypen

Dieses Beispiel zeigt, wie Daten über zwei verbundene Planungs-Datensatztypen hinweg abgefragt werden können - einen übergeordneten Datensatztyp und einen Datensatztyp, mit dem er verbunden ist.

### Szenario

Ihr Unternehmen verknüpft Campaign-Datensätze mit taktischen Datensätzen in Workfront Planning. Sie möchten einen Bericht erstellen, der jede Kampagne zusammen mit den wichtigsten Details der zugehörigen Taktik anzeigt. Sie möchten insbesondere den Namen der Taktik, die strategische Priorität und die Budgetzuweisung anzeigen, damit die Führung die Kampagnenaktivitäten nach Taktik organisieren kann.

In Data Connect werden Verbindungen zwischen nativen Planungs-Datensatztypen direkt in der Spalte FIELD_VALUES_RAW von PLANNINGRECORD_CURRENT gespeichert. Bei einem Referenzfeld mit dem Namen „Taktik“ ist der Wert ein JSON-Array von verbundenen Datensatz-Objekten, von denen jedes eine ID-Eigenschaft mit der RECORDID des verbundenen Datensatzes enthält. Verwenden Sie die Snowflake-Option LATERAL FLATTEN , um dieses Array in Zeilen zu erweitern und mit dem verbundenen Datensatztyp zu verbinden.

### Abfrage

```sql
SELECT
  c.RECORDID AS campaign_id,
  c.FIELD_VALUES:"Name"::text AS campaign_name,
  c.FIELD_VALUES:"Status"::text AS campaign_status,
  t.FIELD_VALUES:"Name"::text AS tactic_name,
  t.FIELD_VALUES:"Strategic Priority"::text AS strategic_priority,
  t.FIELD_VALUES:"Budget Allocation"::float AS budget_allocation
FROM PLANNINGRECORD_CURRENT c,
INNER JOIN REFERENCE_CURRENT R 
ON r.FROM_REFERENCEID = c.REFERENCE_IDS:"Tactics"::text
INNER JOIN PLANNINGRECORD_CURRENT t
-- Join to the Tactic record using the connected record ID from the array
ON t.RECORDID = r.TO_RECORDID
WHERE c.RECORDTYPEID = '<your_campaign_record_type_id>'
ORDER BY tactic_name, campaign_name
```

### Antwort

Die obige Abfrage gibt die folgenden Daten zurück:

* **campaign_id**: Die eindeutige Planungsdatensatz-ID für die Kampagne.
* **campaign_name**: Der Name des Kampagnendatensatzes.
* **campaign_status**: Der aktuelle Status der Kampagne.
* **TACTIC_NAME**: Der Name des verbundenen taktischen Datensatzes.
* **Strategic_priority**: Der Feldwert für die strategische Priorität aus dem verbundenen taktischen Datensatz.
* **budget_allocation**: Der Feldwert für die Budgetzuweisung aus dem verbundenen taktischen Datensatz, der als Gleitkommazahl umgewandelt wird.

### Erklärung - Geänderte KP

Verbindungen zwischen nativen Planungs-Datensatztypen werden in einer REFERENCE_CURRENT JOIN-Tabelle gespeichert.  Die Join-Tabelle REFERENCE_CURRENT wird für Joins zwischen RecordType verwendet.   Beim Verbinden von RecordType sollte das Feld TO_RECORDID verwendet werden.

Die Spalte REFERENCE_ID in der PLANNINGRECORD-Ansicht enthält eine Liste aller REFERENCEID-Felder, die für diesen Planungsdatensatz gelten. Sie können auf die ID zugreifen, indem Sie dieselbe JSON-Notation als field_value verwenden.

```
<reference_ids>:"<reference_name>"::text
```

Die REFERENCE_CURRENT-Ansicht enthält einen oder mehrere Datensätze, bei denen TO_RECORDID auf andere `recordId` in den PLANNINGRECORD_*-Ansichten verweist.

Um ein weiteres REFERENCE-Feld mit zusätzlichen Planungsdatensätzen zu verbinden, werden der obigen Abfrage das gleiche Muster der Verbindung mit REFERENCE_CURRENT und der PLANNINGRECORD_* -Ansicht hinzugefügt.


## Planung: Datensatztyp mit Workfront Workflow-Datenabfrage verknüpft

Dieses Beispiel zeigt, wie ein Workfront Planning-Datensatztyp mithilfe der nativen Verbindungsfunktion von Planning, die externe Objektverweise in der REFERENCE_CURRENT-Ansicht speichert, mit einem nativen Workfront Workflow-Objekt - in diesem Fall einem Projekt - verbunden wird.

### Szenario

Ihr Unternehmen verbindet Campaign-Datensätze in Workfront Planning mit Workfront-Projekten mithilfe der nativen Verbindungsfunktion von Planning. Sie möchten einen kombinierten Bericht erstellen, der die Kampagnendetails zusammen mit den Live-Ausführungsdaten aus dem verknüpften Projekt anzeigt - insbesondere den aktuellen Prozentsatz der Fertigstellung, das geplante Abschlussdatum und den zugewiesenen Projektbesitzer -, damit Kampagnen-Manager den Versandfortschritt verfolgen können, ohne den Arbeitsbereich Planung verlassen zu müssen.

### Abfrage

```sql
SELECT
  c.RECORDID AS campaign_id,
  c.FIELD_VALUES:"Name"::text AS campaign_name,
  c.FIELD_VALUES:"Status"::text AS campaign_status,
  conn.TO_EXTERNALID AS linked_project_id,
  p.name AS project_name,
  p.percentcomplete AS project_percent_complete,
  p.plannedcompletiondate AS project_planned_completion,
  p.ownerid AS project_owner_id,
  u.name AS project_owner_name
FROM WORKFRONT.PLANNING.PLANNINGRECORD_CURRENT c
-- Join to the references table to find Workfront Project connections
INNER JOIN WORKFRONT.PLANNING.REFERENCE_CURRENT conn
ON conn.REFERENCE_ID = c.REFERENCE_IDS:"ProjectId"::text
-- Join to the Workfront Projects table on the external ID
INNER JOIN WORKFRONT.WF.PROJECTS_CURRENT p
ON p.projectid = conn.TO_EXTERNALID
-- Join to Users to resolve the project owner name
LEFT JOIN WORKFRONT.WF.USERS_CURRENT u
ON u.userid = p.ownerid
WHERE c.RECORDTYPEID = '<your_campaign_record_type_id>'
AND p.completiontype != 'CPL' -- Exclude completed projects
ORDER BY campaign_name
```

### Antwort

Die obige Abfrage gibt die folgenden Daten zurück:

* **campaign_id**: Die eindeutige Planungsdatensatz-ID für die Kampagne.
* **campaign_name**: Der Name des Kampagnendatensatzes.
* **campaign_status**: Der aktuelle Status der Kampagne, aus der Planung.
* **link_project_id**: Die Workfront-Projekt-ID aus REFERENCE_CURRENT.TO_EXTERNALID, die das verbundene Workfront-Projekt identifiziert.
* **project_name**: Der native Workfront-Projektname aus PROJECTS_CURRENT.
* **project_percent_complete**: Der aktuelle Wert des Projekts für „Prozent abgeschlossen“.
* **project_scheduled_completion**: Das geplante Abschlussdatum des verknüpften Workfront-Projekts.
* **project_owner_id**: Die Workfront-Benutzer-ID des Projektbesitzers.
* **project_owner_name**: Der Anzeigename des Projektbesitzers, der durch die Verknüpfung mit USERS_CURRENT aufgelöst wird.

### Erklärung

Verbindungen von einem Planungs-Datensatztyp zu einem nativen Workfront Workflow-Objekt werden in REFERENCE_CURRENT gespeichert. Jede Zeile in dieser Ansicht stellt eine direktionale Relation dar: TO_EXTERNALID enthält die ID des verbundenen Workfront-Objekts. Zeilen, die Workfront-Verbindungen darstellen, werden durch `TO_EXTERNALCONNECTIONNAME = 'workfront'` und einen TO_EXTERNALOBJECTNAME-Wert identifiziert, der dem API-Code des Workfront-Objekttyps entspricht - z. B. PROJ für Projekte.

Die Spalte REFERENCE_ID in den PLANNINGRECORD-Tabellen enthält eine Liste aller REFERENCEID-Felder, die für diesen Datensatz gelten.  Sie können auf die ID zugreifen, indem Sie dieselbe JSON-Notation als field_value verwenden.\
Eine einzelne REFERENCE_ID in PLANNINGRECORD_CURRENT kann eine oder mehrere Referenzverknüpfungen in der REFERENCE_CURRENT-Tabelle enthalten, die mit Objekten eines bestimmten Objekttyps in der Workfront-Tabelle verknüpft sind.

```
<reference_ids>:"<reference_name>"::text
```

Beachten Sie, dass sich Planning-Ansichten (PLANNINGRECORD_CURRENT, REFERENCE_CURRENT) im WORKFRONT.PLANNING-Schema befinden, während native Workfront-Workflow-Ansichten (PROJECTS_CURRENT, USERS_CURRENT usw.) im WORKFRONT.WF-Schema gespeichert sind. Für Schema-übergreifende Joins sind vollständig qualifizierte Tabellennamen erforderlich.

Die Abfrage führt drei Joins durch:

1. **Planungsdatensätze zur Referenztabelle:** REFERENCE_CURRENT wird auf `TO_RECORDID = c.RECORDID` verbunden, um alle Verbindungen zu finden, die von jedem Kampagnendatensatz stammen. Die Filter für `TO_EXTERNALCONNECTIONNAME = 'workfront'` und `TO_EXTERNALOBJECTNAME = 'PROJ'` grenzen die Ergebnisse auf Zeilen ein, die speziell Verbindungen zu Workfront-Projekten darstellen.
1. **Referenztabelle für Workfront-Projekte:** TO_EXTERNALID enthält die native Workfront-Projekt-ID für das verbundene Projekt. Dieser wird direkt mit `PROJECTS_CURRENT.projectid` verknüpft, um Live-Projektdaten abzurufen.
1. **Projekte für Benutzer:** EIN LINKER JOIN an USERS_CURRENT löst den Fremdschlüssel „ownerID“ des Projekts in einen für Menschen lesbaren Namen auf. Hier wird ein LINKER JOIN verwendet, damit Projekte ohne zugewiesenen Eigentümer weiterhin in die Ergebnisse einbezogen werden.

>[!NOTE]
>
>Verwenden Sie beim Verbinden mit Tabellen, die nicht zu Planning gehören, NICHT das Feld TO_RECORDID in der Abfrage.  Dies ist beim Verbinden mit externen Tabellen nicht erforderlich.
>
>Dieses Muster kann auf jedes Workfront-Workflow-Objekt angewendet werden, das Planning beim Herstellen einer Verbindung unterstützt, z. B. Projekte, Portfolios oder Programme, indem der Filter TO_EXTERNALOBJECTNAME in den entsprechenden Objekt-API-Code geändert wird (z. B. PORT für Portfolios oder PRGM für Programme) und eine Verbindung zur entsprechenden WORKFRONT.WF-Tabelle hergestellt wird. Im Datenwörterbuch für Workfront Data Connect finden Sie die richtigen Tabellen- und ID-Spaltennamen für jeden Objekttyp.

Um ein weiteres REFERENCE-Feld mit zusätzlichen externen Datensätzen zu verbinden, werden dasselbe Verbindungsmuster mit REFERENCE_CURRENT und den Workfront Workflow-Ansichten der obigen Abfrage hinzugefügt.

Externe und Planungs-Datensatzwerte können in derselben Abfrage zusammengefügt werden, indem sie mehrmals mit der REFERENCE_CURRENT-Tabelle verbunden werden und das entsprechende Join-Muster verwenden.


<!--
## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.
-->
