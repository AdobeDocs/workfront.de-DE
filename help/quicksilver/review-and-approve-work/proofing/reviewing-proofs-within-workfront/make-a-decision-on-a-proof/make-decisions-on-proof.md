---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Treffen einer Entscheidung zu einem Korrekturabzug im Proofing Viewer
description: Sie können eine Entscheidung zu einem Korrekturabzug direkt in der Proofing-Anzeige treffen.
author: Courtney
feature: Digital Content and Documents
exl-id: cf74ac54-b8c1-4404-b35f-2aa94831ecad
TQID: https://experienceleague.adobe.com/Qnt76jLepqi5CO0Ws7mi-jiyilJdIs2bGEjINaf1img
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 326
ht-degree: 23%

---

# Treffen einer Entscheidung zu einem Korrekturabzug im Proofing Viewer

Sie können eine Entscheidung zu einem Korrekturabzug direkt in der Proofing-Anzeige treffen.

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
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Korrekturabzug-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Rolle des Korrekturabzugs</td> 
   <td>Genehmigende Person, Prüfende Person und genehmigende Person, Autor, Moderator</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriffrecht „Bearbeiten“ für Dokumente</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Treffen einer Entscheidung zu einem Korrekturabzug im Proofing Viewer

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

1. (Bedingt) Wenn der Adobe Workfront- oder Workfront Proof-Administrator einen Abschnitt „Gründe“ hinzugefügt hat, wählen Sie einen der Gründe für Ihre Entscheidung aus. Weitere Informationen dazu, wie Admins Entscheidungsgründe konfigurieren können, finden Sie unter [Konfigurieren von Genehmigungsentscheidungsoptionen in Workfront Proof](../../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md).
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
