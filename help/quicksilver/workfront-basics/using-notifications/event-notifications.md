---
content-type: overview
navigation-topic: notifications
title: Ereignisbenachrichtigungen
description: Ereignisbenachrichtigungen sind E-Mails, die von verschiedenen Ereignistypen für Objekte wie Projekte, Aufgaben oder Probleme ausgelöst werden. Sie werden gesendet, wenn im Projekt etwas passiert, von dem andere wissen müssen. Je nach Ereignis erhalten Benutzer sofortige, tägliche oder sowohl sofortige als auch tägliche E-Mail-Benachrichtigungen darüber.
author: Lisa
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# Ereignisbenachrichtigungen

Ereignisbenachrichtigungen sind E-Mails, die von verschiedenen Ereignistypen für Objekte wie Projekte, Aufgaben oder Probleme ausgelöst werden. Sie werden gesendet, wenn im Projekt etwas passiert, von dem andere wissen müssen. Je nach Ereignis erhalten Benutzer sofortige, tägliche oder sowohl sofortige als auch tägliche E-Mail-Benachrichtigungen darüber.

>[!NOTE]
>
>Ereignisbenachrichtigungen sind eine von mehreren Arten von [!DNL Adobe Workfront]. Informationen zu allen [!DNL Workfront] Benachrichtigungstypen finden Sie unter [[!DNL Adobe Workfront] Benachrichtigungen](../../workfront-basics/using-notifications/wf-notifications.md).

## Konfigurieren von Ereignisbenachrichtigungen

Ereignisbenachrichtigungs-E-Mails können auf den folgenden Ebenen konfiguriert werden. Bei der Konfiguration einer Ereignisbenachrichtigung wird diese aktiviert oder deaktiviert.

* **Systemebene**: Ein [!DNL Workfront]-Administrator kann Ereignisbenachrichtigungen auf Systemebene aktivieren und deaktivieren, wie in [Konfigurieren von Ereignisbenachrichtigungen für alle Personen im System](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md) beschrieben.

  Alle Gruppen erben standardmäßig Systembenachrichtigungen, Gruppenadministratoren können jedoch möglicherweise einige Konfigurationen auf Gruppenebene ändern, wenn der [!DNL Workfront] dies zulässt, wie im nächsten Aufzählungselement unten beschrieben.

* **Gruppenebene** Ein Gruppenadministrator kann eine Ereignisbenachrichtigung für von ihm verwaltete Gruppen konfigurieren, nachdem ein [!DNL Workfront] diese Funktion für Gruppen freigegeben hat. Wenn es Gruppen oberhalb der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für [!DNL Workfront] Administratoren (für jede Gruppe). Weitere Informationen finden Sie unter [Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

  >[!NOTE]
  >
  >Diese Funktion steht zunächst nur Kunden auf Cluster 4 im Rahmen eines schrittweisen Rollouts zur Verfügung. Kurz darauf wird es für andere Cluster verfügbar sein. Dieser Artikel wird aktualisiert, sobald dieser auftritt.

* **Benutzerebene**: Alle Ereignisbenachrichtigungen, die systemweit aktiviert sind, werden im Abschnitt [!UICONTROL Benachrichtigungen] jedes Benutzers in seinem individuellen Profil aufgelistet. Dort können Benutzer ihre individuellen Ereignisbenachrichtigungen aktivieren und deaktivieren.

  [!DNL Workfront] und Benutzer mit Zugriff auf die Bearbeitung anderer Benutzer können Benachrichtigungen auch im Profil einzelner Benutzer aktivieren und deaktivieren.

  Weitere Informationen finden Sie unter [Eigene E-Mail-Benachrichtigungen ändern](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  >[!NOTE]
  >
  >Benachrichtigungen auf Benutzerebene enthalten auch [!DNL Workfront Goals]. Der [!DNL Workfront] oder Gruppenadministrator kann jedoch keine Benachrichtigungen für [!DNL Workfront Goals] konfigurieren. Jeder Benutzer muss in seinem Profil seine eigenen [!DNL Workfront Goals]-Benachrichtigungen konfigurieren. Wenn Sie Zugriff auf die Bearbeitung von Benutzern haben, können Sie diese Benachrichtigungen auch für andere Benutzer ändern. Informationen zum Aktivieren [!DNL Workfront Goals] Benachrichtigungen für Ihr Profil oder andere Benutzer, auf die Sie Zugriff haben, um sie zu bearbeiten, finden Sie unter [Benachrichtigungen: Ziele](../../workfront-basics/using-notifications/notifications-goals.md).

  Weitere Informationen dazu, welche Benachrichtigungen der [!DNL Workfront]-Administrator konfigurieren kann, finden Sie unter [Konfigurieren von Ereignisbenachrichtigungen für alle Personen im System](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). [!DNL Workfront Goals] sind nur in der neuen [!DNL Adobe Workfront] verfügbar.

## Inhalt der Ereignisbenachrichtigung

Eine Ereignis-Benachrichtigungs-E-Mail enthält Informationen zum stattgefundenen Ereignis sowie einen Link zu [!DNL Workfront], in dem Sie das Ereignis im System sehen können. Weitere Informationen zum Empfang von E-Mail-Benachrichtigungen finden Sie unter [[!DNL Adobe Workfront] Benachrichtigungen](../../workfront-basics/using-notifications/wf-notifications.md).

Ein [!DNL Workfront] kann den Inhalt der E-Mail-Benachrichtigungen nicht ändern, da sie von [!DNL Workfront] konfiguriert werden. Sie können jedoch die Betreffzeilen von Ereignis-E-Mails ändern. Weitere Informationen finden Sie unter [Anpassen von E-Mail-Betreffen für Ereignisbenachrichtigungen](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

Eine Liste aller [!DNL Workfront] Ereignisbenachrichtigungen mit einer kurzen Beschreibung der einzelnen Ereignisse und ob sie standardmäßig aktiv oder inaktiv sind, finden Sie unter [Ereignisbenachrichtigungen verfügbar in [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
