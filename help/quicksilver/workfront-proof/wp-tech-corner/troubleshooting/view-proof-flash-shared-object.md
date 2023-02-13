---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Probleme bei der Anzeige von Testsendungen - Erläuterung von freigegebenen Objekten für Flash
description: "Hinweis: Die Informationen in diesem Artikel beziehen sich auf Funktionen, die derzeit nicht mehr unterstützt werden und aus [!DNL Workfront] 2018. Es wird empfohlen, den neuen Web Proofing Viewer (wie unter Testsendungen im Web Proofing Viewer überprüfen beschrieben) oder den Desktop Proofing Viewer (wie unter Testsendungen im Desktop Proofing Viewer beschrieben) zu verwenden."
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f1f3561e-8660-4c1e-b48f-446eb0eaac06
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Probleme bei der Anzeige von Testsendungen - [!DNL Flash] Freigegebene Objekte - Erklärung

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen in [!DNL Adobe Workfront], siehe [Testversand](../../../review-and-approve-work/proofing/proofing.md).

>[!NOTE]
>
>Die Informationen in diesem Artikel beziehen sich auf Funktionen, die derzeit nicht mehr unterstützt werden und aus [!DNL Workfront] 2018. Es wird empfohlen, den neuen Web Proofing-Viewer zu verwenden (wie hier beschrieben: [Überprüfen von Testsendungen im Web Proofing-Viewer](https://support.workfront.com/hc/en-us/sections/115000275214-Reviewing-Proofs-in-the-Web-Proofing-Viewer)) oder dem Desktop Proofing Viewer (wie unter [Überprüfen von Testsendungen im Desktop Testversand-Viewer](https://support.workfront.com/hc/en-us/sections/360000686434-Reviewing-Proofs-in-the-Desktop-Proofing-Viewer)).

## [!DNL Flash] Freigegebene Objekte

Lokales freigegebenes Objekt, manchmal auch als[!DNL Flash] Cookie&quot; ist eine Datendatei, die auf Ihrem Computer von den besuchten Sites erstellt werden kann. Gemeinsame Objekte werden meist verwendet, um das Surfen im Internet zu verbessern. A [!DNL Flash] -Cookie ist eine Meldung, die in [!DNL Adobe Flash] wird von einem Webserver an einen Webbrowser gesendet und dann als Datendatei im Browser gespeichert.

Seit [!DNL Workfront Proof] Der Viewer basiert auf [!DNL Flash], wäre es sinnvoll zu überprüfen, für welchen Speicher es zulässig ist [!DNL Flash] Anwendungen auf Ihrem Computer.

## [!DNL Flash] Freigegebene Objekte - bekannte Probleme

Wenn die Variable [!DNL Flash] Speicher auf 0 KB festgelegt ist oder eine andere Einstellung hat, die blockiert [!DNL Flash] -Anwendungen die Daten nicht lokal speichern, kann dies zu bekannten Problemen in der [!DNL Workfront Proof] Betrachter:

* Das Popup &quot;Erste Schritte&quot;der Tour wird weiterhin angezeigt, obwohl die Option, sie nicht erneut anzuzeigen, ausgewählt wurde
* [!DNL Workfront Proof] Die Viewer-Leistung verlangsamt sich aufgrund der zunehmenden Anzahl von Kommentaren, die zu den Testsendungen hinzugefügt werden
* Testsendungen werden nicht geladen und Sie erhalten den &quot;grauen Bildschirm&quot;anstelle eines tatsächlichen Bildes.

## Zulassen [!DNL Flash] Freigegebene Objekte

Stellen Sie sicher, dass Sie [!DNL Flash] Freigegebene Objekte sind auf dem Computer zulässig und die Speicherbegrenzung beträgt nicht 0.

So überprüfen Sie, ob die freigegebenen Objekte zulässig sind:

1. Klicken Sie mit der rechten Maustaste auf die [!DNL Workfront Proof] Viewer.
1. Auswählen **[!UICONTROL Globale Einstellungen]** aus dem Kontextmenü aus.
1. Navigieren Sie zu **[!UICONTROL Speicherung]** Registerkarte.
1. Stellen Sie sicher, dass **[!UICONTROL Speichern von Informationen auf diesem Computer durch Websites zulassen]** ausgewählt ist (1).
1. ![2017-06-09_1929.png](assets/2017-06-09-1929-350x267.png)

## Erhöhen [!DNL Flash] Speicher

Standardmäßig [!DNL Flash] -Anwendungen können bis zu 100 KB Daten auf dem Laufwerk des Benutzers speichern, dies kann jedoch von den Benutzern einfach geändert werden. Die Lösung für die vielen [!DNL Flash] damit zusammenhängende Fragen die interne [!DNL Flash] Speicher. Dies kann direkt über die [!DNL Workfront Proof] Betrachter:

1. Öffnen Sie einen Testversand.
1. Öffnen Sie das Kontextmenü des Testversands.
1. Klicken **[!UICONTROL Einstellungen]** , um [!DNL Flash] -Einstellungen.
1. Navigieren Sie zu **[!UICONTROL Lokal]** Speicherregisterkarte.
1. Erhöhen Sie den Speicher auf z. B. 100 KB (1).
1. Schließen Sie das Einstellungsfenster und öffnen Sie den Testversand erneut.

![2017-06-09_1926.png](assets/2017-06-09-1926-350x274.png)
