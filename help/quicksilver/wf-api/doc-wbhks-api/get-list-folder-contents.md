---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Listet Metadaten für Dateien oder Ordner auf
description: Listet Metadaten für Dateien oder Ordner auf
author: Becky
feature: Workfront API
role: Developer
exl-id: 9c9f9222-59ac-4643-8297-d4939bec7e64
TQID: https://experienceleague.adobe.com/nZv42xMbDRJbkwR-lFKI6dAbeszSzGWAwn--qkKhVVM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 101
ht-degree: 12%

---

# Abrufen der Elementliste des Ordnerinhalts

Listet Metadaten für die Dateien und Ordner für einen bestimmten Ordner auf.

**URL**

GET /files

## Abfrageparameter

| Name  | Beschreibung |
|---|---|
| parentId  | Die Ordner-ID. Um die Metadaten des Stammverzeichnisses abzurufen, verwenden Sie den Wert &quot;/&quot;. |
| max  | Die maximale Anzahl an zurückzugebenden Elementen. Wird für die Paginierung verwendet. |
| Versatz  |  Der Seitenversatz, verwendet in Verbindung mit „max“. |


## Antwort

JSON mit einer Liste von Dateien und Ordnern. Die Metadaten für jedes Element sind mit denen identisch, die vom Endpunkt /metadata zurückgegeben werden.

**Beispiel:** https://www.acme.com/api/files?parentId=123456

```
[ 
{
title:"Folder A",
kind:"folder"
id":"2lj23lkj",
viewLink:" https://www.acme.com/viewDocument?id=2lj23lkj ",
downloadLink:"https://www.acme.com/downloadDocument?id=2lj23lkj",
mimeType:"",
dateModified:"2014­06­05T17:39:45.251Z"
size: ""
},
{
title:"My Document",
kind:"file"
id":"da8cj234",
viewLink:" https://www.acme.com/viewDocument?id=da8cj234 ",
downloadLink:"https://www.acme.com/downloadDocument?id=da8cj234",
mimeType:"image/png",
dateModified:"2014­06­05T17:39:45.251Z"
size: "32554694"
}
]
```
