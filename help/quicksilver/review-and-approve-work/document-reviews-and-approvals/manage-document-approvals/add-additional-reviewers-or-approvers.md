---
product-area: documents
navigation-topic: approvals
title: Hinzufügen zusätzlicher Genehmiger oder Validierer zu einem Dokument
description: Sie können einem Dokument, für das bereits ausstehende Genehmigungen vorliegen, weitere Genehmiger oder Validierer hinzufügen.
author: Nolan
feature: Work Management
source-git-commit: 2ae69970ebf5c72d4c192f8158bdc412c084ce35
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---


# Hinzufügen zusätzlicher Genehmiger oder Validierer zu einem Dokument

Sie können einem Dokument, für das bereits ausstehende Genehmigungen vorliegen, weitere Genehmiger oder Validierer hinzufügen.

>[!IMPORTANT]
>
>Der Inhalt dieses Artikels bezieht sich auf die aktualisierte Funktion zur Dokumentgenehmigung, die nur für bestimmte Konten verfügbar ist. Informationen zu Standardgenehmigungsverfahren finden Sie in den Artikeln unter [Arbeitsgenehmigungen](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte, Aufgaben, Probleme, Vorlagen, Portfolios, Programme, Berichte, Dashboards und Kalender, Dokumente anzeigen oder höher</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder höherer Zugriff auf das Objekt, das mit dem Anforderungszugriff oder der Genehmigung verknüpft ist </p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Zusätzliche Genehmiger oder Validierer von der Dokumentseite hinzufügen

1. Klicken Sie auf die Dokumentseite, um auf den Namen des Dokuments zu klicken, und wählen Sie dann die Version des Dokuments aus, zu der Sie im Dropdown-Menü Version einen Genehmiger oder Überprüfer hinzufügen möchten. Standardmäßig wird die neueste Version ausgewählt.

1. Auswählen **Genehmigungen** im linken Bereich. Alle vorhandenen Genehmiger und Validierungsverantwortlichen sind hier aufgeführt.

1. Um einen Genehmiger hinzuzufügen, stellen Sie sicher, dass das **Genehmiger** das Kontrollkästchen aktiviert ist und die Eingabe im **Überprüfer** Textfeld. Sie können Workfront-Benutzer oder -Teams anhand des Namens hinzufügen. Wenn Sie stattdessen einen Validierer hinzufügen möchten, deaktivieren Sie einfach die **Genehmiger** vor der Eingabe.

1. Wiederholen Sie den vorherigen Schritt, um weitere Genehmiger oder Validierer hinzuzufügen.

## Fügen Sie im Bereich &quot;Dokumentzusammenfassung&quot;zusätzliche Genehmiger oder Validierer hinzu

1. Wechseln Sie zum Projekt, zur Aufgabe oder zum Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente**.

1. Klicken Sie auf das gewünschte Dokument und der Bereich Dokumentzusammenfassung wird geöffnet.

1. Wählen Sie die Version des Dokuments aus, zu dem Sie einen Genehmiger oder Überprüfer im Dropdown-Menü Version hinzufügen möchten. Standardmäßig wird die neueste Version ausgewählt.

1. Scrollen Sie nach unten zum **Genehmigungen** im Bereich &quot;Dokumentzusammenfassung&quot;, in dem alle vorhandenen Genehmiger und Validierer aufgelistet sind. Um einen Genehmiger hinzuzufügen, stellen Sie sicher, dass das **Genehmiger** das Kontrollkästchen aktiviert ist und die Eingabe im **Überprüfer** Textfeld. Sie können Workfront-Benutzer oder -Teams anhand des Namens hinzufügen. Wenn Sie stattdessen einen Validierer hinzufügen möchten, deaktivieren Sie einfach die **Genehmiger** vor der Eingabe.

1. Wiederholen Sie den vorherigen Schritt, um weitere Genehmiger oder Validierer hinzuzufügen.

<!--
## Add additional approvers or reviewers from Home

1. Click the **Home** icon ![](assets/home-icon-30x29.png) in the upper-left corner of Adobe Workfront.

   >[!NOTE]
   >
   >Your Workfront administrator might make the following changes to the Home icon in your environment:
   >
   >* Replace it with an image customized to illustrate your organization. In this case, the icon will look different that shown in this article. 
   >* Replace the page linked to it with a different page. In this case, click the **Main Menu** ![](assets/main-menu-icon.png) in the upper-right corner of the page, then click **Home**.

1. In the **Work List** area, Go to the **Approvals I've Submitted** grouping.

1. Select a **Document** approval.  

1. Click **Manage Approvals**&nbsp;in the upper-right corner of the right panel.
1. In the **Have someone approve this document** box, type the name of the approver.

   If your Adobe Workfront administrator has enabled the capability to collaborate with people who don't use Workfront, as described in [Configure system security preferences](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md), you can type their email addresses to include them.

1. Click **Save**.
-->