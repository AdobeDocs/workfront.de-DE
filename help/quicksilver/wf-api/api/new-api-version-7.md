---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in API Version 7
description: Sammlungen
author: Becky
feature: Workfront API
role: Developer
exl-id: 8c575251-677b-474d-84aa-02b637ef7760
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 40%

---

# Neue Funktionen in API Version 7

## Neue Objekte

### Proof Bean

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | Suchen |
| adLine |   |   |   |   |   |   |
| name |   |   |   |   |   |   |

{style="table-layout:auto"}

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

{style="table-layout:auto"}

### TestversandApproval

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | Anzahl |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | Bericht |
|   |   |   |   |   |   | Suchen |

{style="table-layout:auto"}

 

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

{style="table-layout:auto"}

 

### UserGroups

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| groupID | Gruppe |   |   |   |   |   |
| isOwner  | Benutzer  |   |   |   |   |   |
| userID  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

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

{style="table-layout:auto"}

 

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

{style="table-layout:auto"}

 

### DocMetadataLinkGroup

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | Anzahl |
| articleName  |   |   |   |   |   | Get |
| pageID  |   |   |   |   |   | Bericht |
| url  |   |   |   |   |   | Suchen |

{style="table-layout:auto"}

 

 

 

## Aktualisierte Objekte

Änderungen an vorhandenen Objekten: Hinzufügungen werden einfach aufgelistet, Entfernungen sind durchgestrichen, Änderungen an vorhandenen Objekten haben einen angehängten Hinweis nach der Tabelle

### UpdateBean

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Änderungen an möglichen Werten 

 

### ApprovalServiceObject

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate<sup>1</sup> |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |    |

{style="table-layout:auto"}

 

### AccessRule<sup>1</sup>

<sup>1</sup> Als meldepflichtig markiert

 

### Genehmigungsprozess

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   | `AttachedApprovalPaths`  |   |   |   |   |

{style="table-layout:auto"}

  

### Validierungspfad<sup>1</sup>

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | `Add` |
|   |   |   |   |   |   | `Delete` |
|   |   |   |   |   |   | `Edit` |

{style="table-layout:auto"}

<sup>1</sup> Entferntes berichtspflichtiges Flag

 

### Work Service-Objekt

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Datumsvalidierung hinzugefügt

<sup>2</sup> Nicht-filterbare Markierung hinzugefügt

 

### Zuweisung

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|  workPerDayList |   |   |   | assignUserToRoleOnProjects<sup>1</sup> |   |   |
|   |   |   |   | swapUsersOnProjects<sup>1</sup> |   |   |
|   |   |   |   | unassignUserFromProjects<sup>1</sup> |   |   |

{style="table-layout:auto"}

<sup>1</sup> Feld includeIssues hinzugefügt

 

### Kunde 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| bizRuleExclusions<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Änderungen an möglichen Werten 

 

### Benutzerdefinierte Enumeration 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| groupID  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### Dokument 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| checkOutTimestamp |   |   |   |  createProof |   |   |

{style="table-layout:auto"}

 

### DocumentVersion 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   |  getProofingTokens |   |   |

{style="table-layout:auto"}

 

### Gruppe

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| isPublic |  layoutTemplate | userGroups  |   |   |   |   |
| layoutTemplateID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Änderung des PRÄZISION-Validators für 8 bis 9

 

### HourType

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   |   | defaultOpTaskHourType |   |
|   |   |   |   |   | defaultProjectHourType |   |
|   |   |   |   |   | defaultTaskHourType  |   |
|   |   |   |   |   | globalHourTypes  |   |
|   |   |   |   |   | objectHourTypes  |   |

{style="table-layout:auto"}

 

### Journaleintrag

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| changeType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Änderungen an möglichen Werten

 

### Optask (Problem)

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |  assignMultiple |   |   |
| approvalStartDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

 

### Projekt

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

 

### QueueDef

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| allowedLegacyQueueTopicIDs |  |  |  | getQueueDefTree |   |   |

{style="table-layout:auto"}

 

### QueueTopic

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   |   |  queueTopicID |   |

{style="table-layout:auto"}

 

### Zuletzt

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   |  updateLastViewedObject |   |   |

{style="table-layout:auto"}

 

### Aufgabe

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   | assignMultiple  |   |   |
| approvalStartDate |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### TemplateTask

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Typ geändert von &quot;Int&quot;zu &quot;Double&quot; 

 

### Benutzerin oder Benutzer

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

{style="table-layout:auto"}

 

 

### CustomerPrefObject

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|  name |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Änderungen an möglichen Werten
