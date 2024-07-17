---
product-previous: workfront-proof
product-area: documents
navigation-topic: proof-types
title: Erstellen eines statischen Website-Testversands mit  [!DNL Workfront Proof]
description: Sie können statische Testsendungen aus Ihren Webseiten erstellen. Zusätzlich können Sie verschiedene Geräte simulieren, indem Sie die Bildschirmauflösung der Aufnahmen definieren.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b93ed288-1bf2-4268-96c3-6263ab6be633
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Erstellen eines statischen Website-Testversands mit [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Sie können statische Testsendungen aus Ihren Webseiten erstellen. Zusätzlich können Sie verschiedene Geräte simulieren, indem Sie die Bildschirmauflösung der Aufnahmen definieren.

## Erstellen eines statischen Website-Testversands

1. Öffnen Sie die Seite [!UICONTROL Neuer Testversand], wie unter [Testsendungen in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) generieren beschrieben.
1. Fügen Sie Ihre URL in das Feld **www.shareyourlink.com** ein oder geben Sie sie ein.
1. Sie können diesen Schritt wiederholen, um mehrere URLs hinzuzufügen.
1. Klicken Sie direkt unter diesem Feld auf die Auflösung (der Standardwert ist 1366x768) und wählen Sie dann die gewünschten Auflösungen im Feld **[!UICONTROL Bildschirmauflösung]** aus.
Wählen Sie eine kleinere Auflösung aus, wenn Sie Designs für Mobilgeräte testen möchten. Im Allgemeinen werden Designs gemäß der Auflösung des Bildschirms/Browser-Fensters geladen.

1. Klicken Sie auf **[!UICONTROL Suchen nach Unterseiten]** , wenn Sie verbundene Seiten einbeziehen möchten, die sich in derselben Domäne/Subdomäne wie die eingegebene URL befinden.
   [!DNL Workfront Proof] scannt die verbundenen Seiten und listet sie unter der Option **[!UICONTROL Suchen nach Unterseiten]** auf. Sie können die Seiten auswählen, die Sie einbeziehen möchten.

1. Mit der Funktion [!UICONTROL Testsendungen kombinieren] können Sie alle Webseiten als einen einzigen mehrseitigen Testversand senden.
1. Klicken Sie auf **[!UICONTROL Fertig]** und konfigurieren Sie dann Ihren Testversand wie unter [Testsendungen in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) generieren beschrieben.

## Über kennwortgeschützte Seiten und Seiten, für die eine Autorisierung erforderlich ist

[!DNL Workfront Proof] kann eine kennwortgeschützte Website nicht als statischen Testversand erfassen.

Um Testsendungen von Seiten zu erstellen, für die eine Autorisierung erforderlich ist, muss Ihr IT-Team eine der folgenden URLs zur Zulassungsliste Ihres Unternehmens hinzufügen, über die unser Weberfassungs-Tool eine Verbindung herstellt:

**AWS-Cluster in den USA**: webcapture.proofhq.com

**GCP-Cluster in den USA**: webcapture.gcp.proofhq.com

**EMEA-Cluster**: webCapture.proofhq.eu

>[!NOTE]
>
>Für interne Seiten, für die eine Autorisierung und kennwortgeschützte Websites erforderlich sind, empfehlen wir interaktive Testsendungen anstelle statischer Testsendungen. Weitere Informationen finden Sie unter [Übersicht über interaktive Inhaltsanalysen](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

## Über die Verarbeitung von statischen Website-Testsendungen

* Animationen, eingebettete Videos, Skripte und Interaktionen können nicht in Testsendungen für statische Websites enthalten sein. Informationen zum Testen interaktiver Inhalte finden Sie unter [Testsendungen in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) generieren in [Testsendungen in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

* Testseiten werden im Allgemeinen mit einer Geschwindigkeit von etwa 20 Sekunden pro Seite vorbereitet. Die Gesamtvorbereitungszeit hängt jedoch auch von den Servern ab, auf denen die Seiten gehostet werden. Das Tool wartet 60 Sekunden, bis jede gesendete URL geladen wird. Wenn diese Wartezeit überschritten wird, schlägt der Testversand fehl.
* Wenn bei kombinierten Testsendungen eine der URLs nicht auf das Erfassungswerkzeug reagiert, schlägt der Testversand fehl.
* [!DNL Workfront Proof] erfasst Webseiten mit einer Länge von bis zu 195 Zoll nach dem Rastern. Wenn die Webseite länger ist, schlägt der Testversand fehl.
* Die Textextraktion ist für alle Textelemente verfügbar, aber Text, der als Bilder platziert wird, wird nicht extrahiert.
* Text-Hyperlinks können in den Testsendungen angeklickt werden und die verknüpften Seiten werden in den neuen Browser-Registerkarten geöffnet.
* Hyperlinks in den Bildern können nicht angeklickt werden, wenn die style=&quot;display:block&quot;-Elemente innerhalb der `<a>` -Tags verwendet werden. Es wird empfohlen, diese Teile des Seitenentwurfs anzupassen.
* Um optimale Ergebnisse zu erzielen, empfehlen wir, die Seiten mit den besten Kodierungspraktiken und anerkannten Standards zu erstellen.
