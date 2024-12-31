---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in der API-Version 6
description: Neue Funktionen in der API-Version 6
author: Becky
feature: Workfront API
role: Developer
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 39%

---

# Neue Funktionen in der API-Version 6

## Neue Objekte

### Ressourcenmanager

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID | Kunde |   |   |   |   | Hinzufügen |
| customerID | Projekt |   |   |   |   | Anzahl |
| projectID | resourceManager |   |   |   |   | Löschen |
| resourceManagerID | Vorlage |   |   |   |   | Abrufen |
| templateID |   |   |   |   |   | Bericht  |
|   |   |   |   |   |   | Suche  |


### EWS

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| fileName |   |   |   |   | Upload |   |
| handhaben |   |   |   |   |   |   |
| objCode |   |   |   |   |   |   |


### Benutzerdefinierter Titel

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   | checkDelete | customLabels | Hinzufügen |
|   |   |   |   | inUseByOtherLayoutTemplate | userCustomLabels | Anzahl |
|   |   |   |   | removeCustomLabel |   | Löschen |
|   |   |   |   |   |   | Abrufen |
|   |   |   |   |   |   | Bericht |
|   |   |   |   |   |   | Suchen |


## Aktualisierte Objekte

Änderungen an vorhandenen Objekten: Ergänzungen werden einfach aufgelistet, Entfernungen werden durchgestrichen, Änderungen an vorhandenen Objekten werden mit einer Notiz nach der Tabelle versehen

### Aktualisieren

 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> Änderungen an möglichen Werten

<sup>2</sup> hasFilters-Attribut in true geändert

 

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

<sup>2</sup> NOT_FILTERABLE-Flag hinzugefügt

 

### Genehmigungsprozess

|   | Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|---|
|   |  | `attachedApprovalPaths` |   |   |   |   |   |

{style="table-layout:auto"}

 

### Genehmigungsschritt

 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| approvalType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Änderungen an möglichen Werten

 

### Genehmigungspfad<sup>1</sup>

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| approvalStatus |   |   |   |   |   | Hinzufügen |
| approvalStatusLabel |   |   |   |   |   | Anzahl |
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

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| constraintDate<sup>1</sup> |   |   |   | getMyWorkCountFiltered |   |   |
| workRequired<sup>2</sup> |   |   |   | workItemStatusLabels  |   |   |

{style="table-layout:auto"}

<sup>1</sup> Datumsvalidierung hinzugefügt

<sup>2</sup> NOT_FILTERABLE-Flag hinzugefügt

 

### Zuweisung

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnProjects |   |   |
|   |   |   |   | swapUsersOnProjects |   |   |
|   |   |   |   | unassignUserFromProjects |   |   |

{style="table-layout:auto"}

 

### Baseline 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> NOT_FILTERABLE-Flag hinzugefügt

 

### Baseline-Aufgabe

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> NOT_FILTERABLE-Flag hinzugefügt

 

### Abrechnungseintrag

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| billingDate<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Feld NO_TIME hinzugefügt

### Burndown-Ereignis 

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

 

Benutzerdefinierte Enumeration 

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

<sup>1</sup> Geänderter PRÄZISIONS-Validator für 8 bis 9

 

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

 

### Aufgabe (Problem)<sup>1</sup> 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Als WIEDERHERSTELLBAR gekennzeichnet

<sup>2</sup> NOT_FILTERABLE-Flag hinzugefügt

 

### project<sup>1</sup> 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
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

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| constraintDate<sup>2</sup> |   |   |   |   |   |   |
| workRequired<sup>3</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Als WIEDERHERSTELLBAR gekennzeichnet

<sup>2</sup> AT_DATE_YEAR_BEFORE Validator hinzugefügt

<sup>3</sup> NOT_FILTERABLE-Flag hinzugefügt

 

### Team

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style="table-layout:auto"}

 

### template<sup>1</sup> 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   | resourceManager | resourceManagerIDs |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Als WIEDERHERSTELLBAR und RESOURCE_MANAGEABLE gekennzeichnet

### Vorlagenaufgabe<sup>1</sup> 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Als WIEDERHERSTELLBAR gekennzeichnet

<sup>2</sup> NOT_FILTERABLE-Flag hinzugefügt

 

### Benutzerin oder Benutzer

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| myInfo<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> MAX_LENGTH-Verletzungen

 

### Benutzerhinweis

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| eventType<sup>1</sup> |   |   |   |   | myNotifications<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> Mögliche Werte geändert

<sup>2</sup> hat Filter in `[true]` geändert

 

### Ankündigung

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
