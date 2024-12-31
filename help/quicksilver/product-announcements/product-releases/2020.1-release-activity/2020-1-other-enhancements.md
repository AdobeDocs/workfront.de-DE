---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: 2020.1 Weitere Verbesserungen
description: Auf dieser Seite werden alle Verbesserungen beschrieben, die mit der Version 2020.1 an allgemeinen Bereichen von Workfront vorgenommen wurden. Diese Verbesserungen sind derzeit in der Vorschau -Umgebung verfügbar und werden Ende März oder Anfang April 2020 in der Produktionsumgebung verfügbar gemacht.
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

Auf dieser Seite werden alle Verbesserungen beschrieben, die mit der Version 2020.1 an allgemeinen Bereichen von Workfront vorgenommen wurden. Diese Verbesserungen sind derzeit in der Vorschau -Umgebung verfügbar und werden Ende März oder Anfang April 2020 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller mit Version 2020.1 verfügbaren Änderungen finden Sie unter [Übersicht über die Version 2020.1](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## Zum Hinzufügen von Korrekturabzügen zur Zulassungsliste erforderliche Änderung

>[!NOTE]
>
>Diese Funktion wurde aus der Version 2020.1 entfernt. Sie wird zu einem späteren Zeitpunkt zur Verfügung gestellt.

Die Proofing-Domain wird von proofhq.com in workfront.com geändert.

Wenn Ihre Firewall oder Ihr E-Mail-Server so konfiguriert ist, dass er nur bestimmten Anbietern Zugriff gewährt, müssen Sie die folgende zusätzliche URL zu Ihrer Zulassungsliste hinzufügen, um sicherzustellen, dass Benutzende in Ihrem Unternehmen Korrekturabzüge in Workfront sowohl im Proofing-Viewer als auch im Desktop-Proofing-Viewer anzeigen können:

&#42;.workfront.com

Die URL &#42;proofhq.com ist ebenfalls weiterhin erforderlich.

Weitere Informationen zum Aktualisieren der Zulassungsliste finden Sie [Zulassungsliste zur Firewall konfigurieren](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

>[!NOTE]
>
>Dieses Update gilt nur für das Proofing innerhalb von Workfront. Es gilt nicht für die Verwendung der eigenständigen Workfront Proof-Anwendung.

## Das Workfront-Cookie-Verhalten wurde aktualisiert, um die Kompatibilität mit Chrome zu gewährleisten

Um die Kompatibilität mit einem bevorstehenden Google Chrome-Update (Chrome v80) zu gewährleisten, haben wir die Workfront-Plattform aktualisiert, um sicherzustellen, dass Cookies mit Anfragen ordnungsgemäß gesendet werden.

Diese Chrome-Aktualisierung ändert den Standardwert des SameSite-Cookie-Attributs. Wenn Sie testen möchten, wie sich Ihre Workfront-Instanz nach der Aktualisierung von Google Chrome verhält, passen Sie die Flags in Chrome an und aktivieren Sie die folgenden Optionen:

* „Standard-SameSite-Cookies“
* „Cookies ohne SameSite müssen sicher sein“

## Synchronisierung von Workfront-Kommentaren mit Jira

Die Integration von Workfront für Jira synchronisiert jetzt Ihre Workfront-Kommentare mit dem nativen Jira-Kommentar-Stream.

Zuvor konnten Sie Kommentare von Jira mit Workfront synchronisieren, aber nicht von Workfront mit Jira.

Weitere Informationen finden Sie unter [Konfigurieren von Adobe Workfront für Jira](../../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Der Flash Portfolio Optimizer wurde entfernt

Die Möglichkeit, aus der Workfront Classic-Umgebung für alle Kunden zwischen dem neuen und dem alten (auf Flash basierenden) Portfolio Optimizer zu wechseln, wurde entfernt. Der Legacy Portfolio Optimizer ist eine veraltete Funktion, und die neuen Tools bieten heute dieselben Funktionen.

Informationen zum Portfolio-Optimizer finden Sie unter https://experience.workfront.com/s/article/Understanding-the-Portfolio-Optimizer-356650079

Informationen zur Einstellung von Flash-basierten Tools in Workfront finden Sie [Ersetzen von Flash-basierten Tools in Adobe Workfront](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).
