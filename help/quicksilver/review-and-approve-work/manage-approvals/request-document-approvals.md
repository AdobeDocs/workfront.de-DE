---
product-area: documents
navigation-topic: approvals
title: Legacy-Dokumentgenehmigung anfordern
description: Sie können eine Genehmigung von Managern oder anderen Benutzern für ein Dokument in Adobe Workfront anfordern. Sie können auch Dokumentgenehmigungen von Personen ohne Workfront-Konten anfordern, wenn Ihr Workfront-Administrator diese Funktion aktiviert hat, wie in Konfigurieren von Systemsicherheitseinstellungen beschrieben.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
TQID: https://experienceleague.adobe.com/NQgXFcbc-4DiObeNE2nRgaW9iKeCKRD5v7J1PRfHkHU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 530
ht-degree: 6%

---

# Legacy-Dokumentgenehmigung anfordern

Sie können eine Genehmigung von Managern oder anderen Benutzern für ein Dokument in Adobe Workfront anfordern. Sie können auch Dokumentgenehmigungen von Personen ohne Workfront-Konten anfordern, wenn Ihr Workfront-Administrator diese Funktion aktiviert hat, wie in [Konfigurieren von Systemsicherheitseinstellungen](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md) beschrieben.

>[!NOTE]
>
>Die Informationen in diesem Artikel beziehen sich auf ältere Dokumentengenehmigungen. <br>
>Informationen zur neuen einheitlichen Überprüfung und Genehmigung finden Sie unter [Einheitliche Überprüfung und Genehmigung - Übersicht](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).


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
   <p>Beitragen oder höher</p>
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

## Dokumentengenehmigung anfordern

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente**.
1. Suchen Sie das Dokument, das Sie benötigen.

1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** in der Zusammenfassung und beginnen Sie mit der Eingabe in das Textfeld **Genehmigende Person hinzufügen**. Sie können Workfront-Benutzer nach Namen oder externe Benutzer nach E-Mail hinzufügen.

1. Wenn Ihr Adobe Workfront-Administrator die Funktion zur Zusammenarbeit mit Personen aktiviert hat, die Workfront nicht verwenden, wie in [Konfigurieren von Systemsicherheitseinstellungen](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md) beschrieben, können Sie deren E-Mail-Adressen eingeben, um sie einzuschließen.

   Sie können keine Genehmigung von Teams oder Gruppen anfordern.

1. Wiederholen Sie den vorherigen Schritt, um weitere genehmigende Personen hinzuzufügen.

## Erneutes Senden einer Genehmigung für eine neue Version

Entscheidungen zu Dokumentgenehmigungen werden beim Hochladen einer neuen Version nicht automatisch zurückgesetzt. Wenn Ihr Dokument beispielsweise mit Änderungen genehmigt wurde, zeigt die Entscheidung „Änderungen“ als Entscheidung an, auch wenn Sie eine neue Version mit den angegebenen Änderungen hochladen. Sie können die Entscheidung für eine neue Version löschen, wenn Sie die Genehmigung manuell erneut übermitteln.

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
