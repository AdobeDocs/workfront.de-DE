---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Erstellen eines mehrseitigen Testversands
description: Sie können mehrere Dateien zu einem mehrseitigen Testversand kombinieren. Überprüfer können die Navigationstools im Testversand-Viewer verwenden, um die Seiten in einem mehrseitigen Testversand zu durchsuchen.
author: Courtney
feature: Digital Content and Documents
exl-id: a8ad80d8-0758-4fea-824e-8c206424e295
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---

# Erstellen eines mehrseitigen Testversands

Sie können mehrere Dateien zu einem mehrseitigen Testversand kombinieren. Überprüfer können die Navigationstools im Testversand-Viewer verwenden, um die Seiten in einem mehrseitigen Testversand zu durchsuchen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Veralteter Plan: Wählen Sie oder Premium</p> <p>Weitere Informationen zum Testen des Zugriffs mit den verschiedenen Plänen finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Testfunktion in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Aktueller Plan: Arbeit oder Plan</p> <p>Veralteter Plan: Beliebig (Sie müssen die Testfunktion für den Benutzer aktiviert haben)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um zu erfahren, welchen Plan, welche Lizenz oder welches Testprofil Sie verwenden.

## Erstellen eines mehrseitigen Testversands

Wenn diese Option aktiviert ist, sind statische Dateien und Websites in einem einzigen Testversand verfügbar. Wenn diese Option deaktiviert ist, werden alle Dokumente und Websites als individuelle Testsendungen generiert und Sie können bis zu 100 Dateien gleichzeitig hochladen.

So erstellen Sie einen mehrseitigen Testversand:

1. Wechseln Sie zum Projekt, zur Aufgabe oder zur Ausgabe, an der Sie den Testversand durchführen möchten, und klicken Sie dann auf den Abschnitt **Dokumente** .
1. Klicken Sie auf **Neu hinzufügen** > **Testversand** .
1. Ziehen Sie die Dateien per Drag-and-Drop in den Arbeitsbereich oder durchsuchen Sie sie und wählen Sie sie aus dem Dateiexplorer aus. Sie können bis zu 50 Dateien gleichzeitig hochladen. Informationen zu Dateibeschränkungen finden Sie im Abschnitt [Zu beachten](#considerations) in diesem Artikel.

   >[!NOTE]
   >
   >Interaktive Dateien, einschließlich Videos und interaktive Websites, können nicht zu einem Testversand kombiniert werden.

1. Aktivieren Sie unter **Einzelversand** die Option **Alle kompatiblen Dateien in einem Testversand zusammenfassen**.
1. Geben Sie im Feld **Testversand-Name** einen neuen Namen für den kombinierten Testversand an.
1. (Optional) Ordnen Sie die Dateien in der Liste der hochgeladenen Dateien durch Ziehen neu an. Die Reihenfolge der Dateien entspricht der Seitenreihenfolge des kombinierten Testversands.
1. (Optional) Um eine einzelne Datei aus der Seite Neuer Testversand zu entfernen, halten Sie den Mauszeiger über die Datei und klicken Sie auf das rechts angezeigte Symbol **Papierkorb** .

   Oder

   Um alle gleichzeitig hochgeladenen Dateien zu löschen, klicken Sie oben rechts in der Liste auf **Alle löschen** .

1. Nachdem alle Ihre Dateien hochgeladen wurden, müssen Sie entscheiden, ob Sie einen einfachen Testversand oder einen automatisierten Testversand konfigurieren möchten:

   * Mit einem einfachen Testversand können Sie so viele Validierungsverantwortliche hinzufügen, wie Sie möchten. Diese sind jedoch nicht in Phasen unterteilt. Alle hinzugefügten Validierungsverantwortlichen können sofort nach der Erstellung auf den Testversand zugreifen. Informationen zum Konfigurieren eines einfachen Testversands finden Sie unter [Erstellen eines erweiterten Testversands mit einem einfachen Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md).
   * Mit einem automatisierten Testversand wechselt der Testversand von einer Phase zur nächsten und Adobe Workfront benachrichtigt jeden Benutzer, wenn er an der Reihe ist, ihn zu überprüfen. Informationen zum Konfigurieren eines automatisierten Testversands finden Sie unter [Erstellen eines erweiterten Testversands mit einem automatisierten Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Überlegungen {#considerations}

Beachten Sie beim Zusammenführen von Dateien zu einem Testversand Folgendes:

* Sie können bis zu 500 separate Dateien hochladen.
* Sie können statische Dateien unterschiedlicher Typen (z. B. PDF, JPG, DOC, PPT, EXC) mit bis zu 2.000 Seiten kombinieren.
* Sie können statische Webaufzeichnungen kombinieren.
* Sie können GIF-Dateien kombinieren, animierte GIF werden jedoch als statische Dateien verarbeitet.
* Sie können keine AV-Dateien und interaktiven Webaufzeichnungen kombinieren.
* Das Miniaturbild des Testversands wird von der ersten Seite des Testversands übernommen (siehe [Details des Testversands in Workfront Proof verwalten](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)).
* Sie können die Namen der kombinierten Dateien überprüfen, um den Testversand auf der Seite mit den Testversanddetails zu erstellen. Weitere Informationen finden Sie unter [Verwalten von Testversanddetails in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
* Wenn die Option zum Herunterladen der Originaldateien auf dem Testversand aktiviert ist, können Sie alle kombinierten Dateien herunterladen, um den Testversand als ZIP-Datei zu erstellen. Weitere Informationen finden Sie unter  [Herunterladen von Dateien, die in Workfront Proof gespeichert sind](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).
