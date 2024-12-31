---
product-area: documents
navigation-topic: proofing-overview
title: Übersicht über die Neuverarbeitung von Dokumenten für das Proofing
description: Wenn Sie ein Dokument (DOCX, PDF, XLSX, AI) für das Proofing übermitteln, verarbeitet Adobe Workfront es erneut, sodass es in der Proofing-Ansicht ohne die Software-Anwendung angezeigt werden kann, die Sie zum Erstellen verwendet haben.
author: Courtney
feature: Digital Content and Documents
exl-id: e577fa71-4828-4fc2-93a2-0eddbb5ad2ad
source-git-commit: 332c744ab9b760268620461ed2cb2551caf383cf
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 0%

---

# Übersicht über die Neuverarbeitung von Dokumenten für das Proofing

Wenn Sie ein Dokument (DOCX, PDF, XLSX, AI) für das Proofing übermitteln, verarbeitet Adobe Workfront es erneut, sodass es in der Proofing-Ansicht ohne die Software-Anwendung angezeigt werden kann, die Sie zum Erstellen verwendet haben. 

Jede Seite Ihres Dokuments wird im Proofing Viewer als Miniaturbild angezeigt. Wenn Sie auf eine Miniatur klicken, können Sie eine Bitmap-Version dieser Seite zu 100 %, 200 % und 400 % einzoomen. Für Korrekturabzüge mit einer Höhe oder Breite von mehr als 800 mm beträgt der maximale Zoom-Faktor 200 %.

Die Farben in Ihrem Dokument werden in sRGB mit Farbkonvertierung von der neuesten Adobe-Bibliothek angezeigt. Der Proofing Viewer unterstützt alle im Dokument eingebetteten ICC-Profile (International Color Consortium).

Der gesamte Schrifttext wird in seiner Ebene extrahiert, sofern Sie beim Hochladen des Dokuments in das System die richtige Dateierweiterung angeben. Als Bilder oder Kurven enthaltener Text wird nicht angezeigt.

>[!NOTE]
>
>Workfront unterstützt derzeit Dokumente mit bis zu 2.000 Seiten. Dazu gehören kombinierte Korrekturabzüge. Weitere Informationen finden Sie unter [Erstellen eines mehrseitigen Korrekturabzugs](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

## Allgemeine Tipps

* Da PDF-Dateien die standardisiertesten und zuverlässigsten sind, empfehlen wir, Dokumente vor dem Hochladen in dieses Format zu konvertieren.
* Verwenden Sie die neueste Version Ihrer Software, um Ihre Originaldokumente zu erstellen.
* Wenn Sie sich nicht sicher sind, welche Einstellungen beim Speichern oder Exportieren Ihrer Dokumente in der Anwendung, in der Sie sie erstellt haben, verwendet werden sollen, verwenden Sie die Standardeinstellungen. 
* Stellen Sie sicher, dass Sie alle Schriftarten, die Sie in einem Dokument verwenden, darin einbetten. Wenn Sie benutzerdefinierte Schriftarten verwenden, zeigt Ihr Dokument diese Schriftarten nur auf Computern an, auf denen sie installiert sind. Da jedoch benutzerdefinierte Schriftarten nicht im Testversandsystem enthalten sind, kann es beim Generieren der Datei keine benutzerdefinierten Schriftarten verwenden, selbst wenn sie eingebettet sind.
* Platzieren Sie nach Möglichkeit alle Textelemente in den oberen Ebenen Ihres Designs. Dadurch sollte sichergestellt sein, dass Ihr Text extrahiert und im Textanmerkungs-Tool ausgewählt werden kann.
* Platzieren Sie alle Bilder und Elemente Ihres Dokuments darin. Wenn Sie sie von externen Quellen verknüpfen, z. B. von einer anderen Datei auf Ihrem Computer, werden sie im erstellten Korrekturabzug nicht angezeigt.
* Erstellen Sie Ihr Dokument mit den für seinen Typ empfohlenen Standards und optimieren Sie es vor dem Hochladen. Dadurch wird sichergestellt, dass das Dokument erfolgreich im Proofing Viewer sowie in allen anderen Anwendungen und Plattformen geöffnet wird.
* Versuchen Sie in Ihrer Design-Software, „PreFlight“-Optionen auszuführen, um zu sehen, ob Ihr Dokument Warnungen erzeugt. Diese Optionen sind in den meisten Anwendungen als Ausgabevorschau, Druckproduktion usw. verfügbar. Weitere Informationen finden Sie in der Dokumentation Ihres Programms.
* Stellen Sie sicher, dass die Farbeinstellungen im gesamten Dokument einheitlich sind.
* Wenn Ihr Dokument vor Aktionen wie dem Kopieren von Dateien geschützt ist, kann das Proofing-Extraktions-Tool möglicherweise nicht auf seinen Inhalt zugreifen.

## Prozesszeiten

Normalerweise dauert die Verarbeitung einige Sekunden pro Seite. Verschiedene Faktoren können dies jedoch verlängern, z. B. der Netzwerk-Traffic/die Bandbreite, die lokalen Verbindungsgeschwindigkeiten und die internationalen Verbindungsgeschwindigkeiten (für Benutzer außerhalb der USA). Folgende Faktoren können sich auch auf die Verarbeitungszeit auswirken:

* Bei statischen Dokumenten und Bildern: Seitenzahl, Seitenabmessungen, Textvolumen, Bild und Komplexität von Objekten (Elemente wie mehrere Vektorelemente, Ebenen, Transparenzen).
* Für Videos: lange Dauer, große Abmessungen und verwendete Codecs.
* Für Web-Erfassung: Ladezeiten von Web-Seiten und Seitenmaße.

## Prozessschritte

Übermittelte Dateien durchlaufen einige oder alle folgenden Schritte:

1. **Übermittlung**. Wenn Sie ein Dokument in das System hochladen, verwenden Sie dazu die Seite Neuer Korrekturabzug oder eine Anwendungsprogrammierschnittstelle (API). 
1. **Warteschlange**. Bei starkem Traffic muss Workfront möglicherweise Übermittlungen in die Warteschlange stellen, um eine Überlastung des Systems zu vermeiden. Die meisten Testsendungen befinden sich nur wenige Sekunden in der Warteschlange. 
1. **Verarbeitung läuft.** Die Dateien gelangen je nach Content-Typ zu den Verarbeitungsmaschinen. Wir verwenden verschiedene Tools zur Bearbeitung von Testsendungen, Web-Aufnahmen, statischen Bildern und Dokumenten. Übermittlungen von Rich-Media-Containern (ZIP) und interaktiver Web-Erfassung erfordern keine Verarbeitung.
