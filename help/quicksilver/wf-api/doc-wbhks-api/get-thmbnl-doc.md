---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Miniaturansicht für ein Dokument abrufen
description: Miniaturansicht für ein Dokument abrufen
author: Becky
feature: Workfront API
role: Developer
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '50'
ht-degree: 2%

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


## Reaktion

Die unformatierten Miniaturansichten.

**Beispiel:**: https://www.acme.com/api/thumbnail?id=123456
