---
product-area: documents
navigation-topic: approvals
title: Hochladen einer neuen Dokumentversion und Anfordern einer Genehmigung
description: Sie können eine neue Dokumentversion hochladen und die Genehmigung von anderen Benutzern in Adobe Workfront anfordern.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/grwYgMUQc-Ft08jC1Fb1n7y18cLi1HNcXvJ3wPX0URg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 66a134507a06c0ce0b4fd78bfa5e32bd95f8f08c
workflow-type: tm+mt
source-wordcount: 798
ht-degree: 7%

---

# Hochladen einer neuen Dokumentversion und Anfordern einer Genehmigung

Wenn ein Dokument in einer früheren Überprüfung als „Überarbeitung erforderlich“ gekennzeichnet ist, können Sie eine neue Version in das Originaldokument hochladen und eine weitere Genehmigungsrunde starten. Nachdem Sie eine neue Version des Dokuments hochgeladen haben, werden die vorherigen Versionen gesperrt.

Wenn der Dateiname der neuen Version vom Dateinamen der vorherigen Version abweicht, zeigt Workfront das Dokument mit dem neueren Dateinamen an.

Wenn einem Dokument mit ausstehenden Genehmigungen eine neue Version hinzugefügt wird, wird die Genehmigung für die vorherige Version als „Zurückgezogen“ angezeigt. Der vorherige Genehmigungsprozess wird geschlossen, auch wenn einige Teilnehmer noch keine Entscheidung getroffen haben.

Wenn die neueste Dokumentversion gelöscht wird, bleiben die vorherigen Versionen gesperrt. Wenn Sie eine frühere Version bearbeiten müssen, müssen Sie sie manuell entsperren.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Jedes Workfront-Paket zur Verwaltung von Genehmigungen unter Verwendung des alten Workfront-Speichers</p>
<p>Beliebiges Workflow-Paket zum Verwalten von Genehmigungen mithilfe des Adobe-Cloud-Speichers</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen</td> 
   <td> <p>Anfragende oder höher</p>
   <p>Mitwirkende oder höher</p>
   <p>Wenn Sie die Frame.io-Integration verwenden, benötigen Sie eine Standardlizenz zum Erstellen von Genehmigungs-Workflows.</p>
    </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriffrecht „Bearbeiten“ für Dokumente</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Bearbeitungszugriff auf das mit dem Dokument verknüpfte Objekt</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++



<!--
## Use drag-and-drop to add a new version in the legacy documents area in Production

