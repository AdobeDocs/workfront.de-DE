---
product-area: documents
navigation-topic: approvals
title: Hinzufügen zusätzlicher genehmigender Personen oder Prüfer zu einem Asset oder Dokument
description: Sie können einem Dokument, das bereits ausstehende Genehmigungen enthält, zusätzliche genehmigende Personen oder Prüfende hinzufügen.
author: Nolan
feature: Work Management, Digital Content and Documents
exl-id: f3d94dff-a855-44ae-9e85-1dcbc4d417a0
source-git-commit: b615236d2666ebcc6db0d1f796fb0baaf362e0f2
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# Hinzufügen zusätzlicher genehmigender Personen oder Prüfer zu einem Asset oder Dokument

Sie können einem Asset oder Dokument, das bereits ausstehende Genehmigungen aufweist, zusätzliche genehmigende Personen oder Prüfende hinzufügen.

>[!IMPORTANT]
>
>Der Inhalt dieses Artikels bezieht sich auf aktualisierte Dokumentgenehmigungsfunktionen, die nur für bestimmte Konten verfügbar sind. Informationen zu standardmäßigen Genehmigungsprozessen finden Sie in den Artikeln, die unter [Arbeitsgenehmigungen“ aufgeführt &#x200B;](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Mitwirkender oder höher</p>
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

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Fügen Sie auf der Seite Dokumentdetails zusätzliche genehmigende Personen oder Prüfende hinzu

1. Gehen Sie zur Dokumentseite, indem Sie auf den Namen des Dokuments klicken, und wählen Sie dann im Dropdown-Menü Version die Version des Dokuments aus, der Sie eine genehmigende Person oder eine prüfende Person hinzufügen möchten. Standardmäßig wird die neueste Version ausgewählt.

1. Wählen **Genehmigungen** im linken Bereich aus. Alle vorhandenen genehmigenden Personen und Prüfer sind hier aufgeführt.

1. Um eine genehmigende Person hinzuzufügen, stellen Sie sicher, dass das **Genehmigende Person** Kontrollkästchen aktiviert ist, und beginnen Sie dann mit der Eingabe in das Textfeld **Prüfende**. Sie können Workfront-Benutzer oder -Teams nach Namen hinzufügen. Wenn Sie stattdessen einen Validierungsverantwortlichen hinzufügen möchten, deaktivieren Sie vor der Eingabe einfach das **Genehmiger**-Kontrollkästchen.

1. Wiederholen Sie den vorherigen Schritt, um weitere genehmigende Personen oder Prüfer hinzuzufügen.

## Hinzufügen zusätzlicher genehmigender Personen oder Prüfer aus der Dokumentzusammenfassung

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente**.

1. Klicken Sie auf das gewünschte Dokument. Daraufhin wird der Bereich Dokumentzusammenfassung geöffnet.

1. Wählen Sie in der Dropdown-Liste Version die Version des Dokuments aus, dem Sie eine genehmigende Person oder eine prüfende Person hinzufügen möchten. Standardmäßig wird die neueste Version ausgewählt.

1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** im Bereich Dokumentzusammenfassung, in dem alle vorhandenen genehmigenden Personen und Prüfer aufgeführt sind. Um eine genehmigende Person hinzuzufügen, stellen Sie sicher, dass das **Genehmigende Person** Kontrollkästchen aktiviert ist, und beginnen Sie dann mit der Eingabe in das Textfeld **Prüfende**. Sie können Workfront-Benutzer oder -Teams nach Namen hinzufügen. Wenn Sie stattdessen einen Validierungsverantwortlichen hinzufügen möchten, deaktivieren Sie vor der Eingabe einfach das **Genehmiger**-Kontrollkästchen.

1. Wiederholen Sie den vorherigen Schritt, um weitere genehmigende Personen oder Prüfer hinzuzufügen.

## Hinzufügen zusätzlicher Überprüfungen und genehmigender Personen aus einer früheren Version

Wenn Sie eine Genehmigung für eine neue Dokumentversion benötigen, können Sie einfach Folgendes hinzufügen

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
