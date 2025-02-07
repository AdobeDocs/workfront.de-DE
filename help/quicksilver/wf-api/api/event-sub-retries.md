---
content-type: api
navigation-topic: api-navigation-topic
title: Wiederholungen von Ereignisabonnements
description: Wiederholungen von Ereignisabonnements
author: Becky
feature: Workfront API
role: Developer
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Wiederholungen von Ereignisabonnements

Bei der Implementierung eines Nachrichtenversand-Systems müssen einige Einschränkungen beachtet werden, um Stabilität, Konsistenz und ein gutes Benutzererlebnis zu gewährleisten. Einer der Mängel eines Nachrichtenversand-Systems besteht darin, sicherzustellen, dass Nachrichten ihr Ziel erfolgreich erreichen und wissen, was zu tun ist, wenn Nachrichten nicht ankommen.

Einige Integrationen können einen fehlgeschlagenen Versand akzeptieren, die Nachricht dann ablegen und zur nächsten Nachricht wechseln.  In anderen Integrationen kann die Nichtbereitstellung einer Nachricht nicht ignoriert werden. Beispielsweise kann eine Finanzintegration versuchen, eine Nachricht zuzustellen, stattdessen erhält sie den HTTP-Status-Code 404, der angibt, dass der Server den Endpunkt, an den die Nachricht zugestellt werden sollte, nicht finden konnte. In solchen Fällen könnte eine fehlende Nachricht bedeuten, dass jemand nicht für seine Zeit bezahlt wird oder dass eine Organisation über das Budget für vertraglich gebundene Ressourcen hinausgeht.

## Adobe Workfront-Strategie für weitere Zustellversuche bei Ereignisabonnements

Da Kundinnen und Kunden die Workfront-Plattform als Kernstück ihrer täglichen Wissensarbeit nutzen, bietet das Workfront Event Subscription Framework einen Mechanismus, der sicherstellt, dass der Versand jeder Nachricht im größtmöglichen Umfang versucht wird.

Ereignisgesteuerte ausgehende Nachrichten, die nicht an Kundenendpunkte gesendet werden können, werden bis zu einem Zeitraum von 48 Stunden erneut gesendet, bis der Versand erfolgreich war. Während dieser Zeit werden weitere Zustellversuche mit einer inkrementell erhöhten Häufigkeit durchgeführt, bis der Versand erfolgreich ist oder bis 11 Zustellversuche unternommen wurden.

Die Formel für diese Wiederholungsversuche lautet:

`((2^attempt) - 1) * 84800ms`

Der erste erneute Versuch findet nach 1,5 Minuten statt, der zweite nach fast 5 Minuten und der elfte nach etwa 48 Stunden.

Kunden müssen sicherstellen, dass alle Endpunkte, die ausgehende Nachrichten von Workfront-Ereignisabonnements verarbeiten, so eingerichtet sind, dass bei erfolgreichem Versand eine Antwortnachricht der Ebene 200 an Workfront zurückgegeben wird.

## Deaktivierte und eingefrorene Abonnementregeln

* Eine Abonnement-URL **deaktiviert** wenn sie eine Fehlerrate von über 70 % mit über 100 Versuchen aufweist ODER wenn sie 2.000 aufeinander folgende Fehler aufweist
* Eine Abonnement-URL **eingefroren** wenn sie mehr als 2.000 aufeinander folgende Fehler aufweist und der letzte Erfolg mehr als 72 Stunden zurückliegt ODER wenn sie 50.000 aufeinander folgende Fehler in einem beliebigen Zeitrahmen aufweist.
* Eine **deaktivierte** Abonnement-URL versucht weiterhin alle 10 Minuten einen Versand und wird bei einem erfolgreichen Versand erneut aktiviert.
* Eine **eingefrorene** Abonnement-URL versucht nie die Bereitstellung, es sei denn, sie wird manuell durch eine API-Anfrage aktiviert.




<!--

## Handling Failed Event-Triggered Outbound Messages

The following flowchart shows the strategy for reattempting message deliveries with Workfront Event Subscriptions:

![Event sub retries](assets/event-subscription-circuit-breaker-retries-350x234.png)

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
