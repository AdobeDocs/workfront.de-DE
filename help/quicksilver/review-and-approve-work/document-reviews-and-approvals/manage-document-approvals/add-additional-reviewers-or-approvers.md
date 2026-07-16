---
product-area: documents
navigation-topic: approvals
title: Hinzufügen zusätzlicher genehmigender Personen oder Prüfer zu einem Workflow für die Dokumentvalidierung
description: Sie können einem Dokument, das bereits ausstehende Genehmigungen enthält, zusätzliche genehmigende Personen oder Prüfende hinzufügen.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f3d94dff-a855-44ae-9e85-1dcbc4d417a0
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jo3N878hmvHRqo6kCepxPDk2-zlalLvqQbMjHHB8aGE
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
source-git-commit: 632c8690acc30121fe72338326ec8ab58c0fd3a6
workflow-type: tm+mt
source-wordcount: 746
ht-degree: 5%

---

# Hinzufügen zusätzlicher genehmigender Personen oder Prüfer zu einem Workflow für die Dokumentvalidierung

Sie können einem Workflow für Dokumentgenehmigungen, der bereits ausstehende Genehmigungen aufweist, zusätzliche genehmigende Personen oder Prüfende hinzufügen.

>[!IMPORTANT]
>
>Der Inhalt dieses Artikels bezieht sich auf aktualisierte Dokumentgenehmigungsfunktionen, die nur für bestimmte Konten verfügbar sind. Informationen zu standardmäßigen Genehmigungsprozessen finden Sie in den Artikeln, die unter [Arbeitsgenehmigungen“ aufgeführt &#x200B;](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Jedes Workfront-Paket zur Verwaltung von Genehmigungen unter Verwendung des alten Workfront-Speichers</p>
<p>Beliebiges Workflow-Paket zum Verwalten von Genehmigungen mithilfe des Adobe-Cloud-Speichers</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Mitwirkende oder höher</p>
   <p>Überprüfen oder höher</p> 
   <p>Wenn Sie die Frame.io-Integration verwenden, benötigen Sie eine Standardlizenz zum Erstellen von Genehmigungs-Workflows.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Anzeigen oder Erweitern des Zugriffs auf Projekte, Aufgaben, Probleme, Vorlagen, Portfolios, Programme, Berichte, Dashboards, Kalender und Dokumente</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen des oder eines höheren Zugriffs auf das Objekt, das mit der Zugriffsanfrage oder Genehmigung verknüpft ist </p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++



<!--
## Add additional approvers or reviewers in the legacy documents area in Production

If your organization is on Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront storage, see [Differences between Adobe cloud storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

To add additional approvers or reviewers from the Document Summary:

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document you need and the Document Summary panel for that document will open.

1. Select the version of the document you would like to add an approver or reviewer to in the version drop-down menu. The latest version is selected by default.

1. Scroll down to the **Approvals** section, then click **Edit workflow**.

   ![edit approval workflow](assets/edit-approval-in-legacy.png)

1. Locate the stage you would like to add approvers or reviewers to, then add the user's name or email in the text box. You can also add an entire team if needed. 

1. Once their name is added, choose if they are an approver or reviewer. 

   ![approver or reviewer drop-down](assets/choose-approver-or-reviewer.png)

1. Repeat steps 5-6 to add additional approvers or reviewers.
 Once you save, the participants added receive an email notification that their approval or review is needed on the document.
-->

## Hinzufügen zusätzlicher genehmigender Personen oder Prüfer im Bereich für veraltete Dokumente

Wenn sich Ihr Unternehmen im Workfront-Speicher befindet, wird der Bereich für veraltete Dokumente angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Weitere Informationen zu Workfront-Speicher finden Sie unter [Unterschiede zwischen Adobe-Cloud-Speicher und Legacy-Workfront-Speicher](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

So fügen Sie in der Dokumentzusammenfassung zusätzliche genehmigende Personen oder Prüfende hinzu:

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen **Dokumente** im linken Bereich aus.

1. Klicken Sie auf das gewünschte Dokument. Das Bedienfeld Dokumentzusammenfassung für dieses Dokument wird geöffnet.

1. Wählen Sie im Dropdown-Menü Version die Version des Dokuments aus, dem Sie eine genehmigende Person oder eine prüfende Person hinzufügen möchten. Standardmäßig ist die neueste Version ausgewählt.

1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** und klicken Sie dann auf **Workflow bearbeiten**. Das Dialogfeld Genehmigung anfordern wird in dem Modus geöffnet, in dem die Genehmigung zuletzt gespeichert wurde: Standard für einstufige Genehmigungen oder Erweitert für mehrstufige Genehmigungen und Genehmigungen mit parallelen Pfaden.

1. Fügen Sie den Benutzer, das Team oder die E-Mail hinzu:

   * Geben Sie im Standardmodus den Namen oder die E-Mail in das Feld **Namen oder E-Mails hinzufügen** ein.
   * Wählen Sie im erweiterten Modus den Pfad aus, der den zu aktualisierenden Schritt enthält, und geben Sie dann den Namen oder die E-Mail in das Feld **Namen oder E-Mails hinzufügen** des Schritts ein.

1. Wählen Sie für jede hinzugefügte Person aus, ob sie eine genehmigende Person oder eine prüfende Person ist.

   ![Dropdown „Genehmiger oder Prüfer“](assets/choose-reviewer-or-approver.png)

1. Klicken Sie auf **Speichern**. Die hinzugefügten Teilnehmer erhalten eine E-Mail-Benachrichtigung, dass ihre Genehmigung oder Überprüfung für das Dokument erforderlich ist.

>[!TIP]
>
>Um eine Grundmodusgenehmigung in eine Mehrstufen- oder Mehrpfad-Genehmigung umzustrukturieren, klicken Sie oben **auf** Zum Erweiterten wechseln“. Ihre vorhandenen Teilnehmer werden als Pfad 1, Schritt 1 beibehalten. Nach dem Speichern können Sie nicht mehr in den Standardmodus wechseln. Weitere Informationen finden Sie unter [Erstellen eines Dokumentgenehmigungs-Workflows](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

<!--
## Add additional approvers or reviewers in the new Documents area in Production

If your organization uses Adobe cloud storage, you will see the new Documents area when you access documents in Workfront. For more information about Adobe cloud storage, see [Adobe cloud storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).


1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document, then click the **Approvals** icon on the right side of the page. 

   ![Add approvers in document summary](assets/approvals-icon-new.png)


1. Click **Edit workflow**.

1. Locate the stage you would like to add approvers or reviewers to, then add the user's name or email in the text box. You can also add an entire team if needed. 

1. Once their name is added, choose if they are an approver or reviewer. 

   ![approver or reviewer drop-down](assets/choose-approver-or-reviewer.png)

1. Repeat steps 5-6 to add additional approvers or reviewers.
 Once you save, the participants added receive an email notification that their approval or review is needed on the document.
-->

## Fügen Sie zusätzliche genehmigende Personen oder Prüfende aus der Dokumentzusammenfassung im Bereich Neue Dokumente hinzu

Wenn Ihr Unternehmen Adobe Cloud Storage verwendet, wird der Bereich Neue Dokumente angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Weitere Informationen zu Adobe Cloud-Speicher finden Sie unter [Übersicht über Adobe Cloud-Speicher](/help/quicksilver/review-and-approve-work/esm-overview.md).

So fügen Sie in der Dokumentzusammenfassung zusätzliche genehmigende Personen oder Prüfende hinzu:

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen **Dokumente** im linken Bereich aus.

1. Klicken Sie auf das Dokument und dann auf **Genehmigungen** rechts auf der Seite.

   ![Genehmigende Personen in der Dokumentzusammenfassung hinzufügen](assets/approvals-icon-new.png)

1. Klicken Sie **Workflow bearbeiten**. Das Dialogfeld Genehmigung anfordern wird in dem Modus geöffnet, in dem die Genehmigung zuletzt gespeichert wurde: Standard für einstufige Genehmigungen oder Erweitert für mehrstufige Genehmigungen und Genehmigungen mit parallelen Pfaden.

1. Fügen Sie den Benutzer, das Team oder die E-Mail hinzu:

   * Geben Sie im Standardmodus den Namen oder die E-Mail in das Feld **Namen oder E-Mails hinzufügen** ein.
   * Wählen Sie im erweiterten Modus den Pfad aus, der den zu aktualisierenden Schritt enthält, und geben Sie dann den Namen oder die E-Mail in das Feld **Namen oder E-Mails hinzufügen** des Schritts ein.

1. Wählen Sie für jede hinzugefügte Person aus, ob sie eine genehmigende Person oder eine prüfende Person ist.

   ![Dropdown „Genehmiger oder Prüfer“](assets/choose-reviewer-or-approver.png)

1. Klicken Sie auf **Speichern**. Die hinzugefügten Teilnehmer erhalten eine E-Mail-Benachrichtigung, dass ihre Genehmigung oder Überprüfung für das Dokument erforderlich ist.

>[!TIP]
>
>Um eine Grundmodusgenehmigung in eine Mehrstufen- oder Mehrpfad-Genehmigung umzustrukturieren, klicken Sie oben **auf** Zum Erweiterten wechseln“. Ihre vorhandenen Teilnehmer werden als Pfad 1, Schritt 1 beibehalten. Nach dem Speichern können Sie nicht mehr in den Standardmodus wechseln. Weitere Informationen finden Sie unter [Erstellen eines Dokumentgenehmigungs-Workflows](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).
