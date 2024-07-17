---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Löschen eines Dokuments oder Ordners
description: Löschen eines Dokuments oder Ordners
author: Becky
feature: Workfront API
role: Developer
exl-id: b56ec13a-1ee1-4bef-b39b-e625d00e4952
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '84'
ht-degree: 3%

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



## Reaktion

Eine JSON-Zeichenfolge, die den Erfolg oder Fehler angibt, wie im Abschnitt Umgang mit Fehlern unten angegeben.

### Beispiel

PUT https://www.example.com/api/deleteid=1234
* gibt `status: "success"` zurück

* gibt `status: "failure", error: "File not found"` zurück
