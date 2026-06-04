---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in der API-Version 10
description: Aktualisierte Ressourcen
author: Becky
feature: Workfront API
role: Developer
exl-id: 8ac384ae-5d65-4c0e-98c1-cf38cfbff460
TQID: https://experienceleague.adobe.com/7paMh3l4zsoBaafv6U6pp1M-SQjk-kdmSho9GYa15SU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 484
ht-degree: 60%

---

# Neue Funktionen in der API-Version 10

* [Neue Ressourcen](#new-resources)
* [Ressourcen aktualisiert](#updated-resources)
* [Entfernte Ressourcen](#removed-resources)

## Neue Ressourcen {#new-resources}

### ActivityLog

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | HINZUFÜGEN |
|   |   |   |   |   |   | ANZAHL |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### Kalendereintrag

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | HINZUFÜGEN |
|   |   |   |   |   |   | ANZAHL  |
|   |   |   |   |   |   | LÖSCHEN  |
|   |   |   |   |   |   | BEARBEITEN  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | BERICHT  |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### CalendarEntryExternalReference

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | ANZAHL |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | BERICHT  |
|   |   |   |   |   |   | SEARCH  |

{style="table-layout:auto"}

### ExternalAuthToken

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | HINZUFÜGEN |
|   |   |   |   |   |   | ANZAHL |
|   |   |   |   |   |   | LÖSCHEN  |
|   |   |   |   |   |   | BEARBEITEN  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | BERICHT  |
|   |   |   |   |   |   | SEARCH  |

{style="table-layout:auto"}

### LicenseTypeGroupLimit

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| customerID | Kundin bzw. Kunde |   |   |   |   |   |
| groupID | Gruppe |   |   |   |   |   |
| planLimit |   |   |   |   |   |   |
| usedLicenses |   |   |   |   |   |   |
| Arbeitsgrenze |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

### UserHomeCalendarPreference

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| customerID | Kundin bzw. Kunde |   |   |   |   | HINZUFÜGEN |
| edTime | Benutzerin bzw. Benutzer |   |   |   |   | ANZAHL |
| firstDayOfWeek |   |   |   |   |   | LÖSCHEN |
| ID |   |   |   |   |   | BEARBEITEN |
| showPTO |   |   |   |   |   | GET |
| startTime |   |   |   |   |   | BERICHT |
| userID |   |   |   |   |   | SEARCH |
| workDate |   |   |   |   |   |   |

{style="table-layout:auto"}

**Ressourcen aktualisiert**

Die folgenden vorhandenen Ressourcen wurden mit dieser Version der Workfront-API aktualisiert. An einer Ressource vorgenommene Änderungen werden wie folgt angezeigt:

* Ergänzungen werden einfach aufgelistet
* Entfernungen werden durch durchgestrichenen Text gekennzeichnet
* Änderungen werden in der Anmerkung nach der Tabelle aufgeführt

### Genehmigung

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| Kanban-Flag |  |  | `<sup>1</sup>` ausstehend   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |
| projectBudgetedCost  |   |   |   |   |   |   |
| projectNetValue  |   |   |   |   |   |   |
| projectROI  |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost  |   |   |   |   |   |   |

{style="table-layout:auto"}

`<sup>1</sup> Type changed from null to boolean`

### Zuweisung

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| assignmentPercent-`<sup>1</sup>` |   |   |   |   |   |   |
| viewedByAssignedToUser |   |   |   |   |   |   |

{style="table-layout:auto"}

`<sup>1</sup>`hat Validator LESS_THAN_EQUAL hinzugefügt

### Budgetierte Stunde

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### Kundenpräferenzen

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| Name `<sup>1</sup>` |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Änderungen an possibleValues

### DocMetadataLinkGroup

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   | getMetadataForDocument |   |   |

{style="table-layout:auto"}

### Dokument

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |   |   |   |   |   |

{style="table-layout:auto"}

### DocumentRequest

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

DocumentVersion

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| externalIntegrationType <sup>1</sup> |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Änderungen an possibleValues

Ausgabe

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Gruppe

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   | licenseTypeLimit |   |   | addRemoveLicenseTypeLimits  |   |   |
|   |   |   |   | setLicenseTypeLimit |   |   |

{style="table-layout:auto"}

### LinkedFolder

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| externalIntegrationType.<sup></sup> |  |  |  |  |   |   |

{style="table-layout:auto"}

<sup>1</sup> Änderungen an possibleValues

### OpTask

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| priorityColor |   |  | pendingApproval<sup>1</sup> |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Typ von null in boolesch geändert

### Portalabschnitt

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |  |   | groupIDs |   |   |   |

{style="table-layout:auto"}

### Portfolio

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| portfolioNetValue |   |   |   |  |  |   |
| portfolioROI |   |   |   |   |   |   |

{style="table-layout:auto"}

### Projekt

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| projectBudgetedCost  |   |   |   | linkExternalObject  |   |   |
| projectNetValue |   |   |   | unlinkExternalObject |   |   |
| projectROI |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost |   |   |   |   |   |   |

{style="table-layout:auto"}

### Testversandvalidierung

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| Genehmigende Entscheidung |   |   |   |   |   |   |

{style="table-layout:auto"}

### Rate

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| rateValue <sup>1</sup> |  |  |  |  |  |   |

{style="table-layout:auto"}

<sup>1</sup>Validator-WÄHRUNG hinzugefügt

### Aufgabe

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| Kanban-Flag |   |   |   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### Team

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| hoursPerPoint <sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Validator LESS_THAN hinzugefügt

### TeamAssignment

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Teamaufgabe

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Arbeitszeittabelle

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

### Aktualisieren

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| updateType `<sup>1</sup>` |   |   |   |   |   | objectUpdatesWithNoteAndJournalEntryIndex  |

{style="table-layout:auto"}

<sup>1</sup> Änderungen an possibleValues

### Benutzerin oder Benutzer

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   | accessLevel  |   |   |   |   |   |

{style="table-layout:auto"}

### UserNote

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| eventType <sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Änderungen an possibleValues

### Arbeit

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| Kanban-Flag |  |  | PendingApproval <sup>1</sup>  |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Typ von null in boolesch geändert

## Entfernte Ressourcen {#removed-resources}

### ResourceBudgetedHour

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | HINZUFÜGEN  |
| budgetierte Stunden |   |   |   |   |   | ANZAHL  |
| ID |   |   |   |   |   | LÖSCHEN  |
| geplante budgetierte Stunden |   |   |   |   |   | BEARBEITEN  |
| projectID |   |   |   |   |   | GET  |
| roleID |   |   |   |   |   | BERICHT  |
| userID |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

 

 

 
