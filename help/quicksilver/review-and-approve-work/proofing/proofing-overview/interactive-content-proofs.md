---
product-area: documents
navigation-topic: proofing-overview
title: Übersicht über interaktive Inhaltsanalysen
description: Interaktive Inhalte bieten mehrere Methoden zum Interagieren von Viewern. Agenturen können den Erfolg ihrer Kampagnen mithilfe von Analysen messen, die aus Antworten auf diesen Inhalt gewonnen wurden.
author: Courtney
feature: Digital Content and Documents
exl-id: fdcad9c6-5508-476a-bfb8-2fe3bfbb007b
source-git-commit: 45dac4c5e8ff584546783d561c04d137697a03a4
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# Übersicht über interaktive Inhaltsanalysen

<!-- Audited: 01/2024 -->

Interaktive Inhalte bieten mehrere Methoden zum Interagieren von Viewern. Agenturen können den Erfolg ihrer Kampagnen mithilfe von Analysen messen, die aus Antworten auf diesen Inhalt gewonnen wurden.

Beispiele für interaktive Inhalte:

* Websites
* Eingebettete oder Streaming-Videos
* Interaktive Banner
* HTML5 Animationen
* Microsites
* Interaktive E-Mails

## Über die Erstellung von Testsendungen für interaktive Inhalte

Sie können einen Testversand für interaktive Inhalte auf eine der folgenden Arten erstellen:

* Erstellen Sie einen Testversand aus einer ZIP-Datei, die den interaktiven Inhalt enthält.

  Adobe Workfront entpackt den Inhalt aus der ZIP-Datei und speichert ihn auf einem Workfront-Server. Da der Inhalt auf diese Weise gespeichert wird, können Sie sich darauf verlassen, dass der Inhalt während des gesamten Prüfzyklus des Testversands gleich bleibt.

* Geben Sie die URL für den Inhalt an.

  Dies ist die einfachste Möglichkeit, einen Testversand für interaktive Inhalte zu erstellen. Dies ist auch die einzige Möglichkeit, Ihre Inhalte interaktiv zu überprüfen, da sie von Benutzern im Internet genutzt werden.

  Bei diesem Ansatz speichert und hostet ein externer Server, der Workfront nicht bekannt ist, den Inhalt.

  Wir empfehlen diese Methode für große Websites, da es schwierig ist, alle Dateien zu sammeln, aus denen eine große Website besteht. Da der Testversand-Inhalt jedoch extern gespeichert wird, kann Workfront ihn nicht vor Änderungen schützen, die von den daran arbeitenden Entwicklern vorgenommen wurden. Daher können Sie sich möglicherweise nicht darauf verlassen, dass der Inhalt während des gesamten Prüfzyklus des Testversands gleich bleibt.

## Informationen zum Vorbereiten von interaktiven Inhalten in einer ZIP-Datei für die Prüfung

Wenn Sie interaktive Inhalte in einer ZIP-Datei zum Testen bündeln, stellen Sie sicher, dass sie die folgenden Spezifikationen enthält:

* Alle Assets wie CSS, JavaScript, Videos, Sounds und Bilder sollten in die Bundle-Datei aufgenommen werden.
* Interaktive Inhalte sollten die Hauptdatei (index.html, index.htm) enthalten. Wenn sich diese Datei nicht im Stammverzeichnis befindet, durchsucht das Tool automatisch den Ordner, um ihn zu finden. Die Hauptdatei muss nicht index.html/index.htm heißen. Es kann jedoch nur eine .html/.htm-Datei am Hauptspeicherort platziert werden.
* Die Datei muss mindestens eine statische Datei-Webseite enthalten.
* Die maximale Bundle-Größe beträgt 500 MB.
* Bei in iOS erstellten ZIP-Dateien identifiziert das Tool automatisch den Ordner, in dem sich der Inhalt befindet.
* Interaktive Projekte werden nur als ZIP-Archive unterstützt. Standardmäßige .zip-Dateiübermittlungen schlagen fehl.
* Die Website muss sicher sein (HTTPS).

  Dies ist bei Verwendung des Desktop Proofing Viewers nicht erforderlich.

  Weitere Informationen finden Sie unter [Grundlegendes zum Desktop Proofing Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

* Die Website muss in einem iframe angezeigt werden dürfen.

  Dies ist bei Verwendung des Desktop Proofing Viewers nicht erforderlich.

  Weitere Informationen finden Sie unter [Grundlegendes zum Desktop Proofing Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

## Über die Erstellung eines interaktiven Testversands

Nachdem Sie die ZIP-Bundle-Datei vorbereitet haben, erstellen Sie einen interaktiven Testversand.

Weitere Informationen finden Sie unter [Erstellen eines Testversands für interaktive Inhalte in einer ZIP-Datei](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content-.md).

Wenn Sie Workfront Testversand verwenden, lesen Sie den Abschnitt . [Erstellen eines Testversands für interaktive Inhalte](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md#generate-a-proof-for-interactive-content) im Artikel [Testsendungen in Workfront Testversand generieren](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Über die Überprüfung interaktiver Testsendungen

Es wird empfohlen, den Standalone Desktop Proofing Viewer als Standard-Viewer für interaktive Testsendungen zu verwenden. Wenn die Richtlinien Ihres Unternehmens jedoch die Verwendung der Desktop Proofing Viewer-App nicht zulassen, kann Ihr Workfront-Administrator Ihr System so konfigurieren, dass Sie interaktive Inhalte, die in einer ZIP-Archivdatei enthalten sind, im Web Proofing Viewer überprüfen können. Vergleichsinformationen zum Desktop Proofing Viewer und zum Web Proofing Viewer finden Sie unter [Unterschiede zwischen dem Web Proofing Viewer und dem Desktop Proofing Viewer - Übersicht](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).
