---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: Bearbeiten von Phasen und prüfenden Personen für einen Korrekturabzug
description: Erfahren Sie, wie Sie Testversandphasen und Prüfer bearbeiten.
author: Courtney
feature: Digital Content and Documents
exl-id: 91549c2d-d7b1-461c-a3c4-ad0032acfb23
TQID: https://experienceleague.adobe.com/yh9htEooQ267a5ZSL60NXX5xNSuUJcBC2sjZOwF8VBY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 25d403b9266c31a39c1dce6c1c45ad96ee90af28
workflow-type: tm+mt
source-wordcount: 608
ht-degree: 9%

---

# Bearbeiten von Phasen und prüfenden Personen für einen Korrekturabzug

Sie können die Phasen und die Details der Prüfer in einem Korrekturabzug bearbeiten, wenn Sie der/die Verantwortliche oder Ersteller des Korrekturabzugs sind oder Ihnen die richtige Rolle zugewiesen wurde.

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
   <p>Standard</p>
   <p>Arbeit oder Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Korrekturabzug-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Rolle des Korrekturabzugs</td> 
   <td>Autor oder Moderator </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriffrecht „Bearbeiten“ für Dokumente</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Bearbeiten eines Schritts

1. Bewegen Sie in einer Dokumentliste, die das Dokument enthält, den Mauszeiger über die Zeile, die das Dokument enthält, und klicken Sie dann auf **Proofing-Workflow**.

   ODER

   Klicken Sie in der eigenständigen Workfront Proof auf das **Mehr**-Menü (drei Punkte) rechts neben dem Korrekturabzug und dann auf **Details des Korrekturabzugs anzeigen**.

1. Nehmen Sie im Abschnitt **Workflow** eine der folgenden Änderungen vor:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Fristablauf bearbeiten</td> 
      <td> <p>Wählen Sie das Datum und wählen Sie ein neues Datum im Kalender, das angezeigt wird. Um die Frist vollständig zu entfernen, wählen Sie das Datum aus und wählen Sie dann <strong>Löschen</strong> unter dem angezeigten Kalender aus.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entfernen einzelner Reviewer</td> 
      <td> <p>Wählen Sie das <strong>Mehr</strong>-Menü rechts neben dem Namen des Reviewers aus und klicken Sie dann </strong> Dropdown-Menü auf <strong>Entfernen“. Klicken Sie <strong>Bestätigen</strong> in dem Feld, das angezeigt wird, um den Prüfer aus dem Korrekturabzug zu entfernen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mehrere Reviewer entfernen</td> 
      <td>Aktivieren Sie die Kontrollkästchen neben ihren Namen und klicken Sie dann auf das <strong>Löschen</strong>-Symbol in der oberen rechten Ecke des Abschnitts „Phase“.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nachricht an alle Reviewer</td> 
      <td>Wählen Sie das <strong>Mehr</strong>-Menü in der oberen rechten Ecke des Abschnitts „Phase“ und dann <strong>Nachricht an alle</strong> aus. Konfigurieren Sie Ihre Nachricht und wählen Sie dann <strong>Senden</strong> aus.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hinzufügen eines Reviewers zum Schritt</td> 
      <td>Wählen Sie das <strong>Mehr</strong>-Menü in der oberen rechten Ecke des Abschnitts „Phase“ und dann <strong>Freigeben</strong>. Fügen Sie den Benutzer hinzu, konfigurieren Sie seine Rolle und E-Mail-Warnhinweise und wiederholen Sie den Vorgang bei Bedarf. Klicken Sie abschließend auf <strong>Freigeben</strong>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Stadium löschen</td> 
      <td> <p>Wählen Sie das <strong>Mehr</strong>-Menü in der oberen rechten Ecke des Abschnitts „Phase“ und wählen Sie <strong>Löschen</strong>.</p> <p>Hinweis: Wenn es nur einen Schritt gibt, kann der Schritt nicht gelöscht werden.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Wenn die validierungsverantwortliche Person, die Sie entfernen, bereits eine Entscheidung über den Korrekturabzug getroffen hat, wird im Feld Entscheidung der genehmigenden Person für diese Person im Bericht Korrekturabzugsgenehmigung ein Bindestrich (-) angezeigt. Weitere Informationen finden Sie unter [Entscheidung der genehmigenden Person zeigt im Bericht zu Korrekturabzugsgenehmigungen einen Bindestrich an](../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/approver-decision-shows-hyphen.md).

## Reviewer-Details bearbeiten

1. Bewegen Sie in Workfront den Mauszeiger über den Korrekturabzug und klicken Sie dann auf **Korrekturabzugsdetails**, um die Seite mit den Korrekturabzugsdetails zu öffnen.
1. Klicken **Abschnitt „Workflow** auf das Menü **Mehr** ![Mehr](assets/more-button-small.png) rechts neben dem Namen des Reviewers und klicken Sie dann im angezeigten Dropdown-Menü auf **Bearbeiten**.

1. Bearbeiten Sie **angezeigten** „Reviewer bearbeiten“ eine der folgenden Details:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Anzeigename*</td> 
      <td> <p>Um den Anzeigenamen des Reviewers im Korrekturabzug zu ändern, klicken Sie in das Textfeld und bearbeiten Sie seinen Namen inline.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rolle</td> 
      <td>Um die Rolle des Validierungsverantwortlichen im Testversand zu ändern, öffnen Sie das Dropdown-Menü und wählen Sie die bevorzugte Rolle aus. Weitere Informationen finden Sie unter.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">E-Mail-Warnungen</td> 
      <td>Um den E-Mail-Warnhinweis des Reviewers für den Testversand zu ändern, öffnen Sie das Dropdown-Menü und wählen Sie den gewünschten E-Mail-Warnhinweis aus. Weitere Informationen finden Sie im Artikel <a href="../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md" class="MCXref xref">Benachrichtigungen für Korrekturabzugskommentare und Entscheidungen - Übersicht</a>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Entscheidung*</td> 
      <td> <p>Um die Entscheidung des Reviewers bezüglich des Korrekturabzugs zu ändern, öffnen Sie das Dropdown-Menü und wählen Sie die bevorzugte Entscheidung aus. Beachten Sie, dass alle Entscheidungen, die Sie im Namen eines anderen Benutzers treffen, im Abschnitt Aktivität des Korrekturabzugs vermerkt sind. Diese Option wird nur angezeigt, wenn die Überprüfung eine Entscheidung getroffen hat.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Staging</td> 
      <td>Es ist nicht möglich, Reviewer zwischen verschiedenen Phasen zu verschieben. Sie können jedoch einen Reviewer mit einer anderen Frist entfernen und erneut hinzufügen.</td> 
     </tr> 
    </tbody> 
   </table>

   &#42; Sie müssen der Ersteller oder Inhaber des Korrekturabzugs sein, um dieses Feld bearbeiten zu können.

1. Klicken Sie auf **Speichern**.
