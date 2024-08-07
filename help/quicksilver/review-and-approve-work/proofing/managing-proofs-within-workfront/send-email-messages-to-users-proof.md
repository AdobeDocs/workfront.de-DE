---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Versand von E-Mail-Nachrichten an Prüfer anhand eines Testversands
description: Während des Prüfungs- und Validierungsprozesses können Sie einem oder allen Validierungsverantwortlichen eine Nachricht über einen Testversand senden. Nachrichten sind eine einfache Möglichkeit, Prüfer daran zu erinnern, ihre Überprüfung eines Testversands abzuschließen oder andere Informationen im Zusammenhang mit dem Testversand bereitzustellen.
author: Courtney
feature: Digital Content and Documents
exl-id: e7d60d6f-b6bd-4082-b50c-e42d4b72c149
source-git-commit: 7477b62cf0e2e61966f8e74cf268217e2ceb67ef
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 1%

---

# Versand von E-Mail-Nachrichten an Prüfer anhand eines Testversands

Während des Prüfungs- und Validierungsprozesses können Sie einem oder allen Validierungsverantwortlichen eine Nachricht über einen Testversand senden. Nachrichten sind eine einfache Möglichkeit, Prüfer daran zu erinnern, ihre Überprüfung eines Testversands abzuschließen oder andere Informationen im Zusammenhang mit dem Testversand bereitzustellen.

Sie können zwischen dem Versand einer generischen E-Mail zur Erinnerung oder dem Versand einer benutzerdefinierten Nachricht an einen oder alle mit einer bestimmten Phase verknüpften Benutzer wählen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

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
   <td>Autor oder Moderator</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um zu erfahren, welchen Plan, welche Rolle oder welches Profil für die Testberechtigung Sie haben.

+++

## E-Mail-Nachrichten an Benutzer auf einem Testversand senden

1. Suchen Sie das Dokument für den Testversand, das die Benutzer enthält, die Sie benachrichtigen möchten.
1. Bewegen Sie den Mauszeiger über das Dokument und klicken Sie dann auf **Testversand-Workflow**.

   ![](assets/proof-workflow-doc-list-350x92.png)

1. Um eine Nachricht an alle Benutzer auf der Bühne zu senden, klicken Sie auf das Menü **Mehr** auf der Bühne und wählen Sie **Nachricht an alle**.

   ![](assets/message-stage-350x122.png)

1. Um eine Nachricht an einen einzelnen Benutzer zu senden, klicken Sie auf das Menü **Mehr** neben dem Benutzer und wählen Sie **Nachricht**.

   ![](assets/message-user-350x121.png)

1. Geben Sie im Abschnitt **Nachrichtendetails** die folgenden Informationen an:

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
      <td> <p>Klicken Sie auf <strong>Benutzerdefinierte Nachricht verwerfen</strong> , wenn Sie nur den standardmäßigen E-Mail-Inhalt einbeziehen möchten.</p> <p>Die Standard-E-Mail zur Erinnerung enthält folgende Informationen:</p> 
       <ul> 
        <li>Persönlicher Link zum Testversand<br>Miniaturansicht des Testversandbilds<br></li> 
        <li>Die folgenden Details zum Testversand: Testversand, Versionsnummer, Ordnername (falls zutreffend) sowie eine Liste der validierungsverantwortlichen Benutzer und deren Fortschritt beim Testversand.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Betreff</td> 
      <td>Geben Sie einen Nachrichtenbetreff ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nachricht</td> 
      <td>Geben Sie Ihren Nachrichteninhalt ein.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Senden.**
