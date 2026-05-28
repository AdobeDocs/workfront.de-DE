---
product-area: documents
navigation-topic: approvals
title: Hinzufügen zusätzlicher genehmigender Personen oder Prüfer zu einem Workflow für die Dokumentvalidierung
description: Sie können einem Dokument, das bereits ausstehende Genehmigungen enthält, zusätzliche genehmigende Personen oder Prüfende hinzufügen.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f3d94dff-a855-44ae-9e85-1dcbc4d417a0
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 7fc5fe2f2692841a8663740441f70be0c82c4073
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 6%

---

# Hinzufügen zusätzlicher genehmigender Personen oder Prüfer zu einem Workflow für die Dokumentvalidierung

Sie können einem Workflow für Dokumentgenehmigungen, der bereits ausstehende Genehmigungen aufweist, zusätzliche genehmigende Personen oder Prüfende hinzufügen.

>[!IMPORTANT]
>
>Der Inhalt dieses Artikels bezieht sich auf aktualisierte Dokumentgenehmigungsfunktionen, die nur für bestimmte Konten verfügbar sind. Informationen zu standardmäßigen Genehmigungsprozessen finden Sie in den Artikeln, die unter [Arbeitsgenehmigungen“ aufgeführt ](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

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



## Fügen Sie zusätzliche genehmigende Personen oder Prüfende aus der Dokumentzusammenfassung im Bereich für veraltete Dokumente hinzu

Wenn sich Ihr Unternehmen im Workfront-Speicher befindet, wird der Bereich für veraltete Dokumente angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Weitere Informationen zu Workfront-Speicher finden Sie unter [Unterschiede zwischen Adobe-Cloud-Speicher und Legacy-Workfront-Speicher](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

So fügen Sie in der Dokumentzusammenfassung zusätzliche genehmigende Personen oder Prüfende hinzu:

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen **Dokumente** im linken Bereich aus.

1. Klicken Sie auf das gewünschte Dokument, und das Bedienfeld Dokumentzusammenfassung für dieses Dokument wird geöffnet.

1. Wählen Sie im Dropdown-Menü Version die Version des Dokuments aus, dem Sie eine genehmigende Person oder eine prüfende Person hinzufügen möchten. Standardmäßig ist die neueste Version ausgewählt.

1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** und klicken Sie dann auf **Workflow bearbeiten**.

   ![Genehmigungs-Workflow bearbeiten](assets/edit-approval-in-legacy.png)

1. Suchen Sie die Phase, der Sie Genehmigende Personen oder Prüfende hinzufügen möchten, und fügen Sie dann den Namen oder die E-Mail-Adresse des Benutzers in das Textfeld ein. Sie können bei Bedarf auch ein ganzes Team hinzufügen.

1. Nachdem ihr Name hinzugefügt wurde, wählen Sie aus, ob sie eine genehmigende Person oder eine prüfende Person sind.

   ![Dropdown „Genehmiger oder Prüfer“](assets/choose-approver-or-reviewer.png)

1. Wiederholen Sie die Schritte 5 bis 6, um weitere genehmigende Personen oder Prüfende hinzuzufügen.
Nach dem Speichern erhalten die hinzugefügten Teilnehmer eine E-Mail-Benachrichtigung, dass ihre Genehmigung oder Überprüfung für das Dokument erforderlich ist.



## Fügen Sie zusätzliche genehmigende Personen oder Prüfende aus der Dokumentzusammenfassung im Bereich Neue Dokumente hinzu

Wenn Ihr Unternehmen Adobe Cloud Storage verwendet, wird der Bereich Neue Dokumente angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Weitere Informationen zu Adobe Cloud-Speicher finden Sie unter [Übersicht über Adobe Cloud-Speicher](/help/quicksilver/review-and-approve-work/esm-overview.md).


1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen **Dokumente** im linken Bereich aus.

1. Klicken Sie auf das Dokument und dann auf **Genehmigungen** rechts auf der Seite.

   ![Genehmigende Personen in der Dokumentzusammenfassung hinzufügen](assets/approvals-icon-new.png)


1. Klicken Sie **Workflow bearbeiten**.

1. Suchen Sie die Phase, der Sie Genehmigende Personen oder Prüfende hinzufügen möchten, und fügen Sie dann den Namen oder die E-Mail-Adresse des Benutzers in das Textfeld ein. Sie können bei Bedarf auch ein ganzes Team hinzufügen.

1. Nachdem ihr Name hinzugefügt wurde, wählen Sie aus, ob sie eine genehmigende Person oder eine prüfende Person sind.

   ![Dropdown „Genehmiger oder Prüfer“](assets/choose-approver-or-reviewer.png)

1. Wiederholen Sie die Schritte 5 bis 6, um weitere genehmigende Personen oder Prüfende hinzuzufügen.
Nach dem Speichern erhalten die hinzugefügten Teilnehmer eine E-Mail-Benachrichtigung, dass ihre Genehmigung oder Überprüfung für das Dokument erforderlich ist.







<!--
## Add additional approvers or reviewers from Home

1. Click the **Home** icon ![Home icon](assets/home-icon-30x29.png) in the upper-left corner of Adobe Workfront.

   >[!NOTE]
   >
   >Your Workfront administrator might make the following changes to the Home icon in your environment:
   >
   >* Replace it with an image customized to illustrate your organization. In this case, the icon will look different that shown in this article. 
   >* Replace the page linked to it with a different page. In this case, click the **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner of the page, then click **Home**.

1. In the **Work List** area, Go to the **Approvals I've Submitted** grouping.

1. Select a **Document** approval.  

1. Click **Manage Approvals**&nbsp;in the upper-right corner of the right panel.
1. In the **Have someone approve this document** box, type the name of the approver.

   If your Adobe Workfront administrator has enabled the capability to collaborate with people who don't use Workfront, as described in [Configure system security preferences](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md), you can type their email addresses to include them.

1. Click **Save**.
-->
