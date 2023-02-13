---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in API Version 6
description: Neue Funktionen in API Version 6
author: John
feature: Workfront API
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
source-git-commit: 2ec05c03a5bfa842008870ca47fb617b81fd6ebd
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 42%

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
|   |   |   |   |   |   | Suchen  |


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

Änderungen an vorhandenen Objekten: -Hinzufügungen werden einfach aufgelistet, Entfernungen sind durchgestrichen, Änderungen an vorhandenen haben einen angehängten Hinweis nach der Tabelle.

### Aktualisieren

 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| updateType¹ |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID² |   |

{style=&quot;table-layout:auto&quot;}

¹ Änderungen an möglichen Werten

² hasFilters attribute changed to true

 

### Genehmigung

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| completedHours |   | resourceManager | resourceManagerIDs |   |   |   |
| constraintDate¹ |   |   |   |   |   |   |
| isOriginalPlannedHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Datumsvalidierung hinzugefügt

² Markierung NOT_FILTERABLE hinzugefügt

 

### Genehmigungsprozess

|   | Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|---|
|  |  | `attachedApprovalPaths` |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Validierungsschritt

 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| approvalType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Änderungen an möglichen Werten

 

### Genehmigungspfad¹

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| authorisedStatus |   |   |   |   |   | Hinzufügen |
| authorisedStatusLabel |   |   |   |   |   | Anzahl |
| Kommentar |   |   |   |   |   | Löschen |
| enterByID |   |   |   |   |   | Bearbeiten |
| entryDate |   |   |   |   |   | Get |
| globalPathID |   |   |   |   |   | Bericht |
| isPrivate |   |   |   |   |   | Suchen |
| lastUpdateDate |   |   |   |   |   |   |
| lastUpdateByID |   |   |   |   |   |   |
| name² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ In MELDEPFLICHTIG geändert

² Max Length Validator hinzugefügt

 

### Work Service-Objekt

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| constraintDate¹ |   |   |   | getMyWorkCountFiltered |   |   |
| workRequired² |   |   |   | workItemStatusLabels  |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Datumsvalidierung hinzugefügt

² Nicht-filterbares Flag hinzugefügt

 

### Zuweisung

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnProjects |   |   |
|   |   |   |   | swapUsersOnProjects |   |   |
|   |   |   |   | unassignUserFromProjects |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Ausgangsbasis 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| workRequired¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Nicht-filterbare Markierung hinzugefügt

 

### Baseline-Aufgabe

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| workRequired¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Nicht-filterbare Markierung hinzugefügt

 

### Rechnungsnachweis

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| billingDate¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Markierung für Feld NO_TIME hinzugefügt

### Niedergangsereignis 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| eventInitiator |   |   |   |   |   | `ADD` |
|   |   |   |   |   |   | `DELETE` |

{style=&quot;table-layout:auto&quot;}

 

### Kategorie 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   | getCascadingRules |   |   |
|   |   |   |   | reorderCategories |   |   |

{style=&quot;table-layout:auto&quot;}

 

Benutzerdefinierte Enumeration 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   | getGroupDefaultProjectStatus | opTaskGroupStatuses |   |
|   |   |   |   | isPossibleToUnlockStatus | projectGroupStatuses |   |
|   |   |   |   |   | taskGroupStatuses |   |

{style=&quot;table-layout:auto&quot;}

 

Dokument 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   |  isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

Wechselkurs 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| rate¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Änderung des PRÄZISION-Validators für 8 bis 9

 

### Integration

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| syncBurndownDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Journaleintrag

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| changeType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Änderungen an möglichen Werten

 

### Optask (Problem)¹ 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Als RESTORABLE gekennzeichnet

² Nicht-filterbares Flag hinzugefügt

 

### Projekt¹ 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalPlannedHoursSet |   | resourceManager | resourceManagerIDs  |   |   |   |
| originalWorkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| Arbeit |   |   |   |   |   |   |
| workRequired |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Als RESTORABLE und RESOURCE_MANAGEABLE gekennzeichnet

² Nicht-filterbares Flag hinzugefügt

 

### Aufgabe¹

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| constraintDate² |   |   |   |   |   |   |
| workRequired³ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Als RESTORABLE gekennzeichnet

² AT_DATE_YEAR_BEFORE -Validator hinzugefügt

³ Nicht-filterbare Markierung hinzugefügt

 

### Team

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Vorlage¹ 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   | resourceManager | resourceManagerIDs |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Als RESTORABLE und RESOURCE_MANAGEABLE gekennzeichnet

### Vorlagenaufgabe¹ 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Als RESTORABLE gekennzeichnet

² Nicht-filterbares Flag hinzugefügt

 

### Benutzer

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| myInfo¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ MAX_LENGTH-Geiger

 

### Benutzerhandbuch

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| eventType¹ |   |   |   |   | myNotifications² |   |

{style=&quot;table-layout:auto&quot;}

¹ Mögliche Werte geändert

² hat Filter geändert zu `[true]`

 

### Ankündigung

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
