---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Entscheidung über einen Korrekturabzug in der Korrekturabzugsansicht treffen
description: Sie können eine Entscheidung zu einem Korrekturabzug direkt in der Proofing-Anzeige treffen.
author: Courtney
feature: Digital Content and Documents
exl-id: cf74ac54-b8c1-4404-b35f-2aa94831ecad
source-git-commit: 8af531868249f609113af6d2a8465af01edcbc3f
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 2%

---

# Entscheidung über einen Korrekturabzug in der Korrekturabzugsansicht treffen

Sie können eine Entscheidung zu einem Korrekturabzug direkt in der Proofing-Anzeige treffen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Legacy-Plan: Auswählen oder Premium</p> <p>Weitere Informationen zum Proofing-Zugriff für die verschiedenen Pläne finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Proofing-Funktionalität in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Aktueller Plan: Arbeits- oder Plan</p> <p>Legacy-Plan: Beliebig (Proofing muss für den Benutzer aktiviert sein)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Rolle des Korrekturabzugs</td> 
   <td>Genehmigende Person, Prüfende Person und genehmigende Person, Autor, Moderator</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um herauszufinden, über welchen Plan, welche Rolle oder welches Proof-Berechtigungsprofil Sie verfügen.

+++

## Entscheidung über einen Korrekturabzug in der Korrekturabzugsansicht treffen

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente**.
1. Suchen Sie den benötigten Korrekturabzug und klicken Sie dann auf **Korrekturabzug öffnen**.

1. Klicken **oben** der Proofing-Anzeige auf „Entscheidung treffen“.

1. Klicken **im angezeigten** „Korrekturabzugsentscheidung“ auf eine der folgenden Entscheidungen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Genehmigt</td> 
      <td>Der Korrekturabzug ist bereit, mit dem nächsten Schritt des automatisierten Workflows fortzufahren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mit Änderungen genehmigt</td> 
      <td>Der Korrekturabzug erfordert einige Änderungen, aber Sie müssen die Revision nicht sehen, bevor er zur nächsten Phase des automatisierten Workflows übergeht.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erforderliche Änderungen</td> 
      <td>Der Korrekturabzug erfordert Änderungen, und Sie müssen eine weitere Revision sehen, bevor er zur nächsten Phase des automatisierten Workflows übergeht.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nicht relevant</td> 
      <td>Der Korrekturabzug ist für Sie nicht relevant und Sie müssen keine Entscheidung treffen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzerdefinierte Entscheidung</td> 
      <td> <p>Bei Select- und Premium-Plänen kann der Workfront- oder Workfront Proof-Administrator Entscheidungen umbenennen, neu anordnen und ausblenden. Weitere Informationen finden Sie unter <a href="../../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md" class="MCXref xref">Konfigurieren von Genehmigungsentscheidungsoptionen in Workfront Proof</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Bedingt) Wenn der Adobe Workfront- oder Workfront Proof-Administrator einen Abschnitt „Gründe“ hinzugefügt hat, wählen Sie einen der Gründe für Ihre Entscheidung aus. Weitere Informationen dazu, wie Administratoren Entscheidungsgründe konfigurieren können, finden Sie unter  [Konfigurieren von Genehmigungsentscheidungsoptionen in Workfront Proof](../../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md).
1. (Optional) Wählen Sie **E-Mail-Bestätigung senden**, um eine E-Mail-Bestätigung Ihrer Entscheidung zu erhalten.
1. Klicken Sie **Entscheidung treffen**.

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