If your organization is on Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront storage, see [Differences between Adobe cloud storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

>[!NOTE]
>
>Drag-and-drop does not work with Internet Explorer.


If you need another round of review and approval on a document, you can create a new document version in Workfront.

You can add the previous participants, new participants, or a mix of both. You can view information about previous versions and participants on the Document Details page. 

To add a new version:

1. Navigate to the document in Workfront.
1. Drag and drop the new file on top of the previous document. This automatically creates a new version. 

1. Once the document finishes uploading, select the document to open the Document Summary panel. Here you'll see the version number at the top of the panel.


1. Scroll down to the **Approvals** section.

1. Click **Create workflow**, then fill in the following details:

   <table>
   <tr>
   <td><strong>Stage name</strong></td>
   <td>Add a stage name. You can change the name to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Add names or emails</strong></td>
   <td>Begin typing a user or team name to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.</td>
   </tr>
   <tr>
   <td><strong>One decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Due date (optional)</strong></td>
   <td>Set a due date for the approval. Users and teams are notified by email 72 hours, then 24 hours before the specified due date.</td>
   </tr>
   </table>

1. (Optional) Repeat the previous step to add additional stages as needed.

   >[!NOTE]
   >
   >If you add multiple stages, the approval workflow proceeds in the order the stages are listed. When all required decisions are made, the next stage begins and the previous stage is locked.



1. (Optional) To add an existing approval template, select a template from the left side of the dialog.

   >[!TIP]
   >
   >   Users with a Standard license can create reusable Approval Templates from the Setup area. For more information, see [Create an approval workflow template for documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).



1. Once you have added all the stages and participants you need, click **Request approval**.

   The approval workflow starts and the approvers receive a notification that their approval is needed on the new document version. The previous document version is locked and any outstanding approvals on the previous version are withdrawn.

    ![request approval](assets/request-approval.png)
-->

<!--1. To add all previous participants, click **Add all**. You can also add new participants or remove previous participants as needed.-->

## Verwenden Sie Drag-and-Drop, um im Bereich für veraltete Dokumente eine neue Version hinzuzufügen

Wenn sich Ihr Unternehmen im Workfront-Speicher befindet, wird der Bereich für veraltete Dokumente angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Weitere Informationen zu Workfront-Speicher finden Sie unter [Unterschiede zwischen Adobe-Cloud-Speicher und Legacy-Workfront-Speicher](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

>[!NOTE]
>
>Drag-and-Drop funktioniert nicht mit Internet Explorer.

Wenn Sie eine weitere Runde der Überprüfung und Genehmigung für ein Dokument benötigen, können Sie in Workfront eine neue Dokumentversion erstellen. Sie können die vorherigen Teilnehmer, neue Teilnehmer oder eine Mischung aus beiden hinzufügen. Informationen zu früheren Versionen und Teilnehmern finden Sie auf der Seite Dokumentdetails .

Das Dialogfeld Genehmigung anfordern wird standardmäßig im Standardmodus für eine einstufige Genehmigung geöffnet. Wechseln Sie in den erweiterten Modus, um mehrstufige Genehmigungen oder parallele Pfade zu konfigurieren.

So fügen Sie eine neue Version hinzu und fordern die Genehmigung an:

1. Navigieren Sie zum Dokument in Workfront.

1. Ziehen Sie die neue Datei auf das vorherige Dokument. Workfront erstellt automatisch eine neue Version.

1. Nachdem das Dokument hochgeladen wurde, wählen Sie das Dokument aus, um das Bedienfeld Dokumentzusammenfassung zu öffnen. Die Versionsnummer wird oben im Bedienfeld angezeigt.

1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** und klicken Sie dann auf **Workflow erstellen**. Das **„Genehmigung anfordern** wird im Standardmodus geöffnet.

1. Konfigurieren des Validierungs-Workflows. Beschreibung der Felder, des erweiterten Modus-Umschalters und der parallelen Flusspfade finden Sie unter [Erstellen eines Workflow für die Dokumentvalidierung](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

1. Um dieselben Prüfer und genehmigenden Personen aus der vorherigen Dokumentversion zu kopieren, klicken Sie auf **Kopieren**.
1. Klicken Sie **Genehmigung anfordern**.

   Der Genehmigungs-Workflow wird gestartet und die genehmigenden Personen erhalten eine Benachrichtigung, dass ihre Genehmigung für die neue Dokumentversion erforderlich ist. Die vorherige Dokumentversion ist gesperrt und alle ausstehenden Genehmigungen für die vorherige Version werden zurückgezogen.

## Verwenden Sie Drag-and-Drop, um eine neue Version im Bereich Neue Dokumente hinzuzufügen

Wenn Ihr Unternehmen Adobe Cloud Storage verwendet, wird der Bereich Neue Dokumente angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Weitere Informationen zu Adobe Cloud-Speicher finden Sie unter [Übersicht über Adobe Cloud-Speicher](/help/quicksilver/review-and-approve-work/esm-overview.md).

>[!NOTE]
>
>Drag-and-Drop funktioniert nicht mit Internet Explorer.

Wenn Sie eine weitere Runde der Überprüfung und Genehmigung für ein Dokument benötigen, können Sie in Workfront eine neue Dokumentversion erstellen. Sie können der neuen Version des Dokuments einen Genehmigungs-Workflow hinzufügen.

<!--
the previous participants, new participants, or a mix of both. You can view information about previous versions and participants on the Document Details page.
-->

Das Dialogfeld Genehmigung anfordern wird standardmäßig im Standardmodus für eine einstufige Genehmigung geöffnet. Wechseln Sie in den erweiterten Modus, um mehrstufige Genehmigungen oder parallele Pfade zu konfigurieren.

So fügen Sie eine neue Version hinzu und fordern die Genehmigung an:

1. Navigieren Sie zum Dokument in Workfront.

1. Ziehen Sie die neue Datei auf das vorherige Dokument. Workfront erstellt automatisch eine neue Version.

1. Nachdem das Dokument hochgeladen wurde, wählen Sie das Dokument aus, um das Bedienfeld Zusammenfassung zu öffnen. Standardmäßig ist die neueste Version des Dokuments ausgewählt.

1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** und klicken Sie dann auf **Workflow erstellen**. Das **„Genehmigung anfordern** wird im Standardmodus geöffnet.

1. Konfigurieren des Validierungs-Workflows. Beschreibung der Felder, des erweiterten Modus-Umschalters und der parallelen Flusspfade finden Sie unter [Erstellen eines Workflow für die Dokumentvalidierung](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

1. Um dieselben Prüfer und genehmigenden Personen aus der vorherigen Dokumentversion zu kopieren, klicken Sie auf **Kopieren**.
1. Klicken Sie **Genehmigung anfordern**.

   Der Genehmigungs-Workflow wird gestartet und die genehmigenden Personen erhalten eine Benachrichtigung, dass ihre Genehmigung für die neue Dokumentversion erforderlich ist. Die vorherige Dokumentversion ist gesperrt und alle ausstehenden Genehmigungen für die vorherige Version werden zurückgezogen.
