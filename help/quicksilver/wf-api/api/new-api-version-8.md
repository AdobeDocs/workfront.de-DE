---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in der API-Version 8
description: Dies ist eine Liste der Ressourcen, die neu in der API-Version 9 sind. Eine Liste der Aktualisierungen, die an den Ressourcen von Version 8 vorgenommen wurden, finden Sie unter Aktualisierungen der API-Version 8 .
author: Becky
feature: Workfront API
role: Developer
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
TQID: https://experienceleague.adobe.com/bKFAN--rVO1yxgFLiyhXolgUBajVGYQxM7pBUuqy3v8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 269
ht-degree: 47%

---

# Neue Funktionen in der API-Version 8

## Neue Ressourcen

Dies ist eine Liste der Ressourcen, die neu in der API-Version 9 sind. Eine Liste der Aktualisierungen, die an den Ressourcen der Version 8 vorgenommen wurden, finden Sie unter [Aktualisierungen der API-Version 8](../../wf-api/api/new-api-version-8-updates.md)

**AgileWork**

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| Auftragsbestand | Kundin bzw. Kunde |   |   | BulkCopy  |   | KOPIEREN |
| color | Wiederholung  |   |   |   |   | ANZAHL |
| customerID | lastUpdatedBy |   |   |   |   | LÖSCHEN |
| Kalkulation | Aufgabe |   |   |   |   | BEARBEITEN |
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
| type |   |   |   |   |   |   |
| uiObjCode |   |   |   |   |   |   |
| uiObjectID |   |   |   |   |   |   |

{style="table-layout:auto"}

### APIVersionMetadata

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| EinstellungRelease |   |   |   |   |   | ANZAHL  |
| removeRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | BERICHT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**KanbanBoard**

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | HINZUFÜGEN |
| name |   |   |   |   |   | ANZAHL |
|   |   |   |   |   |   | LÖSCHEN |
|   |   |   |   |   |   | BEARBEITEN |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | BERICHT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### ProofApprovalStatus

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style="table-layout:auto"}

**ProofFileMetadata**

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| documentVersionID | documentVersion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| fileName |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style="table-layout:auto"}

**ResourceBudgetedHour**

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | HINZUFÜGEN |
| budgetierte Stunden |   |   |   |   |   | ANZAHL |
| geplante budgetierte Stunden |   |   |   |   |   | LÖSCHEN |
| projectID |   |   |   |   |   | BEARBEITEN |
| roleID |   |   |   |   |   | GET |
| userID |   |   |   |   |   | BERICHT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### ResourcePlannerFilter

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | HINZUFÜGEN |
| name |   |   |   |   |   | ANZAHL |
|   |   |   |   |   |   | LÖSCHEN |
|   |   |   |   |   |   | BEARBEITEN |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | BERICHT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**RichTextNote**

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | ANZAHL |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | BERICHT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### Abonnieren

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | Abonnenten | HINZUFÜGEN |
|   |   |   |   | removeSubscribers |   | ANZAHL  |
|   |   |   |   | Anmeldungen |   | LÖSCHEN |
|   |   |   |   | Abmeldungen |   | GET |
|   |   |   |   |   |   | BERICHT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### UserRole

| Felder | Referenzen | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| roleID | Rolle |   |   |   |   |   |
| timePercentage | Benutzerin bzw. Benutzer |   |   |   |   |   |
| userID |   |   |   |   |   |   |
