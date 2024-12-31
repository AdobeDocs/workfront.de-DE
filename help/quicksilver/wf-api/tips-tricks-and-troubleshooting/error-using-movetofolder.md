---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Aktion zum Verschieben von Dokumenten funktioniert nicht
description: Bei Verwendung der Aktion „Document moveToFolder“ wird ein 422-Fehler zurückgegeben.
author: Becky
feature: Workfront API
role: Developer
exl-id: 811efabc-e101-4de5-a800-a1447654dc3e
source-git-commit: 53edc378e000e5b36fe0ce5750b8917fb13cfde1
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---

# Aktion zum Verschieben von Dokumenten funktioniert nicht

## Problem

Bei Verwendung der `moveToFolder`-Aktion des Dokumentobjekts wird ein 422-Fehler zurückgegeben.

Oder

Wenn Sie diese Aktion über das Adobe Authenticator-Modul in Workfront Fusion verwenden, wird das Dokument nicht verschoben, es gibt jedoch keinen Hinweis auf den Fehler. Der Fehler ist derselbe, aber das Adobe Authenticator-Modul zeigt ihn nicht an.

## Lösung

Eine mögliche Ursache für einen 422-Fehler bei dieser Aktion ist, dass die Aktion versucht, ein Dokument in einem verknüpften Ordner in einen anderen verknüpften Ordner zu verschieben.

Stellen Sie sicher, dass sich das zu verschiebende Dokument nicht bereits in einem verknüpften Ordner befindet.
