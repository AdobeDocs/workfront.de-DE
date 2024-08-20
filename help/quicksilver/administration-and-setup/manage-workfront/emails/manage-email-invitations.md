---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Verwalten von E-Mail-Einladungen für neue Benutzer
description: Als Adobe Workfront-Administrator können Sie Workfront mithilfe von E-Mail-Einladungen Benutzer hinzufügen und diese über das Hinzufügen benachrichtigen.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: e13e3479-391f-4aec-b998-e9b6057f256b
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 0%

---

# E-Mail-Einladungen für neue Benutzende verwalten

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in die Admin Console integriert wurden. Wenn Ihr Unternehmen in der Adobe Admin Console integriert wurde, müssen Sie diese Aktion über die Adobe Admin Console durchführen.
>
>Eine Liste der Verfahren, die sich je nachdem, ob Ihr Unternehmen in die Adobe Admin Console integriert wurde, unterscheiden, finden Sie unter [Plattformbasierte Verwaltungsunterschiede (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Als Adobe Workfront-Administrator können Sie Workfront mithilfe von E-Mail-Einladungen Benutzer hinzufügen und diese über das Hinzufügen benachrichtigen.

Die Einladung per E-Mail ermöglicht es neuen Benutzern, einem Link zu folgen, über den sie ein Kennwort für ihr Workfront-Konto auswählen können. Anschließend können sie die Einrichtung ihres Kontos abschließen.

Um die Sicherheit der neuen Konten zu gewährleisten, empfehlen wir Ihnen, E-Mail-Einladungen für Ihre neuen Benutzer zu verwenden, damit diese ihr eigenes Kennwort wählen können. Alternativ können Sie bei der Erstellung des Kontos auch ein Kennwort für einen neuen Benutzer auswählen. Weitere Informationen zum Hinzufügen neuer Benutzer zu Workfront finden Sie unter [Benutzer hinzufügen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Sie können die neuen Benutzer-E-Mails für Folgendes konfigurieren:

* Jeder neue Benutzer, der zu Workfront hinzugefügt wurde
* Benutzer, die Workfront mit einer Requestor-Lizenz hinzugefügt wurden

Alle neuen Benutzer sehen dieselbe E-Mail, wenn eine Einladung in eine E-Mail gesendet wird.

Informationen zum Empfangen von E-Mail-Einladungen finden Sie unter [Empfangen von E-Mail-Einladungen und Erstellen eines Kennworts für Adobe Workfront](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/receive-email-invitations.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Systemadministrator</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## E-Mail-Einladungen generieren {#generate-email-invitations}

E-Mail-Einladungen werden in den folgenden Szenarien generiert:

* Wenn Sie einen neuen Benutzer erstellen und im Formular **Neuer Benutzer** die Option **Einladungs-E-Mail an diese Person senden** auswählen. Weitere Informationen zum Erstellen neuer Benutzer finden Sie unter [Benutzer hinzufügen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Wenn Sie mehrere neue Benutzer importieren und die Option **Einladungs-E-Mails an diese Personen senden** auswählen. Weitere Informationen zum Importieren mehrerer neuer Benutzer finden Sie unter [Benutzer importieren](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).
* Nachdem die Benutzer erstellt wurden, können Sie die Einladungen manuell für Benutzer generieren, die ihr Konto noch nicht bei Workfront registriert haben und noch kein Workfront-Kennwort festgelegt haben.\
  Benutzer, die ein Konto erstellt, aber noch kein Konto registriert haben, werden in Workfront als **Abgemeldet** markiert.

  >[!NOTE]
  >
  >Wenn Sie bei der Erstellung des Benutzers das Feld **E-Mail-Einladung an diese Person senden** deaktivieren, kann die E-Mail-Einladung nicht manuell generiert werden. Das manuelle Zurücksetzen der E-Mail-Einladungen ist nur für Benutzer möglich, die zum Zeitpunkt der Kontoerstellung die ursprüngliche E-Mail-Einladung erhalten haben. Weitere Informationen zum Erstellen neuer Benutzer finden Sie unter [Benutzer hinzufügen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

So generieren Sie manuell E-Mail-Einladungen für bestehende nicht registrierte Benutzer:

{{step-1-to-users}}

1. Wählen Sie den Benutzer aus, der die Bezeichnung **Unregistered** nach seinem Namen anzeigt.

   ![](assets/unreg-user-qs-350x221.png)

1. Klicken Sie auf das Symbol &quot;Mehr&quot;![](assets/more-icon.png) und dann auf **Benutzer zur Registrierung erinnern**.

   Dem neuen Benutzer wird eine E-Mail-Einladung mit einem neuen Link gesendet, den er zum Erstellen seines Workfront-Kennworts verwenden kann.

   >[!NOTE]
   >
   >Wenn Ihr Unternehmen in die Admin Console integriert wurde und Sie einen Benutzer über Workfront hinzufügen, haben Sie keine Möglichkeit, eine Einladung per E-Mail an neue Benutzer zu senden.
   >
   >Neue Adobe-Benutzer werden der Admin Console hinzugefügt und die Admin Console stellt eine E-Mail bereit, um sie zum Abschluss des Registrierungsprozesses einzuladen. Alle Benutzer müssen den Registrierungsprozess abschließen, um auf ein beliebiges Adobe-System zugreifen zu können.
   >
   >Für bestehende Adobe-Benutzer kann der Benutzer eine E-Mail über die Verfügbarkeit von Workfront erhalten oder auch nicht. Dies ist eine vom Adobe-Administrator kontrollierte Voreinstellung für das Produkt.

## E-Mail-Einladungen konfigurieren {#configure-email-invitations}

Als Workfront-Administrator können Sie die Nachricht konfigurieren, die Sie in die E-Mail-Einladungen für neue Benutzer einfügen.

{{step-1-to-setup}}

1. Klicken Sie links in der Liste auf **E-Mail** > **Einladungen**.

1. Nehmen Sie im Abschnitt **Allgemeine Optionen** eine der folgenden Änderungen vor:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Deaktivieren von Einladungs-Links nach ... Tagen</strong> </td> 
      <td> <p>Wählen Sie die Zeitspanne aus, nach der die E-Mail-Einladungen keinen gültigen Link mehr zu Workfront enthalten. Der Standardzeitraum beträgt 45 Tage.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Eine Meldung und/oder eine Dienstdauer einschließen</strong> </td> 
      <td> <p>Wählen Sie diese Option aus, wenn Sie die Einladung für alle neuen Benutzer ändern möchten, die zu Workfront hinzugefügt wurden. Benutzer mit einer Requestor-Lizenz sind hiervon nicht betroffen.</p> 
       <ul> 
        <li><strong>Nachricht</strong>: Wenn Sie die Einladung in die E-Mail für alle neuen Benutzer ändern möchten, geben Sie den Text an, den Sie in Ihre E-Mail-Einladungen aufnehmen möchten.</li> 
        <li><strong>Nutzungsbedingungen</strong>: Wenn Sie die Einladung in die E-Mail für alle neuen Benutzer ändern möchten, geben Sie den Text an, den Sie in Ihre E-Mail-Einladungen aufnehmen möchten.<br></li> 
        <li><strong>Nachricht und/oder Dienstdauer für Helpdesk-Benutzer einschließen</strong>: Wählen Sie diese Option aus, wenn Sie die Einladung für alle neuen Benutzer ändern möchten, die zu Workfront hinzugefügt wurden und über eine Requestor-Lizenz verfügen.</li> 
        <li><strong>Nachricht</strong>: Wenn Sie die Einladung in die E-Mail für alle neuen Benutzer mit der Lizenz "Anforderer"ändern möchten, geben Sie den Text an, den Sie in Ihre E-Mail-Einladungen aufnehmen möchten.</li> 
        <li><strong>Nutzungsbedingungen</strong>: Wenn Sie die E-Mail-Einladung für alle neuen Benutzer mit der Lizenz "Antragsteller"ändern möchten, geben Sie den Text an, den Sie in Ihre E-Mail-Einladungen aufnehmen möchten.<br></li> 
        <li> <p>Im Abschnitt <strong>Einladungsvorschau</strong> können Sie eine Vorschau Ihrer E-Mail-Einladung anzeigen. Wenn Sie sich dafür entschieden haben, eine benutzerdefinierte Nachricht in Ihre E-Mail-Einladung aufzunehmen, wird die angepasste Nachricht in diesem Bereich angezeigt.</p> <p> <img src="assets/email-invitation-for-all-users-preview-qs-350x190.png" style="width: 350;height: 190;"> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.
