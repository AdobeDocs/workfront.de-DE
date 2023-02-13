---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in API Version 10
description: Aktualisierte Ressourcen
author: John
feature: Workfront API
exl-id: 8ac384ae-5d65-4c0e-98c1-cf38cfbff460
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 46%

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

{style=&quot;table-layout:auto&quot;}

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

{style=&quot;table-layout:auto&quot;}

### CalendarEntryExternalReference

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | BERICHT  |
|   |   |   |   |   |   | SEARCH  |

{style=&quot;table-layout:auto&quot;}

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

{style=&quot;table-layout:auto&quot;}

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

{style=&quot;table-layout:auto&quot;}

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

{style=&quot;table-layout:auto&quot;}

**Aktualisierte Ressourcen**

Die folgenden vorhandenen Ressourcen wurden mit dieser Version der Workfront-API aktualisiert. An einer Ressource vorgenommene Änderungen werden wie folgt angegeben:

* Hinzufügungen werden einfach aufgelistet
* Entfernungen werden mit Durchstreichen angezeigt
* Änderungen werden in der Anmerkung nach der Tabelle aufgeführt

### Genehmigung

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval `¹`   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |
| projectBudgetedCost  |   |   |   |   |   |   |
| projectNetValue  |   |   |   |   |   |   |
| projectRoi  |   |   |   |   |   |   |
| resourcePlannerBudgetedLabourCost  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

`¹ Type changed from null to boolean`

### Zuweisung

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| assignmentPercent `¹` |   |   |   |   |   |   |
| displayedByAssignedToUser |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

`¹`Validator hinzugefügt: LESS_THAN_EQUAL

### BudgetedHour

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### CustomerPreferences

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| name `¹` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Änderungen an möglichen Werten

### DocMetadataLinkGroup

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   | getMetadataForDocument |   |   |

{style=&quot;table-layout:auto&quot;}

### Dokument

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### DocumentRequest

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

DocumentVersion

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| externalIntegrationType ¹ |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Änderungen an möglichen Werten

Ausgabe

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Gruppe

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   | licenseTypeLimit |   |   | addRemoveLicenseTypeLimits  |   |   |
|   |   |   |   | setLicenseTypeLimit |   |   |

{style=&quot;table-layout:auto&quot;}

### LinkedFolder

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| externalIntegrationType¹ |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹ Änderungen an möglichen Werten

### OpTask

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| priorityColor |  |  | pendingApproval¹ |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹ Der Typ wurde von null in boolesch geändert.

### PortalSection

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|  |  |  | groupIDs |  |  |  |

{style=&quot;table-layout:auto&quot;}

### Portfolio

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| portfolioNetValue |  |  |  |  |  |  |
| portfolioRoi |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Projekt

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| projectBudgetedCost  |   |   |   | linkExternalObject  |   |   |
| projectNetValue |   |   |   | unlinkExternalObject |   |   |
| projectRoi |   |   |   |   |   |   |
| resourcePlannerBudgetedLabourCost |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### TestversandApproval

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| approveDecision |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### Satz

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| rateValue ¹ |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

1 hinzugefügte Validator-WÄHRUNG

### Aufgabe

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| kanbanFlag |   |   |   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Team

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| hoursPerPoint ¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Validator LESS_THAN hinzugefügt

### TeamAssignment

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### TeamTask

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Arbeitszeittabelle

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Aktualisieren

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| updateType `¹` |   |   |   |   |   | objectUpdatesWithNoteAndJournalEntryIndex  |

{style=&quot;table-layout:auto&quot;}

¹ Änderungen an möglichen Werten

### Benutzer

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   | accessLevel  |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### UserNote

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| eventType ¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Änderungen an möglichen Werten

### Arbeit

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval ¹  |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Der Typ wurde von null in boolesch geändert.

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

{style=&quot;table-layout:auto&quot;}

 

 

 
