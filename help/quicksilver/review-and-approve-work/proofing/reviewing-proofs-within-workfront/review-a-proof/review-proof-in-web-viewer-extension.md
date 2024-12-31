---
product-area: documents
navigation-topic: proofing-overview
title: Überprüfen interaktiver Inhalte in der Web Proofing Viewer-Erweiterung
description: Das Adobe Workfront-Überprüfungs-Tool ist eine Browser-Erweiterung, mit der Sie interaktive Inhalte in einer ZIP-Datei oder mit einer URL prüfen können.
author: Courtney
feature: Digital Content and Documents
exl-id: 4fea13cc-2d56-466e-8851-6134782e7e80
source-git-commit: 9bc1502149d99624d8494aef86e11e18a95f563b
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 1%

---

# Überprüfen interaktiver Inhalte mit dem Adobe Workfront-Überprüfungs-Tool

<span class="preview">Das Adobe Workfront Review-Tool ist ab dem 7. November 2024 verfügbar. Diese Erweiterung befindet sich derzeit in der Betaphase.</span>

Das Adobe Workfront-Überprüfungs-Tool ist eine Web-basierte Browser-Erweiterung, mit der Sie interaktive Inhalte in einer ZIP-Datei oder mit einer URL prüfen können. Das Adobe Workfront-Überprüfungs-Tool ist in den folgenden Browsern verfügbar:

* Firefox
* Chrome
* Edge

Es wird empfohlen, den Desktop Proofing Viewer zu verwenden, wenn sich der zu überprüfende Inhalt auf einer Website befindet, die

* Erfordert SSO-Authentifizierung
* Eröffnet ihre Website in iFrames, wie Figma



## Festlegen des Adobe Workfront-Überprüfungs-Tools als Standard-Viewer für URL- und ZIP-Korrekturabzüge

Um das Web-Überprüfungs-Tool für URL- und ZIP-Korrekturabzüge zu verwenden, muss ein Workfront-Administrator die Standardeinstellung für interaktive Korrekturabzüge anpassen.

1. Klicken Sie im Hauptmenü von Workfront auf **Proofing**.
1. Klicken Sie **Kontoeinstellungen** und dann auf die Registerkarte **Einstellungen**.
1. Suchen Sie im Abschnitt **Standardeinstellungen für** Desktop Proofing Viewer **interaktives Proofing** und klicken Sie auf **Setup**.
1. Wählen Sie im Dropdown-Menü &quot;**&quot;**. Interaktive Korrekturabzüge, die aus einer URL- oder ZIP-Datei erstellt wurden, werden jetzt automatisch im Adobe Workfront-Überprüfungs-Tool, einem Web-basierten Browser, geöffnet.
1. Klicken Sie auf **Speichern**.

>[!NOTE]
>
>Diese Änderung gilt für alle interaktiven Korrekturabzüge in Ihrer Vorschau- und Produktionsumgebung. Es wird empfohlen, das neue Erlebnis in der Vorschau-Umgebung zu testen, bevor es in der Produktionsumgebung aktiviert wird. Sie können einfach zum Desktop-Viewer zurückkehren, indem Sie die Kontoeinstellung wieder auf &quot;**für alle interaktiven Korrekturabzüge aktiviert“**.

## Festlegen des Adobe Workfront-Überprüfungs-Tools als Standard-Viewer nur für ZIP-Korrekturabzüge

Um das Web-Überprüfungs-Tool nur für ZIP-Korrekturabzüge zu verwenden, muss ein Workfront-Administrator die Standardeinstellung für interaktive Korrekturabzüge anpassen.

1. Klicken Sie im Hauptmenü von Workfront auf **Proofing**.
1. Klicken Sie **Kontoeinstellungen** und dann auf die Registerkarte **Einstellungen**.
1. Suchen Sie im Abschnitt **Standardeinstellungen für** Desktop Proofing Viewer **interaktives Proofing** und klicken Sie auf **Setup**.
1. Wählen Sie im Dropdown-Menü **Nur für interaktive Korrekturabzüge aktivieren, die aus einer URL erstellt wurden** aus. Interaktive Korrekturabzüge, die aus einer ZIP-Datei erstellt wurden, werden jetzt automatisch im Adobe Workfront-Überprüfungs-Tool geöffnet, einem Web-basierten Browser. Interaktive Korrekturabzüge, die von einer URL erstellt wurden, werden weiterhin im Desktop Proofing Viewer geöffnet.
1. Klicken Sie auf **Speichern**.

>[!NOTE]
>
>Diese Änderung gilt für alle interaktiven Korrekturabzüge in Ihrer Vorschau- und Produktionsumgebung. Es wird empfohlen, das neue Erlebnis in der Vorschau-Umgebung zu testen, bevor es in der Produktionsumgebung aktiviert wird. Sie können einfach zum Desktop-Viewer zurückkehren, indem Sie die Kontoeinstellung wieder auf &quot;**für alle interaktiven Korrekturabzüge aktiviert“**.

## Installieren der Erweiterung

Reviewer und genehmigende Personen müssen das Adobe Workfront-Überprüfungs-Tool installieren. in einem der folgenden Browser:

* [Firefox-Erweiterung](https://addons.mozilla.org/en-US/firefox/addon/adobe-workfront-review-tool/)

* [Chrome-Erweiterung](https://chromewebstore.google.com/detail/adobe-workfront-review-to/lhdepbgeilldghlfnankdnponhljpgml)

* [Edge](https://microsoftedge.microsoft.com/addons/detail/adobe-workfront-review-to/llhapmaiiddmcamgeapaipjpagnoijen)

Nach der Installation der Erweiterung werden interaktive Korrekturabzüge automatisch im Adobe Workfront-Überprüfungs-Tool geöffnet.

>[!IMPORTANT]
>
>Sie müssen die veraltete Web-Viewer-Erweiterung entfernen, um das Adobe Workfront-Überprüfungs-Tool verwenden zu können.
