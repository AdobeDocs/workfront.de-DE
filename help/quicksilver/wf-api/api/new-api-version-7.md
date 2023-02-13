---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in API Version 7
description: Sammlungen
author: John
feature: Workfront API
exl-id: 8c575251-677b-474d-84aa-02b637ef7760
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 50%

---

# Neue Funktionen in API Version 7

## Neue Objekte

### Proof Bean

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | Suchen |
| adLine |   |   |   |   |   |   |
| name |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### DocMetadataLink

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Felder</th> 
   <th>Verweise</th> 
   <th> <p data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type&quot;}">Sammlungen</p> <p data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type&quot;}">+++++++++++ </p> </th> 
   <th>Suchen</th> 
   <th>Aktionen</th> 
   <th>Abfragen</th> 
   <th>Vorgänge</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>ID</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>Hinzufügen</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>Anzahl </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>Löschen </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>Get  </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>Bericht </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>Suchen </td> 
  </tr> 
 </tbody> 
</table>

### DocMetadataLinkGroup

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | Hinzufügen |
|   |   |   |   |   |   | Anzahl |
|   |   |   |   |   |   | Löschen |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | Bericht |
|   |   |   |   |   |   | Suchen |

{style=&quot;table-layout:auto&quot;}

### TestversandApproval

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | Anzahl |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | Bericht |
|   |   |   |   |   |   | Suchen |

{style=&quot;table-layout:auto&quot;}

 

### ResourceContour

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | Hinzufügen |
|   |   |   |   |   |   | Anzahl |
|   |   |   |   |   |   | Löschen |
|   |   |   |   |   |   | Bearbeiten |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | Bericht |
|   |   |   |   |   |   | Suchen |

{style=&quot;table-layout:auto&quot;}

 

### UserGroups

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| groupID | Gruppe |   |   |   |   |   |
| isOwner  | Benutzer  |   |   |   |   |   |
| userID  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### TimesheetProfile

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |  hourTypes |   |   |   | Hinzufügen |
| name |   |   |   |   |   | Kopieren |
|   |   |   |   |   |   | Anzahl |
|   |   |   |   |   |   | Löschen |
|   |   |   |   |   |   | Bearbeiten |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | Bericht |
|   |   |   |   |   |   | Suchen |
|   |   |   |   |   |   | Ersetzen |

{style=&quot;table-layout:auto&quot;}

 

### RsrcPool

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID | customer | Benutzer |   |   |   | Hinzufügen |
| customerID  | enterBy  |   |   |   |   | Anzahl |
| description  | lastUpdatedBy  |   |   |   |   | Löschen |
| enterByID  |   |   |   |   |   | Bearbeiten |
| entryDate  |   |   |   |   |   | Get |
| extRefID  |   |   |   |   |   | Bericht |
| lastUpdateDate |   |   |   |   |   | Suchen |
| lastUpdateByID |   |   |   |   |   |   |
| name |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### DocMetadataLinkGroup

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | Anzahl |
| articleName  |   |   |   |   |   | Get |
| pageID  |   |   |   |   |   | Bericht |
| url  |   |   |   |   |   | Suchen |

{style=&quot;table-layout:auto&quot;}

 

 

 

## Aktualisierte Objekte

Änderungen an vorhandenen Objekten: -Hinzufügungen werden einfach aufgelistet, Entfernungen sind durchgestrichen, Änderungen an vorhandenen haben einen angehängten Hinweis nach der Tabelle.

### UpdateBean

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| updateType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Änderungen an möglichen Werten 

 

### ApprovalServiceObject

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate¹ |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |    |

{style=&quot;table-layout:auto&quot;}

 

### AccessRule¹

¹ Als meldepflichtig gekennzeichnet

 

### Genehmigungsprozess

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   | `AttachedApprovalPaths`  |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

  

### Genehmigungspfad¹

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | `Add` |
|   |   |   |   |   |   | `Delete` |
|   |   |   |   |   |   | `Edit` |

