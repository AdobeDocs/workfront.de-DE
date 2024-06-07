---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: Data Lake-Datenwörterbuch
description: Diese Seite enthält Informationen zur Datenstruktur und zum Dateninhalt im Workfront Data Lake.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: 81f8477dd26b828c4255c678b36d98789cd81ff8
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 5%

---

# Workfront Data Lake-Datenwörterbuch

Diese Seite enthält Informationen zur Datenstruktur und zum Dateninhalt im Workfront Data Lake.

>[!NOTE]
>
>Die Daten im Workfront Data Lake werden alle vier Stunden aktualisiert, sodass aktuelle Änderungen möglicherweise nicht sofort übernommen werden.

## Tabellenarten

Es gibt eine Reihe von Tabellentypen, die Sie verwenden können, um Ihre Workfront-Daten so anzuzeigen, dass sie den größten Einblick bieten.

* **Aktuelle Tabelle**

  Die Tabelle &quot;Aktuell&quot;gibt Daten ähnlich an wie in Workfront, jedem Objekt und seinem aktuellen Status. Es kann jedoch mit einer wesentlich geringeren Latenz als in Workfront navigiert werden.

* **Ereignistabelle**

  Die Tabelle &quot;Event&quot;verfolgt jeden Änderungsdatensatz in Workfront: Jedes Mal, wenn ein Objekt den Status ändert, wird ein Datensatz erstellt, der anzeigt, wann die Änderung erfolgte, wer die Änderung vorgenommen hat und was geändert wurde. Daher ist diese Tabelle für Point-in-Time-Vergleiche nützlich. Diese Tabelle enthält nur Aufzeichnungen aus den letzten drei Jahren.

* **Tägliche Verlaufstabelle**

  Die Tabelle &quot;Täglicher Verlauf&quot;bietet eine abgekürzte Version der Tabelle &quot;Ereignis&quot;, da sie den Status der einzelnen Objekte täglich anzeigt und nicht, wann jedes einzelne Ereignis aufgetreten ist. Diese Tabelle ist daher für die Trendanalyse nützlich.

<!-- Custom table -->

## Entitätsbeziehungsdiagramm

Objekte in Workfront (und damit in Ihrem Data Lake) werden nicht nur durch ihre individuellen Werte definiert, sondern durch ihre Beziehungen zu anderen Objekten. Das unten stehende Entitätsbeziehungsdiagramm bietet eine allgemeine Zuordnung von Objektbeziehungen im Workfront Data Lake. Das Diagramm kann über den folgenden Link angezeigt und heruntergeladen werden:

