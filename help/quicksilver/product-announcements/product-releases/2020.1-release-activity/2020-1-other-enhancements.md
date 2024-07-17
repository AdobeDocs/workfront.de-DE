---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: 2020.1 Weitere Verbesserungen
description: Auf dieser Seite werden alle Verbesserungen beschrieben, die mit Version 2020.1 an den allgemeinen Bereichen von Workfront vorgenommen wurden. Diese Verbesserungen sind derzeit in der Vorschau-Umgebung verfügbar und werden Ende März oder Anfang April 2020 in der Produktionsumgebung verfügbar gemacht.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a716590c-c833-458a-a138-9bc0723e5896
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# 2020.1 Weitere Verbesserungen

Auf dieser Seite werden alle Verbesserungen beschrieben, die mit Version 2020.1 an den allgemeinen Bereichen von Workfront vorgenommen wurden. Diese Verbesserungen sind derzeit in der Vorschau-Umgebung verfügbar und werden Ende März oder Anfang April 2020 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die mit Version 2020.1 verfügbar sind, finden Sie unter [Versionsübersicht 2020.1](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## Zum Hinzufügen von Testsendungen zur Zulassungsliste erforderliche Änderung

>[!NOTE]
>
>Diese Funktion wurde aus der Version 2020.1 entfernt. Sie wird zu einem späteren Zeitpunkt zur Verfügung gestellt.

Die Testversanddomäne ändert sich from proofhq.com in workfront.com.

Wenn Ihre Firewall- oder Mailserver so konfiguriert ist, dass nur bestimmte Anbieter Zugriff erhalten, müssen Sie Ihrer Zulassungsliste die folgende zusätzliche URL hinzufügen, um sicherzustellen, dass Benutzer in Ihrer Organisation Testsendungen in Workfront sowohl im Browser-Testversand-Viewer als auch im Desktop-Testversand-Viewer anzeigen können:

&#42;.workfront.com

Die URL &#42;proofhq.com ist weiterhin erforderlich.

Weitere Informationen zum Aktualisieren Ihrer Zulassungsliste finden Sie unter [Konfigurieren der Zulassungsliste Ihrer Firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

>[!NOTE]
>
>Diese Aktualisierung gilt nur für Testsendungen in Workfront. Sie gilt nicht für die Verwendung der eigenständigen Workfront Proof-Anwendung.

## Das Cookie-Verhalten von Workfront wurde aktualisiert, um die Kompatibilität mit Chrome zu gewährleisten

Um die Kompatibilität mit einem bevorstehenden Google Chrome-Update (Chrome v80) zu gewährleisten, haben wir die Workfront-Plattform aktualisiert, um sicherzustellen, dass Cookies mit Anforderungen ordnungsgemäß gesendet werden.

Durch diese Chrome-Aktualisierung wird der Standardwert des SameSite-Cookie-Attributs geändert. Wenn Sie testen möchten, wie sich Ihre Workfront-Instanz nach der Aktualisierung von Google Chrome verhält, passen Sie die Flags in Chrome an und aktivieren Sie die folgenden Optionen:

* &quot;Standard-SameSite-Cookies&quot;
* &quot;Cookies ohne SameSite müssen sicher sein&quot;

## Synchronisation von Workfront-Kommentaren mit Jira

Die Integration von Workfront für Jira synchronisiert Ihre Workfront-Kommentare jetzt mit dem nativen Kommentar-Stream von Jira.

Zuvor konnten Sie Kommentare von Jira mit Workfront synchronisieren, nicht aber von Workfront mit Jira.

Weitere Informationen finden Sie unter [Adobe Workfront für Jira konfigurieren](../../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Der Flash Portfolio Optimizer wurde entfernt

Wir haben die Möglichkeit entfernt, für alle Kunden zwischen dem neuen und dem alten (auf Flash basierenden) Portfolio Optimizer aus der Workfront Classic-Umgebung zu wechseln. Der ältere Portfolio Optimizer ist eine veraltete Funktion und die neuen Tools bieten heute die gleichen Funktionen.

Informationen zum Portfoliooptimierer finden Sie unter https://experience.workfront.com/s/article/Understanding-the-Portfolio-Optimizer-356650079

Weitere Informationen zur Einstellung von Flash-basierten Tools in Workfront finden Sie unter [Ersetzen von Flash-basierten Tools in Adobe Workfront](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).
