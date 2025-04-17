---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: Testversandeinstellungen bearbeiten
description: Sie können die Einstellungen für den Korrekturabzug jederzeit bearbeiten, nachdem Sie einen Korrekturabzug erstellt haben.
author: Courtney
feature: Digital Content and Documents
exl-id: ee30ce2c-e3dc-4863-a69b-cbc1b8747362
source-git-commit: a036a99c13d80a2ba2305ebcdc799ad6e5b62b39
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 7%

---

# Testversandeinstellungen bearbeiten

Sie können die Einstellungen für den Korrekturabzug jederzeit bearbeiten, nachdem Sie einen Korrekturabzug erstellt haben.

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

## Testversandeinstellungen bearbeiten

Einige Einstellungen können gesperrt werden, wenn sie von Ihrem Workfront-Administrator auf Kontoebene deaktiviert wurden.

1. Wechseln Sie zum Projekt, zur Aufgabe oder zum Problem, in dem bzw. dem Sie den Korrekturabzug anzeigen möchten, und klicken Sie dann auf die Registerkarte **Dokumente**.
1. Bewegen Sie den Mauszeiger über den Korrekturabzug und klicken Sie dann auf **Dokumentdetails**.
1. Klicken Sie im linken Bedienfeld auf **Proofing Viewer-Einstellungen**.
1. Stellen Sie die folgenden Einstellungen ein:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Anmeldung verlangen. Dieser Korrekturabzug darf nicht mit Gastbenutzern geteilt werden.</td> 
      <td> <p>Wenn Sie höhere Sicherheitsstufen für Ihren Prüfungs- und Genehmigungsprozess benötigen, können Sie die Option Anmeldung beim Korrekturabzug erforderlich verwenden. Das bedeutet, dass nur Workfront-Benutzende zum Korrekturabzug hinzugefügt werden können. Sie müssen ihre E-Mail-Adresse und ihr Passwort eingeben, bevor sie darauf zugreifen können.</p> <p>Hinweis: <em style="font-style: normal;">Wenn „Anmeldung erforderlich“ aktiviert ist, können Abonnements nicht aktiviert werden.</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entscheidungen müssen elektronisch signiert werden</td> 
      <td> <p>Sie können eine elektronische Signatur von jedem Prüfer verlangen, der eine Entscheidung über den Korrekturabzug trifft. Wenn eine Überprüfende eine Entscheidung trifft, werden sie in einer Eingabeaufforderung aufgefordert, ihre E-Mail-Adresse und ihr Passwort einzugeben und ihre Entscheidung zu bestätigen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Korrekturabzug sperren, wenn alle erforderlichen Entscheidungen getroffen werden</td> 
      <td> <p>Sie können einen Korrekturabzugsstatus festlegen, der gesperrt wird, wenn die endgültige genehmigende Person ihre Entscheidung trifft. Dies ist nützlich, wenn Sie sicherstellen möchten, dass Ihre Prüfer nicht zum Korrekturabzug zurückkehren und zusätzliche Kommentare hinzufügen oder ihre Entscheidungen ändern können.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Herunterladen der Originaldatei zulassen</td> 
      <td> <p>Sie können Prüferinnen und Prüfern eines Korrekturabzugs erlauben, die Originaldatei herunterzuladen, aus der ein Korrekturabzug erstellt wurde. Dies ist standardmäßig aktiviert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Freigabe des Korrekturabzugs über öffentliche URL oder eingebetteten Code erlauben</td> 
      <td>Sie können Benutzern erlauben, den Korrekturabzug über eine öffentliche URL oder einen Einbettungs-Code freizugeben. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abonnement des Korrekturabzugs über öffentliche URL oder eingebetteten Code erlauben</td> 
      <td> <p>Durch die Aktivierung des Abonnements für den Korrekturabzug können Personen, die nicht explizit zum Korrekturabzug hinzugefügt wurden, den Korrekturabzug selbst abonnieren (sich also zum Korrekturabzug hinzufügen). Ihnen werden dann die Rolle und der E-Mail-Warnhinweis zugewiesen, die Sie in den Abonnementeinstellungen für sie auswählen.</p> <p>Wenn das Abonnement für einen Korrekturabzug aktiviert wurde, werden die folgenden Felder aktiv:</p> 
       <ul> 
        <li><strong>Abonnentenvalidierung erforderlich</strong> - Abonnentinnen und Abonnenten müssen auf einen Link in einer E-Mail klicken, um auf einen Korrekturabzug zuzugreifen. <br> Sie diese Option auswählen, erhält die abonnierende Person keinen sofortigen Zugriff auf den Korrekturabzug, erhält jedoch einen Link zum Korrekturabzug in einer E-Mail. Mit der Abonnentenvalidierung soll sichergestellt werden, dass die Person eine korrekte E-Mail-Adresse eingegeben hat, zu der sie Zugriff hat.</li> 
        <li><strong>Standardrolle für neue Abonnenten -</strong> Dies ist die Standardrolle für den Korrekturabzug, die allen Prüfern zugewiesen wird, die den Korrekturabzug selbst abonnieren.</li> 
        <li><strong>Standard-E-Mail-Warnhinweis für neue Abonnenten</strong> - Dies ist der standardmäßige E-Mail-Warnhinweis, der allen Reviewern zugewiesen wird, die den Testversand selbst abonnieren.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.

 