[Workfront Data Lake-Entitätsbeziehungsdiagramm](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

>[!IMPORTANT]
>
>Das Entitätsbeziehungsdiagramm ist ein laufendes Werk - als solches dient es nur zu Referenzzwecken und kann geändert werden.

## Datumstypen

Es gibt eine Reihe von Datumsobjekten, die Informationen darüber bereitstellen, wann bestimmte Ereignisse auftreten.

* `DL_LOAD_TIMESTAMP`: Dieses Datum wird für interne Referenzzwecke verwendet und gibt an, wann die Daten in die Tabelle &quot;Aktueller Verlauf&quot;, &quot;Ereignis&quot;oder &quot;Täglicher Verlauf&quot;geladen wurden. Dieses Datum sollte nicht für die Datenanalyse verwendet werden und sollte während der Beta-Phase des Workfront Data Lake entfernt werden.
* `CALENDAR_DATE`: Dieses Datum ist nur in der Tabelle Tagesverlauf vorhanden. Diese Tabelle enthält einen Datensatz, wie die Daten für jedes in `CALENDAR_DATE`.
* `BEGIN_EFFECTIVE_TIMESTAMP`: Dieses Datum ist sowohl in den Tabellen Ereignis- als auch Tagesverlauf vorhanden und zeichnet genau auf, wenn sich ein Datensatz geändert hat _nach_ den Wert, den er in der aktuellen Zeile hat.
* `END_EFFECTIVE_TIMESTAMP`: Dieses Datum ist sowohl in den Tabellen Ereignis- als auch Tagesverlauf vorhanden und zeichnet genau auf, wenn sich ein Datensatz geändert hat _von_ den Wert in der aktuellen Zeile in einen Wert in einer anderen Zeile. So aktivieren Sie zwischen Abfragen auf `BEGIN_EFFECTIVE_TIMESTAMP` und `END_EFFECTIVE_TIMESTAMP` ist dieser Wert nie null, auch wenn kein neuer Wert vorhanden ist. Wenn ein Datensatz noch gültig ist (d. h., der Wert hat sich nicht geändert), `END_EFFECTIVE_TIMESTAMP` hat den Wert 2300-01-01.

## Terminologie

In der folgenden Tabelle werden Objektnamen in Workfront (sowie deren Namen in der Benutzeroberfläche und API) mit den entsprechenden Namen im Data Lake korreliert.

<table>
<thead>
  <tr>
    <th>Workfront-Entitätsname</th>
    <th>Schnittstellenverweise</th>
    <th>API-Referenz | Titel</th>
    <th>Data Lake Tables</th>
    <th>Notizen</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Zuweisung</td>
    <td>Zuweisung</td>
    <td>ASSGN | Zuweisung</td>
    <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>CustomEnum</td>
    <td>Bedingung, Priorität, Schweregrad, Status</td>
    <td>CSTEM | Benutzerdefinierte Enum</td>
    <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT</td>
    <td>Der Typ des Datensatzes wird durch die Eigenschaft "enumClass"identifiziert. Die folgenden Typen werden erwartet:<br>CONDITION_OPTASK<br>CONDITION_PROJ<br>CONDITION_TASK<br>PRIORITY_OPTASK<br>PRIORITY_PROJ<br>PRIORITY_TASK<br>SEVERITY_OPTASK<br>STATUS_OPTASK<br>STATUS_PROJ<br>STATUS_TASK</td>
  </tr>
  <tr>
    <td>Dokument</td>
    <td>Dokument</td>
    <td>DOCU | Dokument</td>
    <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT<br><br>DOCUMENTS_CUSTOM_VALUE_CURRENT<br>DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>DOCUMENTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>DocumentVersion</td>
    <td>Dokumentversion</td>
    <td>DOCV | Dokumentversion</td>
    <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Gruppe</td>
    <td>Gruppe</td>
    <td>GRUPPE | Gruppe</td>
    <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Stunde</td>
    <td>Stunde</td>
    <td>STUNDE | Stunde</td>
    <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Stundentyp</td>
    <td>Stundentyp</td>
    <td>HOURT | Stündentyp</td>
    <td>HOURTYPES_CURRENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Meilenstein</td>
    <td>Meilenstein</td>
    <td>MILE | Milestone</td>
    <td>MILESTONES_CURRENT<br>MILESTONES_DAILY_HISTORY<br>MILESTONES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>MilestonePath</td>
    <td>Meilensteinpfad</td>
    <td>MPATH | Milestone-Pfad</td>
    <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Notiz</td>
    <td>Notiz</td>
    <td>NOTE | Hinweis</td>
    <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>OpTask</td>
    <td>Problem, Anfrage</td>
    <td>OPTASK | Problem</td>
    <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT<br><br>OPTASKS_CUSTOM_VALUE_CURRENT<br>OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>OPTASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Portfolio</td>
    <td>Portfolio</td>
    <td>PORT | Portfolio</td>
    <td>PORTFOLIO_CURRENT<br>PORTFOLIO_DAILY_HISTORY<br>PORTFOLIO_EVENT<br><br>PORTFOLIO_CUSTOM_VALUE_CURRENT<br>PORTFOLIO_CUSTOM_VALUE_DAILY_HISTORY<br>PORTFOLIOS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Programm</td>
    <td>Programm</td>
    <td>PRGM | Programm</td>
    <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT<br><br>PROGRAMS_CUSTOM_VALUE_CURRENT<br>PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>PROGRAMS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Projekt</td>
    <td>Projekt</td>
    <td>PROJ | Projekt</td>
    <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT<br><br>PROJECTS_CUSTOM_VALUE_CURRENT<br>PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>PROJECTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Funktion</td>
    <td>Aufgabengebiet</td>
    <td>ROLLE | Auftragsrolle</td>
    <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Zeitplan</td>
    <td>Zeitplan</td>
    <td>GEPLANT | Zeitplan</td>
    <td>ZEDULES_CURRENT<br>ZEDULES_DAILY_HISTORY<br>ZEDULES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Aufgabe</td>
    <td>Aufgabe</td>
    <td>AUFGABE | Aufgabe</td>
    <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT<br><br>TASKS_CUSTOM_VALUE_CURRENT<br>TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>TASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Team</td>
    <td>Team</td>
    <td>TEAMOB | Team</td>
    <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Arbeitszeittabelle</td>
    <td>Arbeitszeittabelle</td>
    <td>TSHET | Datenblatt</td>
    <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>TIMESHEETS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Benutzerin oder Benutzer</td>
    <td>Benutzerin oder Benutzer</td>
    <td>BENUTZER | Benutzer</td>
    <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT<br><br>USERS_CUSTOM_VALUE_CURRENT<br>USERS_CUSTOM_VALUE_DAILY_HISTORY<br>USERS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
</tbody>
</table>
