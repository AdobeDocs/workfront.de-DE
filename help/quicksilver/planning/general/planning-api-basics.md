---
title: Grundlagen zur Adobe Workfront-Planungs-API
description: Das Ziel der Adobe Workfront Planning-API besteht darin, die Erstellung von Integrationen mit Planning zu vereinfachen, indem eine REST-ful-Architektur eingeführt wird, die über HTTP ausgeführt wird. In diesem Dokument wird davon ausgegangen, dass Sie mit REST- und JSON-Antworten vertraut sind, und der von der Planungs-API verfolgte Ansatz beschrieben.
author: Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: afb58d04-fa75-4eb7-9c19-2a8c1748fbc2
source-git-commit: 20e8d45264f9441d9576c7d4d5521e4f6053a7f3
workflow-type: tm+mt
source-wordcount: '973'
ht-degree: 1%

---


# Grundlagen zur Adobe Workfront Planning-API

{{planning-important-intro}}

Das Ziel der Adobe Workfront Planning-API besteht darin, die Erstellung von Integrationen mit Planning zu vereinfachen, indem eine REST-ful-Architektur eingeführt wird, die über HTTP ausgeführt wird. In diesem Dokument wird davon ausgegangen, dass Sie mit REST- und JSON-Antworten vertraut sind, und der von der Planungs-API verfolgte Ansatz beschrieben.

Wenn Sie mit dem Workfront-Planungsschema vertraut sind, können Sie die Datenbankbeziehungen besser verstehen, die Sie zum Abrufen von Daten aus Workfront Planning zu Integrationszwecken verwenden können.

Sie können die Planning-API aus einem externen Suchfeld in einem benutzerdefinierten Workfront-Formular aufrufen.

Weitere Informationen zu externen Suchfeldern finden Sie unter [Beispiele für das externe Suchfeld in einem benutzerdefinierten Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

## Workfront Planning-API-URL

<!--For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

### Vorgänge

Objekte werden durch Senden einer HTTP-Anfrage an den eindeutigen URI bearbeitet. Der auszuführende Vorgang wird durch die HTTP-Methode angegeben.

Die standardmäßigen HTTP-Methoden entsprechen den folgenden Vorgängen:

* **GET** - Ruft ein Objekt nach ID ab und sucht anhand einer Abfrage nach allen Objekten
* **POST** - Fügt ein neues Objekt ein
* **PUT** - Bearbeitet ein vorhandenes Objekt
* **DELETE** - Löscht ein Objekt

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
        <td>Gibt Datensätze zurück, deren Feldwert nicht leer ist  </td>
        <td><ul><li>„“ </li><li>null </li><ul>  </td>
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
| Zahl | $is, $isNot, $größerThan, $größerThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| Prozentsatz | $is, $isNot, $größerThan, $größerThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| Währung | $is, $isNot, $größerThan, $größerThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| Datum | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| Einzelauswahl | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| Mehrfachauswahl | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| Boolescher Wert | $is |
| Benutzer | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
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

Beispiel: die Anfrage

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
....
```

Gibt eine Antwort ähnlich der folgenden zurück:


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

Anfragetext:

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

`POST /v1/records/search `



Anfragetext:

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

Um sicherzustellen, dass Ihre Ergebnisse ordnungsgemäß paginiert werden, verwenden Sie einen Sortierparameter. Dadurch können die Ergebnisse in derselben Reihenfolge zurückgegeben werden, sodass die Paginierung die Ergebnisse nicht wiederholt oder überspringt.

Weitere Informationen zum Sortieren finden Sie unter [Sortieren von Abfrageergebnissen in der API](#sorting-query-results-in-the-api) in diesem Artikel.
