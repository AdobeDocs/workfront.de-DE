---
title: Konfigurieren von Ereignisbenachrichtigungen für alle Benutzer im System
description: Ereignisbenachrichtigungen Trigger-E-Mails an Benutzende, wenn ein bestimmtes Ereignis eintritt. Als Adobe Workfront-Admin oder Benutzende mit Planerzugriffsebene können Sie eine Ereignisbenachrichtigung für alle Benutzenden im System konfigurieren. Bei der Konfiguration einer Ereignisbenachrichtigung wird diese aktiviert oder deaktiviert.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 027ecebd-d9de-4cdd-b15a-88de18367591
source-git-commit: e9c6a01e80d34bc873c9a06ae0782dc65afb2445
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 1%

---

# Ereignisbenachrichtigungen für alle Systembenutzenden konfigurieren

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS-->

Ereignisbenachrichtigungen Trigger-E-Mails an Benutzende, wenn ein bestimmtes Ereignis eintritt. Als Adobe Workfront-Admin oder Benutzende mit Planerzugriffsebene können Sie eine Ereignisbenachrichtigung für alle Benutzenden im System konfigurieren. Bei der Konfiguration einer Ereignisbenachrichtigung wird diese aktiviert oder deaktiviert.

<!--Alina annotation on the word "all" in 2nd sentence: abive, drafted and remains QS only-->

Je nach dem von Ihnen aktivierten Ereignis und den aktivierten Benutzerprofilen erhalten Benutzerinnen und Benutzer beim Eintreten eines Ereignisses sofort, täglich oder sowohl sofort als auch täglich E-Mail-Benachrichtigungen.

Sie müssen zunächst im Bereich Setup Ihrer Workfront-Instanz angeben, welche Benachrichtigungen Sie an alle Ihre Benutzerinnen und Benutzer senden möchten. Nachdem Sie eine Benachrichtigung im Bereich Setup aktiviert haben, wird sie für jeden Benutzer auf seiner Profilseite als aktiviert angezeigt.

Nachdem Benachrichtigungen im Bereich Setup aktiviert wurden und auf den Profilseiten der Benutzer angezeigt werden, können einzelne Benutzer oder ein anderer Benutzer mit einer Planlizenz die aktivierten Benachrichtigungen auch in einem Benutzerprofil konfigurieren, um zu steuern, welche Benachrichtigungen dieser bestimmte Benutzer erhält und wie oft. Weitere Informationen finden Sie unter [Eigene E-Mail-Benachrichtigungen ändern](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Eine Liste aller Ereignisbenachrichtigungen, die Sie aktivieren und deaktivieren können, finden Sie unter [Ereignistypen](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Informationen zum Entsperren einer Ereignisbenachrichtigung, damit Gruppenadministratoren sie für ihre Gruppen konfigurieren können, finden Sie unter [Konfiguration von Ereignisbenachrichtigungen für alle Gruppen entsperren oder sperren](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md) und [Ereignisbenachrichtigungen für eine Gruppe anzeigen und konfigurieren](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

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
   <td> <p>Neu: Standard</p>
 <p>oder</p> 
<p>Aktuell: Plan</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Planer oder höher mit administrativem Zugriff auf Erinnerungsnachrichten</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurieren von Ereignisbenachrichtigungen für alle Benutzer

Sie müssen Benachrichtigungen im Bereich Setup von Workfront aktivieren, bevor Benutzerinnen und Benutzer sie in ihren individuellen Profilen aktivieren oder deaktivieren können.

>[!TIP]
>
>Sie können Benachrichtigungen für Workfront-Ziele nicht über den Bereich „Setup“ aktivieren. Benutzer können diese Benachrichtigungen nur in ihren Profilen aktivieren. Benutzende mit Planlizenzen können sie für andere Benutzende aktivieren. Informationen zur Aktivierung von Workfront Goals-Benachrichtigungen für Benutzerinnen und Benutzer finden Sie unter [Benachrichtigungen: Ziele](../../../workfront-basics/using-notifications/notifications-goals.md).

{{step-1-to-setup}}

1. Klicken Sie auf **E** > **Benachrichtigungen**.

   ![Benachrichtigungsbereich unter „E-Mails einrichten“](assets/notifications-area-under-setup-emails.png)


1. Stellen Sie sicher **dass die Registerkarte** Ereignisbenachrichtigungen“ geöffnet ist.
1. Schalten Sie den Schalter links neben dem Ereignisnamen um, um ihn zu aktivieren oder zu deaktivieren.

   Den Standardbenachrichtigungsstatus für ein Ereignis finden Sie unter [Ereignisbenachrichtigungen](../../../workfront-basics/using-notifications/event-notifications.md).

1. (Optional) Klicken Sie auf den Namen einer Ereignisbenachrichtigung, um die Betreffzeile der E-Mail-Benachrichtigung anzupassen.

   Weitere Informationen zum Anpassen der Betreffzeilen von E-Mail-Benachrichtigungen finden Sie unter [Anpassen von E-Mail-Betreffen für ](../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

1. (Optional) Wenn Sie die Konfiguration einer E-Mail-Benachrichtigung entsperren möchten, damit Gruppenadministratoren sie separat für ihre Gruppen konfigurieren können, klicken Sie auf die Schaltfläche ![Sperren-Umschalter](assets/lock-toggle-button.png) rechts neben der Benachrichtigung, um sie in die entsperrte Position zu ![Entsperren-Umschalter](assets/unlock-toggle-button.png).

   Weitere Informationen finden Sie unter [Konfiguration von Ereignisbenachrichtigungen für alle Gruppen entsperren oder sperren](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

Benutzer können die Häufigkeit dieser Benachrichtigungen in ihrem Benutzerprofil anpassen.