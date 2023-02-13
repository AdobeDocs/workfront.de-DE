---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in API Version 9
description: Dies ist eine Liste der Ressourcen, die neu für API Version 9 sind. Um eine Liste der Aktualisierungen anzuzeigen, die an den Ressourcen von Version 9 vorgenommen wurden, besuchen Sie bitte Aktualisierungen von API Version 9.
author: John
feature: Workfront API
exl-id: 29d922f4-f4c6-45e5-b9fa-43e2068ec66d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 25%

---

# Neue Funktionen in API Version 9

## Neue Ressourcen

Dies ist eine Liste der Ressourcen, die neu für API Version 9 sind. Eine Liste der Aktualisierungen, die an den Ressourcen von Version 9 vorgenommen wurden, finden Sie unter [Aktualisierungen für API Version 9](../../wf-api/api/new-api-version-9-updates.md)

### AccessLevel

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `accessRestrictions` | `customer` | `accessLevelPermissions` |  |  |  | `ADD` |
| `customerID` | `lastUpdatedBy` | `accessRulePreferences` |  |  |  | `COPY` |
| `description` |  |  |  |  |  | `COUNT` |
| `descriptionKey` |  |  |  |  |  | `DELETE` |
| `entryDate` |  |  |  |  |  | `EDIT` |
| `extRefID` |  |  |  |  |  | `GET` |
| `fieldAccessPrivileges` |  |  |  |  |  | `REPLACE` |
| `ID` |  |  |  |  |  | `REPORT` |
| `isAdmin` |  |  |  |  |  | `SEARCH` |
| `isUnsupportedWorkerLicense` |  |  |  |  |  |   |
| `lastUpdatedByID` |  |  |  |  |  |   |
| `lastUpdatedDate` |  |  |  |  |  |  |
| `licenseType` |  |  |  |  |  |  |
| `name` |  |  |  |  |  |  |
| `nameKey` |  |  |  |  |  |  |
| `securityModelType` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### AccessLevelPermissions

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `coreAction` |  |  |  |  |  |   |
| `forbiddenActions` |  |  |  |  |  |   |
| `ID` |  |  |  |  |  |   |
| `isAdmin` |  |  |  |  |  |   |
| `objObjCode` |  |  |  |  |  |  |
| `secondaryActions` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### AccessRulePreference

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `ID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### BudgetedHour

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `allocationDate` |  |  |  |  |  | `ADD` |
| `budgetedHours` |  |  |  |  |  | `DELETE` |
| `GUID` |  |  |  |  |  | `GET` |
| `plannedBudgetedHours` |  |  |  |  |  | `SEARCH` |
| `projectID` |   |   |   |   |   |   |
| `roleID`  |   |   |   |   |   |   |
| `userID`  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### CalendarPortalSection

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `calendarInfoID` | `customer` |  | `displayDescription` |  |  | `ADD` |
| `customerID` | `enteredBy` |  | `displayName` |  |  | `COPY` |
| `enteredByID` |  |  |  |  |  | `COUNT` |
| `entryDate` |  |  |  |  |  | `GET` |
| `ID` |  |  |  |  |  | `REPORT` |
| `name` |  |  |  |  |  | `SEARCH` |
| `objID`  |   |   |   |   |   |   |
| `objObjCode`  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### CalendarSection

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `calendarID` | `customer` | `filters` |  | `getConcatenatedExpressionForm` |  | `ADD` |
| `calEvents` |  |  |  | `getPrettyExpressionForm` |  | `COUNT` |
| `color` |  |  |  |  |  | `DELETE` |
| `customerID` |  |  |  |  |  | `EDIT` |
| `duration` |  |  |  |  |  | `GET` |
| `ID` |  |  |  |  |  | `REPORT` |
| `milestone` |  |  |  |  |  | `SEARCH` |
| `name`  |   |   |   |   |   |   |
| `plannedDate` |   |   |   |   |   |   |
| `startDate` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### ExternalSection

| Felder | Verweise | Sammlungen | Suchen | Aktionen | Abfragen | Vorgänge |
|---|---|---|---|---|---|---|
| `appGlobalID` | `customer` |  | `displayDescription` | `calculateURL` |  | `ADD` |
| `calculatedURL` | `enteredBy` |  | `displayName` | `calculateURLS` |  | `COPY` |
| `customerID` | `view` |  | `linkedCustomersMM` |  |  | `COUNT` |
| `description` |  |  | `linkedUsersMM` |  |  | `DELETE` |
| `descriptionKey` |  |  |  |  |  | `EDIT` |
| `enteredByID` |  |  |  |  |  | `GET` |
| `entryDate` |  |  |  |  |  | `REPORT` |
| `extRefID` |  |  |  |  |  | `SEARCH` |
| `frame`  |   |   |   |   |   |   |
| `friendlyURL`  |   |   |   |   |   |   |
| `globalUIKey`  |   |   |   |   |   |   |
| `height`  |   |   |   |   |   |   |
| `ID`  |   |   |   |   |   |   |
| `name`  |   |   |   |   |   |   |
| `nameKey`  |   |   |   |   |   |   |
| `objID`  |   |   |   |   |   |   |
| `objInterface`  |   |   |   |   |   |   |
| `objObjCode`  |   |   |   |   |   |   |
| `scrolling` |   |   |   |   |   |   |
| `url` |   |   |   |   |   |   |
| `viewID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

Diese Liste wurde in zwei Hälften aufgeteilt. Die zweite Hälfte finden Sie unter [Neue Funktionen in API Version 9 (Fortsetzung)](../../wf-api/api/new-api-version-9-continue.md). Die Liste der Updates für Version 9 finden Sie unter [Aktualisierungen für API Version 9](../../wf-api/api/new-api-version-9-updates.md)
