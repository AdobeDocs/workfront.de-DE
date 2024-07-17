---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Entscheidungsfindung über einen Testversand im Testversand-Viewer
description: Sie können eine Entscheidung über einen Testversand direkt im Testversand-Viewer treffen.
author: Courtney
feature: Digital Content and Documents
exl-id: cf74ac54-b8c1-4404-b35f-2aa94831ecad
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 3%

---

# Entscheidungsfindung über einen Testversand im Testversand-Viewer

Sie können eine Entscheidung über einen Testversand direkt im Testversand-Viewer treffen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Veralteter Plan: Wählen Sie oder Premium</p> <p>Weitere Informationen zum Testen des Zugriffs mit den verschiedenen Plänen finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Testfunktion in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Aktueller Plan: Arbeit oder Plan</p> <p>Veralteter Plan: Beliebig (Sie müssen die Testfunktion für den Benutzer aktiviert haben)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof role</td> 
   <td>Genehmiger, Prüfer und Genehmiger, Autor, Moderator</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um zu erfahren, welchen Plan, welche Rolle oder welches Profil für die Testberechtigung Sie haben.

## Entscheidungsfindung über einen Testversand im Testversand-Viewer

1. Wechseln Sie zum Projekt, zur Aufgabe oder zum Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente** aus.
1. Suchen Sie den gewünschten Testversand und klicken Sie dann auf **Testversand öffnen**.

1. Klicken Sie in der oberen Mitte des Testversand-Viewers auf **Entscheidung treffen** .

1. Klicken Sie im angezeigten Feld **Testversand-Entscheidung** auf eine der folgenden Entscheidungen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Genehmigt</td> 
      <td>Der Testversand ist bereit, zur nächsten Phase des automatisierten Workflows zu wechseln.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mit Änderungen genehmigt</td> 
      <td>Der Testversand erfordert einige Änderungen, Sie müssen die Revision jedoch nicht sehen, bevor sie zur nächsten Phase des automatisierten Workflows wechselt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erforderliche Änderungen</td> 
      <td>Der Testversand erfordert Änderungen und Sie müssen eine weitere Revision sehen, bevor er zur nächsten Phase des automatisierten Workflows wechselt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nicht relevant</td> 
      <td>Der Nachweis ist für Sie nicht relevant und Sie müssen keine Entscheidung treffen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzerdefinierte Entscheidung</td> 
      <td> <p>Bei Auswahl- und Premium-Plänen kann der Workfront-Administrator oder Workfront Proof-Administrator Entscheidungen umbenennen, neu anordnen und ausblenden. Weitere Informationen finden Sie unter <a href="../../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md" class="MCXref xref">Optionen für Genehmigungsentscheidungen in Workfront Proof konfigurieren</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Bedingt) Wenn der Adobe Workfront-Administrator oder Workfront Proof-Administrator den Abschnitt Gründe hinzugefügt hat, wählen Sie die Gründe für Ihre Entscheidung aus. Weitere Informationen dazu, wie Administratoren Entscheidungsgründe konfigurieren können, finden Sie unter  [Konfigurieren Sie die Optionen für Genehmigungsentscheidungen in Workfront Proof](../../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md).
1. (Optional) Wählen Sie **E-Mail-Bestätigung senden** aus, um eine E-Mail-Bestätigung Ihrer Entscheidung zu erhalten.
1. Klicken Sie auf **Entscheidungsfindung vornehmen**.

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Make a decision when the proof is configured with an approval process</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can make decisions on a proof when it is configured with an approval process (within Workfront) and&nbsp;a user has sent you a document approval request, as described in <a href="../../../../review-and-approve-work/manage-approvals/request-document-approvals.md" class="MCXref xref">Request document approvals</a>.</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#make-a-workfront-approval-decision-in-a-proof" class="MCXref xref">Make a Workfront approval decision in a proof</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#change-your-workfront-approval-decision-in-a-proof" class="MCXref xref">Change your Workfront approval decision in a proof</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="make-a-workfront-approval-decision-in-a-proof">Make a Workfront approval decision in a proof</h3>
-->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Open the proof of the document that you want to make a decision on.</p>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the proofing viewer, select whether you want to <strong>Approve</strong>, require <strong>Changes</strong>, or <strong>Reject</strong> the approval request.</li>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="change-your-workfront-approval-decision-in-a-proof">Change your Workfront approval decision in a proof</h3>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Open the proof of the document where you want to change your Workfront approval decision.</li>
<li value="2"> <p>At the top-center of the proofing viewer, click the decision you made previously.</p> </li>
<li value="3">In the <strong>Proof decision</strong> box that appears, select whether you want to <strong>Approve</strong>, require <strong>Changes</strong>, or <strong>Reject</strong> the approval request.</li>
</ol>
-->
