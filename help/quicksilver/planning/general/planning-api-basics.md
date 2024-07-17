---
title: "Grundlagen der Adobe Workfront-Planungs-API"
description: Das Ziel der Adobe Workfront Planning API besteht darin, das Erstellen von Integrationen mit der Planung zu vereinfachen, indem eine REST-fähige Architektur eingeführt wird, die über HTTP ausgeführt wird. In diesem Dokument wird davon ausgegangen, dass Sie mit REST- und JSON-Antworten vertraut sind, und der von der Planungs-API verfolgte Ansatz beschrieben.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: ebdcb8ee2a6efe96c77f863e85f8911d20ab1dd4
workflow-type: tm+mt
source-wordcount: '939'
ht-degree: 2%

---


# Grundlagen der Adobe Workfront-Planungs-API

Das Ziel der Adobe Workfront Planning API besteht darin, das Erstellen von Integrationen mit der Planung zu vereinfachen, indem eine REST-fähige Architektur eingeführt wird, die über HTTP ausgeführt wird. In diesem Dokument wird davon ausgegangen, dass Sie mit REST- und JSON-Antworten vertraut sind, und der von der Planungs-API verfolgte Ansatz beschrieben.

Die Kenntnis des Workfront-Planungs-Schemas hilft Ihnen dabei, die Datenbankbeziehungen zu verstehen, die zum Abrufen von Daten aus der Workfront-Planung für Integrationszwecke genutzt werden können.

## API-URL für die Workfront-Planung

<!--For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

### Vorgänge

Objekte werden bearbeitet, indem eine HTTP-Anfrage an ihren eindeutigen URI gesendet wird. Der auszuführende Vorgang wird durch die HTTP-Methode angegeben.

Die standardmäßigen HTTP-Methoden entsprechen den folgenden Vorgängen:

* **GET** - Ruft ein Objekt nach ID ab, sucht mithilfe einer Abfrage nach allen Objekten
* **POST** - Fügt ein neues Objekt ein
* **PUT** - Bearbeiten eines vorhandenen Objekts
* **DELETE** - Löscht ein Objekt

