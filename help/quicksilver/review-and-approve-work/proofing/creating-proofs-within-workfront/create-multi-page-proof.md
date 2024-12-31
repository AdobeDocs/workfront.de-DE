---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Erstellen eines mehrseitigen Korrekturabzugs
description: Sie können mehrere Dateien in einem mehrseitigen Korrekturabzug kombinieren. Reviewer können die Navigationstools im Proofing Viewer verwenden, um in einem mehrseitigen Korrekturabzug durch die Seiten zu navigieren.
author: Courtney
feature: Digital Content and Documents
exl-id: a8ad80d8-0758-4fea-824e-8c206424e295
source-git-commit: ac908d52d1538b1ffe7d9bfca94cb9921445633d
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 0%

---

# Erstellen eines mehrseitigen Korrekturabzugs

Sie können mehrere Dateien in einem mehrseitigen Korrekturabzug kombinieren. Reviewer können die Navigationstools im Proofing Viewer verwenden, um in einem mehrseitigen Korrekturabzug durch die Seiten zu navigieren.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Legacy-Plan: Auswählen oder Premium</p> <p>Weitere Informationen zum Proofing-Zugriff für die verschiedenen Pläne finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Proofing-Funktionalität in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Aktueller Plan: Arbeits- oder Plan</p> <p>Legacy-Plan: Beliebig (Proofing muss für den Benutzer aktiviert sein)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um herauszufinden, über welchen Plan, welche Lizenz oder welches Proof-Berechtigungsprofil Sie verfügen.

+++

## Erstellen eines mehrseitigen Korrekturabzugs

Wenn diese Option aktiviert ist, sind statische Dateien und Websites in einem einzigen Korrekturabzug verfügbar. Wenn diese Option deaktiviert ist, werden alle Dokumente und Websites als individuelle Korrekturabzüge generiert, und Sie können bis zu 100 Dateien gleichzeitig hochladen.

So erstellen Sie einen mehrseitigen Korrekturabzug:

1. Wechseln Sie zum Projekt, zur Aufgabe oder zum Problem, in dem/der Sie den Korrekturabzug anzeigen möchten, und klicken Sie dann auf den Abschnitt **Dokumente**.
1. Klicken Sie **Neu hinzufügen** > **Testversand** .
1. Ziehen Sie die Dateien per Drag-and-Drop oder durchsuchen Sie sie und wählen Sie sie aus Ihrem Datei-Explorer aus. Sie können bis zu 50 Dateien gleichzeitig hochladen. Informationen zu Dateibeschränkungen finden Sie [ Abschnitt &quot;](#considerations)&quot; in diesem Artikel.

   >[!NOTE]
   >
   >Interaktive Dateien, einschließlich Videos und interaktiver Websites, können nicht in einem einzigen Korrekturabzug kombiniert werden.

1. Aktivieren **unter &quot;** Korrekturabzug“ die Option **Alle kompatiblen Dateien in einem Korrekturabzug zusammenfassen**.
1. Geben Sie im Feld **Name des Korrekturabzugs** einen neuen Namen für den kombinierten Korrekturabzug ein.
1. (Optional) Ordnen Sie die Dateien in der Liste der hochgeladenen Dateien durch Ziehen neu an. Die Reihenfolge der Dateien entspricht der Seitenreihenfolge des kombinierten Korrekturabzugs.
1. (Optional) Um eine einzelne Datei aus der Seite Neuer Korrekturabzug zu entfernen, bewegen Sie den Mauszeiger über die Datei und klicken Sie auf **Symbol „Papierkorb** auf der rechten Seite.

   Oder

   Um alle hochgeladenen Dateien auf einmal zu löschen, klicken **oben rechts** der Liste auf „Alle löschen“.

1. Nachdem alle Ihre Dateien hochgeladen wurden, müssen Sie entscheiden, ob Sie einen einfachen oder einen automatisierten Korrekturabzug konfigurieren möchten:

   * Bei einem einfachen Korrekturabzug können Sie so viele Prüfer hinzufügen, wie Sie möchten, aber sie sind nicht in Phasen unterteilt. Alle Reviewer, die Sie hinzufügen, können sofort nach der Erstellung auf den Korrekturabzug zugreifen. Informationen zum Konfigurieren eines einfachen Korrekturabzugs finden Sie unter [Erstellen eines erweiterten Korrekturabzugs mit einem einfachen Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md).
   * Mit einem automatisierten Korrekturabzug wechselt der Korrekturabzug von Schritt zu Schritt und Adobe Workfront benachrichtigt jeden Benutzer, wenn er an der Reihe ist, ihn zu überprüfen. Informationen zum Konfigurieren eines automatisierten Korrekturabzugs finden Sie unter [Erstellen eines erweiterten Korrekturabzugs mit einem automatisierten Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Aspekte {#considerations}

Beachten Sie beim Kombinieren von Dateien zu einem einzigen Korrekturabzug Folgendes:

* Sie können bis zu 500 separate Dateien hochladen.
* Sie können statische Dateien verschiedener Typen (z. B. PDF, JPG, DOC, PPT, EXC) bis zu insgesamt 2.000 Seiten kombinieren.
* Sie können statische Web-Aufnahmen kombinieren.
* Sie können GIF-Dateien kombinieren. Animierte GIF werden jedoch als Statikdateien verarbeitet.
* Es ist nicht möglich, AV-Dateien und interaktive Web-Aufnahmen zu kombinieren.
* Das Miniaturbild des Korrekturabzugs wird von der ersten Seite des Korrekturabzugs übernommen (siehe [Verwalten von Korrekturabzugsdetails in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)).
* Sie können die Namen der Dateien, die zum Erstellen des Korrekturabzugs kombiniert wurden, auf der Seite mit den Korrekturabzugsdetails überprüfen. Weitere Informationen finden Sie unter [Verwalten von Korrekturabzugsdetails in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
* Wenn die Option zum Herunterladen der Originaldateien im Korrekturabzug aktiviert ist, können Sie alle Dateien herunterladen, die kombiniert wurden, um den Korrekturabzug als ZIP-Datei zu erstellen. Weitere Informationen finden Sie unter  [Herunterladen von in Workfront Proof gespeicherten Dateien](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).
