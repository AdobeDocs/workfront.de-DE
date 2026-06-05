---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Dokumentaktion „moveToFolder“ funktioniert nicht
description: Bei Verwendung der Aktion „Document moveToFolder“ wird ein 422-Fehler zurückgegeben.
author: Becky
feature: Workfront API
role: Developer
exl-id: 811efabc-e101-4de5-a800-a1447654dc3e
TQID: https://experienceleague.adobe.com/UV4VnQEs-jGJau1UqXTLnp7Ak-cmKRpjuJqxgNTF5z8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 121
ht-degree: 12%

---

# Dokumentaktion „moveToFolder“ funktioniert nicht

## Problem

Bei Verwendung der `moveToFolder`-Aktion des Dokumentobjekts wird ein 422-Fehler zurückgegeben.

ODER

Wenn Sie diese Aktion über das Adobe Authenticator-Modul in Workfront Fusion verwenden, wird das Dokument nicht verschoben, es gibt jedoch keinen Hinweis auf den Fehler. Der Fehler ist derselbe, aber das Adobe Authenticator-Modul zeigt ihn nicht an.

## Lösung

Eine mögliche Ursache für einen 422-Fehler bei dieser Aktion ist, dass die Aktion versucht, ein Dokument in einem verknüpften Ordner in einen anderen verknüpften Ordner zu verschieben.

Stellen Sie sicher, dass sich das zu verschiebende Dokument nicht bereits in einem verknüpften Ordner befindet.
