---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Löschen eines Dokuments oder Ordners
description: Löschen eines Dokuments oder Ordners
author: Becky
feature: Workfront API
exl-id: b56ec13a-1ee1-4bef-b39b-e625d00e4952
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '82'
ht-degree: 6%

---


# Löschen eines Dokuments oder Ordners (noch nicht implementiert)

Löscht ein Dokument oder einen Ordner mit der angegebenen ID im externen System. Beim Löschen eines Ordners werden auch die Ordnerinhalte gelöscht.

## URL

PUT/Löschen

## Abfrageparameter

| Name  | Beschreibung |
|---|---|
| documentId  | Die zu löschende Dokument-ID |
| folderId  |  Die zu löschende Ordner-ID |



## Antwort

Eine JSON-Zeichenfolge, die den Erfolg oder Fehler angibt, wie im Abschnitt Umgang mit Fehlern unten angegeben.

### Beispiel

PUT https://www.example.com/api/deleteid=1234
* return `status: “success”`

* return `status: “failure”, error: “File not found”`
