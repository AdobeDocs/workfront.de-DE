---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Endgültige
description: Aktivität "Version 2018.3"
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 38974e97-dea3-4c9e-bc32-bd55665370c7
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1177'
ht-degree: 0%

---

# R1 Endgültige

Die folgende Funktion ist derzeit nicht in der Vorschau oder in Beta verfügbar, wird aber in der Produktionsumgebung in R1 veröffentlicht:

## Festlegen von Genehmigungsentscheidungen für Testsendungen aus dem Arbeitsbereich (Workfront)

Wenn ein Benutzer Sie jetzt einem Testversand hinzufügt und entweder die Rolle &quot;Genehmiger&quot;oder die Rolle &quot;Validierer und Genehmiger&quot;erteilt (entweder über die eigenständige Anwendung &quot;ProofHQ&quot;oder über den automatisierten Workflow in Workfront ), wird die Genehmigungsanfrage auf der Registerkarte &quot;Genehmigungen&quot;in Ihrem Arbeitsbereich angezeigt. Sie können den Testversand ansehen und direkt in Workfront eine Validierungsentscheidung für den Testversand treffen.

Informationen zum Hinzufügen von Benutzern zu einem Testversand mithilfe des automatisierten Workflows finden Sie unter [Freigeben eines Testversands in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Freigeben eines Testversands in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

Informationen dazu, wie Sie Genehmigungsentscheidungen im Arbeitsbereich &quot;Meine Arbeit&quot;treffen, finden Sie unter [Genehmigung der Arbeit](../../../../review-and-approve-work/manage-approvals/approving-work.md) in [Arbeiten genehmigen](../../../../review-and-approve-work/manage-approvals/approving-work.md). 

## Bericht zu Testgenehmigungen in meinem Arbeitsbereich (Workfront)

Jetzt können Sie einen Bericht auf der Basis des Objekts &quot;Proof Approval&quot;erstellen. Dieser Bericht ermöglicht Ihnen die Berichterstellung über die Testversandgenehmigungen aus den &quot;Meine Arbeit&quot;-Bereichen der Benutzer, in denen noch keine Entscheidungen getroffen wurden.

Die Berichte zur Validierung des Testversands enthalten folgende Informationen:

* Dokument, das zur Genehmigung eingereicht wurde
* Name des Genehmigers
* Testversion
* Korrekturabzugs-ID
* Erstellungsdatum des Testversands

Sie können auf diese Genehmigung zugreifen, wenn Sie einen Bericht basierend auf einem Objekt erstellen, wie unter [Benutzerspezifischen Bericht erstellen](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) beschrieben.

Weitere Informationen zum Objektbericht für Testsendungen finden Sie im Abschnitt [Objekte in Adobe Workfront verstehen](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) in [Objekte in Adobe Workfront verstehen](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Automatische Generierung einer neuen Version eines Dokumentennachweises mithilfe von Drag &amp; Drop (Workfront)

Wenn Sie die Drag &amp; Drop-Methode verwenden, um eine neue Version eines Dokuments hinzuzufügen, für das ein Testversand erforderlich ist, wird automatisch ein Testversand generiert. Der Testversand verfügt über dieselben Optionen und Workflows wie der ursprüngliche Testversand oder die vorherige Version.

Zuvor, als Sie eine neue Version des Dokuments hinzugefügt haben, wurde der Testversand nicht automatisch für die neue Version generiert und Sie mussten den Testversand für die neue Version neu generieren.

Wenn Sie das Menü &quot;Mehr Dokumente&quot;zum Hochladen einer neuen Version verwenden, wird kein Testversand automatisch generiert.

Weitere Informationen finden Sie unter  Abschnitt in

## Aktivieren Sie allen Testnutzern, über die Workfront-Benutzeroberfläche (Workfront) direkt auf ProofHQ zuzugreifen.

Jetzt können Sie allen Testversand-Benutzern in Ihrem System einen nahtlosen Zugriff auf Ihr ProofHQ Premium-Konto direkt über die Workfront-Benutzeroberfläche ermöglichen. Wenn diese Option aktiviert ist, sehen alle Benutzer von Testsendungen in der Symbolleiste für globale Navigation ein Symbol für ProofHQ, das sie zur Site &quot;ProofHQ&quot;weiterleitet.

Diese Option ist standardmäßig nicht aktiviert. Wenden Sie sich zur Aktivierung dieser Option an den technischen Support von Workfront und fordern Sie diesen Zugriff für alle Testbenutzer in Ihrem System an.

Weitere Informationen finden Sie unter [Zugriff auf Workfront Proof über Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md) in  [Greifen Sie über Adobe Workfront auf Workfront Proof zu](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

Vor dieser Änderung konnte nur der Workfront-Administrator über die Workfront-Benutzeroberfläche direkt auf die ProofHQ-Site zugreifen.

## Neue Option für sichere TLS-Verbindung für ausgehende Nachrichten (Workfront)

Wenn Sie Ihre Workfront-Kommunikation über Ihren eigenen E-Mail-Server verwalten möchten, können Sie jetzt für Ihre ausgehende E-Mail eine sichere TLS-Verbindung aktivieren.

Vor dieser Verbesserung konnten Sie die Option Ausgehende Mail nur über eine sichere SSL-Verbindung aktivieren.

Weitere Informationen zur Konfiguration Ihrer ausgehenden E-Mail finden Sie unter .

## Neues Feld für die Verwaltung von E-Mails in der Sandbox-Vorschauumgebung

Workfront deaktiviert nun die gesamte E-Mail-Kommunikation aus der Sandbox-Vorschau-Umgebung und der Umgebung Benutzerdefinierte Aktualisierung . Wenn Sie E-Mail-Benachrichtigungen von der Sandbox-Vorschau oder von benutzerdefinierten Aktualisierungsumgebungen erhalten möchten, müssen Sie diese Funktion in Ihren Benutzereinstellungen aktivieren.

Weitere Informationen finden Sie in den folgenden Informationen:

* [Die Adobe Workfront-Vorschau-Sandbox-Umgebung](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) in [Adobe Workfront-Vorschau-Sandbox-Umgebung](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

* &quot;Empfangen von E-Mails von der Sandbox &quot;Benutzerdefinierte Aktualisierung&quot; in [der Sandbox-Umgebung für benutzerdefinierte Adobe Workfront-Aktualisierung](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)

## Outlook für Office 365 (Workfront)

Das Workfront-Add-In für Outlook 365 ist jetzt verfügbar. 

Weitere Informationen zur Verwendung des Add-Ins finden Sie unter [Verwenden des Workfront-Add-Ins mit Outlook für Office 365.](https://support.workfront.com/hc/en-us/sections/205046167)

## Suchen in der mobilen App (Workfront)

Sie können jetzt in der mobilen App ähnlich wie in der Webanwendung nach Objekten suchen. Die neue Suchfunktion sucht zunächst nach Elementen in der Liste &quot;Zuletzt verwendete Elemente&quot;sowie nach Objekten, die zuvor auf Ihr Mobilgerät heruntergeladen wurden. Die Liste der letzten Elemente ist dieselbe Liste wie in der Webanwendung.

>[!NOTE]
>
>Diese Funktion ist ab der ersten Mai 2017-Woche verfügbar.

Weitere Informationen zur Mobile App finden Sie im Abschnitt &quot;Suchen in Mobile&quot;unter  

## Verbesserte Hilfe in der Mobile App: Tutorials (Workfront)

Ab der mobilen Version im April werden Ihnen neue Tutorials angezeigt, die Sie durch Ihr mobiles Erlebnis führen. Wenn Sie sich zum ersten Mal bei der Mobile App anmelden und eine Funktion zum ersten Mal verwenden, wird Ihnen ein kurzes Tutorial angezeigt, in dem Sie erklären, wie die Funktion funktioniert. Das Tutorial wird nur einmal angezeigt, wenn Sie zum ersten Mal eine bestimmte Funktion verwenden.

Weitere Informationen zur Mobile App finden Sie unter .

## Suchen in PDF-Dokumenten (ProofHQ)

Sie können jetzt Suchen in PDF-Dokumenten, Office-Dokumenten und statischen Webseiten durchführen.

Weitere Informationen finden Sie unter  [Suchinhalt in einem Testversand](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/search-in-a-proof.md).

## Aktualisierte globale Navigationsleiste (ProofHQ)

Für in Workfront integrierte ProofHQ Premium-Konten werden jetzt die folgenden Verbesserungen an der globalen Navigationsleiste in ProofHQ angezeigt:

* Neues Benutzerprofilbild 
* Aktualisiertes Erscheinungsbild

## Zusätzliche Informationen in benutzerdefinierte Ansichten einschließen (ProofHQ)

Sie können jetzt die folgenden zusätzlichen Informationen in benutzerdefinierte Ansichten einfügen:

* **Daten auf Empfängerebene**\
  Sie können benutzerdefinierte Ansichten konfigurieren, um die folgenden Spalten für Daten auf Empfängerebene einzuschließen: Rolle, Position, E-Mail-Warnungen, Meine Deadline, Datum zum Testversand hinzugefügt und Empfängersuche.\
  Weitere Informationen finden Sie unter [Erstellen und Verwalten benutzerdefinierter Ansichten im Workfront Proof-Testversand](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **Testen von Daten**\
  Sie können benutzerdefinierte Ansichten so konfigurieren, dass die folgenden Spalten zu Testdaten hinzugefügt werden: Anzahl der Kommentare (alle Versionen), Größe auf Festplatte, Testtyp, Anzahl der Dateien pro Version, Daten der Kommentaranhänge (Größe auf Festplatte, Dateiname) und Filterung nach Unterordner.\
  Weitere Informationen finden Sie unter [Erstellen und Verwalten benutzerdefinierter Ansichten im Workfront Proof-Testversand](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **Daten auf Staging-Ebene im Zusammenhang mit automatisierten Workflows**\
  Sie können benutzerdefinierte Ansichten konfigurieren, um die folgenden Spalten für einzelne Phasen automatisierter Workflows einzuschließen: SOCD-Status, Staging-Deadlines, Name der aktiven Bühne, Name der nächsten Stufe, Name der Staging-Umgebung und Vorlage.\
  Weitere Informationen finden Sie unter [Erstellen und Verwalten benutzerdefinierter Ansichten im Workfront Proof-Testversand](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## Verbesserungen an Testberichten (früher Analytics) (ProofHQ)

Die Berichterstellungsfunktion (ehemals Analytics) umfasst die folgenden Verbesserungen:

* Neue Standard-Berichtstypen:

   * Bearbeitungszeit des Testversands
   * Verspäteter Genehmigungsprozentsatz
   * Erstes Aktivitätserlebnis nachweisen
   * Anzahl der Kommentare und Antworten

* Berichte drucken
* Aktualisiertes Erscheinungsbild

## Anzeigen der Funktion &quot;ProofHQ&quot;in der Vorschauumgebung (ProofHQ)

Funktionen, die an ProofHQ veröffentlicht werden, stehen zunächst zum Testen in der Vorschau-Umgebung zur Verfügung, bevor sie in die Produktionsumgebung freigegeben werden.

Mit diesem neuen Workflow zur Veröffentlichung von Funktionen zur Vorschau vor der Produktion können Sie besser auf zukünftige Aktualisierungen Ihrer ProofHQ-Produktionsumgebung vorbereitet sein.

Weitere Informationen zur ProofHQ-Vorschau-Umgebung finden Sie unter [Vorschau der Sandbox-Testumgebung - Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).
