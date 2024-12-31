---
product-area: documents
navigation-topic: proofing-overview
title: Übersicht über Korrekturabzüge für interaktive Inhalte
description: Interaktive Inhalte bieten verschiedene Methoden, um Betrachter anzusprechen. Agenturen können den Erfolg ihrer Kampagnen mithilfe von Analysen messen, die aus Antworten auf diesen Inhalt gesammelt wurden.
author: Courtney
feature: Digital Content and Documents
exl-id: fdcad9c6-5508-476a-bfb8-2fe3bfbb007b
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# Übersicht über Korrekturabzüge für interaktive Inhalte

<!-- Audited: 01/2024 -->

Interaktive Inhalte bieten verschiedene Methoden, um Betrachter anzusprechen. Agenturen können den Erfolg ihrer Kampagnen mithilfe von Analysen messen, die aus Antworten auf diesen Inhalt gesammelt wurden.

Beispiele für interaktive Inhalte:

* Websites
* Eingebettete oder Streaming-Videos
* Interaktive Banner
* HTML5-Animationen
* Microsites
* Interaktive E-Mails

## Informationen zum Erstellen von Testsendungen für interaktive Inhalte

Sie können einen Korrekturabzug für interaktive Inhalte auf eine der folgenden Arten erstellen:

* Erstellen Sie einen Korrekturabzug aus einer ZIP-Datei, die den interaktiven Inhalt enthält.

  Adobe Workfront entpackt den Inhalt aus der ZIP-Datei und speichert ihn auf einem Workfront-Server. Da sie auf diese Weise gespeichert wird, können Sie sich darauf verlassen, dass die Inhalte während des gesamten Prüfzyklus des Korrekturabzugs gleich bleiben.

* Geben Sie die URL für den Inhalt an.

  Dies ist die einfachste Möglichkeit, einen Korrekturabzug für interaktive Inhalte zu erstellen. Dies ist auch die einzige Möglichkeit, Ihre Inhalte interaktiv zu überprüfen, wenn Benutzer sie im Internet sehen.

  Bei diesem Ansatz speichert und hostet ein externer Server, der Workfront nicht bekannt ist, den Inhalt.

  Wir empfehlen diese Methode für große Websites, da es schwierig ist, alle Dateien einer großen Website zu sammeln. Da der Inhalt des Korrekturabzugs jedoch extern gespeichert wird, kann Workfront ihn nicht vor Änderungen schützen, die von den Entwicklern vorgenommen werden, die daran arbeiten. Daher können Sie sich möglicherweise nicht darauf verlassen, dass der Inhalt während des gesamten Prüfungszyklus des Korrekturabzugs unverändert bleibt.

## Informationen zur Vorbereitung interaktiver Inhalte in einer ZIP-Datei für das Proofing

Wenn Sie interaktive Inhalte zum Proofing in einer ZIP-Datei bündeln, stellen Sie sicher, dass diese die folgenden Spezifikationen enthält:

* Alle Assets wie CSS, JavaScript, Videos, Sounds und Bilder sollten in der Bundle-Datei enthalten sein.
* Interaktive Inhalte sollten die Hauptdatei (index.html, index.htm) enthalten. Wenn diese Datei nicht im Stammverzeichnis abgelegt ist, durchsucht das Tool automatisch den Ordner, um ihn zu finden. Die Hauptdatei muss nicht index.html/index.htm heißen, es kann jedoch nur eine einzige .html/.htm Datei am Hauptspeicherort sein.
* Die Datei muss mindestens eine statische Datei-Webseite enthalten.
* Die maximale Bundle-Größe beträgt 500 MB.
* Bei in iOS erstellten ZIP-Dateien erkennt das Tool automatisch den Ordner, in dem sich die Inhalte befinden.
* Interaktive Projekte werden nur als ZIP-Archive unterstützt. Standardmäßige ZIP-Dateiübermittlungen schlagen fehl.
* Die Website muss sicher sein (HTTPS).

  Dies ist bei Verwendung des Desktop Proofing Viewers nicht erforderlich.

  Weitere Informationen finden Sie unter [Grundlegendes zur Desktop Proofing Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

* Die Website muss in einem iframe angezeigt werden dürfen.

  Dies ist bei Verwendung des Desktop Proofing Viewers nicht erforderlich.

  Weitere Informationen finden Sie unter [Grundlegendes zur Desktop Proofing Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

## Informationen zum Erstellen eines interaktiven Korrekturabzugs

Nachdem Sie Ihre ZIP-Bundle-Datei vorbereitet haben, erstellen Sie einen interaktiven Korrekturabzug.

Weitere Informationen finden Sie unter [Erstellen eines Korrekturabzugs für interaktive Inhalte in einer ZIP-Datei](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content.md).

Wenn Sie Workfront Proof verwenden, lesen Sie den Abschnitt [Erstellen eines Testversands für interaktive Inhalte](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md#generate-a-proof-for-interactive-content) im Artikel [Erstellen von Testsendungen in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Über die Überprüfung interaktiver Korrekturabzüge

Es wird empfohlen, den eigenständigen Desktop Proofing Viewer als Standard-Viewer für interaktive Korrekturabzüge zu verwenden. Wenn die Richtlinien Ihres Unternehmens jedoch die Verwendung der Desktop Proofing Viewer-App nicht zulassen, kann Ihr Workfront-Administrator Ihr System so konfigurieren, dass Sie interaktive Inhalte, die in einer ZIP-Archivdatei gebündelt sind, im Web Proofing Viewer überprüfen können. Vergleichende Informationen zum Desktop Proofing Viewer und zum Web Proofing Viewer finden Sie [Unterschiede zwischen dem Web Proofing Viewer und dem Desktop Proofing Viewer - Übersicht](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).