{style=&quot;table-layout:auto&quot;}

¹ Ausgeführte Kennzeichnung entfernt

 

### Work Service-Objekt

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Datumsvalidierung hinzugefügt

² Nicht-filterbares Flag hinzugefügt

 

### Zuweisung

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|  workPerDayList |   |   |   | assignUserToRoleOnProjects¹ |   |   |
|   |   |   |   | swapUsersOnProjects¹ |   |   |
|   |   |   |   | unassignUserFromProjects¹ |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Felder wurden hinzugefügt, includeIssues

 

### Kunde 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| bizRuleExclusions¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Änderungen an möglichen Werten 

 

### Benutzerdefinierte Enumeration 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| groupID  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Dokument 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| checkOutTimestamp |   |   |   |  createProof |   |   |

{style=&quot;table-layout:auto&quot;}

 

### DocumentVersion 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   |  getProofingTokens |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Gruppe

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| isPublic |  layoutTemplate | userGroups  |   |   |   |   |
| layoutTemplateID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Änderung des PRÄZISION-Validators für 8 bis 9

 

### HourType

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   |   | defaultOpTaskHourType |   |
|   |   |   |   |   | defaultProjectHourType |   |
|   |   |   |   |   | defaultTaskHourType  |   |
|   |   |   |   |   | globalHourTypes  |   |
|   |   |   |   |   | objectHourTypes  |   |

{style=&quot;table-layout:auto&quot;}

 

### Journaleintrag

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| changeType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Änderungen an möglichen Werten

 

### Optask (Problem)

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |  assignMultiple |   |   |
| approvalStartDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

 

### Projekt

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

 

### QueueDef

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| allowedLegacyQueueTopicIDs |  |  |  | getQueueDefTree |   |   |

{style=&quot;table-layout:auto&quot;}

 

### QueueTopic

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   |   |  queueTopicID |   |

{style=&quot;table-layout:auto&quot;}

 

### Zuletzt

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   |  updateLastViewedObject |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Aufgabe

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   | assignMultiple  |   |   |
| approvalStartDate |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### TemplateTask

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| workRequired¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Typ geändert von &quot;Int&quot;zu &quot;Double&quot; 

 

### Benutzer

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Felder</th> 
   <th>Verweise</th> 
   <th>Sammlungen</th> 
   <th>Suchen</th> 
   <th>Aktionen</th> 
   <th>Abfragen</th> 
   <th>Vorgänge</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>
    <code>lastWhatsNew</code> </td> 
   <td> </td> 
   <td>
    <code>roles</code> </td> 
   <td> Rollen</td> 
   <td>addMobileDevice</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <span data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;scheduleDeactivationDate&quot;}" data-sheets-userformat="{&quot;2&quot;:8707,&quot;3&quot;:{&quot;1&quot;:0},&quot;4&quot;:{&quot;1&quot;:2,&quot;2&quot;:14277081},&quot;12&quot;:0,&quot;16&quot;:10}">scheduleDeactivationDate</span></td> 
   <td> </td> 
   <td><span data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;timesheetProfileHourTypes&quot;}" data-sheets-userformat="{&quot;2&quot;:8707,&quot;3&quot;:{&quot;1&quot;:0},&quot;4&quot;:{&quot;1&quot;:2,&quot;2&quot;:14277081},&quot;12&quot;:0,&quot;16&quot;:10}">timesheetProfileHourTypes</span> </td> 
   <td> </td> 
   <td>getAvailableActions</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>hasAnyAccess</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>isUserTerminologyActive</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>removeMobileDevice</p> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>showShouldProofHQNavButton</td> 
   <td> </td> 
   <td>  </td> 
  </tr> 
 </tbody> 
</table>

### Benutzerhandbuch

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `acknowledgedmentIDs` |   |   |   |  unackkenntnisMany |   |   |
| ackDate |   |   |   |   |   |   |
| ackType |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

 

### CustomerPrefObject

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|  name |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Änderungen an möglichen Werten
