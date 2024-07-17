---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2 Testversandverbesserungen
description: Auf dieser Seite werden alle Verbesserungen bei der Prüfung beschrieben, die mit Version 2020.2 in der Produktionsumgebung vorgenommen wurden. Diese Verbesserungen wurden in der Produktionsumgebung in der Woche vom 11. Mai 2020 bereitgestellt.
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 021c6e0c-3593-40f7-8eeb-7e016001893e
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 0%

---

# 2020.2 Testversandverbesserungen

Auf dieser Seite werden alle Verbesserungen bei der Prüfung beschrieben, die mit Version 2020.2 in der Produktionsumgebung vorgenommen wurden. Diese Verbesserungen wurden in der Produktionsumgebung in der Woche vom 11. Mai 2020 bereitgestellt.

Eine Liste aller Änderungen, die mit Version 2020.2 verfügbar sind, finden Sie unter [Versionsübersicht 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Die Testversanddomäne ändert sich von proofhq.com in workfront.com.

>[!NOTE]
>
>Diese Funktion wurde ursprünglich als Teil der Version 2020.1 kommuniziert, wurde aber vor der Veröffentlichung für die Produktion aus der Version entfernt.

Wenn Ihre Firewall- oder Mailserver so konfiguriert ist, dass nur bestimmte Anbieter Zugriff erhalten, müssen Sie Ihrer Zulassungsliste die folgende zusätzliche URL hinzufügen, um sicherzustellen, dass Benutzer in Ihrer Organisation Testsendungen in Workfront sowohl im Browser-Testversand-Viewer als auch im Desktop-Testversand-Viewer anzeigen können:

&#42;.workfront.com

Die URL &#42;proofhq.com ist weiterhin erforderlich.

Weitere Informationen zum Aktualisieren Ihrer Zulassungsliste finden Sie unter [Konfigurieren der Zulassungsliste Ihrer Firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Diese Aktualisierung gilt nur für Testsendungen in Workfront. Sie gilt nicht für die Verwendung der eigenständigen Workfront Proof-Anwendung.

## Im Bereich Updates werden die von den Gästen abgegebenen Proof-Kommentare angezeigt

Um die Zusammenarbeit bei Testsendungen zu optimieren, werden im Bereich Updates Gastkommentare angezeigt.

Zuvor waren die von den Gästen gemachten Kommentare zum Testversand nur im Testversand verfügbar.
