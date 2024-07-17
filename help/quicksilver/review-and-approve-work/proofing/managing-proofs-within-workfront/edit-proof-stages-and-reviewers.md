---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: Testsendungen und Validierungsverantwortliche bearbeiten
description: Hier erfahren Sie, wie Sie Testsendungen und Validierungsverantwortliche bearbeiten.
author: Courtney
feature: Digital Content and Documents
exl-id: 91549c2d-d7b1-461c-a3c4-ad0032acfb23
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 1%

---

# Testsendungen und Validierungsverantwortliche bearbeiten

Sie können die Bühnen und die Reviewer-Details in einem Testversand bearbeiten, wenn Sie Testversand-Besitzer oder -Ersteller sind oder die korrekte Testversandrolle zugewiesen ist.

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
   <td>Autor oder Moderator </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um zu erfahren, welchen Plan, welche Rolle oder welches Profil für die Testberechtigung Sie haben.

## Eine Phase bearbeiten

1. Bewegen Sie in einer Dokumentliste, die das Dokument enthält, den Mauszeiger über die Zeile, die das Dokument enthält, und klicken Sie dann auf **Testversand-Workflow**.

   Oder

   Klicken Sie in der eigenständigen Workfront Proof auf das Menü **Mehr** (drei Punkte) rechts neben dem Testversand und klicken Sie dann auf **Testversanddetails anzeigen**.

1. Nehmen Sie eine der folgenden Änderungen im Abschnitt **Workflow** vor:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Deadline bearbeiten</td> 
      <td> <p>Wählen Sie das Datum aus und wählen Sie ein neues Datum im Kalender aus, der angezeigt wird. Um den Termin vollständig zu entfernen, wählen Sie das Datum aus und klicken Sie dann unter dem angezeigten Kalender auf <strong>Löschen</strong> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entfernen einzelner Validierer</td> 
      <td> <p>Wählen Sie das Menü <strong>Mehr</strong> rechts neben dem Namen des Validierers aus und klicken Sie dann im Dropdown-Menü auf <strong>Entfernen</strong> . Klicken Sie in dem angezeigten Feld auf <strong>Bestätigen</strong> , um den Überprüfer aus dem Testversand zu entfernen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mehrere Validierungsverantwortliche entfernen</td> 
      <td>Aktivieren Sie die Kontrollkästchen neben ihrem Namen und klicken Sie dann oben rechts im Abschnitt "Bühne"auf das Symbol <strong>Löschen</strong> .</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alle Validierungsverantwortlichen benachrichtigen</td> 
      <td>Wählen Sie das Menü <strong>Mehr</strong> in der oberen rechten Ecke des Bereichs "Bühne"aus und wählen Sie dann <strong>Nachricht alle </strong> aus. Konfigurieren Sie Ihre Nachricht und wählen Sie dann <strong>Senden</strong> aus.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hinzufügen eines Validierers zur Bühne</td> 
      <td>Wählen Sie das Menü <strong>Mehr</strong> in der oberen rechten Ecke des Bereichs "Bühne"und dann <strong>Freigabe</strong> aus. Fügen Sie den Benutzer hinzu, konfigurieren Sie seine Rolle und geben Sie Warnhinweise per E-Mail ein und wiederholen Sie diese bei Bedarf. Klicken Sie abschließend auf <strong>Freigabe</strong>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Löschen der Bühne</td> 
      <td> <p>Wählen Sie das Menü <strong>Mehr</strong> in der oberen rechten Ecke des Bereichs "Bühne"aus und wählen Sie die Phase <strong>Löschen</strong> aus.</p> <p>Hinweis: Wenn nur eine Phase vorhanden ist, kann die Phase nicht gelöscht werden.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Bearbeiten von Reviewer-Details

1. Bewegen Sie in Workfront den Mauszeiger über den Testversand und klicken Sie dann auf **Testversand-Details** , um die Seite mit den Testversanddetails zu öffnen.
1. Klicken Sie im Abschnitt **Workflow** auf das Menü **Mehr** ![](assets/more-button-small.png) rechts neben dem Namen des Validierers und klicken Sie dann im angezeigten Dropdown-Menü auf **Bearbeiten** .

1. Bearbeiten Sie im angezeigten Feld **Reviewer bearbeiten** eine der folgenden Details:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Anzeigename*</td> 
      <td> <p>Um den Anzeigenamen des Validierers im Testversand zu ändern, klicken Sie in das Textfeld und bearbeiten Sie den Namen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Funktion</td> 
      <td>Um die Rolle des Validierers beim Testversand zu ändern, öffnen Sie das Dropdown-Menü und wählen Sie die gewünschte Rolle aus. Weitere Informationen finden Sie unter .</td> 
     </tr> 
     <tr> 
      <td role="rowheader">E-Mail-Warnungen</td> 
      <td>Um den E-Mail-Warnhinweis des Prüfers für den Testversand zu ändern, öffnen Sie das Dropdown-Menü und wählen Sie den gewünschten E-Mail-Warnhinweis aus. Weitere Informationen finden Sie im Artikel <a href="../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md" class="MCXref xref">Benachrichtigungen für Testversand-Kommentare und Entscheidungen - Überblick</a>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Entscheidung*</td> 
      <td> <p>Um die Entscheidung des Validierers für den Testversand zu ändern, öffnen Sie das Dropdown-Menü und wählen Sie die gewünschte Entscheidung aus. Beachten Sie, dass alle Entscheidungen, die Sie für einen anderen Benutzer treffen, im Abschnitt Aktivität des Testversands aufgeführt werden. Diese Option wird nur angezeigt, wenn die Überprüfung eine Entscheidung getroffen hat.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Phase</td> 
      <td>Es ist nicht möglich, Prüfer zwischen Phasen zu verschieben. Sie können jedoch einen Überprüfer mit einem anderen Termin entfernen und erneut hinzufügen.</td> 
     </tr> 
    </tbody> 
   </table>

   &#42; Sie müssen der Ersteller oder Eigentümer des Testversands sein, um dieses Feld zu bearbeiten.

1. Klicken Sie auf **Speichern**.
