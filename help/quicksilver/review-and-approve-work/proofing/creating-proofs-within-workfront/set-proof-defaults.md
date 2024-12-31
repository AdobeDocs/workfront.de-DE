---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Konfigurieren von persönlichen Proofing-Standards
description: Sie können Standardeinstellungen für persönliche Korrekturabzüge definieren, die für von Ihnen erstellte Korrekturabzüge gelten. Diese Standardwerte werden jedes Mal angewendet, wenn Sie einen ersten Korrekturabzug generieren oder eine neue Korrekturabzugsversion in Workfront hochladen.
author: Courtney
feature: Digital Content and Documents
exl-id: 278bff89-0305-407b-9def-d06820d908de
source-git-commit: ac908d52d1538b1ffe7d9bfca94cb9921445633d
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---

# Konfigurieren von persönlichen Proofing-Standards

Sie können Standardeinstellungen für persönliche Korrekturabzüge definieren, die für von Ihnen erstellte Korrekturabzüge gelten. Diese Standardwerte werden jedes Mal angewendet, wenn Sie einen ersten Korrekturabzug generieren oder eine neue Korrekturabzugsversion in Workfront hochladen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Legacy-Plan: Auswählen oder höher</p> <p>Weitere Informationen zum Proofing-Zugriff für die verschiedenen Pläne finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Proofing-Funktionalität in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Aktueller Plan: Arbeits- oder Plan</p> <p>Legacy-Plan: Beliebig (Proofing muss für den Benutzer aktiviert sein)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um herauszufinden, über welchen Plan, welche Rolle oder welches Proof-Berechtigungsprofil Sie verfügen.

+++

## Konfigurieren von persönlichen Proofing-Standards

{{step1-to-proofing}}

1. Klicken Sie in der oberen rechten Ecke auf Ihren Avatar und wählen Sie **Persönliche Einstellungen**.
1. Wählen Sie die **Proofing-Standardeinstellungen** und geben Sie dann die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td colspan="2"><strong>Standardeinstellungen für E-Mail-Benachrichtigungen</strong> </td> 
     </tr> 
     <tr> 
      <td>E-Mail-Standardwarnung</td> 
      <td>Wählen Sie aus, wie oft Benutzer E-Mail-Updates erhalten sollen. Alle Aktivitäten auswählen, Antworten auf meine Kommentare, Entscheidungen, Endgültige Entscheidung, Stündliche Zusammenfassung, Tägliche Zusammenfassung oder Deaktiviert.</td> 
     </tr> 
     <tr> 
      <td>Standard-E-Mail-Warnhinweis für neue Gastvalidierer</td> 
      <td>Wählen Sie aus, wie oft Gastreviewer E-Mail-Updates erhalten sollen. Die Optionen sind die gleichen wie für den Standard-E-Mail-Warnhinweis.</td> 
     </tr> 
     <tr> 
      <td>Neue Korrekturabzugsbenachrichtigung</td> 
      <td>Wählen Sie aus, dass Sie eine Benachrichtigung erhalten möchten, wenn Sie zu einem Korrekturabzug hinzugefügt werden.</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>Nachrichteneinstellungen</strong> </td> 
     </tr> 
     <tr> 
      <td>Vorlage für Testversand-Betreff</td> 
      <td>Geben Sie ein, was Benutzende in den Betreff einer E-Mail sehen sollen, wenn Sie ihnen einen Korrekturabzug zeigen.</td> 
     </tr> 
     <tr> 
      <td>Vorlage für Testversandnachrichten</td> 
      <td>Geben Sie ein, was Benutzende im Textkörper einer E-Mail sehen sollen, wenn Sie einen Korrekturabzug für sie freigeben.</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>Standardeinstellungen für Korrekturabzüge</strong> </td> 
     </tr> 
     <tr> 
      <td>Korrekturabzug bei allen Entscheidungen sperren</td> 
      <td>Wählen Sie aus, dass der Korrekturabzug nach allen Entscheidungen automatisch gegen weitere Änderungen gesperrt werden soll.</td> 
     </tr> 
     <tr> 
      <td>Nur eine Entscheidung erforderlich</td> 
      <td>Entscheiden Sie sich dafür, dass für einen Korrekturabzug nur eine Entscheidung erforderlich ist.</td> 
     </tr> 
     <tr> 
      <td>Login erforderlich</td> 
      <td> <p>Wählen Sie aus, dass der Korrekturabzug nur für Benutzer mit Workfront Proof-Anmeldedaten verfügbar sein soll.</p> <p>Hinweis: Workfront Proof-Anmeldeinformationen können sich von Ihren Workfront-Anmeldeinformationen unterscheiden, es sei denn, das SSO wird von Ihren Unternehmensbenutzern verwendet. Es wird empfohlen, diese Funktion nur zu verwenden, wenn Ihr Unternehmen SSO nutzt.</p> </td> 
     </tr> 
     <tr> 
      <td>Subscription enabled</td> 
      <td>Zulassen, dass sich Prüfer außerhalb des Unternehmens über die öffentliche URL oder den Einbettungs-Code für den Korrekturabzug anmelden. Wenn diese Option ausgewählt ist, muss der Abonnent auf einen Link in einer E-Mail klicken, um auf einen Korrekturabzug zuzugreifen, der ebenfalls verfügbar ist. Wählen Sie diese Option aus, damit der externe Prüfer auf einen Link in der E-Mail klicken muss, um auf den Korrekturabzug zuzugreifen. Diese Option ist standardmäßig aktiviert, wenn die Option Öffentliche Freigabe ausgewählt ist, und wird auf alle von diesem Benutzer erstellten Korrekturabzüge angewendet. </td> 
     </tr> 
     <tr> 
      <td>Standardrolle für neue Gast-Reviewer</td> 
      <td>Wählen Sie eine Standardrolle für den Testversand für Gastvalidierer aus. Die Optionen sind die gleichen wie in der Standard-Korrekturabzugsrolle.</td> 
     </tr> 
     <tr> 
      <td>Download der Originaldatei blockieren</td> 
      <td>Benutzer können die Originaldatei nicht herunterladen. </td> 
     </tr> 
     <tr> 
      <td>Meine Standard-Korrekturabzugsrolle</td> 
      <td>Wählen Sie Ihre Standard-Korrekturabzugsrolle aus. </td> 
     </tr> 
     <tr> 
      <td>Meine standardmäßige Markupfarbe</td> 
      <td>Wählen Sie Ihre standardmäßige Markupfarbe aus. </td> 
     </tr> 
    </tbody> 
   </table>
