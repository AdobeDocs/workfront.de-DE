---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Abrufen von Dokumentinhalten über Webhooks
description: Gibt die Rohbytes für ein Dokument zurück.
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '43'
ht-degree: 6%

---

# Abrufen von Dokumentinhalten über Webhooks

Gibt die Rohbytes für ein Dokument zurück.

## URL

GET/Download

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
   <td> <p>ID</p> </td> 
   <td> Die Dokument-ID.</td> 
  </tr> 
 </tbody> 
</table>

## Antwort

Die Rohbytes des Dokuments.

**Beispiel**:  `https://www.acme.com/api/download?id=123456`
