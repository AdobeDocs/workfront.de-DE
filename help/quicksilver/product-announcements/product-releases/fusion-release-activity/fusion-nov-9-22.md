---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: 'Workfront Fusion-Release-Aktivität: Woche vom 7. November 2022"'
description: Auf dieser Seite werden alle Verbesserungen beschrieben, die in der Adobe Workfront Fusion-Woche vom 7. November 2022 vorgenommen wurden.
author: Luke
feature: Product Announcements, Workfront Fusion
hidefromtoc: true
exl-id: 802db851-39bb-4f40-8a66-ecb8c8b3ced6
source-git-commit: 9aaba3062bc5d1166c37821a6a3216f7f1d965b1
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Workfront Fusion-Release-Aktivität: Woche vom 7. November 2022

**Webhook-Warteschlangenoptimierung**

Die Webhook-Warteschlange von Fusion wurde mit dieser Version optimiert. Der Dienst, der Webhooks akzeptiert, ist jetzt von Warteschlangen- und anderen Prozessen getrennt. Diese Änderung ermöglicht es Fusion, Webhook-Warteschlangen schneller und konsistenter zu verarbeiten.

Während der Implementierung dieser Änderung konnten wir die erwartete Protokollverarbeitungszeit für Webhook-Ereignisse in der Warteschlange besser verstehen. Die Web-Hook-Viewer-Seite von Fusion wird voraussichtlich nicht älter als 1 Minute sein.

Um die aktuellen Webhook-Ereignisse in der Warteschlange anzuzeigen, navigieren Sie in der linken Navigation zu Webhooks. Lkw-Symbole mit einer Zahl im Zähler zeigen Warteschlangenereignisse für diesen Webhook an. Klicken Sie auf das LKW-Symbol, um die Ereignisse in der Warteschlange anzuzeigen.

![](assets/fusion-webhook-queue-1866x567.png)


**Nicht verwendete Webhooks werden jetzt deaktiviert oder gelöscht**

Wir haben einige Änderungen an der Handhabung nicht verwendeter Webhooks durch Workfront Fusion vorgenommen. Jetzt werden Webhooks automatisch deaktiviert, wenn eine der folgenden Aktionen zutrifft:

* Der Webhook ist seit mehr als 5 Tagen mit keinem Szenario verbunden.
* Der Webhook wird nur in inaktiven Szenarien verwendet, die seit mehr als 30 Tagen inaktiv sind.

Deaktivierte Webhooks werden automatisch gelöscht und abgemeldet, wenn sie mit keinem Szenario verbunden sind und seit über 30 Tagen deaktiviert sind.
