---
product-area: documents
navigation-topic: proofing-overview
title: Überprüfen interaktiver Inhalte in der Web-Proofing-Viewer-Erweiterung
description: Das Adobe Workfront-Überprüfungstool ist eine Browsererweiterung, mit der Sie interaktive Inhalte in einer ZIP-Datei oder mit einer URL testen können.
author: Courtney
feature: Digital Content and Documents
exl-id: 4fea13cc-2d56-466e-8851-6134782e7e80
source-git-commit: 9bc1502149d99624d8494aef86e11e18a95f563b
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 1%

---

# Überprüfen interaktiver Inhalte mit dem Adobe Workfront-Überprüfungstool

<span class="preview">Das Adobe Workfront-Überprüfungstool ist ab dem 7. November 2024 verfügbar. Diese Erweiterung befindet sich derzeit in der Betaphase.</span>

Das Adobe Workfront-Überprüfungstool ist eine webbasierte Browsererweiterung, mit der Sie interaktive Inhalte in einer ZIP-Datei oder mit einer URL testen können. Das Adobe Workfront-Überprüfungstool ist in den folgenden Browsern verfügbar:

* Firefox
* Chrome
* Edge

Es wird empfohlen, den Desktop Proofing Viewer zu verwenden, wenn sich der zu überprüfende Inhalt auf einer Website befindet, die

* SSO-Authentifizierung erforderlich
* Ermöglicht das Öffnen der Website in iFrames, z. B. Figma



## Adobe Workfront-Überprüfungs-Tool zum Standard-Viewer für URL- und ZIP-Testsendungen machen

Um das Webüberprüfungs-Tool für URL- und ZIP-Testsendungen zu verwenden, muss ein Workfront-Administrator die Standardeinstellung für interaktive Testsendungen anpassen.

1. Klicken Sie im Hauptmenü von Workfront auf **Testversand**.
1. Klicken Sie auf **Kontoeinstellungen** und dann auf die Registerkarte **Einstellungen**.
1. Suchen Sie im Abschnitt **Testversand-Standardeinstellungen** nach **Desktop-Testversand-Viewer für interaktive Prüfung** und klicken Sie auf **Einrichten**.
1. Wählen Sie im Dropdown-Menü **Deaktiviert** aus. Interaktive Testsendungen, die über eine URL- oder ZIP-Datei erstellt wurden, werden jetzt automatisch im Adobe Workfront-Überprüfungs-Tool geöffnet, einem webbasierten Browser.
1. Klicken Sie auf **Speichern**.

>[!NOTE]
>
>Diese Änderung gilt für alle interaktiven Testsendungen in Ihrer Vorschau- und Produktionsumgebung. Es wird empfohlen, das neue Erlebnis in Ihrer Vorschau-Umgebung zu testen, bevor es in der Produktion aktiviert wird. Sie können einfach zum Desktop-Viewer zurückkehren, indem Sie die Kontoeinstellung für alle interaktiven Testsendungen auf **Aktiviert** zurücksetzen.

## Machen Sie das Adobe Workfront-Überprüfungstool zum standardmäßigen Viewer nur für ZIP-Testsendungen

Um das Webüberprüfungs-Tool nur für ZIP-Testsendungen zu verwenden, muss ein Workfront-Administrator die Standardeinstellung für interaktive Testsendungen anpassen.

1. Klicken Sie im Hauptmenü von Workfront auf **Testversand**.
1. Klicken Sie auf **Kontoeinstellungen** und dann auf die Registerkarte **Einstellungen**.
1. Suchen Sie im Abschnitt **Testversand-Standardeinstellungen** nach **Desktop-Testversand-Viewer für interaktive Prüfung** und klicken Sie auf **Einrichten**.
1. Wählen Sie im Dropdown-Menü **Nur für interaktive Testsendungen aktiviert aus, die über eine URL erstellt wurden**. Interaktive Testsendungen, die aus einer ZIP-Datei erstellt wurden, werden jetzt automatisch im Adobe Workfront-Überprüfungs-Tool geöffnet, einem webbasierten Browser. Interaktive Testsendungen, die über eine URL erstellt wurden, werden weiterhin im Desktop Proofing Viewer geöffnet.
1. Klicken Sie auf **Speichern**.

>[!NOTE]
>
>Diese Änderung gilt für alle interaktiven Testsendungen in Ihrer Vorschau- und Produktionsumgebung. Es wird empfohlen, das neue Erlebnis in Ihrer Vorschau-Umgebung zu testen, bevor es in der Produktion aktiviert wird. Sie können einfach zum Desktop-Viewer zurückkehren, indem Sie die Kontoeinstellung für alle interaktiven Testsendungen auf **Aktiviert** zurücksetzen.

## Installieren der Erweiterung

Überprüfer und Genehmiger müssen das Adobe Workfront-Überprüfungstool installieren. in einem der folgenden Browser:

* [Firefox-Erweiterung](https://addons.mozilla.org/en-US/firefox/addon/adobe-workfront-review-tool/)

* [Chrome-Erweiterung](https://chromewebstore.google.com/detail/adobe-workfront-review-to/lhdepbgeilldghlfnankdnponhljpgml)

* [Edge](https://microsoftedge.microsoft.com/addons/detail/adobe-workfront-review-to/llhapmaiiddmcamgeapaipjpagnoijen)

Nach der Installation der Erweiterung werden interaktive Testsendungen automatisch im Adobe Workfront-Überprüfungstool geöffnet.

>[!IMPORTANT]
>
>Sie müssen die ältere Web Viewer-Erweiterung entfernen, um das Adobe Workfront Review-Tool verwenden zu können.
