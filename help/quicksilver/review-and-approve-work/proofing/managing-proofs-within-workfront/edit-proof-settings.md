---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: Testversandeinstellungen bearbeiten
description: Nach der Erstellung eines Testversands können Sie die Testversandeinstellungen jederzeit bearbeiten.
author: Courtney
feature: Digital Content and Documents
exl-id: ee30ce2c-e3dc-4863-a69b-cbc1b8747362
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 7%

---

# Testversandeinstellungen bearbeiten

Nach der Erstellung eines Testversands können Sie die Testversandeinstellungen jederzeit bearbeiten.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Veralteter Plan: Premium</p> <p>Weitere Informationen zum Testen des Zugriffs mit den verschiedenen Plänen finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Testfunktion in Workfront</a>.</p> </td> 
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
   <td role="rowheader">Rolle des Korrekturabzugs</td> 
   <td>Autor oder Moderator</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um zu erfahren, welchen Plan, welche Rolle oder welches Profil für die Testberechtigung Sie haben.

## Testversandeinstellungen bearbeiten

Einige Einstellungen können gesperrt werden, wenn sie vom Workfront-Administrator auf Kontoebene deaktiviert wurden.

1. Wechseln Sie zum Projekt, zur Aufgabe oder zur Ausgabe, an der Sie den Testversand durchführen möchten, und klicken Sie dann auf die Registerkarte **Dokumente** .
1. Bewegen Sie den Mauszeiger über den Testversand und klicken Sie dann auf **Dokumentdetails**.
1. Klicken Sie im linken Bereich auf **Testversand-Viewer-Einstellungen**.
1. Passen Sie die folgenden Einstellungen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Anmeldung verlangen. Dieser Korrekturabzug darf nicht mit Gastbenutzern geteilt werden.</td> 
      <td> <p>Wenn Sie für Ihren Überprüfungs- und Genehmigungsprozess höhere Sicherheitsstufen benötigen, können Sie die Anmeldung beim Testversand erforderlich machen. Dies bedeutet, dass nur Workfront-Benutzer zum Testversand hinzugefügt werden können. Sie müssen ihre E-Mail-Adresse und ihr Passwort eingeben, bevor sie darauf zugreifen können.</p> <p>Hinweis: <em style="font-style: normal;">Wenn die erforderliche Anmeldung aktiviert ist, können Abonnements nicht aktiviert werden.</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entscheidungen müssen elektronisch signiert werden</td> 
      <td> <p>Sie können von jedem Prüfer, der eine Entscheidung über den Testversand trifft, eine elektronische Signatur verlangen. Wenn ein Validierer eine Entscheidung trifft, wird er aufgefordert, seine E-Mail-Adresse und sein Passwort einzugeben und seine Entscheidung zu bestätigen. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information, see 
          <a href="../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md" class="MCXref xref">Understanding electronic signatures in Workfront Proof</a>
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sperren des Testversands, wenn alle erforderlichen Entscheidungen getroffen werden</td> 
      <td> <p>Sie können einen Testversandstatus festlegen, der gesperrt wird, wenn der endgültige Genehmiger seine Entscheidung trifft. Dies ist nützlich, wenn Sie sicherstellen möchten, dass Ihre Prüfer nicht zum Testversand zurückkehren und zusätzliche Kommentare hinzufügen oder ihre Entscheidungen ändern können.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Herunterladen der Originaldatei zulassen</td> 
      <td> <p>Sie können zulassen, dass die Prüfer eines Testversands die Originaldatei herunterladen, aus der ein Testversand erstellt wurde. Dies ist standardmäßig aktiviert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Freigabe des Korrekturabzugs über öffentliche URL oder eingebetteten Code erlauben</td> 
      <td>Sie können Benutzern erlauben, den Testversand mit einer öffentlichen URL oder einem Einbettungscode zu teilen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abonnement des Korrekturabzugs über öffentliche URL oder eingebetteten Code erlauben</td> 
      <td> <p>Durch die Aktivierung des Testversands können Personen, die nicht explizit zum Testversand hinzugefügt wurden, sich für den Testversand anmelden (d. h. sich zum Testversand hinzufügen). Anschließend wird ihnen die Rolle und der E-Mail-Warnhinweis zugewiesen, die Sie in den Abonnementeinstellungen für sie auswählen.</p> <p>Wenn die Option Anmeldung für einen Testversand aktiviert wurde, werden die folgenden Felder aktiv:</p> 
       <ul> 
        <li><strong>Validierung des Abonnenten erforderlich</strong> - Der Abonnent muss auf einen Link in einer E-Mail klicken, um auf einen Testversand zugreifen zu können.<br>Durch Auswahl dieser Option erhält der Abonnent keinen sofortigen Zugriff auf den Testversand, sondern einen Link zum Testversand in einer E-Mail. Die Abonnentenvalidierung soll sicherstellen, dass die Person eine korrekte E-Mail-Adresse eingegeben hat, auf die sie Zugriff hat.</li> 
        <li><strong>Standardrolle für neue Abonnenten -</strong> Dies ist die Standardrolle für den Testversand, die allen Validierern zugewiesen wird, die sich selbst für den Testversand angemeldet haben.</li> 
        <li><strong>Standard-E-Mail-Warnung für neue Abonnenten</strong> - Dies ist der Standard-E-Mail-Warnhinweis, der allen Validierern zugewiesen wird, die sich selbst für den Testversand angemeldet haben.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.

 
