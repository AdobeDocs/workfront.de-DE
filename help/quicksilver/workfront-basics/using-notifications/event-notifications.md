---
content-type: overview
navigation-topic: notifications
title: Ereignisbenachrichtigungen
description: Ereignisbenachrichtigungen sind E-Mails, die von verschiedenen Ereignistypen auf Objekten wie Projekten, Aufgaben oder Problemen ausgelöst werden. Sie werden gesendet, wenn etwas im Projekt auftritt, über das andere wissen müssen. Je nach Ereignis erhalten Benutzer sofortige, tägliche oder sofortige und tägliche E-Mail-Benachrichtigungen.
author: Lisa
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 0%

---

# Ereignisbenachrichtigungen

Ereignisbenachrichtigungen sind E-Mails, die von verschiedenen Ereignistypen auf Objekten wie Projekten, Aufgaben oder Problemen ausgelöst werden. Sie werden gesendet, wenn etwas im Projekt auftritt, über das andere wissen müssen. Je nach Ereignis erhalten Benutzer sofortige, tägliche oder sofortige und tägliche E-Mail-Benachrichtigungen.

>[!NOTE]
>
>Ereignisbenachrichtigungen sind eine von mehreren Arten von [!DNL Adobe Workfront] Benachrichtigungen. Für Informationen über alle [!DNL Workfront] Benachrichtigungstypen, siehe [[!DNL Adobe Workfront] Benachrichtigungen](../../workfront-basics/using-notifications/wf-notifications.md).

## Ereignisbenachrichtigungen konfigurieren

E-Mails zu Ereignisbenachrichtigungen können auf den folgenden Ebenen konfiguriert werden: Die Konfiguration einer Ereignisbenachrichtigung besteht darin, sie zu aktivieren oder zu deaktivieren.

* **Systemebene**: A [!DNL Workfront] Administratoren können Ereignisbenachrichtigungen auf Systemebene aktivieren und deaktivieren, wie unter [Ereignisbenachrichtigungen für alle Benutzer im System konfigurieren](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

  Alle Gruppen übernehmen standardmäßig Systembenachrichtigungen, Gruppenadministratoren können jedoch möglicherweise einige Konfigurationen auf Gruppenebene ändern, sofern dies durch die [!DNL Workfront] Administrator, wie im nächsten Aufzählungszeichen unten beschrieben.

* **Gruppenebene**: Ein Gruppenadministrator kann eine Ereignisbenachrichtigung für Gruppen konfigurieren, die er nach einer [!DNL Workfront] Administrator schließt diese Fähigkeit für Gruppen aus. Wenn es Gruppen über der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für [!DNL Workfront] Administratoren (für jede Gruppe). Weitere Informationen finden Sie unter [Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

  >[!NOTE]
  >
  >Diese Funktion ist zunächst nur für Kunden verfügbar, die Cluster 4 im Rahmen eines stufenweisen Rollouts nutzen. Kurz danach wird es für andere Cluster verfügbar sein. Dieser Artikel wird aktualisiert, sobald dies eintritt.

* **Benutzerebene**: Alle Ereignisbenachrichtigungen, die systemweit aktiviert sind, werden in der [!UICONTROL Benachrichtigungen] auf ihrem jeweiligen Profil. Benutzer können dort ihre individuellen Ereignisbenachrichtigungen aktivieren und deaktivieren.

  [!DNL Workfront] Administratoren und Benutzer mit Zugriff auf die Bearbeitung anderer Benutzer können Benachrichtigungen auch im Profil einzelner Benutzer aktivieren und deaktivieren.

  Weitere Informationen finden Sie unter [Ihre eigenen E-Mail-Benachrichtigungen ändern](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  >[!NOTE]
  >
  >Zu den Benachrichtigungen auf Benutzerebene gehören auch [!DNL Workfront Goals] Benachrichtigungen. Die Variable [!DNL Workfront] -Administrator oder Gruppenadministrator kann keine Benachrichtigungen für [!DNL Workfront Goals]. Jede Verwendung muss ihre eigenen [!DNL Workfront Goals] Benachrichtigungen in ihrem Profil. Wenn Sie Zugriff auf die Bearbeitung von Benutzern haben, können Sie diese Benachrichtigungen auch für andere Benutzer ändern. Für Aktivierung [!DNL Workfront Goals] Benachrichtigungen für Ihr Profil oder für andere Benutzer, auf die Sie Zugriff haben, finden Sie unter [Benachrichtigungen: Ziele](../../workfront-basics/using-notifications/notifications-goals.md).

  Weitere Informationen zu den Benachrichtigungen finden Sie unter [!DNL Workfront] Administratoren können konfigurieren, siehe [Ereignisbenachrichtigungen für alle Benutzer im System konfigurieren](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). [!DNL Workfront Goals] sind nur in der neuen [!DNL Adobe Workfront] Erlebnis.

## Inhalt der Ereignisbenachrichtigungen

Eine Ereignisbenachrichtigungs-E-Mail enthält Informationen zum stattgefundenen Ereignis und einen Link zu [!DNL Workfront] wo das Ereignis im System angezeigt wird. Weitere Informationen zum Empfang von E-Mail-Benachrichtigungen finden Sie unter [[!DNL Adobe Workfront] Benachrichtigungen](../../workfront-basics/using-notifications/wf-notifications.md).

A [!DNL Workfront] Der Administrator kann den Inhalt der E-Mail-Benachrichtigungen nicht ändern, da diese von [!DNL Workfront]. Sie können jedoch die Betreffzeilen von E-Mails mit Ereignisbenachrichtigungen ändern. Weitere Informationen finden Sie unter [Anpassen von E-Mail-Betreffs für Ereignisbenachrichtigungen](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

Für eine Liste alle [!DNL Workfront] Ereignisbenachrichtigungen sowie eine kurze Beschreibung der einzelnen Ereignisse und darüber, ob sie standardmäßig aktiv oder inaktiv sind, finden Sie unter [Verfügbare Ereignisbenachrichtigungen [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
