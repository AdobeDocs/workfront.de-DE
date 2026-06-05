---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: Überblick über Webhooks
description: Überblick über Webhooks
author: Becky
feature: Workfront API
role: Developer
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
TQID: https://experienceleague.adobe.com/5bBLva-jIjwc953MVjAnwo4y0nABq1N0HGDTIurXk40
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 193
ht-degree: 4%

---

# Überblick über Webhooks

Adobe Workfront Document Webhooks definiert einen Satz von API-Endpunkten, über die Workfront autorisierte API-Aufrufe an einen externen Dokumentanbieter sendet. Dadurch kann jeder ein Middleware-Plug-in für einen beliebigen Dokumentspeicheranbieter erstellen.

![Webhooks](assets/mceclip0-350x262.png)

Das Benutzererlebnis bei Webhook-basierten Integrationen ähnelt dem von vorhandenen Dokumentenintegrationen, z. B. Google Drive, Box und Dropbox. Beispielsweise kann ein Workfront-Benutzer die folgenden Aktionen ausführen:

* Navigieren in der Ordnerstruktur des externen Dokumentanbieters
* Dateien durchsuchen
* Verknüpfen von Dateien mit Workfront
* Hochladen von Dateien in den externen Dokumentanbieter
* Anzeigen einer Miniaturansicht für das Dokument

**-Referenzimplementierung**

Um die Entwicklung einer neuen Webhooks-Implementierung zu beschleunigen, bietet Workfront Beispiele für eine Referenzimplementierung. Diese Beispiele finden Sie unter [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). Die Beispiele sind Java-basiert und ermöglichen es Workfront, Dokumente in einem Netzwerk-Dateisystem zu verbinden. 

>[!NOTE]
>
>Die Ressourcen auf GitHub sind nur Beispiele und können keine Implementierung ausführen.

## Versionen

* Version 1.0 (Veröffentlichungsdatum - Mai 2015): Erste Spezifikation

* Version 1.1 (Veröffentlichungsdatum - Juni 2015). /uploadInit - Dokument-ID und Dokument-Version-ID hinzugefügt

* Version 1.2 (Veröffentlichungsdatum - Oktober 2015): hinzugefügt /createFolder

* Anstehende Versionen (Veröffentlichungsdatum - wird noch bekannt gegeben):

   * Hinzugefügt/löschen
   * hinzugefügt/umbenennen
   * Hinzugefügt /serviceInfo
   * Hinzugefügt /customAction
   * Hinzufügen von Paginierung und parentId zu /search
