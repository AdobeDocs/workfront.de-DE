---
user-type: administrator
product-area: system-administration;user-management
keywords: view,group,event,notifications,configure,enable,disable
navigation-topic: create-and-manage-groups
title: Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe
description: Als Gruppenadministrator können Sie die Ereignisbenachrichtigungen anzeigen, die für eine von Ihnen verwaltete Gruppe aktiviert sind. Wenn ein Adobe Workfront-Administrator eine Ereignisbenachrichtigung entsperrt, können Sie sie auch für eine von Ihnen verwaltete Gruppe der obersten Ebene konfigurieren. Die Konfiguration einer Ereignisbenachrichtigung besteht darin, sie zu aktivieren oder zu deaktivieren.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a815aeb1-3403-4491-a8ad-7e47c519905c
source-git-commit: 306d6493ff0413d5814f4aed8ab44fb897f3568d
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe

Als Gruppenadministrator können Sie die Ereignisbenachrichtigungen anzeigen, die für eine von Ihnen verwaltete Gruppe aktiviert sind.

Wenn ein Adobe Workfront-Administrator eine Ereignisbenachrichtigung entsperrt, können Sie sie auch für eine von Ihnen verwaltete Gruppe der obersten Ebene konfigurieren. Die Konfiguration einer Ereignisbenachrichtigung besteht darin, sie zu aktivieren oder zu deaktivieren.

Ein Workfront-Administrator kann dies auch für jede Gruppe tun.

Die Konfiguration einer Ereignisbenachrichtigung für eine Gruppe wirkt sich auf Benutzer aus, für die diese Gruppe oder eine ihrer Untergruppen ihre Startseite ist. In ihren Benutzerprofilen sehen diese Benutzer die Ereignisbenachrichtigungen, die für ihre Startseite aktiviert sind, anstelle der systemweit aktivierten Ereignisbenachrichtigungen.

Informationen dazu, wie ein Workfront-Administrator eine Ereignisbenachrichtigung entsperrt, finden Sie unter [Entsperren oder Sperren der Konfiguration von Ereignisbenachrichtigungen für alle Gruppen](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

Informationen zur standardmäßigen Benachrichtigungseinstellung für ein Ereignis finden Sie unter [In Adobe Workfront verfügbare Ereignisbenachrichtigungen](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Workfront-Abo</a>*</td> 
   <td> <p>Pro oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank">Adobe Workfront-Lizenz</a>*</td> 
   <td> <p>Plan </p> <p>Sie müssen Gruppenadministrator der Gruppe oder Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadministratoren</a> und <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenn Sie herausfinden möchten, welchen Plan oder welchen Lizenztyp Sie haben, wenden Sie sich an Ihren Workfront-Administrator.

## Anzeigen und Konfigurieren von Ereignisbenachrichtigungen einer Gruppe

1. (Bedingt und optional) Wenn Sie Workfront-Administrator sind und sich bereits auf der Seite E-Mail-Benachrichtigungen befinden (Einrichtung > E-Mail > Benachrichtigungen), können Sie Folgendes tun und dann zu Schritt 6 überspringen: Löschen **Systemereignisbenachrichtigungen** Geben Sie in das Feld oberhalb der Liste den Gruppennamen in das Feld ein und klicken Sie dann auf die Gruppenname, sobald sie angezeigt wird.
1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **Gruppen** ![](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe der obersten Ebene.
1. Klicken Sie im linken Menü auf **Ereignisbenachrichtigungen**.

   In der angezeigten Liste wird die **Aktiv** zeigt links an, welche Benachrichtigungen für die Gruppe aktiv (blau) und inaktiv (grau) sind.

1. So aktivieren oder deaktivieren Sie eine Benachrichtigung zum entsperrten Ereignis: Klicken Sie auf die Schaltfläche im <strong>Aktiv</strong> Spalte aktivieren <img src="assets/email-notification-enabled-unlocked.png"> oder deaktivieren Sie <img src="assets/email-notification-disabled-unlocked.png"> es.

   >[!INFO]
   >
   >**Beispiel:** Sie können die beiden wichtigsten Marketing-Gruppe-Ereignisbenachrichtigungen konfigurieren, die unten angezeigt werden und für Gruppen entsperrt wurden.</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* Wenn eine Schaltfläche in <strong>Aktiv</strong> Spalte ist grau und abgeblendet <img src="assets/email-notification-disabled-locked.png">, wird die Ereignisbenachrichtigung für alle Benutzer deaktiviert und Gruppenadministratoren können sie nicht aktivieren oder die Betreffzeile der E-Mail bearbeiten
   >* Wenn eine Schaltfläche in <strong>Aktiv</strong> Spalte ist grau und nicht abgeblendet <img src="assets/email-notification-disabled-unlocked.png">, lautet die Ereignisbenachrichtigung . <strong>deaktiviert für alle Benutzer und</strong> -Gruppenadministratoren können sie für ihre Gruppen aktivieren.
   >* Wenn eine Schaltfläche in <strong>Aktiv</strong> Spalte ist blau und abgeblendet <img src="assets/email-notification-enabled-locked.png">, wird die Ereignisbenachrichtigung für alle Benutzer aktiviert und Gruppenadministratoren können sie nicht deaktivieren oder die E-Mail-Betreffzeile für ihre Gruppen bearbeiten.
   >* Wenn eine Schaltfläche in <strong>Aktiv</strong> Spalte ist blau und nicht abgeblendet <img src="assets/email-notification-enabled-unlocked.png">, lautet die Ereignisbenachrichtigung . <strong>für alle Benutzer aktiviert und</strong> -Gruppenadministratoren können sie für ihre Gruppen deaktivieren.


<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->

