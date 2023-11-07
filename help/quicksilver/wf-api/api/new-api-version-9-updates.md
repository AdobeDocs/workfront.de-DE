---
content-type: api
navigation-topic: api-navigation-topic
title: Aktualisierungen für API Version 9
description: Aktualisierte Ressourcen
author: Becky
feature: Workfront API
role: Developer
exl-id: 51892846-d93f-4363-8416-4118fb2ef84d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 36%

---

# Aktualisierungen für API Version 9

## Aktualisierte Ressourcen

Die folgenden vorhandenen Ressourcen wurden mit dieser Version der Adobe Workfront-API aktualisiert. Um die Ressourcen anzuzeigen, die neu in Version 9 sind, können Sie [Neue Funktionen in API Version 9](../../wf-api/api/new-api-version-9.md) und [Neue Funktionen in API Version 9 (Fortsetzung)](../../wf-api/api/new-api-version-9-continue.md). Änderungen an einer Ressource werden wie folgt angegeben:

* Hinzufügungen werden einfach aufgelistet
* Entfernungen werden mit Durchstreichen angezeigt
* Änderungen werden in der Anmerkung nach der Tabelle aufgeführt

### AgileWork

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `opTaskID`<sup>2</sup> |  |   |  |   |   |  |
| `taskID`<sup>2</sup> |   |   |  |  |  |  |

{style="table-layout:auto"}

<sup>1</sup> Flag entfernt: REPORTABLE\
<sup>2</sup> Flag entfernt: NOT_GROUPABLE

### Genehmigung

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |   |   |   |   |   |

{style="table-layout:auto"}

Zuweisung

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| |   |  |  | `assignUserToRoleOnProjects`<sup>1</sup> |   |   |
|   |   |   |   | `assignUserToRoleOnTasks`<sup>1</sup> |   |   |
|   |   |   |   | `swapUsersOnProjects`<sup>1</sup> |   |   |
|   |   |   |   | `swapUsersOnTasks`<sup>1</sup> |   |   |

{style="table-layout:auto"}

<sup>1</sup> Feld hinzugefügt: lockToRole

### CustomerPreferences

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `name`<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Änderungen an möglichenWerten

### Stunde

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `days` |   |   |   |   |   |   |
| `workHoursPerDay` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Wiederholung

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   | `moveIssues` |   |   |

{style="table-layout:auto"}

### LayoutTemplates

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `groupID` | `group` |   |   |   |   |   |

{style="table-layout:auto"}

### Notiz

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `html` |   |   |   |   |   |   |
| `json` |   |   |   |   |   |   |
| `richTextNoteID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### OpTask

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `color` | `agileWork` |   |   | `convertToProject` |   |   |
| `isReady` |   |   |   | `convertToTask` |   |   |
| `storyBoardOrder` |   |   |   | `linkExternalObject` |   |   |
|   |   |   |   | `unlinkExternalObject` |   |   |

{style="table-layout:auto"}

### ResourceBudget

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `ID` |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Flag entfernt: REPORTABLE

### Zeitplan

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `homeGroupID` | `homeGroup` |   |   |   |   |   |

{style="table-layout:auto"}

### Aufgabe

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   | `agileWork` |   |   | `convertToProject` |   |   |
|   |   |   |   | `linkExternalObject` |   |   |
|   |   |   |   | `unlinkExternalObject` |   |   |

{style="table-layout:auto"}

### Team

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `includeIssues` |   |   |   |   |   |   |

{style="table-layout:auto"}

### TimesheetProfile

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `groupID` | `group` |   |   |   |   |   |

{style="table-layout:auto"}

### UIFilter

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   |   | `filtersForObjCode` |   |

{style="table-layout:auto"}

### UIView

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   |   | `viewsForObjCode` |   |

{style="table-layout:auto"}

### Benutzerin oder Benutzer

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `logTimeInDays` |   |   |   |   |   |   |
| `workHoursPerDay` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Arbeit

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |   |   | `getWFHomeObjects` |   |   |
