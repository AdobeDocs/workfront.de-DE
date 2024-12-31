---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Dokument oder Ordner umbenennen (noch nicht implementiert)
description: Umbenennen von Dokumenten oder Ordnern
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 5b1a4a02-a7fd-41f2-9adb-74b40606270b
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '78'
ht-degree: 2%

---


# Dokument oder Ordner umbenennen (noch nicht implementiert)

Benennt ein Dokument oder einen Ordner mit der angegebenen ID im externen System um.

**URL**

PUT/Umbenennen

## Abfrageparameter

| -Name  | Beschreibung |
|---|---|
| ID | Die umzubenennende Dokument- oder Ordner-ID |
| -Name  | Der neue Name des Dokuments oder Ordners |


## Antwort

Eine JSON-Zeichenfolge, die Erfolg oder Fehler anzeigt, wie im Abschnitt Fehlerbehandlung unten angegeben.

**Beispiel:** PUT https://www.acme.com/api/rename

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
