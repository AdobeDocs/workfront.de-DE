---
product-area: documents
navigation-topic: approvals
title: Request a legacy document approval
description: You can request approval from managers or other users for a document in Adobe Workfront. You can also request document approvals from people without Workfront accounts if your Workfront administrator has enabled this capability, as described in Configure system security preferences.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
source-git-commit: 0c4904a380dd62b9ea01dd1030ee02d82a869541
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 6%

---

# Request a legacy document approval

You can request approval from managers or other users for a document in Adobe Workfront. You can also request document approvals from people without Workfront accounts if your Workfront administrator has enabled this capability, as described in [Configure system security preferences](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

>[!NOTE]
>
>The information in this article refers to legacy document approvals. <br>
>For information about new Unified Review and Approval, see [Unified review and approval overview](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).


## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Contrbute or higher</p>
   <p>Überprüfen oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Anzeigen oder Erweitern des Zugriffs auf Projekte, Aufgaben, Probleme, Vorlagen, Portfolios, Programme, Berichte, Dashboards, Kalender und Dokumente</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten des Zugriffs auf das Objekt, das mit der Zugriffsanforderung oder Genehmigung verknüpft ist </p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Request a document approval

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente**.
1. Suchen Sie das Dokument, das Sie benötigen.

1. Scroll down to the **Approvals** section in the Summary, and begin typing in the **Add Approver** text box. You can add Workfront users by name or external users by email.

1. Wenn Ihr Adobe Workfront-Administrator die Funktion zur Zusammenarbeit mit Personen aktiviert hat, die Workfront nicht verwenden, wie in [Konfigurieren von Systemsicherheitseinstellungen](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md) beschrieben, können Sie deren E-Mail-Adressen eingeben, um sie einzuschließen.

   You cannot request approval from teams or groups.

1. Repeat the previous step to add other approvers.

## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show &quot;changes&quot; as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente**.
1. Suchen Sie das Dokument, das Sie benötigen.

1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** in der Zusammenfassung, klicken Sie auf das Symbol Mehr und dann auf Erneut übermitteln .

   ![Genehmigung erneut übermitteln](assets/nwe-resubmit-approval-350x149.png)

## Löschen einer Dokumentgenehmigungsanfrage

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente**.
1. Suchen Sie das Dokument, das Sie benötigen.

1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** in der Zusammenfassung, klicken Sie dann auf das Menü **Mehr** , das den Namen der genehmigenden Person enthält, und wählen Sie **Löschen**.

   Die Genehmigungsanforderung wird entfernt und die genehmigende Person erhält eine Benachrichtigung, dass ihre Genehmigung nicht mehr erforderlich ist. Ihr genehmigungsbezogener Freigabezugang wird ebenfalls entfernt.

## Erinnerung an eine genehmigende Person senden

Sie können eine Nachricht senden, um eine genehmigende Person daran zu erinnern, dass Sie auf ihr Feedback warten.

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente**.
1. Suchen Sie das Dokument, das Sie benötigen.

1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** in der Zusammenfassung, klicken Sie dann auf das Menü **Mehr** , das den Namen der genehmigenden Person enthält, und wählen Sie **Erinnern** aus.

   Die genehmigende Person erhält eine Benachrichtigung, in der sie darüber informiert wird, dass die Genehmigung noch aussteht. Sie erhalten möglicherweise auch eine E-Mail-Erinnerung, wenn sie diese aktiviert haben.
