---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Mehrere Browser-Registerkarten führen zur Abmeldung von Workfront
description: Wenn ein Benutzer mehrere Browser-Registerkarten geöffnet hat, meldet sich Workfront möglicherweise automatisch ab.
feature: Get Started with Workfront
source-git-commit: ef85b267b3417dddd0c9cc4a2b916b83dc416e14
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Mehrere Browser-Registerkarten führen zur Abmeldung von Workfront

>[!IMPORTANT]
>
>Dieses Problem tritt nur bei Unternehmen auf, die in Adobe IMS integriert wurden.

## Problem

Wenn ein Benutzer mehrere Browser-Registerkarten geöffnet hat und auf eine Registerkarte klickt, die seit einiger Zeit inaktiv ist, ist die Tabulatorsitzung abgelaufen. Der Benutzer kann die Seite, die er geöffnet hatte, nicht sehen und stattdessen wird die folgende Meldung angezeigt:

```
Tab session expired
This tab session has been halted due to inactivity. Refresh the tab to continue where you left off.
```

## Grund

Dieses Verhalten beruht auf Policy-Based Authentication (PBA), einer von Ihrem Unternehmen konfigurierten Sicherheitsmaßnahme. Wenn eine Registerkarte länger als das in der PBA-Konfiguration Ihres Unternehmens festgelegte Zeitlimit inaktiv war, läuft die Registerkartensitzung ab.

## Lösung

Die Lösung hängt davon ab, ob Sie auf einer anderen Registerkarte aktiv waren, die bei Workfront angemeldet ist.

* Wenn Sie eine aktive Workfront-Registerkarte geöffnet haben, laden Sie die abgelaufene Registerkarte neu. Er kehrt zu der Seite zurück, die Sie vor Ablauf geöffnet hatten.

* Wenn Sie keine aktive Registerkarte für Workfront geöffnet haben, melden Sie sich erneut bei Workfront an.