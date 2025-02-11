---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: E-Mail-Einladungen für neue Benutzer verwalten
description: Als Adobe Workfront-Administrator können Sie Benutzer mithilfe von E-Mail-Einladungen zu Workfront hinzufügen und sie darüber benachrichtigen, dass sie hinzugefügt wurden.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: e13e3479-391f-4aec-b998-e9b6057f256b
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '932'
ht-degree: 0%

---

# E-Mail-Einladungen für neue Benutzende verwalten

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in die Admin Console integriert wurden. Wenn Ihre Organisation in die Adobe Admin Console integriert wurde, müssen Sie diese Aktion über die Adobe Admin Console durchführen.
>
>Eine Liste der Verfahren, die sich je nachdem unterscheiden, ob Ihr Unternehmen Adobe Admin Console verwendet hat, finden Sie unter [Plattformbasierte Administrationsunterschiede (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Als Adobe Workfront-Administrator können Sie Benutzer mithilfe von E-Mail-Einladungen zu Workfront hinzufügen und sie darüber benachrichtigen, dass sie hinzugefügt wurden.

Die E-Mail-Einladung ermöglicht es neuen Benutzenden, einem Link zu folgen, über den sie ein Passwort für ihr Workfront-Konto auswählen können. Sie können dann ihr Konto einrichten.

Um die Sicherheit der neuen Konten zu gewährleisten, empfehlen wir, E-Mail-Einladungen für neue Benutzer zu verwenden, damit diese ihr eigenes Passwort auswählen können. Alternativ können Sie auch ein Kennwort für einen neuen Benutzer auswählen, wenn Sie dessen Konto erstellen. Weitere Informationen zum Hinzufügen neuer Benutzer zu Workfront finden Sie unter [Hinzufügen von Benutzern](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Sie können die neuen Benutzer-E-Mails konfigurieren für:

* Jeder neue Benutzer, der zu Workfront hinzugefügt wird
* Benutzende, die mit einer Antragstellerlizenz zu Workfront hinzugefügt wurden

Alle neuen Benutzer sehen dieselbe E-Mail, wenn eine E-Mail-Einladung gesendet wird.

Weitere Informationen zum Empfang von E-Mail-Einladungen finden Sie unter [E-Mail-Einladungen empfangen und Kennwort für Adobe Workfront erstellen](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/receive-email-invitations.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Systemadministrator</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## E-Mail-Einladungen generieren {#generate-email-invitations}

E-Mail-Einladungen werden in den folgenden Szenarien generiert:

* Wenn Sie einen neuen Benutzer erstellen und im Formular **Neuer Benutzer** **die Option „Einladungs-E-Mail an diese Person senden** auswählen. Weitere Informationen zum Erstellen neuer Benutzer finden Sie unter [Benutzer hinzufügen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Wenn Sie mehrere neue Benutzer importieren und die Option **Einladungs-E-Mails an diese Personen senden** auswählen. Weitere Informationen zum Importieren mehrerer neuer Benutzer finden Sie unter [Benutzer importieren](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).
* Nachdem die Benutzer erstellt wurden, können Sie die Einladungen für Benutzer manuell generieren, die ihr -Konto noch nicht bei Workfront registriert haben und kein Workfront-Kennwort eingerichtet haben.\
  Benutzer, die ein Konto erstellt haben, ihr Konto jedoch noch nicht registriert haben, werden in Workfront als **Nicht**) gekennzeichnet.

  >[!NOTE]
  >
  >Wenn Sie das Kontrollkästchen **E-Mail-Einladung an diese Person senden** beim Erstellen des Benutzers deaktivieren, kann die E-Mail-Einladung nicht manuell generiert werden. Das manuelle erneute Senden der E-Mail-Einladungen ist nur für Benutzer möglich, denen bei der Erstellung ihres Kontos die ursprüngliche E-Mail-Einladung gesendet wurde. Weitere Informationen zum Erstellen neuer Benutzer finden Sie unter [Benutzer hinzufügen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

So generieren Sie manuell E-Mail-Einladungen an nicht registrierte Benutzer:

{{step-1-to-users}}

1. Wählen Sie den Benutzer aus, der nach seinem Namen die **Nicht registriert**-Kennzeichnung anzeigt.

   ![Nicht registriert](assets/unreg-user-qs-350x221.png)

1. Klicken Sie auf das Symbol Mehr ![Mehr](assets/more-icon.png) und dann auf **Benutzer an die Registrierung erinnern**.

   Der neue Benutzer erhält eine E-Mail-Einladung mit einem neuen Link, den er zum Erstellen seines Workfront-Kennworts verwenden kann.

   >[!NOTE]
   >
   >Wenn Ihr Unternehmen in die Admin Console integriert wurde und Sie einen Benutzer über Workfront hinzufügen, haben Sie keine Möglichkeit, neue Benutzer per E-Mail einzuladen.
   >
   >Neue Adobe-Benutzer werden der Admin Console hinzugefügt und die Admin Console sendet eine E-Mail, um sie zum Abschluss des Registrierungsprozesses einzuladen. Alle Anwender müssen den Registrierungsprozess abschließen, um auf ein Adobe-System zugreifen zu können.
   >
   >Bestehende Adobe-Benutzer erhalten möglicherweise eine E-Mail, in der sie darauf hingewiesen werden, dass Workfront verfügbar ist. Dies ist eine Voreinstellung, die vom Adobe-Administrator für das Produkt gesteuert wird.

## Konfigurieren von E-Mail-Einladungen {#configure-email-invitations}

Als Workfront-Admin können Sie die Nachricht konfigurieren, die Sie in die E-Mail-Einladungen für neue Benutzende aufnehmen.

{{step-1-to-setup}}

1. Klicken Sie in der Liste auf der linken Seite auf **E** > **Einladungen**.

1. Nehmen **im Abschnitt** Allgemeine Optionen“ eine der folgenden Änderungen vor:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Deaktivieren von Einladungslinks nach … Tagen</strong> </td> 
      <td> <p>Wählen Sie den Zeitraum aus, nach dem die E-Mail-Einladungen keinen gültigen Link mehr zu Workfront enthalten. Der Standardwert für Tage ist 45.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Nachricht und/oder Dienstzeit beifügen</strong> </td> 
      <td> <p>Wählen Sie diese Option aus, wenn Sie die E-Mail-Einladung für alle neuen Benutzer ändern möchten, die zu Workfront hinzugefügt wurden. Dies gilt nicht für Benutzer mit einer Antragstellerlizenz.</p> 
       <ul> 
        <li><strong>Nachricht</strong>: Wenn Sie die E-Mail-Einladung für alle neuen Benutzer ändern möchten, geben Sie den Text an, den Sie in Ihre E-Mail-Einladungen als E-Mail-Textkörper aufnehmen möchten.</li> 
        <li><strong>Geschäftsbedingungen</strong>: Wenn Sie die E-Mail-Einladung für alle neuen Benutzer ändern möchten, geben Sie den Text an, den Sie in Ihre E-Mail-Einladungen als Geschäftsbedingungen aufnehmen möchten.<br></li> 
        <li><strong>Nachricht und/oder Dienstzeit für Helpdesk-Benutzer einschließen</strong>: Wählen Sie diese Option, wenn Sie die E-Mail-Einladung für alle neu zu Workfront hinzugefügten Benutzer ändern möchten, die über eine Antragstellerlizenz verfügen.</li> 
        <li><strong>Nachricht</strong>: Wenn Sie die E-Mail-Einladung für alle neuen Benutzer mit einer Antragstellerlizenz ändern möchten, geben Sie den Text an, den Sie in Ihre E-Mail-Einladungen als Textkörper aufnehmen möchten.</li> 
        <li><strong>Geschäftsbedingungen</strong>: Wenn Sie die E-Mail-Einladung für alle neuen Benutzer mit einer Antragstellerlizenz ändern möchten, geben Sie den Text an, den Sie in Ihre E-Mail-Einladungen als Geschäftsbedingungen aufnehmen möchten.<br></li> 
        <li> <p>Im Abschnitt <strong>Einladungsvorschau</strong> können Sie eine Vorschau Ihrer E-Mail-Einladung anzeigen. Wenn Sie ausgewählt haben, dass eine benutzerdefinierte Nachricht in Ihre E-Mail-Einladung aufgenommen werden soll, wird die angepasste Nachricht in diesem Bereich angezeigt.</p> <p> <img src="assets/email-invitation-for-all-users-preview-qs-350x190.png" style="width: 350;height: 190;"> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.
