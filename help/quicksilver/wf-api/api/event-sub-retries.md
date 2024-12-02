---
content-type: api
navigation-topic: api-navigation-topic
title: Wiederholungen von Ereignisabonnements
description: Wiederholungen von Ereignisabonnements
author: Becky
feature: Workfront API
role: Developer
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 0325d305c892c23046739feff17d4b1fc11100cc
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Wiederholungen von Ereignisabonnements

Bei der Implementierung eines Nachrichtenversandsystems müssen einige Einschränkungen behoben werden, um Stabilität, Konsistenz und ein gutes Benutzererlebnis zu gewährleisten. Eine der Schwachstellen eines Nachrichtenversandsystems besteht darin, sicherzustellen, dass Nachrichten ihr Ziel erfolgreich erreichen, und zu wissen, was zu tun ist, wenn Nachrichten nicht ankommen.

Einige Integrationen können einen fehlgeschlagenen Versand akzeptieren, die Nachricht dann ablegen und zur nächsten Nachricht wechseln.  In anderen Integrationen kann das Fehlschlagen eines Nachrichtenversands nicht ignoriert werden. Beispielsweise könnte eine Finanzintegration versuchen, eine Nachricht zu senden, erhält aber stattdessen den HTTP-Status-Code 404, der angibt, dass der Server den Endpunkt, an den die Nachricht gesendet werden sollte, nicht finden konnte. In solchen Fällen könnte eine fehlende Nachricht bedeuten, dass jemand nicht für seine Zeit bezahlt wird oder dass eine Organisation über das Budget für vertraglich vereinbarte Ressourcen geht.

## Adobe Workfront-Strategie für die Wiederholung von Ereignisanmeldungen

Da Kunden die Workfront-Plattform als Kernstück ihrer täglichen Wissensarbeit nutzen, bietet das Workfront Event Subscription Framework einen Mechanismus, um sicherzustellen, dass der Versand jeder Nachricht so umfassend wie möglich versucht wird.

Ereignisausgelöste ausgehende Nachrichten, die nicht an Kunden-Endpunkte gesendet werden, werden erneut gesendet, bis der Versand für einen Zeitraum von bis zu 48 Stunden erfolgreich war. Während dieser Zeit werden weitere Versuche schrittweise beschleunigt, bis der Versand erfolgreich war oder bis 11 Versuche unternommen wurden.

Die Formel für diese Wiederholungsversuche lautet:

`((2^attempt) - 1) * 84800ms`

Der erste Versuch erfolgt nach 1,5 Minuten, die zweite nach fast 5 Minuten und die elfte nach etwa 48 Stunden.

Kunden müssen sicherstellen, dass alle Endpunkte, die ausgehende Nachrichten aus Workfront-Ereignisabonnements verarbeiten, so eingerichtet sind, dass sie bei erfolgreicher Bereitstellung eine 200-Grad-Antwortnachricht an Workfront zurückgeben.

## Deaktivierte und eingefrorene Abonnementregeln

* Eine Anmelde-URL ist **deaktiviert** , wenn sie bei mehr als 100 Versuchen eine Fehlerrate von über 70 % aufweist ODER bei 2.000 aufeinander folgenden Fehlern
* Eine Anmelde-URL ist **eingefroren** , wenn sie mehr als 2.000 aufeinander folgende Fehler aufweist und der letzte Erfolg vor mehr als 72 Stunden erfolgte ODER wenn innerhalb eines beliebigen Zeitraums 50.000 aufeinander folgende Fehler aufgetreten sind.
* Eine **disabled**-Anmelde-URL versucht weiterhin alle 10 Minuten, einen Versand durchzuführen, und wird bei einem erfolgreichen Versand wieder aktiviert.
* Eine Abonnement-URL vom Typ **frozen** versucht nie, den Versand durchzuführen, es sei denn, sie wird durch eine API-Anfrage manuell aktiviert.



<!--

## Handling Failed Event-Triggered Outbound Messages

The following flowchart shows the strategy for reattempting message deliveries with Workfront Event Subscriptions:

![](assets/event-subscription-circuit-breaker-retries-350x234.png)

The following explanations correspond with the steps depicted in the flowchart:

1. Message fails to be delivered. 
1. Message delivery failure information is logged.

   All failed attempts to deliver a message are logged so that debugging may be performed to determine the root cause of a given failure or series of failures. 

1. URL failures incremented. 
1. Message attempt count is incremented. 
1. Calculate the delay until this message's delivery will be attempted again. 
1. Message is placed onto the message retry queue.

   As shown in the preceding flowchart, the message queue used for processing message delivery retries is a separate queue from the one that processes the initial delivery attempt for each message. This allows the near real-time flow of messages to continue unimpeded by the failure of any subset of messages. 

1. URL circuit status is evaluated. One of the following occurs:

   * If the circuit is open and not allowing deliveries at this time, restart the process at step 5.
   * If the circuit is half-open, this implies that our circuit is currently open, but enough time has passed to allow testing of the URL to see if the problem with delivering to it has been resolved.
   * If the message delivery attempt limits have been reached (48 hours of retrying) then the message is dropped

1. If the URL circuit is closed and allowing deliveries, attempt to deliver the message. If this delivery fails, the message will restart at step 1 

1. If the URL circuit is closed and allowing deliveries, attempt to deliver the message. If this delivery fails, the message will restart at step 1.
   -->
