---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Senden von E-Mail-Nachrichten an Prüfer im Rahmen eines Testversands
description: Während des Prüfungs- und Genehmigungsprozesses können Sie eine Nachricht an einen oder alle Prüfer eines Korrekturabzugs senden. Nachrichten sind eine einfache Möglichkeit, Prüfende daran zu erinnern, ihre Prüfung eines Korrekturabzugs abzuschließen oder andere Informationen im Zusammenhang mit dem Korrekturabzug bereitzustellen.
author: Courtney
feature: Digital Content and Documents
exl-id: e7d60d6f-b6bd-4082-b50c-e42d4b72c149
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 1%

---

# Senden von E-Mail-Nachrichten an Prüfer im Rahmen eines Testversands

Während des Prüfungs- und Genehmigungsprozesses können Sie eine Nachricht an einen oder alle Prüfer eines Korrekturabzugs senden. Nachrichten sind eine einfache Möglichkeit, Prüfende daran zu erinnern, ihre Prüfung eines Korrekturabzugs abzuschließen oder andere Informationen im Zusammenhang mit dem Korrekturabzug bereitzustellen.

Sie können zwischen dem Versand einer allgemeinen Erinnerungs-E-Mail oder dem Versand einer benutzerdefinierten Nachricht an einen oder alle mit einem bestimmten Stadium verbundenen Benutzer wählen.

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
   <td>Autor oder Moderator</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um herauszufinden, über welchen Plan, welche Rolle oder welches Proof-Berechtigungsprofil Sie verfügen.

+++

## Senden von E-Mail-Nachrichten an Benutzer im Rahmen eines Testversands

1. Suchen Sie das Dokument für den Korrekturabzug, der die Benutzer enthält, die Sie benachrichtigen möchten.
1. Bewegen Sie den Mauszeiger über das Dokument und klicken Sie dann auf **Proofing-Workflow**.

   ![Proofing-Workflow](assets/proof-workflow-doc-list-350x92.png)

1. Um eine Nachricht an alle Benutzer auf der Bühne zu senden, klicken Sie auf das **Mehr**-Menü auf der Bühne und wählen Sie **Nachricht an alle**.

   ![Nachricht auf der Bühne](assets/message-stage-350x122.png)

1. Um eine Nachricht an einen einzelnen Benutzer zu senden, klicken Sie auf das Menü **Mehr** neben dem Benutzer und wählen Sie **Nachricht** aus.

   ![Nachrichtenbenutzer](assets/message-user-350x121.png)

1. Geben **im Abschnitt &quot;**&quot; die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Personen per E-Mail benachrichtigen</td> 
      <td>Diese Option kann nicht deaktiviert werden. Alle Benutzer erhalten die Nachricht per E-Mail.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzerdefinierte Nachricht verwerfen</td> 
      <td> <p>Klicken Sie <strong>Benutzerdefinierte Nachricht verwerfen</strong>, wenn Sie nur den standardmäßigen E-Mail-Inhalt einbeziehen möchten.</p> <p>Die standardmäßige Erinnerungs-E-Mail enthält die folgenden Informationen:</p> 
       <ul> 
        <li>Persönlicher Link zum Korrekturabzug/<br> des Korrekturabzugsbildes<br></li> 
        <li>Die folgenden Details des Korrekturabzugs: Name des Korrekturabzugs, Versionsnummer, Ordnername (falls zutreffend) und Liste der Prüfer und deren Fortschritt beim Korrekturabzug.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Betreff</td> 
      <td>Geben Sie einen Nachrichtenbetreff ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nachricht</td> 
      <td>Geben Sie den Nachrichteninhalt ein.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Senden.**