Weitere Informationen und Beispiele zu den einzelnen Vorgängen finden Sie in der [Dokumentation zur Workfront Planning API für Entwickler](https://developer.adobe.com/wf-planning/) .

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
        <td>Gibt Datensätze aus, deren Feldwert den Filter enthält  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$doesNotContain</td>
        <td><code>"fieldId": { "$doesNotContain": "product" } </code> </td>
        <td>Gibt Datensätze aus, für die der Feldwert den Filter nicht enthält  </td>
        <td>"New Launch"  </td>
    </tr>
    <tr>
        <td>$is </td>
        <td><ul><li><code>"fieldId" : { "$is": "new product launch" } </code></li><li><code>"fieldId" : { "new product launch" } </code></li><ul> </td>
        <td>Gibt Datensätze zurück, deren Feldwert exakt mit dem Filter übereinstimmt  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$isNot </td>
        <td><code>"fieldId": { "$isNot": "product" } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert exakt nicht mit dem Filter übereinstimmt  </td>
        <td>"New Product Launch"  </td>
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
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$greaterThan </td>
        <td><code>"fieldId": { "$greaterThan": 10 } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert größer als der Filter ist  </td>
        <td><ul><li>20</li><li>25</li><ul> </td>
    </tr>
    <tr>
        <td>$greaterThanOrEqual </td>
        <td><code>"fieldId": { "$greaterThanOrEqual": 10 } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert größer oder gleich dem Filter ist  </td>
        <td><ul><li>10</li><li>20</li><ul><li>25</li> </td>
    </tr>
    <tr>
        <td>$lessThan </td>
        <td><code>"fieldId": { "$lessThan": 10 } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert kleiner als der Filter ist  </td>
        <td><ul><li>5</li><li>9</li><ul> </td>
    </tr>
    <tr>
        <td>$lessThanOrEqual </td>
        <td><code>"fieldId": { "$lessThanOrEqual": 10 } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert kleiner oder gleich dem Filter ist </td>
        <td><ul><li>5</li><li>9</li><ul><li>10</li> </td>
    </tr>
    <tr>
        <td>$isAfter </td>
        <td><code>"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert hinter dem Filter liegt  </td>
        <td>"2024-05-15T20:00:00.000Z"  </td>
    </tr>
    <tr>
        <td>$isBefore </td>
        <td><code>"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert vor dem Filter liegt </td>
        <td>"2024-05-12T20:00:00.000Z" </td>
    </tr>
    <tr>
        <td>$isBetween </td>
        <td><code>"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert zwischen dem Filter liegt  </td>
        <td><ul><li>"2024-05-12T20:00:00.000Z" </li><li>"2024-05-14T20:00:00.000Z" </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotBetween </td>
        <td><code>"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert nicht zwischen dem Filter liegt  </td>
        <td><ul><li>"2024-05-09T20:00:00.000Z"  </li><li>"2024-05-17T20:00:00.000Z"  </li><ul>  </td>
    </tr>
    <tr>
        <td>$isAnyOf </td>
        <td><code>"fieldId": { "$isAnyOf": ["active", "completed"] } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert einem der Filter entspricht  </td>
        <td><ul><li>"active" </li><li>"completed" </li><ul> </td>
    </tr>
    <tr>
        <td>$isNoneOf </td>
        <td><code>"fieldId": { "$isNoneOf": ["active", "completed"] } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert keiner der Filter ist </td>
        <td><ul><li>"finished"  </li><li>"fixed"  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAnyOf </td>
        <td><code>"fieldId": { "$hasAnyOf": ["active", "completed"] } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert einen der Filter aufweist  </td>
        <td><ul><li>["active", "fixed"]  </li><li>["fixed", "completed", "finished"]  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAllOf </td>
        <td><code>"fieldId": { "$hasAllOf": ["active", "completed"] } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert den gesamten Filter aufweist  </td>
        <td><ul><li>["active", "completed"]   </li><li>["active", "completed", "finished"]   </li><ul> </td>
    </tr>
    <tr>
        <td>$hasNoneOf </td>
        <td><code>"fieldId": { "$hasNoneOf": ["active", "completed"] } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert keinen Filter enthält </td>
        <td>["fixed", "finished"]  </td>
    </tr>
    <tr>
        <td>$isExactly </td>
        <td><code>"fieldId": { "$isExactly": ["active", "completed"] } </code> </td>
        <td>Gibt Datensätze zurück, deren Feldwert genau dem Filter entspricht  </td>
        <td>["active", "completed"]  </td>
    </tr>
</table>

#### Feldtypen

Nachstehend finden Sie eine Liste der unterstützten Feldtypen und darüber, welche Suchmodifikatoren mit jedem dieser Feldtypen verwendet werden können

| Feldtyp | Unterstützte Suchmodifikatoren |
|---|---|
| text | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| long-text | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| number | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| Prozentsatz | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| currency | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| Datum | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| Einzelauswahl | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| Mehrfachauswahl | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| Boolescher Wert | $is |
| Benutzer | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| Formel | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| url | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| created-by | $is, $isNot, $isAnyOf, $isNoneOf |
| created-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween |
| aktualisiert von | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| updated-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| reference | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| Nachschlagen | Hängt vom verknüpften Feld ab |

### Verwenden von &quot;And&quot;- und &quot;Or&quot;-Anweisungen

Im API-Aufruf können Sie Filter haben, die auf mehreren Kriterien basieren, die durch die Anweisungen $and&quot; und &quot;$or&quot;kombiniert werden

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

### Verwenden des Feldanfrageparameters

Mit dem Feldanforderungsparameter können Sie eine kommagetrennte Liste bestimmter Felder angeben, die zurückgegeben werden sollen. Bei diesen Feldnamen wird zwischen Groß- und Kleinschreibung unterschieden.

Beispielsweise die Anfrage

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

gibt eine Antwort ähnlich der folgenden zurück:


```
{ 
    "priority": 2, 
    "name": "first task", 
    "ID": "4c7c08fa0000002ff924e298ee148df4", 
    "plannedStartDate": "2010-08-30T09:00:00:000-0600" 
} 
```

### Sortieren von Abfrageergebnissen in der API

Sie können Ihre Ergebnisse nach jedem Feld sortieren, wenn Sie Folgendes an Ihren API-Aufruf anhängen:


`/v1/records/search`

Anfrageinhalt:

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

Standardmäßig geben API-Anfragen zur Planung 500 Ergebnisse zurück, beginnend mit dem Anfang der Liste. Um die Standardbegrenzung für die Anzahl der Ergebnisse zu überschreiben, können Sie den Parameter `limit` in Ihren Anforderungen verwenden und ihn auf eine andere Zahl mit bis zu 2000 Ergebnissen setzen.

Es wird empfohlen, paginierte Antworten für große Datensätze zu verwenden, indem Sie den Parameter `offset` zu Ihren Anforderungen hinzufügen. Paginierte Antworten ermöglichen es Ihnen, den Speicherort des ersten zurückzugebenden Ergebnisses anzugeben.

Wenn Sie beispielsweise die Ergebnisse 2001-4000 zurückgeben möchten, können Sie die folgende Anfrage verwenden. In diesem Beispiel werden seit dem 2001. Ergebnis 2000 Datensätze zurückgegeben, die sich im aktiven Status befinden:

`POST /v1/records/search `



Anfrageinhalt:

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

Verwenden Sie einen Sortierparameter, um sicherzustellen, dass Ihre Ergebnisse korrekt paginiert werden. Dadurch können die Ergebnisse in derselben Reihenfolge zurückgegeben werden, sodass die Paginierung die Ergebnisse nicht wiederholt oder überspringt.

Weitere Informationen zum Sortieren finden Sie unter [Sortieren von Abfrageergebnissen in der API](#sorting-query-results-in-the-api) in diesem Artikel.



