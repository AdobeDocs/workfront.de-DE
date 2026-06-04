---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Umbenennen eines Dokuments oder eines Ordners (noch nicht implementiert)
description: Umbenennen von Dokumenten oder Ordnern
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 5b1a4a02-a7fd-41f2-9adb-74b40606270b
TQID: https://experienceleague.adobe.com/-HmJkcMckTK6upblNcqX5LZkdYQxoWPDeuHkFjJarh4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 81
ht-degree: 29%

---

# Umbenennen eines Dokuments oder eines Ordners (noch nicht implementiert)

Benennt ein Dokument oder einen Ordner mit der angegebenen ID im externen System um.

**URL**

PUT/Umbenennen

## Abfrageparameter

| Name  | Beschreibung |
|---|---|
| id | Die umzubenennende Dokument- oder Ordner-ID |
| name  | Der neue Name des Dokuments oder Ordners |


## Antwort

Eine JSON-Zeichenfolge, die Erfolg oder Fehler anzeigt, wie im Abschnitt Fehlerbehandlung unten angegeben.

**example:** PUT https://www.acme.com/api/rename

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

Rückgabe

```
{status: "success"
 }returns
 {
 status: "failure", error: "Folder cannot be renamed because a folder with that name already exists."
 }
```
