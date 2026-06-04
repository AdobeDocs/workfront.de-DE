---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Abrufen einer Miniaturansicht für ein Dokument
description: Abrufen einer Miniaturansicht für ein Dokument
author: Becky
feature: Workfront API
role: Developer
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
TQID: https://experienceleague.adobe.com/-LE1gxQ9aViRNuN0sI14HlZaIcLc6Mmm8XmS1zaRCFQ
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 55
ht-degree: 47%

---

# Abrufen einer Miniaturansicht für ein Dokument

Gibt die rohen Miniaturbyte für ein Dokument zurück.

**URL**

GET/thumbnail

## Abfrageparameter

| Name  | Beschreibung |
|---|---|
| id  | Die Dokument-ID. |
| size  |  Die Breite der Miniaturansicht. |


## Antwort

Die rohen Miniaturansichten in Bytes.

**Beispiel:**: https://www.acme.com/api/thumbnail?id=123456
