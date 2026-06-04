---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Suche über Dokument-Webhooks
description: Suche über Dokument-Webhooks
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 8a3bf0c4-4a20-4311-8c05-15f4ef3a1d42
TQID: https://experienceleague.adobe.com/flRrmTOPVSGP83tVYfKG9AZOT7CNZN4IeWZNsVwcOO4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 139
ht-degree: 14%

---

# Suche über Dokument-Webhooks

Gibt Metadaten für die bei einer Suche zurückgegebenen Dateien und Ordner zurück. Dies kann als Volltextsuche oder als reguläre Datenbankabfrage implementiert werden. Adobe Workfront ruft den /search-Endpunkt auf, wenn der Benutzer eine Suche über den externen Dateibrowser durchführt.

## URL

GET/search

## Abfrageparameter

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Name </th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Abfrage</td> 
   <td>Der Suchbegriff oder die Phrase.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(optional) Die Ordner-ID, von der aus die Suche ausgeführt wurde. Hinweis: Dies ist ein Platzhalter für eine zukünftige Funktion in Workfront. Derzeit gibt Workfront diesen Parameter nicht weiter. </p> </td> 
  </tr> 
  <tr> 
   <td>max</td> 
   <td>Die maximale Anzahl an zurückzugebenden Elementen. Wird für die Paginierung verwendet.</td> 
  </tr> 
  <tr> 
   <td>Versatz</td> 
   <td> Der Seitenversatz, verwendet in Verbindung mit „max“.</td> 
  </tr> 
 </tbody> 
</table>

 

## Antwort

JSON mit einer Liste von Metadaten für Dateien und Ordner, die mit der Abfrage übereinstimmen. Was eine „Übereinstimmung“ darstellt, wird vom Webhook-Anbieter bestimmt. Idealerweise sollte dies eine Volltextsuche sein. Eine auf Dateinamen basierende Suche funktioniert ebenfalls.

**Beispiel:**

Beispiel: `https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```
