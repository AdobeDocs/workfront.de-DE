---
content-type: api
navigation-topic: api-navigation-topic
title: Aktualisierungen für API Version 8
description: 'Die folgenden vorhandenen Ressourcen wurden mit dieser Version der Adobe Workfront-API aktualisiert. Informationen zu den Ressourcen, die neu in Version 8 sind, finden Sie unter Neue Funktionen in API Version 8. Änderungen, die an einer Ressource vorgenommen werden, werden wie folgt angegeben: BEARBEITEN SIE MICH.'
author: John
feature: Workfront API
exl-id: c6d7d2d2-cd21-4ca8-a5a0-afe3669dc959
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 37%

---

# Aktualisierungen für API Version 8

## Aktualisierte Ressourcen

Die folgenden vorhandenen Ressourcen wurden mit dieser Version der Adobe Workfront-API aktualisiert. Informationen zu den Ressourcen, die neu in Version 8 sind, finden Sie unter [Neue Funktionen in API Version 8](../../wf-api/api/new-api-version-8.md). Änderungen an einer Ressource werden wie folgt angegeben:

* Hinzufügungen werden einfach aufgelistet
* Entfernungen werden mit Durchstreichen angezeigt
* Änderungen werden in der Anmerkung nach der Tabelle aufgeführt

### AccessRequest

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| Aktion¹  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Änderungen an möglichen Werten

### AccessRule¹ 

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| coreAction²  |   |   |   |   |   |   |
| forbiddenActions² |   |   |   |   |   |   |
| secondaryActions² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Markierung entfernt: REPORTABLE\
² Änderungen an möglichen Werten

### Genehmigung

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  | resourcePools |   |   |   |   |
| backlogOrder² | kanbanBoard  |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

1 Änderungen an möglichen Werten\
Überprüfungsfelder hinzugefügt: DYNAMIC, LAZY_READ und NOT_GROUPABLE

### Zuweisung

|   |   |   |   | Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnTasks | getAssignAssignmentsForTasks  |   |   |   |   |   |
|   |   |   |   | swapUsersOnTasks | getUnassignAssignmentsForTasks |   |   |   |   |   |
|   |   |   |   | unassignUserFromTasks |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Kunde

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| bizRuleExclusions¹ |   |   |   | getPackagingOptionValue |   |   |
| proofPlan¹ |   |   |   | isPackagingOptionEnabled |   |   |

{style=&quot;table-layout:auto&quot;}

1 Änderungen an möglichen Werten

### CustomerPreferences

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| name¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

1 Änderungen an möglichen Werten

### DocumentApproval

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| ID¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

1 Flag hinzugefügt: NOT_FILTERABLE

### DocumentVersion

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| activeProofStages |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Gruppe

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   | Eigentümer |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### HourType

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| appGlobalID¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

1 Flag hinzugefügt: NOT_FILTERABLE

### Wiederholung

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   |   |   | moveStories |   |   |

{style=&quot;table-layout:auto&quot;}

### Gefällt mir

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Notiz

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| auditType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

1 Änderungen an möglichen Werten

### OpTask

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  |   |   |   | defaultShownTimesheetIssues  |   |
| backlogOrder | iteration |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| Schätzung |   |   |   |   |   |   |
| iterationID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

1 Änderungen an möglichen Werten

### Portfolio

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| auditTypes¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

1 Änderungen an möglichen Werten

### Programm

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| auditTypes¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

1 Änderungen an möglichen Werten

### Projekt

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| auditTypes¹ |   | resourcePools |   |   | defaultShownTimesheetProjects |   |

{style=&quot;table-layout:auto&quot;}

1 Änderungen an möglichen Werten

### TestversandApproval

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| approveID | Genehmiger |   |   |   |   |   |
| documentVersionID | documentVersion |   |   |   |   |   |
| ID¹ |   |   |   |   |   |   |
| proofCreationDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

1 Flag hinzugefügt: NOT_FILTERABLE

### QueueDef

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| requestorCoreAction¹ |   |   |   |   |   |   |
| requestorForbiddenActions¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

1 Änderungen an möglichen Werten

### Satz

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| endDate |   |   |   | setRatesForRole  |   |   |
| name |   |   |   |   |   |   |
| startDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### ReservedTime

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| extRefID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### ResourceManager

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| projectPriority |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Aufgabe

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  |   |   |   | allTasksOnIterations  |   |
| backlogParent | kanbanBoard |   |   |   | defaultShownTimesheetTasks |   |
| kanbanBoardID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

1 Änderungen an möglichen Werten

### Team

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| agileMethodology |   |   |   |   |   |   |
| autoAddNextStory |   |   |   |   |   |   |
| includeIssues |   |   |   |   |   |   |
| teamStoryBoardIssueStatuses |   |   |   |   |   |   |
| wipLimit |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Vorlage

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### TemplateTask

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| auditTypes¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

1 Änderungen an möglichen Werten

Aktualisieren

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| updateType¹ | `updateEndorsement` |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

1 Änderungen an möglichen Werten

### Benutzer

|   |   | Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |   |   |
|   |   | userGroups |   |   |   |   |   |   |
|   |   | userRoles |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### UserNote

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |
| `endorsementShareID` | `endorsementShare` |   |   |   |   |   |
| eventType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

1 Änderungen an möglichen Werten

### Arbeit

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  |   |   |   |   |   |
| backlogOrder² | kanbanBoard  |   |   |   |   |   |
| backlogParent  |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

1 Änderungen an möglichen Werten\
Überprüfungsfelder hinzugefügt: DYNAMIC, LAZY_READ und NOT_GROUPABLE
