---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Dokument oder Ordner löschen
description: Dokument oder Ordner löschen
author: Becky
feature: Workfront API
role: Developer
exl-id: b56ec13a-1ee1-4bef-b39b-e625d00e4952
source-git-commit: 48de4553478fc42d88d81ea953440337f6684e50
workflow-type: tm+mt
source-wordcount: '84'
ht-degree: 4%

---


# Dokument oder Ordner löschen (noch nicht implementiert)

Löscht ein Dokument oder einen Ordner mit der angegebenen ID im externen System. Beim Löschen eines Ordners werden auch die Ordnerinhalte gelöscht.

## URL

PUT/Löschen

## Abfrageparameter

| -Name  | Beschreibung |
|---|---|
| documentId  | Die zu löschende Dokument-ID |
| folderId  |  Die zu löschende Ordner-ID |



## Antwort

Eine JSON-Zeichenfolge, die Erfolg oder Fehler anzeigt, wie im Abschnitt Fehlerbehandlung unten angegeben.

### Beispiel

PUT https://www.example.com/api/delete­­­­­­­­­­­­­­­­­­­­­­­­­­­­­id=1234
* Gibt `status: "success"`

* Gibt `status: "failure", error: "File not found"`
