---
content-type: api
navigation-topic: api-navigation-topic
title: Aktualisierungen für API Version 9
description: Aktualisierte Ressourcen
author: Becky
feature: Workfront API
exl-id: 51892846-d93f-4363-8416-4118fb2ef84d
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 47%

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
| `opTaskID`<sup>2</sup> |  |  |  |  |  |  |
| `taskID`<sup>2</sup> |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹ Markierung entfernt: REPORTABLE\
² Flag entfernt: NOT_GROUPABLE

### Genehmigung

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

Zuweisung

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|  |  |  |  | `assignUserToRoleOnProjects`<sup>1</sup> |  |  |
|  |  |  |  | `assignUserToRoleOnTasks`<sup>1</sup> |  |  |
|  |  |  |  | `swapUsersOnProjects`<sup>1</sup> |  |  |
|  |  |  |  | `swapUsersOnTasks`<sup>1</sup> |  |  |

{style=&quot;table-layout:auto&quot;}

¹ Feld hinzugefügt: lockToRole

### CustomerPreferences

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `name`<sup>1</sup> |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Änderungen an möglichen Werten

### Stunde

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `days` |  |  |  |  |  |  |
| `workHoursPerDay` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### Wiederholung

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|  |  |  |  | `moveIssues` |  |  |

{style=&quot;table-layout:auto&quot;}

### LayoutTemplates

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `groupID` | `group` |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### Notiz

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `html` |  |  |  |  |  |  |
| `json` |  |  |  |  |  |  |
| `richTextNoteID` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### OpTask

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `color` | `agileWork` |  |  | `convertToProject` |  |  |
| `isReady` |  |  |  | `convertToTask` |  |  |
| `storyBoardOrder` |  |  |  | `linkExternalObject` |  |  |
|  |  |  |  | `unlinkExternalObject` |  |  |

{style=&quot;table-layout:auto&quot;}

### ResourceBudget

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `ID` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹ Markierung entfernt: REPORTABLE

### Zeitplan

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `homeGroupID` | `homeGroup` |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### Aufgabe

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|  | `agileWork` |  |  | `convertToProject` |  |  |
|  |  |  |  | `linkExternalObject` |  |  |
|  |  |  |  | `unlinkExternalObject` |  |  |

{style=&quot;table-layout:auto&quot;}

### Team

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `includeIssues` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### TimesheetProfile

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `groupID` | `group` |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### UIFilter

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|  |  |  |  |  | `filtersForObjCode` |  |

{style=&quot;table-layout:auto&quot;}

### UIView

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|  |  |  |  |  | `viewsForObjCode` |  |

{style=&quot;table-layout:auto&quot;}

### Benutzer

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `logTimeInDays` |  |  |  |  |  |  |
| `workHoursPerDay` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### Arbeit

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |  |  | `getWFHomeObjects` |  |  |
