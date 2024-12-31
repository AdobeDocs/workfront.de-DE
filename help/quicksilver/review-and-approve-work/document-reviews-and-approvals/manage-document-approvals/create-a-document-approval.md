---
product-area: documents
navigation-topic: approvals
title: Erstellen einer Prüfungs- oder Genehmigungsanfrage für ein Dokument
description: Sie können die Genehmigung anderer Benutzer für ein Dokument in Adobe Workfront anfordern.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
source-git-commit: a1a5c2bb9395748c4e0103d10dcf66624238032b
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# Erstellen einer Prüfungs- oder Genehmigungsanfrage für ein Dokument

Sie können die Genehmigung anderer Benutzer oder Teams für ein Dokument in Adobe Workfront anfordern oder diese auffordern, ein Dokument zu überprüfen, ohne es genehmigen zu müssen.

>[!IMPORTANT]
>
>Der Inhalt dieses Artikels bezieht sich auf aktualisierte Dokumentgenehmigungsfunktionen, die nur für bestimmte Konten verfügbar sind. Informationen zu standardmäßigen Genehmigungsprozessen finden Sie in den Artikeln, die unter [Arbeitsgenehmigungen“ aufgeführt ](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.


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
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Anzeigen oder Hochladen von Zugriff auf Projekte, Aufgaben, Probleme, Vorlagen, Portfolios, Programme, Berichte, Dashboards, Kalender und Dokumente</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten des Zugriffs auf das Objekt, das mit der Zugriffsanforderung oder Genehmigung verknüpft ist </p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

+++

## Erstellen einer Prüfungs- oder Genehmigungsanfrage für ein Dokument über die Dokumentseite

1. Bewegen Sie den Mauszeiger über das Dokument und klicken Sie dann auf Dokumentdetails.
   ![](assets/doc-details.png)


1. Wählen Sie in der Nähe des Dokumentnamens in der Dropdown-Liste Version die Version des Dokuments aus, für das Sie eine Genehmigung erstellen möchten. Standardmäßig wird die neueste Version ausgewählt.

1. Klicken **im** Bereich auf „Genehmigungen“.

1. (Optional) Legen Sie eine Frist für die Genehmigung fest. Benutzer und Teams werden 72 Stunden und dann 24 Stunden vor dem angegebenen Termin per E-Mail benachrichtigt.

1. Um eine genehmigende Person hinzuzufügen, klicken Sie auf **genehmigende Person** und beginnen Sie mit der Eingabe eines Benutzer- oder Teamnamens.

1. Um einen Reviewer hinzuzufügen, aktivieren Sie das **Reviewer** und geben Sie einen Benutzer- oder Teamnamen ein.

   ![](assets/add-approver-and-deadline.png)

1. Wiederholen Sie den vorherigen Schritt, um weitere genehmigende Personen oder Prüfer hinzuzufügen.

## Erstellen einer Anfrage zur Überprüfung oder Genehmigung von Dokumenten über das Bedienfeld Dokumentzusammenfassung

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente**.

1. Klicken Sie auf das gewünschte Dokument. Daraufhin wird der Bereich Dokumentzusammenfassung für dieses Dokument geöffnet.

1. Wählen Sie in der Dropdown-Liste Version die Version des Dokuments aus, für das Sie eine Genehmigung erstellen möchten. Standardmäßig wird die neueste Version ausgewählt.

1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** im Bereich Dokumentzusammenfassung und klicken Sie dann auf **Hinzufügen**.

![](assets/doc-summary-add-approvers.png)

1. (Optional) Legen Sie eine Frist für die Genehmigung fest. Benutzer und Teams werden 72 Stunden und dann 24 Stunden vor dem angegebenen Termin per E-Mail benachrichtigt.

1. Um eine genehmigende Person hinzuzufügen, klicken Sie auf **genehmigende Person** und beginnen Sie mit der Eingabe eines Benutzer- oder Teamnamens.

1. Um einen Reviewer hinzuzufügen, aktivieren Sie das **Reviewer** und geben Sie einen Benutzer- oder Teamnamen ein.

   ![](assets/add-approver-and-deadline.png)

1. Wiederholen Sie den vorherigen Schritt, um weitere genehmigende Personen oder Prüfer hinzuzufügen.





<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![](assets/nwe-resubmit-approval-350x149.png)
-->
