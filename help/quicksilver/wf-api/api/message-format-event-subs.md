---
content-type: api
navigation-topic: api-navigation-topic
title: Ausgehendes Nachrichtenformat für Ereignisabonnements
description: Ausgehendes Nachrichtenformat für Ereignisabonnements
author: Becky
feature: Workfront API
exl-id: addcf5bc-a101-4bb0-93a6-46b4af67c848
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Ausgehendes Nachrichtenformat für Ereignisabonnements

Mit der Veröffentlichung von Adobe Workfront 2017.3 wird sich das Format für ausgehende Nachrichten für Ereignisabonnationen ändern, um eine verbesserte Leistung und eine bessere Nutzung von Ereignisabonnements für Ihre Integrationen zu ermöglichen.

## Aktualisierungen des Formats ausgehender Nachrichten

Folgende Änderungen werden am Format der ausgehenden Nachricht vorgenommen:

* Ausgehende Nachrichten enthalten den oldState und newState für eine Workfront-Ressource.

   Diese Werte zeigen die Änderungen an, die aufgrund eines Ereignisses in Workfront an einem Objekt vorgenommen wurden.

* Das Metadatenfeld eventTime wird allen ausgehenden Nachrichten hinzugefügt.

   Dieses Feld gibt in Nanosekunden und EpochSeconds den Zeitpunkt an, zu dem ein Ereignis aufgetreten ist. Verwenden Sie eventTime bei der Bestellung von Ereignissen, die von Ihrer Integration verarbeitet werden.

* Das referenzierte Feld owner:companyID in der NOTE-Ressource wird entfernt.
* Das Objekt currentVersion, auf das verwiesen wird. Die DOCU (Document)-Ressource wird entfernt.

Wenn Sie derzeit Workfront-Ereignisabonnements verwenden, müssen Sie Ihre Workfront-Integrationen vor der Version 2017.3 aktualisieren, um diese Änderungen zu berücksichtigen.

Weitere Informationen zu Ereignisanmeldungen finden Sie unter [Ereignisabonnement-API](../../wf-api/general/event-subs-api.md).

## Beispiele für alte und neue Nachrichtenformate

Die folgende CREATE-Meldung im alten Format wird nach Version 2017.3 nicht mehr verwendet:

```
{
  "eventType": "CREATE",
  "subscriptionId": "8a0d839d5ef32c9a015ef33064b00001",
  "fields": {
     "ID": "59d7db3c0000014b05536251b669a3e4",
     "name": "EventSub Test 53350c27-ce58-40e9-af75-a2d45ff13046",
     "objCode": "PROJ",
     "entryDate": "2017-10-06T13:36:28.722-0600",
     "accessorIDs": ["544820df0000142362741fc0c368de19"],
     "lastUpdateDate": "2017-10-06T13:36:28.785-0600",
     "groupID": "544820df0000140f6a9c1faa7cacadd3",
     "sponsorID": null,
     "description": null,
     "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
     "enteredByID": "544820df0000142362741fc0c368de19",
     "ownerID": "544820df0000142362741fc0c368de19",
     "templateID": null,
     "priority": 0,
     "companyID": null,
     "portfolioID": null,
     "referenceNumber": 1891,
     "lastUpdatedByID": "544820df0000142362741fc0c368de19",
     "customerID": "544820df0000135b7719dcca654391f6",
     "currency": null,
     "categoryID": null,
     "status": "CUR",
     "parameterValues": {}
  }
}
```

Die folgende neue CREATE-Meldung wird nach der Version 2017.3 verwendet:

```
{
   "eventType": "CREATE",
   "subscriptionId": "8a0d839d5ef32c9a015ef32e2cde0000",
   "eventTime": {
      "nano": 414000000,
      "epochSecond": 1507318444
   },
   "newState": {
     "ID": "59d7daab0000011b8faebf0f60d25d08",
     "name": "EventSub Test 3700e224-0ef7-4571-b200-09109712152c",
     "objCode": "PROJ",
     "entryDate": "2017-10-06T13:34:03.562-0600",
     "accessorIDs": ["544820df0000142362741fc0c368de19"],
     "lastUpdateDate": "2017-10-06T13:34:04.000-0600",
     "groupID": "544820df0000140f6a9c1faa7cacadd3",
     "sponsorID": null,
     "description": null,
     "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
     "enteredByID": "544820df0000142362741fc0c368de19",
     "ownerID": "544820df0000142362741fc0c368de19",
     "templateID": null,
     "priority": 0,
     "companyID": null,
     "portfolioID": null,
     "referenceNumber": 1890,
     "lastUpdatedByID": "544820df0000142362741fc0c368de19",
     "customerID": "544820df0000135b7719dcca654391f6",
     "currency": null,
     "categoryID": null,
     "status": "CUR",
     "parameterValues": {}
   },
   "oldState": {}
```

