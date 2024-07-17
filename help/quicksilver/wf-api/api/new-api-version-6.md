---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in API Version 6
description: Neue Funktionen in API Version 6
author: Becky
feature: Workfront API
role: Developer
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 34%

---

# Neue Funktionen in API Version 6

## Neue Objekte

### Ressourcenmanager

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID | customer |   |   |   |   | Hinzufügen |
| customerID | Projekt |   |   |   |   | Anzahl |
| projectID | resourceManager |   |   |   |   | Löschen |
| resourceManagerID | template |   |   |   |   | Get |
| templateID |   |   |   |   |   | Bericht  |
|   |   |   |   |   |   | Suche  |


### Ews

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| fileName |   |   |   |   | hochladen |   |
| handle |   |   |   |   |   |   |
| objCode |   |   |   |   |   |   |


### Eigene Bezeichnung

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   | checkDelete | customLabels | Hinzufügen |
|   |   |   |   | inUseByOtherLayoutTemplate | userCustomLabels | Anzahl |
|   |   |   |   | removeCustomLabel |   | Löschen |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | Bericht |
|   |   |   |   |   |   | Suchen |


## Aktualisierte Objekte

Änderungen an vorhandenen Objekten: Hinzufügungen werden einfach aufgelistet, Entfernungen sind durchgestrichen, Änderungen an vorhandenen Objekten haben einen angehängten Hinweis nach der Tabelle

### Aktualisieren

 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> Änderungen an möglichen Werten

Das Attribut <sup>2</sup> hasFilters wurde in true geändert

 

### Genehmigung

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| completedHours |   | resourceManager | resourceManagerIDs |   |   |   |
| constraintDate<sup>1</sup> |   |   |   |   |   |   |
| isOriginalPlannedHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Datumsvalidierung hinzugefügt

Markierung <sup>2</sup> NOT_FILTERABLE hinzugefügt

 

### Genehmigungsprozess

|   | Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|---|
|   |  | `attachedApprovalPaths` |   |   |   |   |   |

{style="table-layout:auto"}

 

### Validierungsschritt

 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| approvalType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Änderungen an möglichen Werten

 

### Genehmigungspfad<sup>1</sup>

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| authorisedStatus |   |   |   |   |   | Hinzufügen |
| authorisedStatusLabel |   |   |   |   |   | Anzahl |
| comment |   |   |   |   |   | Löschen |
| enterByID |   |   |   |   |   | Bearbeiten |
| entryDate |   |   |   |   |   | Get |
| globalPathID |   |   |   |   |   | Bericht |
| isPrivate |   |   |   |   |   | Suchen |
| lastUpdateDate |   |   |   |   |   |   |
| lastUpdateByID |   |   |   |   |   |   |
| name<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> In &quot;MELDEPFLICHTIG&quot;geändert

<sup>2</sup> Max. Length Validator hinzugefügt

 

### Work Service-Objekt

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| constraintDate<sup>1</sup> |   |   |   | getMyWorkCountFiltered |   |   |
| workRequired<sup>2</sup> |   |   |   | workItemStatusLabels  |   |   |

{style="table-layout:auto"}

<sup>1</sup> Datumsvalidierung hinzugefügt

<sup>2</sup> Flag nicht_filtern hinzugefügt

 

### Zuweisung

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnProjects |   |   |
|   |   |   |   | swapUsersOnProjects |   |   |
|   |   |   |   | unassignUserFromProjects |   |   |

{style="table-layout:auto"}

 

### Grundlinie 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Nicht-filterbare Markierung hinzugefügt

 

### Baseline-Aufgabe

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Nicht-filterbare Markierung hinzugefügt

 

### Abrechnungseintrag

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| billingDate<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Markierung für NO_TIME-Feld hinzugefügt

### Niedergangsereignis 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| eventInitiator |   |   |   |   |   | `ADD` |
|   |   |   |   |   |   | `DELETE` |

{style="table-layout:auto"}

 

### Kategorie 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   | getCascadingRules |   |   |
|   |   |   |   | reorderCategories |   |   |

{style="table-layout:auto"}

 

Benutzerdefinierte Enum 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   | getGroupDefaultProjectStatus | opTaskGroupStatuses |   |
|   |   |   |   | isPossibleToUnlockStatus | projectGroupStatuses |   |
|   |   |   |   |   | taskGroupStatuses |   |

{style="table-layout:auto"}

 

Dokument 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   |  isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

Wechselkurs 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| rate<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Änderung des PRÄZISIONSvalidators für 8 bis 9

 

### Integration

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| syncBurndownDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### Journaleintrag

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| changeType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Änderungen an möglichen Werten

 

### optask (issue)<sup>1</sup> 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Gekennzeichnet als RESTORABLE

<sup>2</sup> Flag nicht_filtern hinzugefügt

 

### Projekt<sup>1</sup> 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalPlannedHoursSet |   | resourceManager | resourceManagerIDs  |   |   |   |
| originalWorkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| Arbeit |   |   |   |   |   |   |
| workRequired |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Als RESTORABLE und RESOURCE_MANAGEABLE gekennzeichnet

<sup>2</sup> Flag nicht_filtern hinzugefügt

 

### Aufgabe<sup>1</sup>

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| constraintDate<sup>2</sup> |   |   |   |   |   |   |
| workRequired<sup>3</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Gekennzeichnet als RESTORABLE

<sup>2</sup> AT_DATE_YEAR_BEFORE Validator hinzugefügt

<sup>3</sup> Flag nicht_filtern hinzugefügt

 

### Team

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style="table-layout:auto"}

 

### Vorlage<sup>1</sup> 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   | resourceManager | resourceManagerIDs |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Als RESTORABLE und RESOURCE_MANAGEABLE gekennzeichnet

### Vorlagenaufgabe<sup>1</sup> 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Gekennzeichnet als RESTORABLE

<sup>2</sup> Flag nicht_filtern hinzugefügt

 

### Benutzerin oder Benutzer

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| myInfo<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> MAX_LENGTH-Geiger

 

### Benutzerhandbuch

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| eventType<sup>1</sup> |   |   |   |   | myNotifications<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> Mögliche Werte geändert

<sup>2</sup> hat Filter geändert zu `[true]`

 

### Ankündigung

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
