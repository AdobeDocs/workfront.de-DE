---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Umbenennen eines Dokuments oder Ordners (noch nicht implementiert)
description: Umbenennen eines Dokuments oder Ordners
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 5b1a4a02-a7fd-41f2-9adb-74b40606270b
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '78'
ht-degree: 1%

---


# Umbenennen eines Dokuments oder Ordners (noch nicht implementiert)

Benennt ein Dokument oder einen Ordner mit der angegebenen ID im externen System um.

**URL**

PUT /rename

## Abfrageparameter

| Name  | Beschreibung |
|---|---|
| id | Die umzubenennende Dokument- oder Ordner-ID |
| name  | Der neue Name des Dokuments oder Ordners |


## Reaktion

Eine JSON-Zeichenfolge, die den Erfolg oder Fehler angibt, wie im Abschnitt Umgang mit Fehlern unten angegeben.

**Beispiel:** PUT https://www.acme.com/api/rename

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

return

```
{status: "success"
 }returns
 {
 status: "failure", error: "Folder cannot be renamed because a folder with that name already exists."
 }
```
