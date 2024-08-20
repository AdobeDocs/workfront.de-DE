---
title: Konfigurieren von Ereignisbenachrichtigungen für alle Benutzer im System
description: Ereignisbenachrichtigungen Trigger senden E-Mails an Benutzer, wenn ein bestimmtes Ereignis eintritt. Als Adobe Workfront-Administrator oder Benutzer mit der Zugriffsebene "Planer"können Sie eine Ereignisbenachrichtigung für alle Benutzer im System konfigurieren. Die Konfiguration einer Ereignisbenachrichtigung besteht darin, sie zu aktivieren oder zu deaktivieren.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 027ecebd-d9de-4cdd-b15a-88de18367591
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 1%

---

# Ereignisbenachrichtigungen für alle Systembenutzenden konfigurieren

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS-->

Ereignisbenachrichtigungen Trigger senden E-Mails an Benutzer, wenn ein bestimmtes Ereignis eintritt. Als Adobe Workfront-Administrator oder Benutzer mit der Zugriffsebene &quot;Planer&quot;können Sie eine Ereignisbenachrichtigung für alle Benutzer im System konfigurieren. Die Konfiguration einer Ereignisbenachrichtigung besteht darin, sie zu aktivieren oder zu deaktivieren.

<!--Alina annotation on the word "all" in 2nd sentence: abive, drafted and remains QS only-->

Je nach dem von Ihnen aktivierten Ereignis und der Benutzer bleibt in seinem Profil aktiviert, erhalten Benutzer sofortige, tägliche oder sowohl sofortige als auch tägliche E-Mail-Benachrichtigungen, wenn ein Ereignis eintritt.

Sie müssen zunächst angeben, welche Benachrichtigungen alle Ihre Benutzer im Setup-Bereich Ihrer Workfront-Instanz erhalten sollen. Nachdem Sie eine Benachrichtigung im Bereich Einrichtung aktiviert haben, wird sie für jeden Benutzer auf seiner Profilseite aktiviert.

Nachdem Benachrichtigungen im Bereich Einrichtung aktiviert wurden und auf den Profilseiten der Benutzer angezeigt werden, können einzelne Benutzer oder ein anderer Benutzer mit einer Planungslizenz die aktivierten Benachrichtigungen in einem Benutzerprofil auch konfigurieren, um zu steuern, welche Benachrichtigungen ein bestimmter Benutzer erhält und wie oft. Weitere Informationen finden Sie unter [Ändern Ihrer eigenen E-Mail-Benachrichtigungen](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Eine Liste aller Ereignisbenachrichtigungen, die Sie aktivieren und deaktivieren können, finden Sie unter [Benachrichtigungstypen für Ereignisse](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Informationen zum Entsperren einer Ereignisbenachrichtigung, sodass Gruppenadministratoren sie für ihre Gruppen konfigurieren können, finden Sie unter [Entsperren oder Sperren der Konfiguration von Ereignisbenachrichtigungen für alle Gruppen](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md) und [Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

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
   <td> <p>Neu: Standard</p>
 <p>oder</p> 
<p>Aktuell: Plan</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Planung oder höher mit Administratorzugriff auf Erinnerungsbenachrichtigungen</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ereignisbenachrichtigungen für alle Benutzer konfigurieren

Sie müssen Benachrichtigungen im Einrichtungsbereich von Workfront aktivieren, bevor Benutzer sie in ihren Profilen aktivieren oder deaktivieren können.

>[!TIP]
>
>Sie können keine Benachrichtigungen für Workfront-Ziele über den Bereich &quot;Einrichtung&quot;aktivieren. Benutzer können diese Benachrichtigungen nur in ihren Profilen aktivieren. Benutzer mit Planungslizenzen können sie für andere Benutzer aktivieren. Informationen zum Aktivieren von Workfront-Zielbenachrichtigungen für Benutzer finden Sie unter [Benachrichtigungen: Ziele](../../../workfront-basics/using-notifications/notifications-goals.md).

{{step-1-to-setup}}

1. Klicken Sie auf **E-Mail** > **Benachrichtigungen**.

   ![](assets/notifications-area-under-setup-emails.png)


1. Stellen Sie sicher, dass die Registerkarte **Ereignisbenachrichtigungen** geöffnet ist.
1. Schalten Sie den Schalter links neben dem Ereignisnamen um, um ihn zu aktivieren oder zu deaktivieren.

   Informationen zum standardmäßigen Benachrichtigungsstatus für ein Ereignis finden Sie unter [Ereignisbenachrichtigungen](../../../workfront-basics/using-notifications/event-notifications.md).

1. (Optional) Klicken Sie auf den Namen einer Ereignisbenachrichtigung, um die Betreffzeile der E-Mail-Benachrichtigung anzupassen.

   Weitere Informationen zum Anpassen der Betreffzeilen von E-Mail-Benachrichtigungen finden Sie unter [Anpassen von E-Mail-Betreffs für Ereignisbenachrichtigungen](../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

1. (Optional) Wenn Sie die Konfiguration für eine E-Mail-Benachrichtigung entsperren möchten, damit Gruppenadministratoren sie für ihre Gruppen separat konfigurieren können, klicken Sie auf die Schaltfläche &quot;![](assets/lock-toggle-button.png)&quot; rechts neben der Benachrichtigung, um sie an die entsperrte Position &quot;![](assets/unlock-toggle-button.png)&quot; zu wechseln.

   >[!NOTE]
   >
   >Diese Funktion ist zunächst nur für Kunden verfügbar, die Cluster 4 im Rahmen eines stufenweisen Rollouts nutzen. Kurz danach wird es für andere Cluster verfügbar sein. Dieser Artikel wird aktualisiert, sobald dies eintritt.

   Weitere Informationen finden Sie unter [Entsperren oder Sperren der Konfiguration von Ereignisbenachrichtigungen für alle Gruppen](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).