Die folgende UPDATE-Meldung im alten Format wird nach Version 2017.3 nicht mehr verwendet:

```
{
     "eventType": "UPDATE",
     "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
     "fields": {
     "ID": "59d7dcde000001b2330bda8ac63fee16",
     "name": "EventSub Test updated",
     "objCode": "PROJ",
     "entryDate": "2017-10-06T13:43:26.305-0600",<
     "accessorIDs": [
        "544820df0000142362741fc0c368de19"
     ],
     "lastUpdateDate": "2017-10-06T13:43:49.265-0600",
     "groupID": "544820df0000140f6a9c1faa7cacadd3",
     "sponsorID": null,
     "description": null,
     "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
     "enteredByID": "544820df0000142362741fc0c368de19",
     "ownerID": "544820df0000142362741fc0c368de19",
     "templateID": null,
     "priority": 0,
     "companyID": null,
     "portfolioID": null,
     "referenceNumber": 1892,
     "lastUpdatedByID": "544820df0000142362741fc0c368de19",
     "customerID": "544820df0000135b7719dcca654391f6",
     "currency": null,
     "categoryID": null,
     "status": "CUR",
     "parameterValues": {}
   }
 }
```

Die folgende UPDATE-Meldung im neuen Format wird nach Version 2017.3 verwendet:

```
{
   "eventType": "UPDATE",
   "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
   "eventTime": {
     "nano": 998000000,
     "epochSecond": 1507319336
   },
   "newState": {
     "ID": "59d7ddf7000002322d791eb08bafddfb",
     "name": "EventSub Test updated",
     "objCode": "PROJ",
     "entryDate": "2017-10-06T13:48:07.776-0600",
     "accessorIDs": [
        "544820df0000142362741fc0c368de19"
     ],
     "lastUpdateDate": "2017-10-06T13:48:56.980-0600",
     "groupID": "544820df0000140f6a9c1faa7cacadd3",
     "sponsorID": null,
     "description": null,
     "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
     "enteredByID": "544820df0000142362741fc0c368de19",
     "ownerID": "544820df0000142362741fc0c368de19",
     "templateID": null,
     "priority": 0,
     "companyID": null,
     "portfolioID": null,
     "referenceNumber": 1894,
     "lastUpdatedByID": "544820df0000142362741fc0c368de19",
     "customerID": "544820df0000135b7719dcca654391f6",
     "currency": null,
     "categoryID": null,
     "status": "CUR",
     "parameterValues": {}
  },
  "oldState": {
     "ID": "59d7ddf7000002322d791eb08bafddfb",
     "name": "EventSub Test 180fd595-63fb-4fa9-bd47-58bf6e53d964",
     "objCode": "PROJ",
     "entryDate": "2017-10-06T13:48:07.776-0600",
     "accessorIDs": [
        "544820df0000142362741fc0c368de19"
     ],
     "lastUpdateDate": "2017-10-06T13:48:07.792-0600",
     "groupID": "544820df0000140f6a9c1faa7cacadd3",
     "sponsorID": null,
     "description": null,
     "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
     "enteredByID": "544820df0000142362741fc0c368de19",
     "ownerID": "544820df0000142362741fc0c368de19"
     "templateID": null,
     "priority": 0,
     "companyID": null,
     "portfolioID": null,
     "referenceNumber": 1894,
     "lastUpdatedByID": "544820df0000142362741fc0c368de19",
     "customerID": "544820df0000135b7719dcca654391f6",
     "currency": null,
     "categoryID": null,
     "status": "CUR",
     "parameterValues": {}
  }
}
```
