---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Probleme mit der Geschwindigkeit in [!DNL Workfront Proof]
description: Auf dieser Hilfeseite können Sie feststellen, ob Geschwindigkeitsprobleme, die bei der Verwendung von auftreten [!DNL Workfront Proof]  mit Ihrem ISP oder dem Content Delivery Network  [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 42e999a6-5b27-482d-a7cf-b8030272da32
source-git-commit: 20fcf4dd07c1058559533501f7e297d78c43a70b
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# Probleme mit der Geschwindigkeit in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf Funktionen im eigenständigen [!DNL Workfront Proof]. Informationen zu Proofing in [!DNL Adobe Workfront] finden Sie unter [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Auf dieser Hilfeseite können Sie feststellen, ob Geschwindigkeitsprobleme, die bei der Verwendung von [!DNL Workfront Proof] auftreten könnten, mit Ihrem ISP oder dem Content Delivery Network von [!DNL Workfront Proof] zusammenhängen.

Geschwindigkeitsprobleme sind in der Regel auf die lokale ISP-Verbindung oder die Einrichtung des lokalen Internetzugangs zurückzuführen (z. B. wo ein Proxy-Server verwendet wird) und daher leider außerhalb der Kontrolle von [!DNL Workfront Proof].

Es gibt jedoch einige Schritte, die Sie unternehmen können, um Ihre Verbindungsgeschwindigkeit zu überprüfen, damit die Grundursache der Probleme, die Sie haben, ermittelt werden kann. Alle diese Schritte sind für den Fehlerbehebungsprozess gleichermaßen wichtig, und wir empfehlen Ihnen, sich die Zeit zu nehmen, Informationen über alle aufgelisteten Schritte zu sammeln, um die genaueste Diagnose des Problems sicherzustellen.

Sobald Sie alle Details erfasst haben, empfehlen wir Ihnen, sich mit Ihrer lokalen IT-Abteilung in Verbindung zu setzen, um lokale Probleme zu identifizieren.

## Stellen Sie fest, welcher Teil des Systems langsam ist

Wenn Sie [!DNL Workfront Proof] verwenden, können Sie das Dashboard verwenden, z. B. um Ordnerinhalte und Benutzer zu verwalten, oder um mit dem [!DNL Workfront Proof] Viewer zu arbeiten: Korrekturabzugsüberprüfung, Überprüfung der bereits abgegebenen Kommentare usw.

Um Geschwindigkeitsprobleme zu beheben, müssen Sie zunächst feststellen, welcher Teil des Systems langsam ist. Wenn Sie [!DNL Workfront Proof] als langsam melden, stellen Sie sicher, dass Sie Folgendes beschreiben:

* Gibt es auf anderen Webseiten eine Langsamkeit?
* Tritt das Problem im Dashboard oder [!DNL Workfront Proof] Viewer auf?
* Welcher Teil des Systems ist langsam? (z. B. Bearbeiten eines neuen Korrekturabzugs oder Öffnen eines Kommentars in [!DNL Workfront Proof] Viewer)

## Durchführen von Traceroute- und Ping-Tests

Wenn Leistungsprobleme auftreten, muss der traceroute-Befehl ausgeführt werden, um die Verbindung zu überprüfen. Öffnen Sie dazu die Eingabeaufforderung in Ihrem System (Terminal in Mac/Linux) und führen Sie die folgenden Schritte aus:

1. Geben Sie einen der folgenden Werte ein und warten Sie, bis die Verfolgung abgeschlossen ist:

   * Windows: **tracert app.proofhq.com**
   * Mac/Linux: **traceroute app.proofhq.com**

1. (Nur Windows) Geben Sie **ping app.proofhq.com** ein.
1. Wenn der Ping abgeschlossen ist, klicken Sie mit der rechten Maustaste in die Eingabeaufforderung und wählen Sie „Alle“ aus.
1. Kopieren Sie die Ergebnisse und fügen Sie sie in die Antwort auf Ihre E-Mail ein.
Stellen Sie sicher, dass Sie den Abschluss von Traceroute und Ping zulassen, bevor Sie die Ergebnisse an das Support-Team senden.

## Testen der Verbindungsgeschwindigkeit mit Speedtest.net

1. Öffnen Sie einen Browser und navigieren Sie zu Speedtest.net.
1. Folgen Sie den Anweisungen in der Speedtest-Wissensdatenbank, um die Geschwindigkeit Ihrer Internetverbindung zu testen.
1. Kopieren Sie die Ergebnisse und fügen Sie sie in eine E-Mail unseres Supportteams ein.

## Überprüfen Sie in der Browser-Konsole die Registerkarte Netzwerk .

Die in den modernen Browsern verfügbare Web-Konsole sammelt nützliche Informationen über alle Netzwerklatenzen, die uns helfen, die Grundursache der Geschwindigkeitsprobleme zu ermitteln, die Sie haben.

So überprüfen Sie die Ladezeiten für eine Web-Seite:

1. Öffnen Sie die Browser-Konsole und die Registerkarte Netzwerk .
1. Laden Sie die Seite neu.
1. Nehmen Sie Screenshots auf oder zeichnen Sie einen Screencast der Ergebnisse auf.
1. Teilen Sie die Ergebnisse mit dem Support-Team.

Stellen Sie sicher, dass der Screenshot alle Daten anzeigt - Sie können das Konsolenfenster erweitern, wenn Sie einen Screenshot aufnehmen, oder in einem Screencast nach unten scrollen.

Ausführlichere Anweisungen finden Sie auch in der Dokumentation Ihres Browsers.

## Überprüfen Sie Ihre Verbindung mit einem anderen Netzwerk und Computer.

Die Überprüfung, ob dasselbe Problem bei der Verbindungsgeschwindigkeit mit einem anderen Gerät oder Netzwerk auftritt, ist ein wichtiger Schritt bei der Fehlerbehebung. Versuchen Sie, auf einen anderen Computer oder ein mobiles Gerät umzuschalten, und verwenden Sie ein alternatives Netzwerk (z. B. mobile Daten).

Vergleichen Sie die Verbindung in verschiedenen Kombinationen: Verwenden eines anderen Computers im selben Netzwerk, Verwenden desselben Computers in einem anderen Netzwerk und Verwenden sowohl eines alternativen Computers als auch eines Netzwerks, und teilen Sie dann die Ergebnisse mit dem Support-Team.
