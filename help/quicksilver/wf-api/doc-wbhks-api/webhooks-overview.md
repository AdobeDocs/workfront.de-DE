---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: Webhooks-Übersicht
description: Webhooks-Übersicht
author: Becky
feature: Workfront API
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
source-git-commit: eb738fa8cadaafb0332c5c78a3816d5c346c33b2
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---


# Webhooks-Übersicht

Adobe Workfront Document Webhooks definiert eine Reihe von API-Endpunkten, über die Workfront autorisierte API-Aufrufe an einen externen Dokumentanbieter sendet. Dadurch kann jeder ein Middleware-Plugin für jeden Dokumentenspeicher erstellen.

![](assets/mceclip0-350x262.png)

Das Benutzererlebnis für webhook-basierte Integrationen ähnelt dem von vorhandenen Dokumentenintegrationen wie Google Drive, Box und Dropbox. Ein Workfront-Benutzer kann beispielsweise die folgenden Aktionen durchführen:

* Navigieren zur Ordnerstruktur des externen Dokumentanbieters
* Suchdateien
* Verknüpfen von Dateien in Workfront
* Hochladen von Dateien in den externen Dokumentanbieter
* Anzeigen einer Miniaturansicht für das Dokument

**Referenzimplementierung**

Um die Entwicklung einer neuen Webhooks-Implementierung zu beschleunigen, stellt Workfront Beispiele für eine Referenzimplementierung bereit. Diese Beispiele finden Sie unter [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). Die Beispiele sind Java-basiert und ermöglichen es Workfront, Dokumente in einem Netzwerkdateisystem zu verbinden. 

>[!NOTE]
>
>Die Ressourcen auf GitHub sind nur Beispiele und können keine Implementierung ausführen.

## Versionen

* Version 1.0 (Veröffentlichungsdatum - Mai 2015): Erstspezifikation

* Version 1.1 (Veröffentlichungsdatum - Juni 2015). Aktualisiert /uploadInit - documentId und documentVersionId hinzugefügt

* Version 1.2 (Releasedatum - Oktober 2015): /createFolder hinzugefügt

* Bevorstehende Versionen (Veröffentlichungsdatum - TBD):

   * /delete hinzugefügt
   * /rename hinzugefügt
   * /serviceInfo hinzugefügt
   * /customAction hinzugefügt
   * Hinzufügen von Pagination und parentId zu /search
