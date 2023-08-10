---
title: Ereignisbenachrichtigungen für alle Benutzer im System konfigurieren
description: Ereignisbenachrichtigungen Trigger senden E-Mails an Benutzer, wenn ein bestimmtes Ereignis eintritt. Als Adobe Workfront-Administrator oder Benutzer mit der Zugriffsebene "Planer"können Sie eine Ereignisbenachrichtigung für alle Benutzer im System konfigurieren. Die Konfiguration einer Ereignisbenachrichtigung besteht darin, sie zu aktivieren oder zu deaktivieren.
author: Caroline, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 027ecebd-d9de-4cdd-b15a-88de18367591
source-git-commit: 207a8c8a642f3204a2d007789eb7ee8cd9379f1b
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# Ereignisbenachrichtigungen für alle Benutzer im System konfigurieren

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS-->

Ereignisbenachrichtigungen Trigger senden E-Mails an Benutzer, wenn ein bestimmtes Ereignis eintritt. Als Adobe Workfront-Administrator oder Benutzer mit der Zugriffsebene &quot;Planer&quot;können Sie eine Ereignisbenachrichtigung für alle Benutzer im System konfigurieren. Die Konfiguration einer Ereignisbenachrichtigung besteht darin, sie zu aktivieren oder zu deaktivieren.

<!--Alina annotation on the word "all" in 2nd sentence: abive, drafted and remains QS only-->

Je nach dem von Ihnen aktivierten Ereignis und der Benutzer bleibt in seinem Profil aktiviert, erhalten Benutzer sofortige, tägliche oder sowohl sofortige als auch tägliche E-Mail-Benachrichtigungen, wenn ein Ereignis eintritt.

Sie müssen zunächst angeben, welche Benachrichtigungen alle Ihre Benutzer im Setup-Bereich Ihrer Workfront-Instanz erhalten sollen. Nachdem Sie eine Benachrichtigung im Bereich Einrichtung aktiviert haben, wird sie für jeden Benutzer auf seiner Profilseite aktiviert.

Nachdem Benachrichtigungen im Bereich Einrichtung aktiviert wurden und auf den Profilseiten der Benutzer angezeigt werden, können einzelne Benutzer oder ein anderer Benutzer mit einer Planungslizenz die aktivierten Benachrichtigungen in einem Benutzerprofil auch konfigurieren, um zu steuern, welche Benachrichtigungen ein bestimmter Benutzer erhält und wie oft. Weitere Informationen finden Sie unter [Aktivieren oder Deaktivieren Ihrer eigenen Ereignisbenachrichtigungen](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Eine Liste aller Ereignisbenachrichtigungen, die Sie aktivieren und deaktivieren können, finden Sie unter [In Adobe Workfront verfügbare Ereignisbenachrichtigungen](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Informationen zum Entsperren einer Ereignisbenachrichtigung, damit Gruppenadministratoren sie für ihre Gruppen konfigurieren können, finden Sie unter [Entsperren oder Sperren der Konfiguration von Ereignisbenachrichtigungen für alle Gruppen](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md) und [Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Planung oder höher mit Administratorzugriff auf Erinnerungsbenachrichtigungen</p> <p>Informationen zum Gewähren eines administrativen Zugriffs für Planbenutzer finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Ereignisbenachrichtigungen für alle Benutzer konfigurieren

Sie müssen Benachrichtigungen im Bereich Einrichtung von Workfront aktivieren, bevor Benutzer sie in ihren Profilen aktivieren oder deaktivieren können.

>[!TIP]
>
>Sie können keine Benachrichtigungen für Workfront-Ziele über den Bereich &quot;Einrichtung&quot;aktivieren. Benutzer können diese Benachrichtigungen nur in ihren Profilen aktivieren. Benutzer mit Planungslizenzen können sie für andere Benutzer aktivieren. Informationen zum Aktivieren von Workfront-Zielbenachrichtigungen für Benutzer finden Sie unter [Benachrichtigungen: Ziele](../../../workfront-basics/using-notifications/notifications-goals.md).

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicks **Email** > **Benachrichtigungen**.

   ![](assets/notifications-area-under-setup-emails.png)


1. Stellen Sie sicher, dass **Ereignisbenachrichtigungen** ist geöffnet.
1. Klicken Sie auf den Schalter links neben dem Ereignisnamen, um ihn zu aktivieren oder zu deaktivieren.

   Informationen zum standardmäßigen Benachrichtigungsstatus für ein Ereignis finden Sie unter [Ereignisbenachrichtigungen](../../../workfront-basics/using-notifications/event-notifications.md).

1. (Optional) Klicken Sie auf den Namen einer Ereignisbenachrichtigung, um die Betreffzeile der E-Mail-Benachrichtigung anzupassen.

   Weitere Informationen zum Anpassen der Betreffzeilen von E-Mail-Benachrichtigungen finden Sie unter [Anpassen von E-Mail-Betreffs für Ereignisbenachrichtigungen](../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

1. (Optional) Wenn Sie die Konfiguration für eine E-Mail-Benachrichtigung entsperren möchten, damit Gruppenadministratoren sie für ihre Gruppen einzeln konfigurieren können, klicken Sie auf die Schaltfläche ![](assets/lock-toggle-button.png) rechts neben der Benachrichtigung, um sie in die entsperrte Position zu wechseln ![](assets/unlock-toggle-button.png).

   >[!NOTE]
   >
   >Diese Funktion ist zunächst nur für Kunden verfügbar, die Cluster 4 im Rahmen eines stufenweisen Rollouts nutzen. Kurz danach wird es für andere Cluster verfügbar sein. Dieser Artikel wird aktualisiert, sobald dies eintritt.

   Weitere Informationen finden Sie unter [Entsperren oder Sperren der Konfiguration von Ereignisbenachrichtigungen für alle Gruppen](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).
