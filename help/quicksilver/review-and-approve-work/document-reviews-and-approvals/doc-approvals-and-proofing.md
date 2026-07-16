---
product-area: documents
navigation-topic: approvals
title: Gemeinsames Verwenden von einheitlichen Genehmigungen und Proofing
description: Sie können einheitliche Genehmigungen mit Proofing verwenden.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: be484629-6e70-4809-ad4c-a489d5814da6
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/UBrLQv-1DRwZ-TO3c1SAUn8OF0yOAYnKPGrf-lSS0xM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 632c8690acc30121fe72338326ec8ab58c0fd3a6
workflow-type: tm+mt
source-wordcount: 678
ht-degree: 1%

---

# Gemeinsames Verwenden von einheitlichen Genehmigungen und Proofing

Einheitliche Genehmigungen in Workfront beinhalten jetzt eine Reihe neuer Funktionen, mit denen Sie Dokumente überprüfen und genehmigen können. Sie können einen einheitlichen Genehmigungs-Workflow mit dem vorhandenen Proofing Viewer verwenden, um Kommentare und Markups zu überprüfenden Dokumenten hinzuzufügen.

Es gibt einige wichtige Unterschiede im Workflow bei der gemeinsamen Verwendung von einheitlichen Genehmigungen und Proofing:

* Die Teilnehmer werden in der Dokumentzusammenfassung und nicht im Proofing-Workflow angezeigt.

* Die Details „Gesendet“, „Geöffnet“, „Kommentar“, „Entscheidung (SOCD)“ in der Dokumentliste sind mit Proofing verbunden und spiegeln den Entscheidungsstatus des Dokuments nicht wider.

## Dokument hochladen und Korrekturabzug erstellen

1. Navigieren Sie zum Projekt, zur Aufgabe oder zum Problem, dem bzw. dem Sie ein neues Dokument hinzufügen möchten.
1. Klicken Sie auf **Registerkarte** Dokumente“ und dann auf das **Neu hinzufügen** Dropdown-Menü.
ODER
Ziehen Sie das Dokument per Drag-and-Drop in die Dokumentliste.

   >[!NOTE]
   >
   >Wenn Sie in **Benutzerprofil „Korrekturabzüge beim Hochladen von Dokumenten automatisch generieren** aktiviert haben, erstellt das System automatisch einen einfachen Korrekturabzug.

1. Bewegen Sie den Mauszeiger über das Dokument und klicken Sie dann auf den **Korrekturabzug erstellen** Link, der unter dem Dokumentnamen angezeigt wird, und wählen Sie **Einfacher Korrekturabzug** aus. Sie müssen einen einfachen Korrekturabzug erstellen, da Sie den Proofing-Workflow nicht für Genehmigungen verwenden werden.

Benutzende, die als Teilnehmer zugewiesen sind, können die Proofing Viewer verwenden, um Kommentare und Markups zu dem Dokument hinzuzufügen. Fahren Sie mit dem nächsten Abschnitt fort, um zu erfahren, wie Sie Reviewer hinzufügen.

<!--
## Open the document Summary and assign participants in Production

You have the option to assign reviewers, approvers, or a mix of both:

* **Reviewers** can add comments and mark up assets. Once finished, they can mark their review as complete. Marking the review as complete is not required for the document to move forward in the approval process.
* **Approvers** can add comments and mark up assets. They must make a decision to move the approval process forward. 

To assign participants:

1. Select the document you uploaded and open the document Summary.
    ![Open document summary](assets/open-doc-summary.png)

1. Scroll down to the **Approvals** section, then click **Create workflow**.


1. Fill in the following details:

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

   ![new stage](assets/new-stage.png)

1. Once you've added all reviewers and approvers, click **Request approvals**. Participants are notified via email.
-->

## Öffnen Sie die Dokumentzusammenfassung und weisen Sie Teilnehmer zu

Das Dialogfeld Genehmigung anfordern wird standardmäßig im Standardmodus für eine einstufige Genehmigung geöffnet. Wechseln Sie in den erweiterten Modus, um mehrstufige Genehmigungen oder parallele Pfade zu konfigurieren.

So weisen Sie Teilnehmer zu:

1. Wählen Sie das hochgeladene Dokument aus und öffnen Sie die Dokumentzusammenfassung.

   ![Dokumentzusammenfassung öffnen](assets/open-doc-summary.png)

1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** und klicken Sie dann auf **Workflow erstellen**. Das **„Genehmigung anfordern** wird im Standardmodus geöffnet.

