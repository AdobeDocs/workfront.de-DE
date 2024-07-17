---
product-area: documents
navigation-topic: proofing-overview
title: Dokumenterneuverarbeitung für Testversand - Übersicht
description: Wenn Sie ein Dokument (DOCX, PDF, XLSX, AI) zum Testen einreichen, verarbeitet Adobe Workfront es erneut, sodass es im Testversand-Viewer angezeigt werden kann, ohne dass Sie die Software-Anwendung zum Erstellen des Dokuments verwendet haben.
author: Courtney
feature: Digital Content and Documents
exl-id: e577fa71-4828-4fc2-93a2-0eddbb5ad2ad
source-git-commit: 332c744ab9b760268620461ed2cb2551caf383cf
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 0%

---

# Dokumenterneuverarbeitung für Testversand - Übersicht

Wenn Sie ein Dokument (DOCX, PDF, XLSX, AI) zum Testen einreichen, verarbeitet Adobe Workfront es erneut, sodass es im Testversand-Viewer angezeigt werden kann, ohne dass Sie die Software-Anwendung zum Erstellen des Dokuments verwendet haben. 

Jede Seite Ihres Dokuments wird im Testversand-Viewer als Miniaturbild angezeigt. Wenn Sie auf eine Miniaturansicht klicken, können Sie in eine Bitmap-Version dieser Seite mit 100 %, 200 % und 400 % zoomen. Bei Testsendungen mit einer Höhe oder Breite von mehr als 800 mm beträgt der maximale Zoomfaktor 200 %.

Die Farben in Ihrem Dokument werden in sRGB mit Farbkonvertierung aus der neuesten Adobe-Bibliothek angezeigt. Der Testversand-Viewer unterstützt alle in das Dokument eingebetteten ICC-Profile (International Color Consortium).

Der gesamte Schriftarttext wird in seiner Ebene extrahiert, sofern Sie beim Hochladen des Dokuments in das System die richtige Dateierweiterung angeben. Als Bilder oder Kurven eingeschlossenen Text wird nicht angezeigt.

>[!NOTE]
>
>Workfront unterstützt derzeit Dokumente mit bis zu 2000 Seiten. Dies umfasst kombinierte Testsendungen. Weitere Informationen finden Sie unter [Erstellen eines mehrseitigen Testversands](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

## Allgemeine Tipps

* Da PDF-Dateien die standardisiertesten und zuverlässigsten sind, empfehlen wir, Dokumente in dieses Format zu konvertieren, bevor Sie sie hochladen.
* Verwenden Sie die neueste Version Ihrer Software, um Ihre Originaldokumente zu erstellen.
* Wenn Sie nicht sicher sind, welche Einstellungen beim Speichern oder Exportieren Ihrer Dokumente in der Anwendung, in der Sie sie erstellt haben, verwendet werden sollen, verwenden Sie die Standardeinstellungen. 
* Betten Sie alle Schriftarten, die Sie in einem Dokument verwenden, ein. Wenn Sie benutzerdefinierte Schriftarten verwenden, zeigt Ihr Dokument diese Schriftarten nur auf Computern an, auf denen sie installiert sind. Da jedoch benutzerdefinierte Schriftarten nicht im Testversandsystem enthalten sind, können beim Generieren der Datei keine benutzerdefinierten Schriftarten verwendet werden, selbst wenn sie eingebettet sind.
* Platzieren Sie nach Möglichkeit alle Textelemente in den obersten Ebenen Ihres Designs. Dadurch sollte sichergestellt werden, dass Ihr Text extrahiert und im Text-Anmerkungs-Tool auswählbar ist.
* Platzieren Sie alle Bilder und Elemente Ihres Dokuments darin. Wenn Sie sie aus externen Quellen verknüpfen, z. B. aus einer anderen Datei auf Ihrem Computer, werden sie nicht in dem von Ihnen erstellten Testversand angezeigt.
* Erstellen Sie Ihr Dokument anhand der für seinen Typ empfohlenen Standards und optimieren Sie es, bevor Sie es hochladen. Dadurch wird sichergestellt, dass das Dokument sowohl im Testversand-Viewer als auch in allen anderen Anwendungen und Plattformen erfolgreich geöffnet wird.
* Versuchen Sie in Ihrer Design-Software, &quot;Preflight&quot;-Optionen auszuführen, um zu sehen, ob Ihr Dokument Warnungen generiert. Diese Optionen sind in den meisten Anwendungen als Ausgabevorschau, Druckproduktion usw. verfügbar. Weitere Informationen finden Sie in der Dokumentation Ihrer Anwendung .
* Stellen Sie sicher, dass die Farbeinstellungen im gesamten Dokument konsistent sind.
* Wenn Ihr Dokument vor Aktionen wie dem Kopieren von Dateien geschützt ist, kann das Werkzeug zur Testversand-Extraktion möglicherweise nicht auf den Inhalt zugreifen.

## Prozesszeiten

Normalerweise dauert die Verarbeitung einige Sekunden pro Seite. Verschiedene Faktoren können dies jedoch verlängern, wie z. B. Netzwerkverkehr/Bandbreite, lokale Verbindungsgeschwindigkeiten und internationale Verbindungsgeschwindigkeiten (für Benutzer außerhalb der USA). Die Verarbeitungszeit kann sich auch auf Folgendes auswirken:

* Für statische Dokumente und Bilder: Seitenzahl, Seitendimensionen, Textvolumen, Bild- und Objektkomplexität (Elemente wie mehrere Vektorelemente, Ebenen, Transparenzen).
* Für Videos: lange Dauer, große Dimensionen und verwendete Codecs.
* Für Webaufzeichnungen: Ladezeiten von Webseiten und Seitendimensionen.

## Prozessschritte

Gesendete Dateien durchlaufen einige oder alle der folgenden Schritte:

1. **Übermittlung**. Wenn Sie ein Dokument in das System hochladen, verwenden Sie dazu die Seite Neuer Testversand oder eine Anwendungsprogrammierschnittstelle (API). 
1. **Queue**. In Zeiten hohen Datenverkehrs muss Workfront möglicherweise Übermittlungen in die Warteschlange stellen, damit das System nicht überlastet wird. Die meisten Testsendungen verbringen nur einige Sekunden in einer Warteschlange. 
1. **Verarbeitung.** Die Dateien erreichen die Verarbeitungsmaschinen gemäß dem Inhaltstyp. Wir verwenden verschiedene Tools zur Verarbeitung von Videosendungen, Webaufnahmen, statischen Bildern und Dokumenten. Rich-Media-Container (ZIP) und interaktive Weberfassungen erfordern keine Verarbeitung.
