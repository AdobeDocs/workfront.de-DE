---
content-type: api
navigation-topic: api-navigation-topic
title: Wiederholungen von Ereignisabonnements
description: Wiederholungen von Ereignisabonnements
author: John
feature: Workfront API
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 606d19b8a83b833aba6d6b15231a8683aa2cee40
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# Wiederholungen von Ereignisabonnements

Bei der Implementierung eines Nachrichtenversandsystems müssen einige Einschränkungen behoben werden, um Stabilität, Konsistenz und ein gutes Benutzererlebnis zu gewährleisten. Eine der Schwachstellen eines Nachrichtenversandsystems besteht darin, sicherzustellen, dass Nachrichten ihr Ziel erfolgreich erreichen, und zu wissen, was zu tun ist, wenn Nachrichten nicht ankommen.

Einige Integrationen können einen fehlgeschlagenen Versand akzeptieren, die Nachricht dann ablegen und zur nächsten Nachricht wechseln.  In anderen Integrationen kann das Fehlschlagen eines Nachrichtenversands nicht ignoriert werden. Beispielsweise könnte eine Finanzintegration versuchen, eine Nachricht zu senden, erhält aber stattdessen den HTTP-Status-Code 404, der angibt, dass der Server den Endpunkt, an den die Nachricht gesendet werden sollte, nicht finden konnte. In solchen Fällen könnte eine fehlende Nachricht bedeuten, dass jemand nicht für seine Zeit bezahlt wird oder dass eine Organisation über das Budget für vertraglich vereinbarte Ressourcen geht.

## Adobe Workfront-Strategie für die Wiederholung von Ereignisanmeldungen

Da Kunden die Workfront-Plattform als Kernstück ihrer täglichen Wissensarbeit nutzen, bietet das Workfront Event Subscription Framework einen Mechanismus, um sicherzustellen, dass der Versand jeder Nachricht so umfassend wie möglich versucht wird.

Ereignisausgelöste ausgehende Nachrichten, die nicht an Kunden-Endpunkte gesendet werden, werden erneut gesendet, bis der Versand für einen Zeitraum von bis zu 48 Stunden erfolgreich war. Während dieser Zeit werden weitere Versuche schrittweise reduziert, bis der Versand erfolgreich war oder bis 48 Stunden vergangen sind.

Kunden müssen sicherstellen, dass alle Endpunkte, die ausgehende Nachrichten aus Workfront-Ereignisabonnements verarbeiten, so eingerichtet sind, dass sie bei erfolgreicher Bereitstellung eine 200-Grad-Antwortnachricht an Workfront zurückgeben.

## Umgang mit fehlgeschlagenen, ereignisausgelösten ausgehenden Nachrichten

Das folgende Flussdiagramm zeigt die Strategie für den erneuten Versuch eines Nachrichtenversands mit Workfront-Ereignisabonnements:

![](assets/event-subscription-circuit-breaker-retries-350x234.png)

Die folgenden Erläuterungen entsprechen den im Flussdiagramm dargestellten Schritten:

1. Nachricht kann nicht zugestellt werden.
1. Informationen zu fehlgeschlagenen Nachrichten werden protokolliert.

   Alle fehlgeschlagenen Zustellversuche werden protokolliert, sodass ein Debugging durchgeführt werden kann, um die Grundursache eines bestimmten Fehlers oder einer Reihe von Fehlern zu ermitteln.

1. URL-Fehler wurden erhöht.
1. Die Anzahl der Nachrichtenversuche wird erhöht.
1. Berechnen Sie die Verzögerung, bis der Nachrichtenversand erneut versucht wird.
1. Die Nachricht wird in die Warteschlange für erneute Zustellversuche eingefügt.

   Wie im vorherigen Flussdiagramm gezeigt, ist die für die erneuten Verarbeitungsversuche verwendete Nachrichtenwarteschlange eine separate Warteschlange von der Warteschlange, die den ersten Versandversuch für jede Nachricht verarbeitet. Dadurch kann der nahezu in Echtzeit ablaufende Nachrichtenfluss fortgesetzt werden, ohne dass ein Teil der Nachrichten fehlschlägt.

1. Der URL-Schaltflächenstatus wird ausgewertet. Eine der folgenden Situationen tritt auf:

   * Wenn die Schaltung geöffnet ist und derzeit keine Sendungen zulässt, starten Sie den Prozess in Schritt 5 neu.
   * Wenn der Schaltkreis halb geöffnet ist, bedeutet dies, dass unser Schaltkreis derzeit geöffnet ist, aber genügend Zeit vergangen ist, um die Prüfung der URL zu ermöglichen, um festzustellen, ob das Problem mit dem Versand an ihn gelöst wurde.
   * Wenn die Beschränkungen für den Nachrichtenversand erreicht wurden (48 Stunden Wiederholungsversuch), wird die Nachricht verworfen

1. Wenn die URL-Schaltung geschlossen ist und Sendungen ermöglicht, versuchen Sie, die Nachricht zu senden. Wenn dieser Versand fehlschlägt, wird die Nachricht bei Schritt 1 neu gestartet

1. Wenn die URL-Schaltung geschlossen ist und Sendungen ermöglicht, versuchen Sie, die Nachricht zu senden. Wenn dieser Versand fehlschlägt, wird die Nachricht in Schritt 1 neu gestartet.

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront disables Event Subscriptions when both of the following criteria are met:
   <ul>
   <!--
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The Event Subscription has failed 1000 delivery attempts consecutively</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">48 hours have passed since the last successful delivery</li>
   </ul></li>
   -->
