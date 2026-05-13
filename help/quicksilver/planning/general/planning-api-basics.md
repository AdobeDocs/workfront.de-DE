---
title: Grundlagen zur Adobe Workfront-Planungs-API
description: Das Ziel der Adobe Workfront Planning-API besteht darin, die Erstellung von Integrationen mit Planning zu vereinfachen, indem eine REST-ful-Architektur eingeführt wird, die über HTTP ausgeführt wird. In diesem Dokument wird davon ausgegangen, dass Sie mit REST- und JSON-Antworten vertraut sind, und der von der Planungs-API verfolgte Ansatz beschrieben.
author: Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: afb58d04-fa75-4eb7-9c19-2a8c1748fbc2
source-git-commit: c3d34c4b33164f5fe5b4420f3ddc81f3390abbf1
workflow-type: tm+mt
source-wordcount: '1079'
ht-degree: 14%

---


# Grundlagen zur Adobe Workfront-Planung-API

{{planning-important-intro}}

<!--
Lilit asked me to hide everything in this current article and replace it with her version of it. I kept just the Field type and search modifier section. The rest of the article is a re-write of the original from Lilit. 

She also said we need to reword how we organize the version features, after we get more versions released but for now, she calls out what's different in V1 than the current (V2) with almost every feature. 
-->

<!--
To comment out when we release V2: 

# Adobe Workfront Planning API Basics

The goal of the Adobe Workfront Planning API is to simplify building integrations with Planning by introducing a RESTful architecture that operates over HTTP. This document assumes you are familiar with REST and JSON responses.

For complete endpoint reference, request/ response schemas, and version-specific details, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning).

>[!NOTE]
>
>When using the Planning API, all user-related information is returned using the Adobe Identity Management System (IMS) user ID, not the Workfront user ID. (*************checking with Lilit because this changed in V2**************)


## Authentication

The Workfront Planning API uses the same authentication model as the Workfront API. All organizations on the Adobe Business Platform authenticate via OAuth2.

We support the following two flows:

