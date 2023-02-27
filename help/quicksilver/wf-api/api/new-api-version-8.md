---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in API Version 8
description: Dies ist eine Liste von Ressourcen, die neu in API Version 9 sind. Eine Liste der Aktualisierungen, die an den Ressourcen von Version 8 vorgenommen wurden, finden Sie unter Aktualisierungen von API Version 8 .
author: Becky
feature: Workfront API
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 32%

---

# Neue Funktionen in API Version 8

## Neue Ressourcen

Dies ist eine Liste von Ressourcen, die neu in API Version 9 sind. Eine Liste der Aktualisierungen, die an den Ressourcen von Version 8 vorgenommen wurden, finden Sie unter [Aktualisierungen für API Version 8](../../wf-api/api/new-api-version-8-updates.md)

**AgileWork**

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| backlogOrder | customer |   |   | bulkCopy  |   | KOPIE |
| color | iteration  |   |   |   |   | COUNT |
| customerID | lastUpdatedBy |   |   |   |   | LÖSCHEN |
| Schätzung | opTask |   |   |   |   | BEARBEITEN |
| ID | Projekt |   |   |   |   | GET  |
| isReady | storyboardParent |   |   |   |   | BERICHT |
| iterationID | Aufgabe |   |   |   |   | SEARCH |
| lastUpdateDate | Team |   |   |   |   |   |
| lastUpdatedByID |   |   |   |   |   |   |
| name |   |   |   |   |   |   |
| opTaskID |   |   |   |   |   |   |
| parentStoryBoardOrder |   |   |   |   |   |   |
| projectID |   |   |   |   |   |   |
| storyBoardOrder |   |   |   |   |   |   |
| storyBoardParentID |   |   |   |   |   |   |
| taskID  |   |   |   |   |   |   |
| teamID |   |   |   |   |   |   |
| Typ |   |   |   |   |   |   |
| uiObjCode |   |   |   |   |   |   |
| uiObjectID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### APIVersionMetadata

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| deprecationRelease |   |   |   |   |   | COUNT  |
| removeRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | BERICHT |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

**KanbanBoard**

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | HINZUFÜGEN |
| name |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | LÖSCHEN |
|   |   |   |   |   |   | BEARBEITEN |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | BERICHT |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### TestversandApprovalStatus

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**ProofFileMetadata**

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| documentVersionID | documentVersion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| fileName |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**ResourceBudgetedHour**

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | HINZUFÜGEN |
| budgetHours |   |   |   |   |   | COUNT |
| scheduledBudgetedHours |   |   |   |   |   | LÖSCHEN |
| projectID |   |   |   |   |   | BEARBEITEN |
| roleID |   |   |   |   |   | GET |
| userID |   |   |   |   |   | BERICHT |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### ResourcePlannerFilter

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | HINZUFÜGEN |
| name |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | LÖSCHEN |
|   |   |   |   |   |   | BEARBEITEN |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | BERICHT |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

**RichTextNote**

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | BERICHT |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### Abonnieren

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | subscribers | HINZUFÜGEN |
|   |   |   |   | removeSubscribers |   | COUNT  |
|   |   |   |   | subscribes |   | LÖSCHEN |
|   |   |   |   | unsubscribes |   | GET |
|   |   |   |   |   |   | BERICHT |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### UserRole

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| roleID | Funktion |   |   |   |   |   |
| timePercentage | Benutzer |   |   |   |   |   |
| userID |   |   |   |   |   |   |
