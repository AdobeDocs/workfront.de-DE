---
user-type: administrator
product-area: system-administration;user-management
keywords: view,group,event,notifications,configure,enable,disable
navigation-topic: create-and-manage-groups
title: Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe
description: Als Gruppenadministrator können Sie die Ereignisbenachrichtigungen anzeigen, die für eine von Ihnen verwaltete Gruppe aktiviert sind. Wenn ein Adobe Workfront-Administrator eine Ereignisbenachrichtigung entsperrt, können Sie sie auch für eine von Ihnen verwaltete Gruppe der obersten Ebene konfigurieren. Die Konfiguration einer Ereignisbenachrichtigung besteht darin, sie zu aktivieren oder zu deaktivieren.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a815aeb1-3403-4491-a8ad-7e47c519905c
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe

Als Gruppenadministrator können Sie die Ereignisbenachrichtigungen anzeigen, die für eine von Ihnen verwaltete Gruppe aktiviert sind.

Wenn ein Adobe Workfront-Administrator eine Ereignisbenachrichtigung entsperrt, können Sie sie auch für eine von Ihnen verwaltete Gruppe der obersten Ebene konfigurieren. Die Konfiguration einer Ereignisbenachrichtigung besteht darin, sie zu aktivieren oder zu deaktivieren.

Ein Workfront-Administrator kann dies auch für jede Gruppe tun.

Die Konfiguration einer Ereignisbenachrichtigung für eine Gruppe wirkt sich auf Benutzer aus, für die diese Gruppe oder eine ihrer Untergruppen ihre Startseite ist. In ihren Benutzerprofilen sehen diese Benutzer die Ereignisbenachrichtigungen, die für ihre Startseite aktiviert sind, anstelle der systemweit aktivierten Ereignisbenachrichtigungen.

Informationen dazu, wie ein Workfront-Administrator eine Ereignisbenachrichtigung entsperrt, finden Sie unter [Entsperren oder Sperren der Konfiguration von Ereignisbenachrichtigungen für alle Gruppen](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

Informationen zur standardmäßigen Benachrichtigungseinstellung für ein Ereignis finden Sie unter [Ereignistypen](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> <p>Sie müssen Gruppenadministrator der Gruppe oder Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadministratoren</a> und <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs für Benutzer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, wenn Sie herausfinden möchten, welchen Plan oder welchen Lizenztyp Sie haben.

## Anzeigen und Konfigurieren von Ereignisbenachrichtigungen einer Gruppe

1. (Bedingt und optional) Wenn Sie Workfront-Administrator sind und sich bereits auf der Seite &quot;E-Mail-Benachrichtigungen&quot;befinden (Setup > E-Mail > Benachrichtigungen), können Sie Folgendes tun und dann zu Schritt 6 wechseln: Löschen Sie **Systemereignisbenachrichtigungen** im Feld über der Liste, beginnen Sie mit der Eingabe des Gruppennamen in das Feld und klicken Sie dann auf die Gruppe, wenn sie angezeigt wird.
1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Setup** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie im linken Bereich auf **Gruppen** ![](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe der obersten Ebene.
1. Klicken Sie im linken Menü auf **Ereignisbenachrichtigungen**.

   In der angezeigten Liste zeigt die Spalte **Aktiv** links an, welche Benachrichtigungen für die Gruppe aktiv (blau) und inaktiv (grau) sind.

1. So aktivieren oder deaktivieren Sie eine Benachrichtigung über ein entsperrtes Ereignis: Klicken Sie auf die Schaltfläche in der Spalte <strong>Aktiv</strong> , um sie zu aktivieren <img src="assets/email-notification-enabled-unlocked.png"> oder deaktivieren <img src="assets/email-notification-disabled-unlocked.png"> it.

   >[!INFO]
   >
   >**Beispiel:** Sie können die beiden wichtigsten Marketing-Gruppen-Ereignisbenachrichtigungen konfigurieren, die unten angezeigt werden und für Gruppen entsperrt wurden.</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* Wenn eine Schaltfläche in der Spalte <strong>Aktiv</strong> grau und abgeblendet ist <img src="assets/email-notification-disabled-locked.png">, die Ereignisbenachrichtigung ist für alle Benutzer deaktiviert und Gruppenadministratoren können sie nicht aktivieren oder die Betreffzeile der E-Mail bearbeiten
   >* Wenn eine Schaltfläche in der Spalte <strong>Aktiv</strong> grau und nicht abgeblendet ist <img src="assets/email-notification-disabled-unlocked.png"> ist die Ereignisbenachrichtigung für alle Benutzer deaktiviert und </strong> Gruppenadministratoren können sie für ihre Gruppen aktivieren.<strong>
   >* Wenn eine Schaltfläche in der Spalte <strong>Aktiv</strong> blau und abgeblendet ist <img src="assets/email-notification-enabled-locked.png">, wird die Ereignisbenachrichtigung für alle Benutzer aktiviert und Gruppenadministratoren können sie nicht deaktivieren oder die E-Mail-Betreffzeile für ihre Gruppen bearbeiten.
   >* Wenn eine Schaltfläche in der Spalte <strong>Aktiv</strong> blau und nicht abgeblendet ist <img src="assets/email-notification-enabled-unlocked.png"> ist die Ereignisbenachrichtigung für alle Benutzer aktiviert und </strong> Gruppenadministratoren können sie für ihre Gruppen deaktivieren.<strong>

<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->

