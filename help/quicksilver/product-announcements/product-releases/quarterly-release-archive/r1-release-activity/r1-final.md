---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Endgültig
description: Versionsaktivität 2018.3
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 38974e97-dea3-4c9e-bc32-bd55665370c7
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1177'
ht-degree: 0%

---

# R1 Endgültig

Die folgenden Funktionen sind derzeit weder in der Vorschau noch in Beta verfügbar, werden jedoch in der Produktionsumgebung in R1 freigegeben:

## Genehmigungsentscheidungen für Korrekturabzüge im Bereich „Meine Arbeit“ (Workfront) treffen

Wenn Sie nun von einem Benutzer zu einem Korrekturabzug hinzugefügt werden und Ihnen entweder die Rolle Genehmiger oder die Rolle Prüfer und Genehmiger gewährt wird (entweder über die eigenständige ProofHQ-Anwendung oder durch Verwendung des automatisierten Workflows in Workfront ), wird die Genehmigungsanfrage auf der Registerkarte Genehmigungen in Ihrem Bereich Meine Arbeit angezeigt. Sie können dann den Korrekturabzug anzeigen und direkt aus Workfront eine Genehmigungsentscheidung für den Korrekturabzug treffen.

Informationen zum Hinzufügen von Benutzern zu einem Korrekturabzug mithilfe eines automatisierten Workflows finden Sie unter [Freigeben eines Korrekturabzugs in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Freigeben eines Korrekturabzugs in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

Weitere Informationen dazu, wie Sie Genehmigungsentscheidungen im Bereich Meine Arbeit treffen, finden Sie unter [Genehmigen von &#x200B;](../../../../review-and-approve-work/manage-approvals/approving-work.md)&quot; in [Genehmigen von Arbeit](../../../../review-and-approve-work/manage-approvals/approving-work.md). 

## Berichte zu Proofing-Genehmigungen im Bereich „Meine Arbeit“ (Workfront)

Sie können jetzt einen Bericht auf der Grundlage des Korrekturabzugsgenehmigungsobjekts erstellen. Dieser Bericht ermöglicht es Ihnen, Berichte zu den Korrekturabzugsgenehmigungen aus den Bereichen Meine Arbeit von Benutzern zu erstellen, für die noch keine Entscheidungen getroffen wurden.

Berichte zur Testversandvalidierung enthalten die folgenden Informationen:

* Dokument, das zur Genehmigung eingereicht wurde
* Name der genehmigenden Person
* Korrekturabzug-Version
* Korrekturabzugs-ID
* Erstellungsdatum des Korrekturabzugs

Sie können auf diese Genehmigung zugreifen, wenn Sie einen Bericht auf der Grundlage eines Objekts erstellen, wie in [Erstellen eines benutzerdefinierten Berichts](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) beschrieben.

Weitere Informationen zum Objektbericht für Korrekturabzugsgenehmigungen finden Sie im Abschnitt [Objekte in Adobe Workfront verstehen](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) in [Objekte in Adobe Workfront verstehen](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Automatisches Generieren einer neuen Version eines Korrekturabzugs für Dokumente mithilfe von Drag &amp; Drop (Workfront)

Wenn Sie die Drag-and-Drop-Methode verwenden, um eine neue Version eines Dokuments hinzuzufügen, für das ein Proofing erforderlich ist, wird automatisch ein Korrekturabzug generiert. Der Korrekturabzug verfügt über dieselben Optionen und Workflows wie der ursprüngliche Korrekturabzug oder die vorherige Version.

Wenn Sie eine neue Version des Dokuments hinzugefügt haben, wurde der Korrekturabzug bisher nicht automatisch für die neue Version erstellt, und Sie mussten den Korrekturabzug für die neue Version neu erstellen.

Wenn Sie das Menü Weitere Dokumente verwenden, um eine neue Version hochzuladen, wird nicht automatisch ein Korrekturabzug generiert.

Weitere Informationen finden Sie in der  Abschnitt in

## Ermöglichen Sie allen Proofing-Benutzern den direkten Zugriff auf ProofHQ über die Workfront-Benutzeroberfläche (Workfront)

Jetzt können Sie allen Proofing-Benutzern in Ihrem System nahtlosen Zugriff auf Ihr ProofHQ Premium-Konto direkt über die Workfront-Benutzeroberfläche ermöglichen. Wenn diese Option aktiviert ist, wird allen Proofing-Benutzern in der globalen Navigationsleiste ein ProofHQ-Symbol angezeigt, über das sie zur ProofHQ-Site weitergeleitet werden.

Diese Option ist nicht standardmäßig aktiviert. Um diese Option zu aktivieren, wenden Sie sich an den technischen Support von Workfront und fordern Sie diesen Zugriff für alle Proofing-Benutzer in Ihrem System an.

Weitere Informationen finden Sie unter [Zugriff auf Workfront Proof über Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md) in  [Zugriff auf Workfront Proof über Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

Vor dieser Änderung konnte nur der Workfront-Administrator über die Workfront-Benutzeroberfläche direkten Zugriff auf die ProofHQ-Site haben.

## Neue Option für TLS Secure Connection for Outgoing Mail (Workfront)

Wenn Sie sich dafür entscheiden, Ihre Workfront-Kommunikation mit Ihrem eigenen E-Mail-Server zu verwalten, können Sie jetzt für Ihre ausgehende E-Mail die Verwendung einer sicheren TLS-Verbindung aktivieren.

Vor dieser Verbesserung konnten Sie ausgehende E-Mails nur über eine sichere SSL-Verbindung aktivieren.

Weitere Informationen zur Konfiguration ausgehender E-Mails finden Sie unter .

## Neues Feld zum Verwalten von E-Mails in der Sandbox-Vorschau-Umgebung

Workfront deaktiviert jetzt die gesamte E-Mail-Kommunikation über die Sandbox-Vorschau-Umgebung und die benutzerdefinierte Aktualisierungsumgebung. Wenn Sie E-Mail-Benachrichtigungen von der Vorschau-Sandbox oder von benutzerdefinierten Aktualisierungsumgebungen erhalten möchten, müssen Sie diese Funktion in Ihren Benutzereinstellungen aktivieren.

Weitere Informationen finden Sie in den folgenden Abschnitten:

* [Die Adobe Workfront-Sandbox](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)Vorschau-Umgebung in [Die Adobe Workfront-Sandbox-Vorschau-Umgebung](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

* „Empfangen von E-Mails von der benutzerdefinierten Aktualisierungs-Sandbox“ in [Die benutzerdefinierte Aktualisierungs-Sandbox-Umgebung von Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)

## Outlook für Office 365 (Workfront)

Das Workfront-Add-In für Outlook 365 ist jetzt verfügbar. 

Weitere Informationen zur Verwendung des Add-Ins finden Sie unter [Verwenden des Workfront-Add-Ins mit Outlook für Office 365.](https://support.workfront.com/hc/en-us/sections/205046167)

## Suchen in der Mobile App (Workfront)

Sie können jetzt in der Mobile App nach Objekten suchen, ähnlich wie bei der Suche in der Web-Anwendung. Die neue Suchfunktion sucht zuerst nach Elementen in der Liste der letzten Elemente sowie nach den Objekten, die zuvor auf Ihr Mobilgerät heruntergeladen wurden. Die Liste der letzten Elemente entspricht der Liste, die Sie in der Web-Anwendung sehen.

>[!NOTE]
>
>Diese Funktion wird in der ersten Maiwoche 2017 verfügbar sein.

Weitere Informationen zur Mobile App finden Sie im Abschnitt „Suchen in Mobile“ in  

## Verbesserte Hilfe in der Mobile App: Tutorials (Workfront)

Ab der Mobile-Version im April werden neue Tutorial-Bildschirme angezeigt, die Sie durch Ihr mobiles Erlebnis führen. Wenn Sie sich zum ersten Mal bei der Mobile App anmelden und zum ersten Mal eine Funktion verwenden, sehen Sie ein kurzes Tutorial, in dem erläutert wird, wie die Funktion funktioniert. Das Tutorial wird nur einmal angezeigt, wenn Sie eine bestimmte Funktion zum ersten Mal verwenden.

Weitere Informationen zur Mobile App finden Sie unter .

## Suchen in PDF-Dokumenten (ProofHQ)

Sie können jetzt Suchvorgänge in PDF-Dokumenten, Office-Dokumenten und statischen Web-Seiten durchführen.

Weitere Informationen finden Sie unter  [Durchsuchen von Inhalten in einem Korrekturabzug](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/search-in-a-proof.md).

## Aktualisierte globale Navigationsleiste (ProofHQ)

Für ProofHQ Premium-Konten, die in Workfront integriert sind, wurden in der globalen Navigationsleiste in ProofHQ jetzt die folgenden Verbesserungen vorgenommen:

* Bild eines neuen Benutzerprofils 
* Aktualisiertes Erscheinungsbild

## Zusätzliche Informationen in benutzerdefinierte Ansichten einschließen (ProofHQ)

Sie können jetzt die folgenden zusätzlichen Informationen in benutzerdefinierte Ansichten einfügen:

* **Daten auf Empfängerebene**\
  Sie können benutzerdefinierte Ansichten so konfigurieren, dass sie die folgenden Spalten im Zusammenhang mit Daten auf Empfängerebene enthalten: Rolle, Position, E-Mail-Warnhinweise, Meine Frist, Datum zum Testversand hinzugefügt und Empfängersuche.\
  Weitere Informationen finden Sie unter [Erstellen und Verwalten von benutzerdefinierten Ansichten im Workfront Proof-Korrekturabzug](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **Proofing-Daten**\
  Sie können benutzerdefinierte Ansichten so konfigurieren, dass sie die folgenden Spalten im Zusammenhang mit Proofing-Daten enthalten: Kommentar-Anzahl (alle Versionen), Größe auf der Festplatte, Korrekturabzug-Typ, Anzahl der Dateien pro Version, Kommentar-Anlagendaten (Größe auf der Festplatte, Dateiname) und Filterung nach Unterordner.\
  Weitere Informationen finden Sie unter [Erstellen und Verwalten von benutzerdefinierten Ansichten im Workfront Proof-Korrekturabzug](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **Daten auf Staging-Ebene im Zusammenhang mit automatisierten Workflows**\
  Sie können benutzerdefinierte Ansichten so konfigurieren, dass sie die folgenden Spalten zu den einzelnen Phasen automatisierter Workflows enthalten: SOCD-Status, Staging-Fristen, Name der aktiven Phase, Name der nächsten Phase, Name der Phase und Vorlage.\
  Weitere Informationen finden Sie unter [Erstellen und Verwalten von benutzerdefinierten Ansichten im Workfront Proof-Korrekturabzug](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## Verbesserungen an Proofing-Berichten (früher Analytics) (ProofHQ)

Die Reporting-Funktion (früher als Analytics bezeichnet) enthält die folgenden Verbesserungen:

* Neue standardmäßige Berichtstypen:

   * Korrekturabzug-Durchlaufzeit
   * Prozentsatz verspäteter Genehmigungen
   * Zeit der ersten Testaktivität
   * Anzahl Kommentare und Antworten

* Berichte drucken
* Aktualisiertes Erscheinungsbild

## Anzeigen der ProofHQ-Funktionalität in der Vorschau-Umgebung (ProofHQ)

Funktionen, die für ProofHQ freigegeben werden, stehen vor der Freigabe in der Produktionsumgebung zunächst zum Testen in der Vorschau-Umgebung zur Verfügung.

Dieser neue Workflow der Veröffentlichung von Funktionen zur Vorschau vor der Produktion ermöglicht es Ihnen, besser auf zukünftige Aktualisierungen Ihrer ProofHQ-Produktionsumgebung vorbereitet zu sein.

Weitere Informationen zur ProofHQ-Vorschau-Umgebung finden Sie unter [Vorschau der Sandbox-Testumgebung - Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).
