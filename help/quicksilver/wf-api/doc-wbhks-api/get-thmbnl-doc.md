---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Miniaturansicht für ein Dokument abrufen
description: Miniaturansicht für ein Dokument abrufen
author: Becky
feature: Workfront API
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 7%

---


# Miniaturansicht für ein Dokument abrufen

Gibt die unformatierten Miniaturansichten für ein Dokument zurück.

**URL**

GET /thumbnail

## Abfrageparameter

| Name  | Beschreibung |
|---|---|
| id  | Die Dokument-ID. |
| size  |  Die Breite der Miniaturansicht. |


## Antwort

Die unformatierten Bytes für Miniaturansichten.

**Beispiel:**: https://www.acme.com/api/thumbnail?id=123456
