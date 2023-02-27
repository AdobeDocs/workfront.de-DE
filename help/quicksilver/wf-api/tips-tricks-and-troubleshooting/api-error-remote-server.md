---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: API-Fehlermeldung 400 Bad Request
description: API-Fehlermeldung 400 Bad Request
author: Becky
feature: Workfront API
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 0%

---


# API-Fehler: &quot;Der Remote-Server hat einen Fehler (400) Bad Request zurückgegeben.&quot;

## Problem

Beim Versuch, die API zum Importieren eines benutzerdefinierten Felds in ein Problem zu verwenden, erhalten Sie den folgenden Fehler:

`The remote server returned an error: (400) Bad Request`

## Ursache

Dieser Fehler tritt auf, wenn Sie versuchen, über die API ein benutzerdefiniertes Feld aus einem Projekt zu importieren, dem kein benutzerdefiniertes Formular mit einem Warteschlangenthema zugeordnet ist.

## Lösung

Fügen Sie das richtige benutzerdefinierte Formular zum Thema Warteschlange hinzu.

Weitere Informationen zu Warteschlangenthemen finden Sie unter [Erstellen von Warteschlangenthemen](../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