* **Server-to-server authentication (JWT)**: For automated integrations and backend services. 

    For information, see [Configure and use your organization's custom OAuth 2 applications using JWT flow](/help/quicksilver/wf-api/api/oauth-app-jwt-flow.md).

* **User authentication (Authorization Code flow)**: For integrations acting on behalf of a specific user. 

    For information, see [Configure and use your organization's custom OAuth 2 applications using JWT flow](/help/quicksilver/wf-api/api/oauth-app-jwt-flow.md).

To set up credentials, create an OAuth2 application in Workfront. 

For information, see [Create OAuth2 applications for Workfront integrations](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md). 

>[!NOTE]
>
>The `/login` endpoint and API key authentication are not supported for Workfront Planning. Do not use `sessionID` or `apiKey` parameters.


## API versioning

The Planning API is versioned via the URL path. 

The following are current supported versions: 

| Version   | Release date   |
|-----------|----------------|
| Version 1 | July 2024 |
| Version 2 | May 2026   |

(*****************add deprecation date column above, when we have one*****************)


For more information about the current supported versions, see the article [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning).

We recommend explicitly targeting a version in all integrations:

```
https://{customer-domain}/maestro/api/v2/...

```

When a new major version is released, the previous version will continue to be available until a deprecation date is communicated.

Follow the Workfront release notes to stay informed of API changes.


## URL structure and operations

Objects are manipulated by sending an HTTP request to their unique URI. The operation is specified by the HTTP method.

| Method   | Operation                                                            |
|----------|----------------------------------------------------------------------|
| GET      | Retrieve a single object by ID, or search/list objects               |
| POST     | Create a new object                                                  |
| PUT      | Replace an existing object (full update)                             |
| PATCH    | Partially update an existing object (only provided fields are modified) |
| DELETE   | Delete an object                                                     |

>[!NOTE]
>
>**V1 note:** `PATCH` is not supported in Version 1. Use `PUT` for all updates.


For full endpoint paths and request/response examples, see the **API reference** at [developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning).

## HTTP status codes

The Planning API returns standard HTTP status codes:

| Code                   | Meaning                                         |
|------------------------|-------------------------------------------------|
| 200 OK                 | Successful GET, PUT, or PATCH                   |
| 201 Created            | Successful POST (resource created)              |
| 204 No Content         | Successful DELETE                               |
| 400 Bad Request        | Invalid request — see error response for details |
| 401 Unauthorized       | Missing or invalid authentication token         |
| 403 Forbidden          | Authenticated but insufficient permissions      |
| 404 Not Found          | Resource does not exist                         |
| 429 Too Many Requests  | Rate limit exceeded                             |

>[!NOTE]
>
>**V1 note:** Version 1 returns `200 OK` for all successful operations, including POST and DELETE.


## Error handling

The Planning API returns errors in a consistent format. Each error response includes a human-readable message, a machine-readable error code, and a request ID for support escalation.

Example error response:

```
json
{
  "title": "Validation failed",
  "status": 400,
  "detail": "Request validation failed. See 'errors' for details.",
  "errorCode": "VALIDATION_FAILED",
  "requestId": "req-123",
  "errors": [
    { "field": "name", "message": "must not be blank" }
  ]
}

```

Use `errorCode` (not `status`) to drive programmatic error handling. It provides the most specific classification of the failure.

>[!NOTE]
>
>**V1 note:** Version 1 error responses use a numeric `type` field (e.g. `40001`) instead of a string `errorCode`, and wrap detail in a `report` object rather than a top-level `detail` field.

## Filtering records

Use the `filter` parameter in record search requests to return only records matching specific criteria. Filters use a typed composite structure with explicit logical operators:

```
json
{
  "filter": {
    "operator": "AND",
    "conditions": [
      { "fieldId": "<fieldId>", "condition": "IS", "value": "Active" },
      { "fieldId": "<fieldId>", "condition": "CONTAINS", "value": "marketing" }
    ]
  }
}

```

Filters can be nested using `AND` / `OR` operators to build compound conditions:

```
json
{
  "filter": {
    "operator": "OR",
    "conditions": [
      {
        "operator": "AND",
        "conditions": [
          { "fieldId": "<fieldId>", "condition": "BETWEEN", "value": ["2024-03-31T20:00:00.000Z", "2024-04-01T20:00:00.000Z"] },
          { "fieldId": "<fieldId>", "condition": "IS", "value": "active" }
        ]
      },
      {
        "operator": "AND",
        "conditions": [
          { "fieldId": "<fieldId>", "condition": "BETWEEN", "value": ["2024-04-15T00:00:00.000Z", "2024-04-16T00:00:00.000Z"] },
          { "fieldId": "<fieldId>", "condition": "IS", "value": "planned" }
        ]
      }
    ]
  }
}

```

>[!NOTE]
>
>**V1 note:** Version 1 uses Mongo-style untyped operators in a `filters` object. Operators are prefixed with `$` (e.g. `$and`, `$or`, `$is`, `$contains`, `$isBetween`). Pagination parameters (`offset`, `limit`) and `recordTypeId` are passed in the request body rather than as URL path and query parameters.


## Field types and search modifiers

You can use modifiers and filters with fields to control what data will be returned in results. 

For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).

### Using search modifiers 

Workfront Planning supports the following search modifiers: 

<table>
    <tr>
        <td><b>Modifier</b></td>
        <td><b>Example</b></td>
        <td><b>Description</b></td>
        <td><b>Possible Values</b></td>
    </tr>
    <tr>
        <td>$contains </td>
        <td><code>"fieldId": { "$contains": "product" } </code> </td>
        <td>Returns records whose field value contains the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$doesNotContain</td>
        <td><code>"fieldId": { "$doesNotContain": "product" } </code> </td>
        <td>Returns records where the field value does not contain the filter  </td>
        <td>"New Launch"  </td>
    </tr>
    <tr>
        <td>$is </td>
        <td><ul><li><code>"fieldId" : { "$is": "new product launch" } </code></li><li><code>"fieldId" : { "new product launch" } </code></li><ul> </td>
        <td>Returns records whose field value exactly match the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$isNot </td>
        <td><code>"fieldId": { "$isNot": "product" } </code> </td>
        <td>Returns records whose field value exactly is not match the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$isEmpty </td>
        <td><ul><li><code>"fieldId": "$isEmpty" </code></li><li><code>"fieldId": { "$isEmpty": null } </code></li><ul> </td>
        <td>Returns records whose field value is empty  </td>
        <td><ul><li>"" </li><li>null </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotEmpty </td>
        <td><ul><li><code>"fieldId": "$isNotEmpty"  </code></li><li><code>"fieldId": { "$isNotEmpty": null } </code></li><ul> </td>
        <td>Returns records whose field value is not empty  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$greaterThan </td>
        <td><code>"fieldId": { "$greaterThan": 10 } </code> </td>
        <td>Returns records whose field value is greater than the filter  </td>
        <td><ul><li>20</li><li>25</li><ul> </td>
    </tr>
    <tr>
        <td>$greaterThanOrEqual </td>
        <td><code>"fieldId": { "$greaterThanOrEqual": 10 } </code> </td>
        <td>Returns records whose field value is greater than or equal the filter  </td>
        <td><ul><li>10</li><li>20</li><li>25</li> </ul></td>
    </tr>
    <tr>
        <td>$lessThan </td>
        <td><code>"fieldId": { "$lessThan": 10 } </code> </td>
        <td>Returns records whose field value is less than the filter  </td>
        <td><ul><li>5</li><li>9</li></td></ul> 
    </tr>
    <tr>
        <td>$lessThanOrEqual </td>
        <td><code>"fieldId": { "$lessThanOrEqual": 10 } </code> </td>
        <td>Returns records whose field value is less than or equal the filter </td>
        <td><ul><li>5</li><li>9</li><ul><li>10</li> </td>
    </tr>
    <tr>
        <td>$isAfter </td>
        <td><code>"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Returns records whose field value is after the filter  </td>
        <td>"2024-05-15T20:00:00.000Z"  </td>
    </tr>
    <tr>
        <td>$isBefore </td>
        <td><code>"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Returns records whose field value is before the filter </td>
        <td>"2024-05-12T20:00:00.000Z" </td>
    </tr>
    <tr>
        <td>$isBetween </td>
        <td><code>"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Returns records whose field value is between the filter  </td>
        <td><ul><li>"2024-05-12T20:00:00.000Z" </li><li>"2024-05-14T20:00:00.000Z" </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotBetween </td>
        <td><code>"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Returns records whose field value is not between the filter  </td>
        <td><ul><li>"2024-05-09T20:00:00.000Z"  </li><li>"2024-05-17T20:00:00.000Z"  </li><ul>  </td>
    </tr>
    <tr>
        <td>$isAnyOf </td>
        <td><code>"fieldId": { "$isAnyOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is any of the filter  </td>
        <td><ul><li>"active" </li><li>"completed" </li><ul> </td>
    </tr>
    <tr>
        <td>$isNoneOf </td>
        <td><code>"fieldId": { "$isNoneOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is none of the filter </td>
        <td><ul><li>"finished"  </li><li>"fixed"  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAnyOf </td>
        <td><code>"fieldId": { "$hasAnyOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has any of the filter  </td>
        <td><ul><li>["active", "fixed"]  </li><li>["fixed", "completed", "finished"]  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAllOf </td>
        <td><code>"fieldId": { "$hasAllOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has all of the filter  </td>
        <td><ul><li>["active", "completed"]   </li><li>["active", "completed", "finished"]   </li><ul> </td>
    </tr>
    <tr>
        <td>$hasNoneOf </td>
        <td><code>"fieldId": { "$hasNoneOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has none of the filter </td>
        <td>["fixed", "finished"]  </td>
    </tr>
    <tr>
        <td>$isExactly </td>
        <td><code>"fieldId": { "$isExactly": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is exactly the filter  </td>
        <td>["active", "completed"]  </td>
    </tr>
</table>
 
### Field types 

Below is the list of supported field types and what search modifiers can be used with each of those field types  

| Field Type | Supported search modifiers |
|---|---|
| text |$contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| long-text | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| number | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| percentage | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| currency | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| date | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| single-select | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| multi-select | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| boolean | $is |
| user | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| formula | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| url | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| created-by | $is, $isNot, $isAnyOf, $isNoneOf |
| created-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween |
| updated-by | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| updated-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| reference | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| lookup | Depends on the linked field |

## Supported filter conditions by field type

| Field Type                  | Supported Conditions                                                                                         |
|-----------------------------|--------------------------------------------------------------------------------------------------------------|
| text, long-text             | CONTAINS, DOES_NOT_CONTAIN, IS, IS_NOT, IS_EMPTY, IS_NOT_EMPTY                                              |
| number, percentage, currency| IS, IS_NOT, GREATER_THAN, GREATER_THAN_OR_EQUAL, LESS_THAN, LESS_THAN_OR_EQUAL, IS_EMPTY, IS_NOT_EMPTY      |
| date                        | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN, IS_EMPTY, IS_NOT_EMPTY                         |
| single-select               | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY                                                   |
| multi-select, user          | HAS_ANY_OF, HAS_ALL_OF, IS_EXACTLY, HAS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY                                    |
| boolean                     | IS                                                                                                           |
| formula, url                | CONTAINS, DOES_NOT_CONTAIN, IS, IS_NOT, IS_EMPTY, IS_NOT_EMPTY                                              |
| created-by, updated-by      | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF                                                                            |
| created-at, updated-at      | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN                                                 |
| reference                   | HAS_ANY_OF, HAS_ALL_OF, IS_EXACTLY, HAS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY                                    |
| lookup                      | Depends on the linked field type                                                                             |

>[!NOTE]
>
>**V1 note:** Version 1 uses `$`-prefixed operator names (e.g. `$contains`, `$greaterThan`, `$isAnyOf`, `$hasAllOf`). The set of supported conditions per field type is the same.

## Sorting

Sort results by any field by including a `sort` array in your request:

```
json
{
  "sort": [
    { "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" },
    { "fieldId": "F658afcbd4a0273c67c346fd5", "direction": "desc" }
  ]
}

```

Multiple sort fields are evaluated in order. Always apply a sort when paginating to ensure consistent ordering across pages.

>[!NOTE]
>
>**V1 note:** The array key is `sorting` in Version 1, not `sort`.


---

## Field projection

To limit which fields are returned in a response, use the `fieldIds` or `fieldAliases` query parameters with a comma-separated list. This reduces response payload size and is recommended for high-volume or latency-sensitive integrations.

>[!NOTE]
>
>**V1 note:** Version 1 uses `?attributes=` for projection (e.g. `?attributes=data,createdBy`) rather than `?fieldIds=` or `?fieldAliases=`.

## Pagination

The Planning API supports paginated responses to manage large datasets.

* **Cursor-based pagination** is used for workspace and record type listings. Pass a cursor value from the previous response to retrieve the next page.
* **Page-based pagination** is used for record search. Use `page` and `size` as query parameters.

All paginated responses include a structured envelope indicating whether more results are available. Always apply a sort when paginating to ensure consistent ordering across pages.

>[!NOTE]
>
> **V1 note:** Version 1 uses `offset` and `limit` passed in the request body, with a default of 500 results and a maximum of 2,000. The response is a flat array with a `totalCount` field rather than a structured envelope.

## Bulk operations

The Planning API supports bulk create, update, patch, and delete of records in a single request. Refer to the **API reference** at [developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning) for endpoint paths, request formats, and per-operation record limits.

>[!NOTE]
>
>**V1 note:** Bulk operations are not available in Version 1.


## Permissions

Resource permissions are managed through a dedicated Permissions API, separate from the resource endpoints themselves. This allows you to read current permissions, manage workspace or record type members, and handle access requests independently of data operations. For more information, see the "API references" section in the article [Workfront Planning API](https://developer.adobe.com/wf-planning).

>[!NOTE]
>
>**V1 note:** Version 1 does not expose a public Permissions API. Permission level is embedded directly in resource response DTOs.

## Using the Planning API with Workfront custom forms

You can call the Planning API from an External lookup field in a Workfront custom form to surface Planning data directly within Workfront objects. For more information, see [Examples of the External lookup field in a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

## Related resources

For more API-related documentation, also see the following articles:

* [Workfront Planning API](https://developer.adobe.com/wf-planning) developer documentation and reference
* [Get started with Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)
* [Adobe Workfront Planning access overview](/help/quicksilver/planning/access/access-overview.md)
* [Create OAuth2 applications for Workfront integrations](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)

-->

Das Ziel der Adobe Workfront Planning-API besteht darin, die Erstellung von Integrationen mit Planning zu vereinfachen, indem eine REST-ful-Architektur eingeführt wird, die über HTTP ausgeführt wird. In diesem Dokument wird davon ausgegangen, dass Sie mit REST- und JSON-Antworten vertraut sind, und der von der Planungs-API verfolgte Ansatz beschrieben.

Wenn Sie mit dem Workfront-Planungsschema vertraut sind, können Sie die Datenbankbeziehungen besser verstehen, die Sie zum Abrufen von Daten aus Workfront Planning zu Integrationszwecken verwenden können.

Sie können die Planning-API aus einem externen Suchfeld in einem benutzerdefinierten Workfront-Formular aufrufen.

Weitere Informationen zu externen Suchfeldern finden Sie unter [Beispiele für das externe Suchfeld in einem benutzerdefinierten Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

>[!NOTE]
>
>Bei Verwendung der Planning-API werden alle benutzerbezogenen Informationen mit der Adobe Identity Management System (IMS)-Benutzer-ID und nicht mit der Workfront-Benutzer-ID zurückgegeben.
>
>Weitere Informationen finden Sie unter [Verwalten von Benutzern in der Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

## Workfront Planning-API-Versionen

* Version 1 - veröffentlicht im Juli 2024

  Weitere Informationen finden Sie im Abschnitt [Workfront Planning API Version 1](#workfront-planning-api-version-1) dieses Artikels.
  <!--
    Maybe retitle the "Workfront Planning API" section below to "Workfront Planning API Version 1" when Version 2 releases
    -->

<!--
* Version 2 - released in May 2026

    For more information, see the section [Workfront Planning API Version 2](#workfront-planning-api-version-2) in this article.
-->

## Workfront Planning-API, Version 1

Workfront Planning API Version 1 wurde im Juli 2024 veröffentlicht.

In den folgenden Abschnitten werden Funktionen beschrieben, die in der Workfront-API Version 1 verfügbar gemacht wurden.

Sofern nicht anders angegeben, enthalten alle zukünftigen API-Versionen dieselbe Funktionalität.

<!--
Becky had put the title of this article as"Workfront Planning API URL", but she did not document what that URL is; asking dev and hiding it for now
-->

<!--
For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).
-->

### Vorgänge

Objekte werden durch Senden einer HTTP-Anfrage an den eindeutigen URI bearbeitet. Der auszuführende Vorgang wird durch die HTTP-Methode angegeben.

Die standardmäßigen HTTP-Methoden entsprechen den folgenden Vorgängen:

* **GET** - Ruft ein Objekt nach ID ab und sucht anhand einer Abfrage nach allen Objekten
* **POST**: Fügt ein neues Objekt ein
* **PUT**: Bearbeitet ein vorhandenes Objekt
* **DELETE**: Löscht ein Objekt

Weitere Details und Beispiele für jeden Vorgang finden Sie in der Entwicklerdokumentation zur [Workfront Planning API](https://developer.adobe.com/wf-planning/).

### Feldtypen und Suchmodifikatoren, die mit ihnen verwendet werden

Sie können Modifikatoren und Filter mit Feldern verwenden, um zu steuern, welche Daten in den Ergebnissen zurückgegeben werden.

<!--For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

#### Verwenden von Suchmodifikatoren

Workfront Planning unterstützt die folgenden Suchmodifikatoren:

<table>
    <tr>
        <td><b>Modifikator</b></td>
        <td><b>Beispiel</b></td>
        <td><b>Beschreibung</b></td>
        <td><b>Mögliche Werte</b></td>
    </tr>
    <tr>
        <td>$contains </td>
        <td><code>"fieldId": { "$contains": "product" } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert den Filter enthält  </td>
        <td>„Neue Produkteinführung“  </td>
    </tr>
    <tr>
        <td>$doesNotContains</td>
        <td><code>"fieldId": { "$doesNotContain": "product" } </code> </td>
        <td>Gibt Datensätze zurück, bei denen der Feldwert den Filter nicht enthält  </td>
        <td>„Neue Einführung“  </td>
    </tr>
    <tr>
        <td>$is </td>
        <td><ul><li><code>"fieldId" : { "$is": "new product launch" } </code></li><li><code>"fieldId" : { "new product launch" } </code></li><ul> </td>
        <td>Gibt Datensätze zurück, deren Feldwert genau mit dem Filter übereinstimmt  </td>
        <td>„Neue Produkteinführung“  </td>
    </tr>
    <tr>
        <td>$isNot </td>
        <td><code>"fieldId": { "$isNot": "product" } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert genau nicht mit dem Filter übereinstimmt  </td>
        <td>„Neue Produkteinführung“  </td>
    </tr>
    <tr>
        <td>$isEmpty </td>
        <td><ul><li><code>"fieldId": "$isEmpty" </code></li><li><code>"fieldId": { "$isEmpty": null } </code></li><ul> </td>
        <td>Gibt Datensätze zurück, deren Feldwert leer ist  </td>
        <td><ul><li>"" </li><li>null </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotEmpty </td>
        <td><ul><li><code>"fieldId": "$isNotEmpty"  </code></li><li><code>"fieldId": { "$isNotEmpty": null } </code></li><ul> </td>
        <td>Gibt Datensätze zurück, deren Feldwert nicht leer ist  </td>
        <td>„Neue Produkteinführung“  </td>
    </tr>
    <tr>
        <td>$größer als </td>
        <td><code>"fieldId": { "$greaterThan": 10 } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert größer als der Filter ist  </td>
        <td><ul><li>20</li><li>25</li><ul> </td>
    </tr>
    <tr>
        <td>$größeralsOderGleich </td>
        <td><code>"fieldId": { "$greaterThanOrEqual": 10 } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert größer oder gleich dem Filter ist.  </td>
        <td><ul><li>10</li><li>20</li><li>25</li> </ul></td>
    </tr>
    <tr>
        <td>$kleiner als </td>
        <td><code>"fieldId": { "$lessThan": 10 } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert kleiner als der Filter ist  </td>
        <td><ul><li>5</li><li>9</li></td></ul> 
    </tr>
    <tr>
        <td>$lessThanOrEqual </td>
        <td><code>"fieldId": { "$lessThanOrEqual": 10 } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert kleiner oder gleich dem Filter ist. </td>
        <td><ul><li>5</li><li>9</li><ul><li>10</li> </td>
    </tr>
    <tr>
        <td>$isAfter </td>
        <td><code>"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert nach dem Filter liegt.  </td>
        <td>„2024-05-15T20:00:00.000Z“  </td>
    </tr>
    <tr>
        <td>$isBefore </td>
        <td><code>"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert vor dem Filter liegt. </td>
        <td>„2024-05-12T20:00:00.000Z“ </td>
    </tr>
    <tr>
        <td>$isBetween </td>
        <td><code>"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert zwischen dem Filter liegt.  </td>
        <td><ul><li>„2024-05-12T20:00:00.000Z“ </li><li>„2024-05-14T20:00:00.000Z“ </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotBetween </td>
        <td><code>"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert nicht zwischen den Filtern liegt  </td>
        <td><ul><li>„2024-05-09T20:00:00.000Z“  </li><li>„2024-05-17T20:00:00.000Z“  </li><ul>  </td>
    </tr>
    <tr>
        <td>$isAnyOf </td>
        <td><code>"fieldId": { "$isAnyOf": ["active", "completed"] } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert einer der Filter ist  </td>
        <td><ul><li>„Aktiv“ </li><li>„Abgeschlossen“ </li><ul> </td>
    </tr>
    <tr>
        <td>$isNoneOf </td>
        <td><code>"fieldId": { "$isNoneOf": ["active", "completed"] } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert keiner der Filter ist </td>
        <td><ul><li>„Fertig gestellt“  </li><li>„Behoben“  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAnyOf </td>
        <td><code>"fieldId": { "$hasAnyOf": ["active", "completed"] } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert einen der folgenden Werte aufweist:  </td>
        <td><ul><li>[„aktiv“, „fest“]  </li><li>[„behoben“, „abgeschlossen“, „abgeschlossen“]  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAllOf </td>
        <td><code>"fieldId": { "$hasAllOf": ["active", "completed"] } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert den gesamten Filter enthält  </td>
        <td><ul><li>[„Aktiv“, „Abgeschlossen“]   </li><li>[„Aktiv“, „Abgeschlossen“, „Abgeschlossen“]   </li><ul> </td>
    </tr>
    <tr>
        <td>$hasNoneOf </td>
        <td><code>"fieldId": { "$hasNoneOf": ["active", "completed"] } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert keinen Filter enthält. </td>
        <td>[„behoben“, „fertig“]  </td>
    </tr>
    <tr>
        <td>$isExactly </td>
        <td><code>"fieldId": { "$isExactly": ["active", "completed"] } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert genau dem Filter entspricht  </td>
        <td>[„Aktiv“, „Abgeschlossen“]  </td>
    </tr>
</table>

#### Feldtypen

Nachfolgend finden Sie eine Liste der unterstützten Feldtypen und darüber, welche Suchmodifikatoren mit den einzelnen Feldtypen verwendet werden können

| Feldtyp | Unterstützte Suchmodifikatoren |
|---|---|
| Text | $contains, $doesNotContainer, $is, $isNot, $isEmpty, $isNotEmpty |
| Langtext | $contains, $doesNotContainer, $is, $isNot, $isEmpty, $isNotEmpty |
| number | $is, $isNot, $größerThan, $größerThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| Prozentsatz | $is, $isNot, $größerThan, $größerThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| Währung | $is, $isNot, $größerThan, $größerThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| Datum | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| Einzelauswahl | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| Mehrfachauswahl | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| Boolescher Wert | $is |
| Benutzerin bzw. Benutzer | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| Formel | $contains, $doesNotContainer, $is, $isNot, $isEmpty, $isNotEmpty |
| URL | $contains, $doesNotContainer, $is, $isNot, $isEmpty, $isNotEmpty |
| created-by | $is, $isNot, $isAnyOf, $isNoneOf |
| created-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween |
| Aktualisiert von | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| updated-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| Verweis | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| Lookup | Hängt vom verknüpften Feld ab |

### Verwendung der Anweisungen „Und“ und „Oder“

Im API-Aufruf können Filter enthalten sein, die auf mehreren Kriterien basieren und durch $and“- und &quot;$or“-Anweisungen kombiniert werden

```
{
  "recordTypeId": "recordTypeId",
  "offset": "integer",
  "limit": "integer",
  "filters": [
    {
      "$or": [
        {
          "launch_date": {
            "$isBetween": [
              "2024-03-31T20:00:00.000Z",
              "2024-04-01T20:00:00.000Z"
            ]
          }
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-03-31T20:00:00.000Z",
                  "2024-04-01T20:00:00.000Z"
                ]
              }
            },
            {
              "status": "active"
            }
          ]
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-04-15T00:00:00.000Z",
                  "2024-04-16T00:00:00.000Z"
                ]
              }
            },
            {
              "status": "planned"
            }
          ]
        }
      ]
    }
  ]
}
```

### Verwenden des Anforderungsparameters „fields“

Mit dem Anforderungsparameter fields können Sie eine kommagetrennte Liste bestimmter Felder angeben, die zurückgegeben werden sollen. Bei diesen Feldnamen wird zwischen Groß- und Kleinschreibung unterschieden.

Beispielsweise gibt die Anfrage

`/v1/records/search?attributes=data,createdBy`

```
{
    "records": [
        {
            "id": "Rc6527ecb35df57c441d92ba00",
            "createdBy": "61a9cc0500002f9fdaa7a6f824f557e1",
            "createdAt": null,
            "updatedBy": null,
            "updatedAt": null,
            "customerId": null,
            "imsOrgId": null,
            "recordTypeId": null,
            "data": {
                "F666c0b58b6fee61a2ea6ea81": [
                    {
                        "externalId": null,
                        "id": "Rc665728ff95730b58bc757b13",
                        "value": null
                    },
..
```

eine Antwort ähnlich der folgenden zurück:


```
{ 
    "priority": 2, 
    "name": "first task", 
    "ID": "4c7c08fa0000002ff924e298ee148df4", 
    "plannedStartDate": "2010-08-30T09:00:00:000-0600" 
} 
```

### Sortieren von Abfrageergebnissen in der API

Sie können Ihre Ergebnisse nach einem beliebigen Feld sortieren, wenn Sie Folgendes an Ihren API-Aufruf anhängen:


`/v1/records/search`

Hauptteil der Anfrage:

```
{
    "recordTypeId": "Rt6527ecb25df57c441d92b9fa",
    "filters": [],
    "sorting": [
        {
            "fieldId": "F6527ecb25df57c441d92b9fc",
            "direction": "asc"
        },
        {
            "fieldId": "F658afcbd4a0273c67c346fd5",
            "direction": "desc"
        }
    ],
    "limit": 500,
    "offset": 0,
    "rowOrderViewId": "V6527ecb75df57c441d92ba03",
    "groupingFieldIds": []
}
```

### Abfragebeschränkungen und paginierte Antworten

Standardmäßig geben Planning-API-Anfragen 500 Ergebnisse zurück, beginnend mit dem Anfang der Liste. Um die standardmäßige Begrenzung für die Anzahl der Ergebnisse zu überschreiben, können Sie den `limit`-Parameter in Ihren Anfragen verwenden und auf eine andere Zahl festlegen, bis zu 2.000 Ergebnisse.

Es wird empfohlen, die Verwendung von paginierten Antworten für große Datensätze zu erwägen, indem Sie den `offset`-Parameter zu Ihren Anfragen hinzufügen. Mit paginierten Antworten können Sie den Speicherort des ersten Ergebnisses angeben, das zurückgegeben werden soll.

Wenn Sie beispielsweise die Ergebnisse 2001-4000 zurückgeben möchten, können Sie die folgende Anfrage verwenden. In diesem Beispiel werden 2.000 Datensätze im Status Aktiv zurückgegeben, beginnend mit dem Ergebnis 2001:

`POST /v1/records/search`



Hauptteil der Anfrage:

```
{ 
    "recordTypeId": "recordTypeId", 
    "offset": "2001", 
    "limit": "2000", 
    "filters": [ 
        { "status": "active" } 
    ] 
} 
```

Um sicherzustellen, dass Ihre Ergebnisse ordnungsgemäß paginiert werden, verwenden Sie einen Sortierparameter. Dadurch können die Ergebnisse in derselben Reihenfolge zurückgegeben werden, sodass die Ergebnisse bei der Paginierung nicht wiederholt oder übersprungen werden.

Weitere Informationen zum Sortieren finden Sie unter [Sortieren von Abfrageergebnissen in der API](#sorting-query-results-in-the-api) in diesem Artikel.

<!--

Lilit did not want this organized like this - keeping this for reference: 

## Workfront Planning API Version 2

Version of the Workfront Planning API was released in May 2026. 

In addition to all the information contained in Version 1, the following enhancements were added in Version 2: 

* Search by the user's Workfront ID field instead of the user's IMS ID.

    This is applicable to custom People fields, as well as system fields such as Created By and Last Updated By fields.

* Ability to search by external connections (Workfront or AEM objects) via the API.

* Ability to link cross-workspace shared records through API. 

* Support all CRUD operations for workspaces, record types, fields, and views. 

* Enable permissions sharing for all sharable entities via API. 

    This includes workspaces, record types, and views. (***********and in the future also records and fields.*********)

* Support for uploading record thumbnail through API. 

-->