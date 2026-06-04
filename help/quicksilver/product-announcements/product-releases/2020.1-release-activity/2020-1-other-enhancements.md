---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: Weitere Verbesserungen in Version 2020.1
description: Auf dieser Seite werden alle Verbesserungen beschrieben, die mit der Version 2020.1 an allgemeinen Bereichen von Workfront vorgenommen wurden. Diese Verbesserungen sind derzeit in der Vorschau -Umgebung verfügbar und werden Ende März oder Anfang April 2020 in der Produktionsumgebung verfügbar gemacht.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a716590c-c833-458a-a138-9bc0723e5896
TQID: https://experienceleague.adobe.com/I5djuVv0ixHspF6afQaa5-jTkl0uXl26VlKf8BXqhO4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: b8ea32d4-f1fe-4c71-8871-afe5a702a009
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 433
ht-degree: 1%

---

# Weitere Verbesserungen in Version 2020.1

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

Die Möglichkeit, zwischen der neuen und der veralteten (auf Flash basierenden) Portfolio Optimizer-Umgebung zu wechseln, wurde aus der Workfront Classic-Umgebung für alle Kunden entfernt. Der alte Portfolio Optimizer ist eine veraltete Funktion, und die neuen Tools bieten heute dieselben Funktionen.

Informationen zum Portfolio-Optimizer finden Sie unter https://experience.workfront.com/s/article/Understanding-the-Portfolio-Optimizer-356650079

Informationen zur Einstellung von Flash-basierten Tools in Workfront finden Sie [Ersatz von Flash-basierten Tools in Adobe Workfront](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).
