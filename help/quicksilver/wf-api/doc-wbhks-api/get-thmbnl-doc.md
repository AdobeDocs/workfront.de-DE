---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Miniaturansicht für ein Dokument abrufen
description: Miniaturansicht für ein Dokument abrufen
author: John
feature: Workfront API
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
source-git-commit: 5cb65c3a0c3ffd374c4002867c9c48985378e03c
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
