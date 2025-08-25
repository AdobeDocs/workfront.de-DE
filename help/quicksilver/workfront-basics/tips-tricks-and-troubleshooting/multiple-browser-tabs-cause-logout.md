---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Mehrere Browser-Registerkarten führen dazu, dass sich Workfront abmeldet
description: Wenn mehrere Registerkarten im Browser geöffnet sind, meldet sich Workfront möglicherweise automatisch ab.
feature: Get Started with Workfront
exl-id: 1cc8bf6c-0eda-41ef-8efd-bba3a5f33b08
source-git-commit: 99113ac4f2ceca6bd50f078916e33cec7f577362
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 32%

---

# Mehrere Browser-Registerkarten führen dazu, dass sich Workfront abmeldet

## Problem

Wenn ein(e) Benutzende(r) mehrere Browser-Registerkarten geöffnet hat und auf eine Registerkarte klickt, die seit einiger Zeit inaktiv ist, ist die Registerkartensitzung abgelaufen. Der/die Benutzende kann die Seite, die er/sie geöffnet hatte, nicht sehen und sieht stattdessen die folgende Meldung:

```
Tab session expired
This tab session has been halted due to inactivity. Refresh the tab to continue where you left off.
```

## Grund

Dieses Verhalten ist auf die richtlinienbasierte Authentifizierung (Policy-Based Authentication, PBA) zurückzuführen, eine Sicherheitsmaßnahme, die von Ihrer Organisation konfiguriert wurde. Wenn eine Registerkarte länger als das in der PBA-Konfiguration Ihres Unternehmens festgelegte Zeitlimit inaktiv war, läuft die Registerkartensitzung ab.

## Lösung

Die Lösung hängt davon ab, ob Sie auf einer anderen Registerkarte aktiv waren, die bei Workfront angemeldet ist.

* Wenn eine aktive Workfront-Registerkarte geöffnet ist, laden Sie die abgelaufene Registerkarte neu. Dadurch wird wieder die Seite angezeigt, die vor dem Ablauf geöffnet war.

* Wenn keine aktive Workfront-Registerkarte geöffnet ist, melden Sie sich erneut bei Workfront an.
