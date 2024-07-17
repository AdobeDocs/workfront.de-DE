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
source-wordcount: '554'
ht-degree: 0%

---

# Ereignisbenachrichtigungen

Ereignisbenachrichtigungen sind E-Mails, die von verschiedenen Ereignistypen auf Objekten wie Projekten, Aufgaben oder Problemen ausgelöst werden. Sie werden gesendet, wenn etwas im Projekt auftritt, über das andere wissen müssen. Je nach Ereignis erhalten Benutzer sofortige, tägliche oder sofortige und tägliche E-Mail-Benachrichtigungen.

>[!NOTE]
>
>Ereignisbenachrichtigungen sind eine von mehreren Arten von [!DNL Adobe Workfront] -Benachrichtigungen. Informationen zu allen [!DNL Workfront]-Benachrichtigungstypen finden Sie unter [[!DNL Adobe Workfront] Benachrichtigungen](../../workfront-basics/using-notifications/wf-notifications.md).

## Ereignisbenachrichtigungen konfigurieren

E-Mails zu Ereignisbenachrichtigungen können auf den folgenden Ebenen konfiguriert werden: Die Konfiguration einer Ereignisbenachrichtigung besteht darin, sie zu aktivieren oder zu deaktivieren.

* **Systemebene**: Ein [!DNL Workfront] -Administrator kann Ereignisbenachrichtigungen auf Systemebene aktivieren und deaktivieren, wie unter [Ereignisbenachrichtigungen für alle Benutzer im System konfigurieren](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md) beschrieben.

  Alle Gruppen erben standardmäßig Systembenachrichtigungen. Gruppenadministratoren können jedoch möglicherweise einige Konfigurationen auf Gruppenebene ändern, sofern dies vom Administrator [!DNL Workfront] erlaubt wird, wie im nächsten Aufzählungszeichen unten erläutert.

* **Gruppenebene**: Ein Gruppenadministrator kann eine Ereignisbenachrichtigung für Gruppen konfigurieren, die er verwaltet, nachdem ein [!DNL Workfront] -Administrator diese Fähigkeit für Gruppen entsperrt hat. Wenn es Gruppen über der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für [!DNL Workfront] -Administratoren (für jede Gruppe). Weitere Informationen finden Sie unter [Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

  >[!NOTE]
  >
  >Diese Funktion ist zunächst nur für Kunden verfügbar, die Cluster 4 im Rahmen eines stufenweisen Rollouts nutzen. Kurz danach wird es für andere Cluster verfügbar sein. Dieser Artikel wird aktualisiert, sobald dies eintritt.

* **Benutzerebene**: Alle systemweit aktivierten Ereignisbenachrichtigungen werden im Abschnitt [!UICONTROL Benachrichtigungen] der Benutzer in ihrem jeweiligen Profil aufgelistet. Benutzer können dort ihre individuellen Ereignisbenachrichtigungen aktivieren und deaktivieren.

  [!DNL Workfront] -Administratoren und Benutzer mit Zugriff zur Bearbeitung anderer Benutzer können Benachrichtigungen auch im Profil einzelner Benutzer aktivieren und deaktivieren.

  Weitere Informationen finden Sie unter [Ändern Ihrer eigenen E-Mail-Benachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  >[!NOTE]
  >
  >Benachrichtigungen auf Benutzerebene enthalten auch [!DNL Workfront Goals] -Benachrichtigungen. Der Administrator [!DNL Workfront] oder der Gruppenadministrator kann jedoch keine Benachrichtigungen für [!DNL Workfront Goals] konfigurieren. Jeder Benutzer muss seine eigenen [!DNL Workfront Goals]-Benachrichtigungen in seinem Profil konfigurieren. Wenn Sie Zugriff auf die Bearbeitung von Benutzern haben, können Sie diese Benachrichtigungen auch für andere Benutzer ändern. Informationen zum Aktivieren von [!DNL Workfront Goals] -Benachrichtigungen für Ihr Profil oder für andere Benutzer, die Sie bearbeiten können, finden Sie unter [Benachrichtigungen: Ziele](../../workfront-basics/using-notifications/notifications-goals.md).

  Weitere Informationen dazu, welche Benachrichtigungen der [!DNL Workfront]-Administrator konfigurieren kann, finden Sie unter [Ereignisbenachrichtigungen für alle Benutzer im System konfigurieren](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). [!DNL Workfront Goals] sind nur im neuen Erlebnis [!DNL Adobe Workfront] verfügbar.

## Inhalt der Ereignisbenachrichtigungen

Eine E-Mail mit einer Ereignisbenachrichtigung enthält Informationen über das Ereignis, das stattgefunden hat, und einen Link zu &quot;[!DNL Workfront]&quot;, in dem das Ereignis im System angezeigt wird. Weitere Informationen zum Empfang von E-Mail-Benachrichtigungen finden Sie unter [[!DNL Adobe Workfront] Benachrichtigungen](../../workfront-basics/using-notifications/wf-notifications.md).

Ein [!DNL Workfront] -Administrator kann den Inhalt der E-Mail-Benachrichtigungen nicht ändern, da er von [!DNL Workfront] konfiguriert wurde. Sie können jedoch die Betreffzeilen von E-Mails mit Ereignisbenachrichtigungen ändern. Weitere Informationen finden Sie unter [Anpassen von E-Mail-Betreffs für Ereignisbenachrichtigungen](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

Eine Liste aller [!DNL Workfront] -Ereignisbenachrichtigungen sowie eine kurze Beschreibung der einzelnen Ereignisse und darüber, ob sie standardmäßig aktiv oder inaktiv sind, finden Sie unter [In  [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md) verfügbare Ereignisbenachrichtigungen.
