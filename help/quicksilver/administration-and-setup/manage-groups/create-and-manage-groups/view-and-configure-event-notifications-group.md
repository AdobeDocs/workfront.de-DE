---
user-type: administrator
product-area: system-administration;user-management
keywords: Anzeigen,Gruppe,Ereignis,Benachrichtigungen,Konfigurieren,Aktivieren,Deaktivieren
navigation-topic: create-and-manage-groups
title: Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe
description: Als Gruppenadministrator können Sie die Ereignisbenachrichtigungen anzeigen, die für eine von Ihnen verwaltete Gruppe aktiviert sind. Wenn ein Adobe Workfront-Administrator eine Ereignisbenachrichtigung entsperrt, können Sie sie auch für eine von Ihnen verwaltete Gruppe auf oberster Ebene konfigurieren. Bei der Konfiguration einer Ereignisbenachrichtigung wird diese aktiviert oder deaktiviert.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a815aeb1-3403-4491-a8ad-7e47c519905c
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 0%

---

# Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe

Als Gruppenadministrator können Sie die Ereignisbenachrichtigungen anzeigen, die für eine von Ihnen verwaltete Gruppe aktiviert sind.

Wenn ein Adobe Workfront-Administrator eine Ereignisbenachrichtigung entsperrt, können Sie sie auch für eine von Ihnen verwaltete Gruppe auf oberster Ebene konfigurieren. Bei der Konfiguration einer Ereignisbenachrichtigung wird diese aktiviert oder deaktiviert.

Ein Workfront-Administrator kann dies auch für jede Gruppe tun.

Die Konfiguration einer Ereignisbenachrichtigung für eine Gruppe wirkt sich auf Benutzende aus, für die diese Gruppe oder eine ihrer Untergruppen ihre Hauptgruppe ist. In ihren Benutzerprofilen sehen diese Benutzer die Ereignisbenachrichtigungen, die für ihre Hauptgruppe aktiviert sind, anstelle der Ereignisbenachrichtigungen, die systemweit aktiviert sind.

Informationen dazu, wie ein Workfront-Administrator eine Ereignisbenachrichtigung entsperrt, finden Sie unter [Konfiguration von Ereignisbenachrichtigungen für alle Gruppen entsperren oder sperren](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

Weitere Informationen über die standardmäßige Benachrichtigungseinstellung für ein Ereignis finden Sie unter [Ereignistypen](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

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
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anzeigen und Konfigurieren der Ereignisbenachrichtigungen einer Gruppe

>[!TIP]
>
>Wenn Sie Workfront-Administrator sind und sich bereits auf der Seite „E-Mail-Benachrichtigungen“ befinden (Einstellungen > E-Mail > Benachrichtigungen), können Sie Folgendes tun und dann mit Schritt 6 fortfahren: Löschen **Systemereignis-Benachrichtigungen** im Feld über der Liste, Beginnen Sie, den Namen der Gruppe in das Feld einzugeben, und klicken Sie dann auf die Gruppe, wenn sie angezeigt wird.

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Gruppen** ![](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe der obersten Ebene.
1. Klicken Sie im linken Menü auf **Ereignisbenachrichtigungen**.

   In der angezeigten Liste zeigt die Spalte **Aktiv** auf der linken Seite, welche Benachrichtigungen für die Gruppe aktiv (blau) und inaktiv (grau) sind.

1. So aktivieren oder deaktivieren Sie eine entsperrte Ereignisbenachrichtigung: Klicken Sie zum Aktivieren auf die Schaltfläche in der Spalte <strong>Aktiv</strong>. <img src="assets/email-notification-enabled-unlocked.png"> oder deaktivieren <img src="assets/email-notification-disabled-unlocked.png">.

   >[!INFO]
   >
   >**Beispiel** Sie könnten die beiden unten gezeigten Ereignisbenachrichtigungen für Marketing-Gruppen konfigurieren, die für Gruppen entsperrt wurden.</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* Wenn eine Schaltfläche in der Spalte <strong>Aktiv</strong> grau und abgeblendet ist <img src="assets/email-notification-disabled-locked.png"> ist die Ereignisbenachrichtigung für alle Benutzer deaktiviert und Gruppenadministratoren können sie nicht aktivieren oder die Betreffzeile der E-Mail bearbeiten
   >* Wenn eine Schaltfläche in der Spalte <strong>Aktiv</strong> grau und nicht abgeblendet ist <img src="assets/email-notification-disabled-unlocked.png"> ist die Ereignisbenachrichtigung für <strong> Benutzer deaktiviert und </strong> können sie für ihre Gruppen aktivieren.
   >* Wenn eine Schaltfläche in der Spalte <strong>Aktiv</strong> blau und abgeblendet ist <img src="assets/email-notification-enabled-locked.png"> ist die Ereignisbenachrichtigung für alle Benutzer aktiviert und Gruppenadministratoren können sie nicht deaktivieren oder die Betreffzeile der E-Mail für ihre Gruppen bearbeiten.
   >* Wenn eine Schaltfläche in der Spalte <strong>Aktiv</strong> blau und nicht abgeblendet ist <img src="assets/email-notification-enabled-unlocked.png"> wird die Ereignisbenachrichtigung für <strong> Benutzer aktiviert und </strong> können sie für ihre Gruppen deaktivieren.

<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->

