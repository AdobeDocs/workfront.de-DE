---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Mehrere Registerkarten im Browser führen zur Abmeldung von Workfront
description: Wenn mehrere Registerkarten im Browser geöffnet sind, meldet sich Workfront möglicherweise automatisch ab.
feature: Get Started with Workfront
author: Becky
exl-id: 1cc8bf6c-0eda-41ef-8efd-bba3a5f33b08
TQID: https://experienceleague.adobe.com/Zof7zbTOm-w1vyBTchiXJv2QrNYbOxw9O4DYIjYQ6Ss
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 165
ht-degree: 42%

---

# Mehrere Registerkarten im Browser führen zur Abmeldung von Workfront

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
