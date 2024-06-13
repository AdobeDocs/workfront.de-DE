---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Die Aktion "Dokument verschiebenToFolder"funktioniert nicht
description: Bei Verwendung der Aktion "Dokument verschiebenToFolder"wird ein 422-Fehler zurückgegeben.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 86c0517443537ec5af640036c290b3a495825fdc
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---


# Die Aktion &quot;Dokument verschiebenToFolder&quot;funktioniert nicht

## Problem

Bei Verwendung des Dokumentobjekts `moveToFolder` -Aktion verwenden, wird ein 422-Fehler zurückgegeben.

Oder

Wenn Sie diese Aktion über das Adobe Authenticator-Modul in Workfront Fusion verwenden, wird das Dokument nicht verschoben, es gibt jedoch keinen Hinweis auf den Fehler. Der Fehler ist identisch, aber das Adobe Authenticator-Modul zeigt ihn nicht an.

## Lösung

Eine mögliche Ursache für einen 422-Fehler bei dieser Aktion ist, dass die Aktion versucht, ein Dokument in einem verknüpften Ordner in einen anderen verknüpften Ordner zu verschieben.

Vergewissern Sie sich, dass sich das zu verschiebende Dokument nicht bereits in einem verknüpften Ordner befindet.
