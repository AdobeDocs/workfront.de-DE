---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in der API-Version 8
description: Dies ist eine Liste der Ressourcen, die neu in der API-Version 9 sind. Eine Liste der Aktualisierungen, die an den Ressourcen von Version 8 vorgenommen wurden, finden Sie unter Aktualisierungen der API-Version 8 .
author: Becky
feature: Workfront API
role: Developer
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 33%

---

# Neue Funktionen in der API-Version 8

## Neue Ressourcen

Dies ist eine Liste der Ressourcen, die neu in der API-Version 9 sind. Eine Liste der Aktualisierungen, die an den Ressourcen der Version 8 vorgenommen wurden, finden Sie unter [Aktualisierungen der API-Version 8](../../wf-api/api/new-api-version-8-updates.md)

**AgileWork**

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| Auftragsbestand | Kunde |   |   | BulkCopy  |   | KOPIEREN |
| Farbe | Wiederholung  |   |   |   |   | ANZAHL |
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
| Typ |   |   |   |   |   |   |
| uiObjCode |   |   |   |   |   |   |
| uiObjectID |   |   |   |   |   |   |

{style="table-layout:auto"}

### APIVersionMetadata

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| EinstellungRelease |   |   |   |   |   | ANZAHL  |
| removeRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | BERICHT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**KanbanBoard**

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
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

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style="table-layout:auto"}

**ProofFileMetadata**

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| documentVersionID | documentVersion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| fileName |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style="table-layout:auto"}

**ResourceBudgetedHour**

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
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

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
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

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | ANZAHL |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | BERICHT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### Abonnieren

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | Abonnenten | HINZUFÜGEN |
|   |   |   |   | removeSubscribers |   | ANZAHL  |
|   |   |   |   | Anmeldungen |   | LÖSCHEN |
|   |   |   |   | Abmeldungen |   | GET |
|   |   |   |   |   |   | BERICHT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### UserRole

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| roleID | Rolle |   |   |   |   |   |
| timePercentage | Benutzer |   |   |   |   |   |
| userID |   |   |   |   |   |   |
