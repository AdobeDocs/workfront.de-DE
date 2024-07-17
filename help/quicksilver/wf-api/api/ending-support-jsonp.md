---
content-type: api
navigation-topic: api-navigation-topic
title: Beenden der Unterstützung für JSONP
description: Beenden der Unterstützung für JSONP
author: Becky
feature: Workfront API
role: Developer
exl-id: 681336c2-2f41-4746-8cba-be077f556742
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# Beenden der Unterstützung für JSONP

Da JSONP (JavaScript mit Padding) ein alter Standard mit bekannten Sicherheitslücken ist, unterstützt Adobe Workfront JSONP ab November 2018 nicht mehr. Dieser Beschluss unterstützt unsere umfassendere Initiative zur Modernisierung der Workfront-Plattform.

JSONP ist ein Standard, mit dem ursprungsübergreifende oder Site-übergreifende Anforderungen durchgeführt werden können. Viele Workfront-Kunden und -Partner verwenden JSONP, um im Rahmen einer Integration von einem System in ihrer eigenen Domäne auf Workfront zuzugreifen. JSONP ermöglicht die Verarbeitung von Anforderungen von Nicht-Workfront-Domänen durch die Workfront-Anwendung.

Wenn Sie JSONP als Teil Ihrer Workfront-Integrationen verwenden, müssen Sie Ihre Integration aktualisieren, um den CORS-Standard (Cross-Origin Resource Sharing) zu verwenden. Für diese Aktualisierung müssen Sie Folgendes tun:

1. Senden Sie eine Anfrage an das Workfront-Supportteam, um Domänen zu haben, die für ursprungsübergreifende Anfragen an unsere Zulassungsliste verwendet werden.

   Wenn Sie möchten, dass Ihre Domänen zur Zulassungsliste für CORS hinzugefügt werden, wenden Sie sich unter 844-306-HELP(4357) an den Workfront-Support oder senden Sie ein Supportticket online.

   >[!NOTE]
   >
   >Das Hinzufügen von Domänen zur Zulassungsliste für CORS wird nur für Kunden unterstützt, die JSONP vor dem 1. August 2018 verwendet haben.


1. Nehmen Sie Änderungen an Ihrem Integrationscode vor, um CORS zu verwenden.
