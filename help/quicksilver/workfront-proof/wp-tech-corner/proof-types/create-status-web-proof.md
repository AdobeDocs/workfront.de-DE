---
product-previous: workfront-proof
product-area: documents
navigation-topic: proof-types
title: Erstellen Sie einen statischen Website-Korrekturabzug mit [!DNL Workfront Proof]
description: Sie können von Ihren Web-Seiten aus statische Korrekturabzüge erstellen. Darüber hinaus können Sie verschiedene Geräte simulieren, indem Sie die Bildschirmauflösung der Aufnahmen definieren.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b93ed288-1bf2-4268-96c3-6263ab6be633
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Erstellen eines statischen Website-Korrekturabzugs mit [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf Funktionen im eigenständigen [!DNL Workfront Proof]. Informationen zu Proofing in [!DNL Adobe Workfront] finden Sie unter [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Sie können von Ihren Web-Seiten aus statische Korrekturabzüge erstellen. Darüber hinaus können Sie verschiedene Geräte simulieren, indem Sie die Bildschirmauflösung der Aufnahmen definieren.

## Erstellen eines statischen Website-Korrekturabzugs

1. Öffnen Sie die Seite [!UICONTROL Neuer Korrekturabzug], wie unter [Erstellen von Korrekturabzügen in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) beschrieben.
1. Fügen Sie Ihre URL in das Feld **www.shareyourlink.com** ein oder geben Sie sie ein.
1. Sie können diesen Schritt wiederholen, um mehrere URLs hinzuzufügen.
1. Klicken Sie direkt unter diesem Feld auf die Auflösung (standardmäßig 1366 x 768) und wählen Sie dann im Feld **[!UICONTROL Bildschirmfoto-Auflösung]** die gewünschten Auflösungen aus.
Wählen Sie eine niedrigere Auflösung aus, wenn Sie Designs für Mobilgeräte prüfen möchten. Im Allgemeinen werden Designs gemäß der Bildschirm-/Browser-Fensterauflösung geladen.

1. Klicken Sie **[!UICONTROL Nach Unterseiten suchen]**, wenn Sie verbundene Seiten einbeziehen möchten, die sich in derselben Domain/Subdomain wie die eingegebene URL befinden.
   [!DNL Workfront Proof] scannt die verbundenen Seiten und listet sie unter der Option **[!UICONTROL Nach Unterseiten suchen]** auf. Sie können die Seiten auswählen, die Sie einbeziehen möchten.

1. Mit der Funktion [!UICONTROL Testsendungen kombinieren] können Sie alle Web-Seiten als einen einzigen mehrseitigen Testversand senden.
1. Klicken Sie **[!UICONTROL Fertig]** und schließen Sie dann die Konfiguration Ihres Korrekturabzugs ab, wie unter [Erstellen von Korrekturabzügen in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) beschrieben.

## Über kennwortgeschützte Seiten und Seiten, die autorisiert werden müssen

[!DNL Workfront Proof] können eine kennwortgeschützte Website nicht als statischen Korrekturabzug erfassen.

Um Korrekturabzüge von Seiten zu erstellen, für die eine Autorisierung erforderlich ist, muss Ihr IT-Team eine der folgenden URLs zur -Zulassungsliste Ihres Unternehmens hinzufügen, über die sich unser Web-Erfassungs-Tool verbindet:

**AWS-Cluster in den USA**: webcapture.proofhq.com

**GCP-Cluster in den USA**: webcapture.gcp.proofhq.com

**EMEA-Cluster**: webcollection.proofhq.eu

>[!NOTE]
>
>Wir empfehlen interaktives Proofing anstelle eines statischen Proofings für interne Seiten, die eine Autorisierung erfordern, und kennwortgeschützte Websites. Weitere Informationen finden Sie unter [Übersicht über Korrekturabzüge für interaktive Inhalte](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

## Informationen zur Verarbeitung statischer Website-Testsendungen

* Animationen, eingebettete Videos, Skripte und Interaktionen können nicht in statische Website-Korrekturabzüge eingeschlossen werden. Wenn Sie interaktive Inhalte prüfen möchten, lesen Sie [Korrekturabzüge generieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) in [Korrekturabzüge generieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

* Korrekturabzugseiten werden im Allgemeinen mit einer Rate von etwa 20 Sekunden pro Seite vorbereitet und erfasst. Die gesamte Vorbereitungszeit hängt jedoch auch von den Servern ab, auf denen die Seiten gehostet werden. Das Tool wartet 60 Sekunden, bis jede gesendete URL geladen wird. Wenn diese Wartezeit überschritten wird, schlägt der Korrekturabzug fehl.
* Wenn bei kombinierten Korrekturabzügen eine der URLs nicht auf das Erfassungs-Tool reagiert, schlägt der Korrekturabzug fehl.
* [!DNL Workfront Proof] erfasst Web-Seiten mit einer Länge von bis zu 195 Zoll nach dem Rastern. Wenn die Web-Seite länger als diese ist, schlägt der Korrekturabzug fehl.
* Textextraktion ist für alle Textelemente verfügbar, als Bilder platzierter Text wird jedoch nicht extrahiert.
* Auf die Korrekturabzüge können Sie auf Text-Hyperlinks klicken, und die verknüpften Seiten werden in den neuen Browser-Registerkarten geöffnet.
* Auf Hyperlinks auf den Bildern kann nicht geklickt werden, wenn die style=„display:block“-Elemente innerhalb der `<a>` Tags verwendet werden. Es wird empfohlen, diese Teile des Seiten-Designs anzupassen.
* Um optimale Ergebnisse zu erzielen, empfehlen wir, die Seiten unter Verwendung der besten Kodierungsverfahren und anerkannten Standards zu erstellen.
