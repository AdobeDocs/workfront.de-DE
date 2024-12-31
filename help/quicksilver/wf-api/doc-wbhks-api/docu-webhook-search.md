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
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 2%

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
   <th>-Name </th> 
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
