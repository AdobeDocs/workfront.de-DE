---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Konfigurieren der Standardeinstellungen für persönliche Testsendungen
description: Sie können die Standardeinstellungen für den persönlichen Testversand definieren, die für von Ihnen erstellte Testsendungen gelten. Diese Standardeinstellungen werden jedes Mal angewendet, wenn Sie einen erstmaligen Testversand erstellen oder eine neue Testversand-Version in Workfront hochladen.
author: Courtney
feature: Digital Content and Documents
exl-id: 278bff89-0305-407b-9def-d06820d908de
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# Konfigurieren der Standardeinstellungen für persönliche Testsendungen

Sie können die Standardeinstellungen für den persönlichen Testversand definieren, die für von Ihnen erstellte Testsendungen gelten. Diese Standardeinstellungen werden jedes Mal angewendet, wenn Sie einen erstmaligen Testversand erstellen oder eine neue Testversand-Version in Workfront hochladen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Veralteter Plan: Auswählen oder höher</p> <p>Weitere Informationen zum Testzugang für die verschiedenen Pläne finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Testversandfunktion in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Aktueller Plan: Arbeit oder Plan</p> <p>Veralteter Plan: Beliebig (Sie müssen die Testversandfunktion für den Benutzer aktiviert haben)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront-Testversandadministrator, um zu erfahren, welchen Plan, welche Rolle oder welches Profil für die Testberechtigung Sie haben.

## Konfigurieren der Standardeinstellungen für persönliche Testsendungen

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Testversand**.

1. Klicken Sie oben rechts auf Ihren Avatar und wählen Sie **Persönliche Einstellungen**.
1. Wählen Sie die **Standardeinstellungen für die Prüfung** und geben Sie dann die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td colspan="2"><strong>Standard-E-Mail-Benachrichtigungseinstellungen</strong> </td> 
     </tr> 
     <tr> 
      <td>Standard-E-Mail-Warnhinweis</td> 
      <td>Wählen Sie aus, wie häufig der Benutzer E-Mail-Aktualisierungen erhält. Wählen Sie "Alle Aktivitäten", "Antworten auf meine Kommentare", "Entscheidungen", "Endgültige Entscheidung", "Stündliche Zusammenfassung", "Tägliche Zusammenfassung"oder "Deaktiviert".</td> 
     </tr> 
     <tr> 
      <td>Standard-E-Mail-Warnung für neue Gastreviewer</td> 
      <td>Wählen Sie aus, wie häufig Gastreviewer E-Mail-Aktualisierungen erhalten. Die Optionen entsprechen denen für Standard-E-Mail-Warnhinweis.</td> 
     </tr> 
     <tr> 
      <td>Neue Benachrichtigung zum Testversand</td> 
      <td>Wählen Sie den Erhalt einer Benachrichtigung aus, wenn Sie zum Testversand hinzugefügt werden.</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>Nachrichteneinstellungen</strong> </td> 
     </tr> 
     <tr> 
      <td>Vorlage für Testversand-Betreff</td> 
      <td>Geben Sie ein, was Benutzer sehen sollen, wenn Sie einen Testversand für sie freigeben.</td> 
     </tr> 
     <tr> 
      <td>Vorlage für Testnachrichten</td> 
      <td>Geben Sie ein, was Benutzer sehen sollen, wenn Sie einen Testversand für sie freigeben.</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>Standardmäßige Testversandeinstellungen</strong> </td> 
     </tr> 
     <tr> 
      <td>Sperren des Testversands bei allen Entscheidungen</td> 
      <td>Wählen Sie diese Option, um den Testversand automatisch vor weiteren Änderungen zu sperren, nachdem alle Entscheidungen getroffen wurden.</td> 
     </tr> 
     <tr> 
      <td>Nur eine Entscheidung erforderlich</td> 
      <td>Wählen Sie aus, nur eine Entscheidung für einen Testversand erforderlich zu machen.</td> 
     </tr> 
     <tr> 
      <td>Erforderliche Anmeldung</td> 
      <td> <p>Wählen Sie diese Option, um den Testversand nur Benutzern mit Workfront Testversand-Anmeldedaten zur Verfügung zu stellen.</p> <p>Hinweis: Die Workfront-Testversanddaten können sich von Ihren Workfront-Anmeldedaten unterscheiden, es sei denn, Ihre Unternehmensbenutzer SSO. Es wird empfohlen, diese Funktion nur zu verwenden, wenn Ihre Unternehmensbenutzer SSO verwenden.</p> </td> 
     </tr> 
     <tr> 
      <td>Abonnement aktiviert</td> 
      <td>Validierer, die nicht dem Unternehmen angehören, können sich über die öffentliche URL oder den Einbettungscode für den Testversand registrieren. Wenn diese Option aktiviert ist, muss der Abonnent auf einen Link in einer E-Mail klicken, um auf einen Testversand zugreifen zu können. Wählen Sie diese Option aus, damit der externe Validierer auf einen Link in der E-Mail klicken muss, um auf den Testversand zugreifen zu können. Diese Option ist standardmäßig aktiviert, wenn die Option Öffentliche Freigabe ausgewählt ist und auf alle von diesem Benutzer erstellten Testsendungen angewendet wird. </td> 
     </tr> 
     <tr> 
      <td>Standardrolle für neue Gastreviewer</td> 
      <td>Wählen Sie eine standardmäßige Testversand-Rolle für Gastreviewer aus. Die Optionen sind mit denen in der Rolle Standardversand identisch.</td> 
     </tr> 
     <tr> 
      <td>Blockdownload der Originaldatei</td> 
      <td>Wählen Sie diese Option, um Benutzer vom Herunterladen der Originaldatei abzuhalten. </td> 
     </tr> 
     <tr> 
      <td>Meine standardmäßige Testprofil-Rolle</td> 
      <td>Wählen Sie Ihre standardmäßige Testversand-Rolle aus. </td> 
     </tr> 
     <tr> 
      <td>Meine standardmäßige Markup-Farbe</td> 
      <td>Wählen Sie Ihre standardmäßige Markup-Farbe aus. </td> 
     </tr> 
    </tbody> 
   </table>
