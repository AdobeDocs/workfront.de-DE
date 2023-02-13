---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Suchen über Document Webhooks
description: Suchen über Document Webhooks
author: John
feature: Workfront API, Digital Content and Documents
exl-id: 8a3bf0c4-4a20-4311-8c05-15f4ef3a1d42
source-git-commit: 338cc745a7660ffed8e4d44e19dcadfdc13bc345
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 4%

---

# Suchen über Document Webhooks

Gibt Metadaten für die Dateien und Ordner zurück, die von einer Suche zurückgegeben wurden. Dies kann als Volltextsuche oder als reguläre Datenbankabfrage implementiert werden. Adobe Workfront ruft den Endpunkt /search auf, wenn der Benutzer eine Suche über den externen Dateibrowser durchführt.

## URL

GET /search

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
   <td>Der Suchbegriff oder -ausdruck.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(optional) Die Ordner-ID, von der aus die Suche ausgeführt wurde. Hinweis: Dies ist ein Platzhalter für eine zukünftige Funktion in Workfront. Derzeit wird dieser Parameter nicht von der Arbeitsfläche übergeben. </p> </td> 
  </tr> 
  <tr> 
   <td>max</td> 
   <td>Die maximale Anzahl der zurückzugebenden Elemente. Wird für die Paginierung verwendet.</td> 
  </tr> 
  <tr> 
   <td>offset</td> 
   <td> Der Seitenversatz, der zusammen mit "max"verwendet wird.</td> 
  </tr> 
 </tbody> 
</table>

 

## Antwort

JSON mit einer Liste von Metadaten für Dateien und Ordner, die mit der Abfrage übereinstimmen. Was eine &quot;Übereinstimmung&quot;ausmacht, wird vom Webhook-Provider bestimmt. Idealerweise sollte eine Volltextsuche durchgeführt werden. Eine filename-basierte Suche funktioniert ebenfalls.

**Beispiel:**

Beispiel:  `https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```
