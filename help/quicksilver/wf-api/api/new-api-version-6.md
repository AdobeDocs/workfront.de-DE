---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in der API-Version 6
description: Neue Funktionen in der API-Version 6
author: Becky
feature: Workfront API
role: Developer
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
TQID: https://experienceleague.adobe.com/ZXBvvhz5ObfHlwX2BBBs2-F2DbSmgY4lj8TwWnMCzBM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 513
ht-degree: 54%

---

# Neue Funktionen in der API-Version 6

## Neue Objekte

### Ressourcenmanager

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID | Kundin bzw. Kunde |   |   |   |   | Hinzufügen |
| customerID | Projekt |   |   |   |   | Count |
| projectID | resourceManager |   |   |   |   | Löschen |
| resourceManagerID | Vorlage |   |   |   |   | Abrufen |
| templateID |   |   |   |   |   | Bericht  |
|   |   |   |   |   |   | Suchen  |


### EWS

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| fileName |   |   |   |   | Upload |   |
| handhaben |   |   |   |   |   |   |
| objCode |   |   |   |   |   |   |


### Benutzerdefinierter Titel

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   | checkDelete | customLabels | Hinzufügen |
|   |   |   |   | inUseByOtherLayoutTemplate | userCustomLabels | Count |
|   |   |   |   | removeCustomLabel |   | Löschen |
|   |   |   |   |   |   | Abrufen |
|   |   |   |   |   |   | Bericht |
|   |   |   |   |   |   | Suchen |


## Aktualisierte Objekte

Änderungen an vorhandenen Objekten: Ergänzungen werden einfach aufgelistet, Entfernungen werden durchgestrichen, Änderungen an vorhandenen Objekten werden mit einer Notiz nach der Tabelle versehen

### Aktualisieren

 

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> Änderungen an möglichen Werten

<sup>2</sup> hasFilters-Attribut in true geändert

 

### Genehmigung

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| completedHours |   | resourceManager | resourceManagerIDs |   |   |   |
| constraintDate<sup>1</sup> |   |   |   |   |   |   |
| isOriginalPlannedHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Datumsvalidierung hinzugefügt

<sup>2</sup> NOT_FILTERABLE-Flag hinzugefügt

 

### Genehmigungsprozess

|   | Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|---|
|   |  | `attachedApprovalPaths` |   |   |   |   |   |

{style="table-layout:auto"}

 

### Genehmigungsschritt

 

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| approvalType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Änderungen an möglichen Werten

 

### Genehmigungspfad<sup>1</sup>

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| approvalStatus |   |   |   |   |   | Hinzufügen |
| approvalStatusLabel |   |   |   |   |   | Count |
| Kommentar |   |   |   |   |   | Löschen |
| enteredByID |   |   |   |   |   | Bearbeiten |
| entryDate |   |   |   |   |   | Abrufen |
| globalPathID |   |   |   |   |   | Bericht |
| isPrivate |   |   |   |   |   | Suchen |
| lastUpdateDate |   |   |   |   |   |   |
| lastUpdateByID |   |   |   |   |   |   |
| name<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> In Berichterstellbar geändert

<sup>2</sup> Maximallängen-Validator hinzugefügt

 

### Work Service-Objekt

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| constraintDate<sup>1</sup> |   |   |   | getMyWorkCountFiltered |   |   |
| workRequired<sup>2</sup> |   |   |   | workItemStatusLabels  |   |   |

{style="table-layout:auto"}

<sup>1</sup> Datumsvalidierung hinzugefügt

<sup>2</sup> NOT_FILTERABLE-Flag hinzugefügt

 

### Zuweisung

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnProjects |   |   |
|   |   |   |   | swapUsersOnProjects |   |   |
|   |   |   |   | unassignUserFromProjects |   |   |

{style="table-layout:auto"}

 

### Baseline 

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> NOT_FILTERABLE-Flag hinzugefügt

 

### Baseline-Aufgabe

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> NOT_FILTERABLE-Flag hinzugefügt

 

### Abrechnungseintrag

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| billingDate<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Feld NO_TIME hinzugefügt

### Burndown-Ereignis 

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| eventInitiator |   |   |   |   |   | `ADD` |
|   |   |   |   |   |   | `DELETE` |

{style="table-layout:auto"}

 

### Kategorie 

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   | getCascadingRules |   |   |
|   |   |   |   | reorderCategories |   |   |

{style="table-layout:auto"}

 

Benutzerdefinierte Aufzählung 

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   | getGroupDefaultProjectStatus | opTaskGroupStatuses |   |
|   |   |   |   | isPossibleToUnlockStatus | projectGroupStatuses |   |
|   |   |   |   |   | taskGroupStatuses |   |

{style="table-layout:auto"}

 

Dokument 

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   |  isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

Wechselkurs 

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| rate<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Geänderter PRÄZISIONS-Validator für 8 bis 9

 

### Integration

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| syncBurndownDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### Journaleintrag

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| changeType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Änderungen an möglichen Werten

 

### Aufgabe (Problem)<sup>1</sup> 

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Als WIEDERHERSTELLBAR gekennzeichnet

<sup>2</sup> NOT_FILTERABLE-Flag hinzugefügt

 

### project<sup>1</sup> 

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalPlannedHoursSet |   | resourceManager | resourceManagerIDs  |   |   |   |
| originalWorkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| Arbeit |   |   |   |   |   |   |
| WorkRequired |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Als WIEDERHERSTELLBAR und RESOURCE_MANAGEABLE gekennzeichnet

<sup>2</sup> NOT_FILTERABLE-Flag hinzugefügt

 

### Aufgabe<sup>1</sup>

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| constraintDate<sup>2</sup> |   |   |   |   |   |   |
| workRequired<sup>3</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Als WIEDERHERSTELLBAR gekennzeichnet

<sup>2</sup> AT_DATE_YEAR_BEFORE Validator hinzugefügt

<sup>3</sup> NOT_FILTERABLE-Flag hinzugefügt

 

### Team

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style="table-layout:auto"}

 

### template<sup>1</sup> 

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   | resourceManager | resourceManagerIDs |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Als WIEDERHERSTELLBAR und RESOURCE_MANAGEABLE gekennzeichnet

### Vorlagenaufgabe<sup>1</sup> 

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Als WIEDERHERSTELLBAR gekennzeichnet

<sup>2</sup> NOT_FILTERABLE-Flag hinzugefügt

 

### Benutzerin oder Benutzer

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| myInfo<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> MAX_LENGTH-Verletzungen

 

### Benutzerhinweis

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| eventType<sup>1</sup> |   |   |   |   | myNotifications<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> Mögliche Werte geändert

<sup>2</sup> hat Filter in `[true]` geändert

 

### Ankündigung

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