1. Konfigurieren des Validierungs-Workflows. Beschreibung der Felder, des erweiterten Modus-Umschalters und der parallelen Flusspfade finden Sie unter [Erstellen eines Workflow für die Dokumentvalidierung](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

1. Klicken Sie **Genehmigung anfordern**. Die Teilnehmer werden per E-Mail benachrichtigt.

<!--
## Create a new version as needed in Production

If you need another round of review and approval, you can create a new proof version and add the previous participants, new participants, or a mix of both. You can view information about previous versions and participants in the document Summary.

To add a new version:

1. Drag and drop the new file on top of the previous document in Workfront. This automatically creates a new version. 

1. Once the document finishes uploading, select the document, then click **Create proof** > **Simple proof**. 

1. Select the document again, and open the document Summary.
    ![Open document summary](assets/open-doc-summary.png)

1. Scroll down to the **Approvals** section, then click **Create workflow**.


1. Fill in the following details:

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

   ![new stage](assets/new-stage.png)

1. Once you've added all reviewers and approvers, click **Request approvals**. Participants are notified via email.
-->

## Erstellen Sie nach Bedarf eine neue Version

Wenn Sie eine weitere Runde der Überprüfung und Genehmigung benötigen, können Sie eine neue Korrekturabzugsversion erstellen und die vorherigen Teilnehmer, neue Teilnehmer oder eine Mischung aus beiden hinzufügen. In der Dokumentzusammenfassung können Sie Informationen zu früheren Versionen und Teilnehmern anzeigen.

Das Dialogfeld Genehmigung anfordern wird standardmäßig im Standardmodus für eine einstufige Genehmigung geöffnet. Wechseln Sie in den erweiterten Modus, um mehrstufige Genehmigungen oder parallele Pfade zu konfigurieren.

Hinzufügen einer neuen Version:

1. Ziehen Sie die neue Datei per Drag-and-Drop auf das vorherige Dokument in Workfront. Workfront erstellt automatisch eine neue Version.

1. Nachdem das Dokument hochgeladen wurde, wählen Sie das Dokument aus und klicken Sie auf **Korrekturabzug erstellen** > **Einfacher Korrekturabzug**.

1. Wählen Sie das Dokument erneut aus und öffnen Sie dann die Dokumentzusammenfassung.

   ![Dokumentzusammenfassung öffnen](assets/open-doc-summary.png)

1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** und klicken Sie dann auf **Workflow erstellen**. Das **„Genehmigung anfordern** wird im Standardmodus geöffnet.

1. Konfigurieren des Validierungs-Workflows. Beschreibung der Felder, des erweiterten Modus-Umschalters und der parallelen Flusspfade finden Sie unter [Erstellen eines Workflow für die Dokumentvalidierung](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

1. Klicken Sie **Genehmigung anfordern**. Die Teilnehmer werden per E-Mail benachrichtigt.

## Korrekturabzug prüfen und eine Entscheidung treffen

Das Dokument wechselt erst dann in den Status Genehmigt , wenn alle zugewiesenen genehmigenden Personen „Genehmigt“ auswählen.

So überprüfen und genehmigen Sie ein Dokument:

1. Gehen Sie zu Ihrer E-Mail-Benachrichtigung und klicken Sie auf **Zum Überprüfen gehen**.

1. Wenn Sie sich in Workfront befinden, klicken Sie auf **Zum Korrekturabzug gehen**.

1. Überprüfen Sie den Inhalt und fügen Sie Kommentare oder Markup hinzu. Weitere Informationen zur Verwendung der Proofing-Anzeige finden Sie unter [Testsendungen in Adobe Workfront überprüfen: Artikelindex](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Wählen Sie eine der folgenden Entscheidungen:

   * **Genehmigen**: Das Dokument muss nicht geändert werden und ist einsatzbereit.
   * **Mit Änderungen genehmigen**: Das Dokument benötigt Änderungen und ist nach deren Vornahme zur Verwendung bereit. Eine zusätzliche Genehmigung ist nicht erforderlich.
   * **Muss überarbeitet werden**: Das Dokument muss geändert werden und ist nicht einsatzbereit. Sobald die angegebenen Änderungen vorgenommen wurden, muss das Dokument als neue Version hochgeladen werden und eine weitere Genehmigungsrunde durchlaufen. Weitere Informationen zum Hochladen einer neuen Version finden Sie unter [Erstellen einer neuen Version nach Bedarf](#create-a-new-version-as-needed) in diesem Artikel.

Sobald Sie eine Entscheidung treffen, wird der Dokumentverantwortliche per E-Mail benachrichtigt.