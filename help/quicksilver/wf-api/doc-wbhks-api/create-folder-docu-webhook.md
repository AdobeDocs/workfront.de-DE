---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Erstellen eines Ordners mit Document Webhooks
description: Erstellen eines Ordners mit Document Webhooks
author: John
feature: Workfront API
exl-id: 50905915-58c9-4b50-b8a1-133833884a88
source-git-commit: 1b11a4c5f0fdf1987e9f02f7aa06ec6ec36426d3
workflow-type: tm+mt
source-wordcount: '66'
ht-degree: 7%

---


# Erstellen eines Ordners mit Document Webhooks

Erstellt einen Ordner in einem bestimmten Verzeichnis.

## URL

POST /createFolder

## Abfrageparameter

| **Name** | **Beschreibung** |
|---|---|
| parentId  | Die Ordner-ID, in der der Ordner erstellt werden soll |
| name  | Der Name des neuen Ordners |




**Reaktion**

Die Metadaten für den neu erstellten Ordner, wie vom Endpunkt /metadata definiert.

## Beispiel

```
POST https://www.acme.com/api/createFolder
­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------
parentId=1234
name=New Folder 
-------------------------------
```

return

```
{title:"New Folder",br /> kind:"folder"
 id":"5678",
 viewLink:"”,
 downloadLink:"",
 mimeType:"",
 dateModified:"2014­06­05T17:39:45.251Z"
 size: ""
 }
```
