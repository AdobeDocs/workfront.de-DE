---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Konvertieren eines einfachen Workflows in einen automatisierten Workflow für einen Korrekturabzug
description: Wenn Sie der Inhaber des Korrekturabzugs sind, können Sie den grundlegenden Workflow eines vorhandenen Korrekturabzugs in einen automatisierten Workflow konvertieren.
author: Courtney
feature: Digital Content and Documents
exl-id: c676c696-ab7d-415b-bf5e-5d0335a3920f
source-git-commit: f252e3562b8ea73486d407138251b3d15d4b9f3a
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 1%

---

# Konvertieren eines einfachen Workflows in einen automatisierten Workflow für einen Korrekturabzug

Wenn Sie der Inhaber des Korrekturabzugs sind, können Sie den grundlegenden Workflow eines vorhandenen Korrekturabzugs in einen automatisierten Workflow konvertieren.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Legacy-Plan: Premium</p> <p>Weitere Informationen zum Proofing-Zugriff für die verschiedenen Pläne finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Proofing-Funktionalität in Workfront</a>.</p> </td> 
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
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um herauszufinden, über welchen Plan, welche Rolle oder welches Proof-Berechtigungsprofil Sie verfügen.

+++

## Konvertieren eines einfachen Workflows in einen automatisierten Workflow

1. Bewegen Sie in der Dokumentliste den Mauszeiger über das Dokument und klicken Sie dann auf **Proofing-Workflow** wenn es angezeigt wird.
1. Klicken Sie in der rechten oberen Ecke von Adobe Workfront auf **In automatisierten Workflow konvertieren**.
1. Klicken Sie **Neues Stadium** in der oberen rechten Ecke des Bildschirms.
1. Geben Sie Folgendes an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong> </td> 
      <td>Fügen Sie einen Namen für Ihr Stadium hinzu.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Frist</strong> </td> 
      <td>Wählen Sie ein Datum für die Frist aus.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p><strong>Phase aktivieren</strong> </p> </td> 
      <td>Wählen Sie aus, wann die Phase aktiviert werden soll.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fristoptionen</strong> </td> 
      <td>Auswählen, wie die Frist Trigger.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Schleusenbühne</strong> </td> 
      <td>Wählen Sie aus, ob die Phase gesperrt werden soll.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Primärer Entscheidungsträger</strong> </td> 
      <td>Geben Sie den primären Entscheidungsträger an.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Entscheidung</strong> </td> 
      <td>Wählen Sie aus, ob nur eine Entscheidung erforderlich ist. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Datenschutz</strong> </td> 
      <td>Wählen Sie aus, ob die Phase privat ist.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Benutzer hinzufügen</strong> </td> 
      <td>Geben Sie einen Kontaktnamen oder eine E-Mail-Adresse ein, wählen Sie die Rolle des Korrekturabzugs aus und konfigurieren Sie dann E-Mail-Warnungen.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie **Phase hinzufügen**.
1. (Optional) Wiederholen Sie die Schritte 3 und 4, bis Sie mit Ihrem Workflow zufrieden sind.
