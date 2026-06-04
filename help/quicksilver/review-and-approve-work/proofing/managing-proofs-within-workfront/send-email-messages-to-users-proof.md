---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Senden von E-Mail-Nachrichten an prüfende Personen für einen Korrekturabzug
description: Während des Prüfungs- und Genehmigungsprozesses können Sie eine Nachricht an einen oder alle Prüfer eines Korrekturabzugs senden. Nachrichten sind eine einfache Möglichkeit, Prüfende daran zu erinnern, ihre Prüfung eines Korrekturabzugs abzuschließen oder andere Informationen im Zusammenhang mit dem Korrekturabzug bereitzustellen.
author: Courtney
feature: Digital Content and Documents
exl-id: e7d60d6f-b6bd-4082-b50c-e42d4b72c149
TQID: https://experienceleague.adobe.com/dVr9KslUMAN4leS62t2kTOLYnQhHaf21kJB4SVLKsX4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 354
ht-degree: 16%

---

# Senden von E-Mail-Nachrichten an prüfende Personen für einen Korrekturabzug

Während des Prüfungs- und Genehmigungsprozesses können Sie eine Nachricht an einen oder alle Prüfer eines Korrekturabzugs senden. Nachrichten sind eine einfache Möglichkeit, Prüfende daran zu erinnern, ihre Prüfung eines Korrekturabzugs abzuschließen oder andere Informationen im Zusammenhang mit dem Korrekturabzug bereitzustellen.

Sie können zwischen dem Versand einer allgemeinen Erinnerungs-E-Mail oder dem Versand einer benutzerdefinierten Nachricht an einen oder alle mit einem bestimmten Stadium verbundenen Benutzer wählen.

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
   <td>Autor oder Moderator</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriffrecht „Bearbeiten“ für Dokumente</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

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
