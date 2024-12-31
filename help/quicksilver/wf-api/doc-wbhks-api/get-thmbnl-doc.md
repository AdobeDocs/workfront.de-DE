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
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '50'
ht-degree: 4%

---


# Abrufen einer Miniaturansicht für ein Dokument

Gibt die rohen Miniaturbyte für ein Dokument zurück.

**URL**

GET/Thumbnail

## Abfrageparameter

| -Name  | Beschreibung |
|---|---|
| ID  | Die Dokument-ID. |
| Größe  |  Die Breite der Miniaturansicht. |


## Antwort

Die rohen Miniaturansichten in Bytes.

**Beispiel:**: https://www.acme.com/api/thumbnail?id=123456
