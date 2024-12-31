---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 'API-Fehlermeldung 400: Fehlerhafte Anfrage'
description: 'API-Fehlermeldung 400: Fehlerhafte Anfrage'
author: Becky
feature: Workfront API
role: Developer
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '93'
ht-degree: 0%

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
