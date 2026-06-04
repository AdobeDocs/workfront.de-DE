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
TQID: https://experienceleague.adobe.com/AIN65ofKDJA95iMpvNwoe3oQapmyxzDC16dpf5ehwH0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 43
ht-degree: 39%

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

Die Rohbytes des Dokuments.

**Beispiel**: `https://www.acme.com/api/download?id=123456`
