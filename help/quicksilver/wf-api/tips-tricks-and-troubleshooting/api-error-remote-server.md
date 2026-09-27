---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 'API-Fehlermeldung 400: Fehlerhafte Anfrage'
description: 'API-Fehlermeldung 400: Fehlerhafte Anfrage'
author: Becky
feature: Workfront API
role: Developer
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
TQID: 'https://experienceleague.adobe.com/19PIdv4u8de0BlasXD0Yy6GssO3vv6Jt8BzcljB-m1w'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
    internal-label: APIs
  - id: 682536a8-4872-5ee6-a8a6-8012d713482c
    internal-label: Workfront API
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '93'
ht-degree: 3%
---
# API-Fehler: „Der Remote-Server hat einen Fehler zurückgegeben (400): Ungültige Anfrage“

## Problem

Beim Versuch, die API zum Importieren eines benutzerdefinierten Felds in ein Problem zu verwenden, wird die folgende Fehlermeldung angezeigt:

`The remote server returned an error: (400) Bad Request`

## Ursache

Dieser Fehler tritt auf, wenn Sie versuchen, über die API ein benutzerdefiniertes Feld aus einem Projekt zu importieren, dem kein benutzerdefiniertes Formular mit einem Warteschlangenthema verknüpft ist.

## Lösung

Fügen Sie dem Warteschlangenthema das richtige benutzerdefinierte Formular hinzu.

Weitere Informationen zu Warteschlangenthemen finden Sie unter [Warteschlangenthemen erstellen](../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
