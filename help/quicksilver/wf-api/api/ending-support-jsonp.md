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

Da JSONP (JavaScript mit Abstand) ein alter Standard mit bekannten Sicherheitslücken ist, unterstützt Adobe Workfront JSONP ab November 2018 nicht mehr. Dieser Beschluss unterstützt unsere größere Initiative zur Modernisierung der Workfront-Plattform.

JSONP ist ein Standard, mit dem ursprungsübergreifende oder Site-übergreifende Anforderungen ausgeführt werden können. Viele Kunden und Partner von Workfront verwenden JSONP, um im Rahmen einer Integration von einem System in ihrer eigenen Domain aus auf Workfront zuzugreifen. JSONP ermöglicht die Verarbeitung von Anfragen von Nicht-Workfront-Domains durch das Workfront-Programm.

Wenn Sie JSONP als Teil einer Ihrer Workfront-Integrationen verwenden, müssen Sie Ihre Integration aktualisieren, um den CORS-Standard (Cross-Origin Resource Sharing) zu verwenden. Für dieses Update sind folgende Schritte erforderlich:

1. Senden Sie eine Anfrage mit dem Workfront-Supportteam, um über alle Domains zu verfügen, die für herkunftsübergreifende Anfragen an unsere Zulassungsliste verwendet werden.

   Auf die Zulassungsliste setzen Um Ihre Domains zur für CORS hinzufügen zu lassen, wenden Sie sich unter 844-306-HELP(4357) an den Kunden-Support von Workfront oder senden Sie ein Support-Ticket online.

   >[!NOTE]
   >
   >Das Hinzufügen von Domains zur Zulassungsliste für CORS wird nur für Kunden unterstützt, die JSONP vor dem 1. August 2018 verwendet haben.


1. Nehmen Sie Änderungen am Integrations-Code vor, um CORS zu verwenden.
