---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Geschwindigkeitsprobleme in [!DNL Workfront Proof]
description: Auf dieser Hilfeseite können Sie feststellen, ob bei der Verwendung von [!DNL Workfront Proof] auftretende Geschwindigkeitsprobleme mit Ihrem ISP oder dem Inhaltsbereitstellungsnetzwerk von [!DNL Workfront Proof] in Zusammenhang stehen.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 42e999a6-5b27-482d-a7cf-b8030272da32
source-git-commit: 20fcf4dd07c1058559533501f7e297d78c43a70b
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# Geschwindigkeitsprobleme in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Auf dieser Hilfeseite können Sie feststellen, ob bei der Verwendung von [!DNL Workfront Proof] auftretende Geschwindigkeitsprobleme mit Ihrem ISP oder dem Inhaltsbereitstellungsnetzwerk von [!DNL Workfront Proof] in Zusammenhang stehen.

Geschwindigkeitsprobleme sind in der Regel auf die lokale ISP-Verbindung oder die Einrichtung des lokalen Internet-Zugriffs zurückzuführen (z. B. wo ein Proxy-Server verwendet wird) und stehen daher leider außerhalb der Kontrolle von [!DNL Workfront Proof].

Es gibt jedoch einige Schritte, die Sie unternehmen können, um Ihre Verbindungsgeschwindigkeit zu überprüfen, wodurch die Ursache der Probleme, die Sie erleben, ermittelt werden kann. Alle diese Schritte sind für die Fehlerbehebung gleichermaßen wichtig, und wir möchten Sie ermutigen, sich die Zeit zu nehmen, Informationen über alle aufgelisteten Schritte zu sammeln, um eine möglichst genaue Diagnose des Problems zu gewährleisten.

Wenn Sie alle Details erfasst haben, empfehlen wir Ihnen, sich mit Ihrer lokalen IT-Abteilung in Verbindung zu setzen, um lokale Probleme zu ermitteln.

## Festlegen, welcher Teil des Systems langsam ist

Wenn Sie [!DNL Workfront Proof] verwenden, arbeiten Sie möglicherweise mit dem Dashboard, z. B. mit der Verwaltung von Ordnerinhalten und Benutzern, oder mit dem Viewer [!DNL Workfront Proof]: Durchführen einer Überprüfung des Testversands, Überprüfen der bereits abgegebenen Kommentare usw.

Die Ermittlung des genauen Teils des Systems ist ein erster Schritt zur Fehlerbehebung bei Geschwindigkeitsproblemen. Wenn Sie [!DNL Workfront Proof] als langsam melden, beschreiben Sie Folgendes:

* Sind Sie auf anderen Webseiten langsam?
* Tritt das Problem im Dashboard oder im [!DNL Workfront Proof] Viewer auf?
* Welcher genaue Teil des Systems ist langsam? (z. B. Verarbeitung eines neuen Testversands oder Öffnen eines Kommentars im [!DNL Workfront Proof] Viewer)

## Ausführen von Traceroute- und Ping-Tests

Wenn Leistungsprobleme auftreten, ist es wichtig, den traceroute -Befehl auszuführen, um die Verbindung zu überprüfen. Öffnen Sie dazu die Eingabeaufforderung in Ihrem System (Terminal in Mac/Linux) und führen Sie die folgenden Schritte aus:

1. Geben Sie einen der folgenden Werte ein und warten Sie, bis das Tracerout abgeschlossen ist:

   * Windows: **track app.proofhq.com**
   * Mac/Linux: **traceroute app.proofhq.com**

1. (Nur Windows) Geben Sie **ping app.proofhq.com** ein.
1. Wenn der Ping abgeschlossen ist, klicken Sie mit der rechten Maustaste in die Eingabeaufforderung und wählen Sie Alle aus.
1. Kopieren Sie die Ergebnisse und fügen Sie sie in die Antwort auf Ihre E-Mail ein.
Stellen Sie sicher, dass Sie die Fertigstellung von Traceroute und Ping zulassen, bevor Sie die Ergebnisse an das Supportteam senden.

## Testen der Verbindungsgeschwindigkeit mit Speedtest.net

1. Öffnen Sie einen Browser und navigieren Sie zu Speedtest.net.
1. Befolgen Sie die Anweisungen in der Speedtest Wissensdatenbank, um die Geschwindigkeit Ihrer Internetverbindung zu testen.
1. Kopieren Sie die Ergebnisse und fügen Sie sie in eine E-Mail an unser Supportteam ein.

## Überprüfen Sie die Registerkarte &quot;Netzwerk&quot;in der Browser-Konsole

Die in modernen Browsern verfügbare Web-Konsole erfasst nützliche Informationen über Netzwerklatenzen, was uns bei der Ermittlung der Ursache für die Probleme mit der Geschwindigkeit, mit der Sie konfrontiert sind, hilft.

So überprüfen Sie die Ladezeiten für eine Webseite:

1. Öffnen Sie die Konsole Ihres Browsers und die Registerkarte Netzwerk .
1. Laden Sie die Seite erneut.
1. Erstellen Sie Screenshots oder zeichnen Sie einen Screencast der Ergebnisse auf.
1. Teilen Sie die Ergebnisse mit dem Supportteam.

Stellen Sie sicher, dass im Screenshot alle Daten angezeigt werden. Sie können das Konsolenfenster erweitern, wenn Sie einen Screenshot machen oder in einem Screencast nach unten scrollen.

Detaillierte Anweisungen finden Sie auch in der Dokumentation Ihres Browsers.

## Überprüfen Sie Ihre Verbindung auf einem anderen Netzwerk und Computer.

Die Überprüfung, ob bei der Verbindungsgeschwindigkeit mit einem anderen Gerät oder Netzwerk dasselbe Problem auftritt, ist ein wichtiger Schritt im Prozess der Fehlerbehebung. Versuchen Sie, zu einem anderen Computer oder Mobilgerät zu wechseln und versuchen Sie, ein anderes Netzwerk (z. B. mobile Daten) zu verwenden.

Vergleichen Sie die Verbindung in unterschiedlichen Kombinationen: Verwenden Sie einen anderen Computer im selben Netzwerk, verwenden Sie denselben Computer in einem anderen Netzwerk und verwenden Sie sowohl alternative Computer als auch Netzwerk, und teilen Sie dann die Ergebnisse mit dem Supportteam.
