---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Dokumentinhalte über Webhooks abrufen
description: Gibt die unformatierten Bytes für ein Dokument aus
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '53'
ht-degree: 7%

---

# Dokumentinhalte über Webhooks abrufen

Gibt die unformatierten Bytes für ein Dokument aus

## URL

GET /download

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
   <td> <p>id</p> </td> 
   <td> Die Dokument-ID.</td> 
  </tr> 
 </tbody> 
</table>

## Antwort

Die rohen Bytes des Dokuments.

**Beispiel:**:  [https://www.acme.com/api/download?id=123456](https://www.acme.com/api/download?id=123456)
