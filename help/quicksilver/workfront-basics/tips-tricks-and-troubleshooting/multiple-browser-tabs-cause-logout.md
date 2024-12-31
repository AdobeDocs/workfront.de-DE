---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Mehrere Browser-Registerkarten führen dazu, dass sich Workfront abmeldet
description: Wenn mehrere Browser-Registerkarten geöffnet sind, meldet sich Workfront möglicherweise automatisch ab.
feature: Get Started with Workfront
exl-id: 1cc8bf6c-0eda-41ef-8efd-bba3a5f33b08
source-git-commit: 8428bfba81fa988cf370581af0692e4ff595c0ae
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Mehrere Browser-Registerkarten führen dazu, dass sich Workfront abmeldet

>[!IMPORTANT]
>
>Dieses Problem tritt nur bei Organisationen auf, die in Adobe IMS integriert wurden.

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

* Wenn Sie eine aktive Workfront-Registerkarte geöffnet haben, laden Sie die abgelaufene Registerkarte neu. Dadurch wird wieder die Seite angezeigt, die Sie vor dem Ablauf geöffnet hatten.

* Wenn keine aktive Workfront-Registerkarte geöffnet ist, melden Sie sich erneut bei Workfront an.
