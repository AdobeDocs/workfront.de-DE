---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in API Version 10
description: Aktualisierte Ressourcen
author: Becky
feature: Workfront API
role: Developer
exl-id: 8ac384ae-5d65-4c0e-98c1-cf38cfbff460
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 35%

---

# Neue Funktionen in API Version 10

* [Neue Ressourcen](#new-resources)
* [Aktualisierte Ressourcen](#updated-resources)
* [Entfernte Ressourcen](#removed-resources)

## Neue Ressourcen {#new-resources}

### ActivityLog

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | HINZUFÜGEN |
|   |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### CalendarEntry

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | HINZUFÜGEN |
|   |   |   |   |   |   | COUNT  |
|   |   |   |   |   |   | LÖSCHEN  |
|   |   |   |   |   |   | BEARBEITEN  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | BERICHT  |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### CalendarEntryExternalReference

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | BERICHT  |
|   |   |   |   |   |   | SEARCH  |

{style="table-layout:auto"}

### ExternalAuthToken

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | HINZUFÜGEN |
|   |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | LÖSCHEN  |
|   |   |   |   |   |   | BEARBEITEN  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | BERICHT  |
|   |   |   |   |   |   | SEARCH  |

{style="table-layout:auto"}

### LicenseTypeGroupLimit

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| customerID | customer |   |   |   |   |   |
| groupID | Gruppe |   |   |   |   |   |
| planLimit |   |   |   |   |   |   |
| usedLicenses |   |   |   |   |   |   |
| worklimit |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

### UserHomeCalendarPreference

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| customerID | customer |   |   |   |   | HINZUFÜGEN |
| edTime | Benutzer |   |   |   |   | COUNT |
| firstDayOfWeek |   |   |   |   |   | LÖSCHEN |
| ID |   |   |   |   |   | BEARBEITEN |
| showPTO |   |   |   |   |   | GET |
| startTime |   |   |   |   |   | BERICHT |
| userID |   |   |   |   |   | SEARCH |
| workDate |   |   |   |   |   |   |

{style="table-layout:auto"}

**Aktualisierte Ressourcen**

Die folgenden vorhandenen Ressourcen wurden mit dieser Version der Workfront-API aktualisiert. An einer Ressource vorgenommene Änderungen werden wie folgt angegeben:

* Hinzufügungen werden einfach aufgelistet
* Entfernungen werden mit Durchstreichen angezeigt
* Änderungen werden in der Anmerkung nach der Tabelle aufgeführt

### Genehmigung

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval `<sup>1</sup>`   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |
| projectBudgetedCost  |   |   |   |   |   |   |
| projectNetValue  |   |   |   |   |   |   |
| projectRoi  |   |   |   |   |   |   |
| resourcePlannerBudgetedLabourCost  |   |   |   |   |   |   |

{style="table-layout:auto"}

`<sup>1</sup> Type changed from null to boolean`

### Zuweisung

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| assignmentPercent `<sup>1</sup>` |   |   |   |   |   |   |
| viewedByAssignedToUser |   |   |   |   |   |   |

{style="table-layout:auto"}

`<sup>1</sup>`Validator hinzugefügt: LESS_THAN_EQUAL

### BudgetedHour

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### CustomerPreferences

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| name `<sup>1</sup>` |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Änderungen an möglichenWerten

### DocMetadataLinkGroup

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   | getMetadataForDocument |   |   |

{style="table-layout:auto"}

### Dokument

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |   |   |   |   |   |

{style="table-layout:auto"}

### DocumentRequest

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

DocumentVersion

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| externalIntegrationType <sup>1</sup> |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Änderungen an möglichenWerten

Ausgabe

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Gruppe

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   | licenseTypeLimit |   |   | addRemoveLicenseTypeLimits  |   |   |
|   |   |   |   | setLicenseTypeLimit |   |   |

{style="table-layout:auto"}

### LinkedFolder

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| externalIntegrationType<sup>1</sup> |  |  |  |  |   |   |

{style="table-layout:auto"}

<sup>1</sup> Änderungen an möglichenWerten

### OpTask

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| priorityColor |   |  | pendingApproval<sup>1</sup> |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Typ geändert von null in boolesch

### PortalSection

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |  |   | groupIDs |   |   |   |

{style="table-layout:auto"}

### Portfolio

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| portfolioNetValue |   |   |   |  |  |   |
| portfolioRoi |   |   |   |   |   |   |

{style="table-layout:auto"}

### Projekt

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| projectBudgetedCost  |   |   |   | linkExternalObject  |   |   |
| projectNetValue |   |   |   | unlinkExternalObject |   |   |
| projectRoi |   |   |   |   |   |   |
| resourcePlannerBudgetedLabourCost |   |   |   |   |   |   |

{style="table-layout:auto"}

### TestversandApproval

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| approveDecision |   |   |   |   |   |   |

{style="table-layout:auto"}

### Satz

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| rateValue <sup>1</sup> |  |  |  |  |  |   |

{style="table-layout:auto"}

<sup>1</sup>Hinzugefügte Validator-WÄHRUNG

### Aufgabe

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| kanbanFlag |   |   |   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### Team

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| hoursPerPoint <sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Validator hinzugefügt LESS_THAN

### TeamAssignment

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### TeamTask

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Arbeitszeittabelle

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

### Aktualisieren

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| updateType `<sup>1</sup>` |   |   |   |   |   | objectUpdatesWithNoteAndJournalEntryIndex  |

{style="table-layout:auto"}

<sup>1</sup> Änderungen an möglichenWerten

### Benutzerin oder Benutzer

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   | accessLevel  |   |   |   |   |   |

{style="table-layout:auto"}

### UserNote

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| eventType <sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Änderungen an möglichenWerten

### Arbeit

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval <sup>1</sup>  |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Typ geändert von null in boolesch

## Entfernte Ressourcen {#removed-resources}

### ResourceBudgetedHour

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | HINZUFÜGEN  |
| budgetHours |   |   |   |   |   | COUNT  |
| ID |   |   |   |   |   | LÖSCHEN  |
| scheduledBudgetedHours |   |   |   |   |   | BEARBEITEN  |
| projectID |   |   |   |   |   | GET  |
| roleID |   |   |   |   |   | BERICHT  |
| userID |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

 

 

 
