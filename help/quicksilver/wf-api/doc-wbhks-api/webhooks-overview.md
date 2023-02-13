---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: Webhooks-Übersicht
description: Webhooks-Übersicht
author: John
feature: Workfront API
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
source-git-commit: a62ae524f922326811423cd17d0656920b7cc9d3
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---


# Webhooks-Übersicht

Adobe Workfront Document Webhooks definiert eine Reihe von API-Endpunkten, über die Workfront autorisierte API-Aufrufe an einen externen Dokumentanbieter sendet. Dadurch kann jeder ein Middleware-Plugin für jeden Dokumentenspeicher erstellen.

![](assets/mceclip0-350x262.png)

Das Benutzererlebnis für webhook-basierte Integrationen ähnelt dem der vorhandenen Dokumentenintegrationen wie Google Drive, Box und Dropbox. Ein Workfront-Benutzer kann beispielsweise die folgenden Aktionen durchführen:

* Navigieren zur Ordnerstruktur des externen Dokumentanbieters
* Suchdateien
* Verknüpfen von Dateien in Workfront
* Hochladen von Dateien in den externen Dokumentanbieter
* Anzeigen einer Miniaturansicht für das Dokument

**Referenzimplementierung**

Um die Entwicklung einer neuen Webhooks-Implementierung zu beschleunigen, stellt Workfront eine Referenzimplementierung bereit. Der Code dafür finden Sie unter [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app) . Diese Implementierung ist Java-basiert und ermöglicht es Workfront, Dokumente in einem Netzwerkdateisystem zu verbinden. 

## Versionen

* Version 1.0 (Releasedatum - Mai 2015): Erstspezifikation

* Version 1.1 (Veröffentlichungsdatum - Juni 2015). Aktualisiert /uploadInit - documentId und documentVersionId hinzugefügt

* Version 1.2 (Veröffentlichungsdatum - Oktober 2015): /createFolder hinzugefügt

* Bevorstehende Versionen (Veröffentlichungsdatum - TBD):

   * /delete hinzugefügt
   * /rename hinzugefügt
   * /serviceInfo hinzugefügt
   * /customAction hinzugefügt
   * Fügen Sie pagination und parentId zu /search hinzu
