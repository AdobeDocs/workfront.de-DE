---
content-type: overview
navigation-topic: notifications
title: Ereignisbenachrichtigungen
description: Ereignisbenachrichtigungen sind E-Mails, die von verschiedenen Ereignistypen für Objekte wie Projekte, Aufgaben oder Probleme ausgelöst werden. Sie werden gesendet, wenn im Projekt etwas passiert, von dem andere wissen müssen. Je nach Ereignis erhalten Benutzer sofortige, tägliche oder sowohl sofortige als auch tägliche E-Mail-Benachrichtigungen darüber.
author: Courtney
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: c79d030ff2d05487e5f7e3457bf98df591822a80
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Ereignisbenachrichtigungen

<!-- Audited: 4/2025 -->

Ereignisbenachrichtigungen sind E-Mails, die von verschiedenen Ereignistypen für Objekte wie Projekte, Aufgaben oder Probleme ausgelöst werden. Sie werden gesendet, wenn im Projekt etwas passiert, von dem andere wissen müssen. Je nach Ereignis erhalten Benutzer sofortige, tägliche oder sowohl sofortige als auch tägliche E-Mail-Benachrichtigungen darüber.

>[!NOTE]
>
>Ereignisbenachrichtigungen sind eine von mehreren Arten von [!DNL Adobe Workfront]. Informationen zu allen [!DNL Workfront] Benachrichtigungstypen finden Sie unter [Benachrichtigungen - Übersicht](../../workfront-basics/using-notifications/wf-notifications.md).

## Konfigurieren von Ereignisbenachrichtigungen

Ereignisbenachrichtigungs-E-Mails können auf den folgenden Ebenen konfiguriert werden:

* **Systemebene**: Ein [!DNL Workfront]-Administrator kann Ereignisbenachrichtigungen auf Systemebene aktivieren und deaktivieren, wie in [Konfigurieren von Ereignisbenachrichtigungen für alle Personen im System](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md) beschrieben.

  Alle Gruppen erben standardmäßig Systembenachrichtigungen, Gruppenadministratoren können jedoch möglicherweise einige Konfigurationen auf Gruppenebene ändern, wenn dies vom [!DNL Workfront]-Administrator genehmigt wurde.

* **Gruppenebene** Ein Gruppenadministrator kann eine Ereignisbenachrichtigung für von ihm verwaltete Gruppen konfigurieren, nachdem ein [!DNL Workfront] diese Funktion für Gruppen freigegeben hat. Wenn es Gruppen oberhalb der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für [!DNL Workfront] Administratoren (für jede Gruppe). Weitere Informationen finden Sie unter [Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

* **Benutzerebene**: Alle Ereignisbenachrichtigungen, die systemweit aktiviert sind, werden im Abschnitt [!UICONTROL Benachrichtigungen] jedes Benutzers in seinem individuellen Profil aufgelistet. Dort können Benutzer ihre individuellen Ereignisbenachrichtigungen aktivieren und deaktivieren.

  [!DNL Workfront] und Benutzer mit Zugriff auf die Bearbeitung anderer Benutzer können Benachrichtigungen auch im Profil einzelner Benutzer aktivieren und deaktivieren.

  Weitere Informationen finden Sie unter [Eigene E-Mail-Benachrichtigungen ändern](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  >[!NOTE]
  >
  >Benachrichtigungen auf Benutzerebene enthalten auch [!DNL Workfront Goals]. Der [!DNL Workfront] oder Gruppenadministrator kann jedoch keine Benachrichtigungen für [!DNL Workfront Goals] konfigurieren. Jeder Benutzer muss in seinem Profil seine eigenen [!DNL Workfront Goals]-Benachrichtigungen konfigurieren. Wenn Sie Zugriff auf die Bearbeitung von Benutzern haben, können Sie diese Benachrichtigungen auch für andere Benutzer ändern. Informationen zum Aktivieren [!DNL Workfront Goals] Benachrichtigungen für Ihr Profil oder andere Benutzer, auf die Sie Zugriff haben, um sie zu bearbeiten, finden Sie unter [Benachrichtigungen: Ziele](../../workfront-basics/using-notifications/notifications-goals.md).

  Weitere Informationen dazu, welche Benachrichtigungen der [!DNL Workfront]-Administrator konfigurieren kann, finden Sie unter [Konfigurieren von Ereignisbenachrichtigungen für alle Personen im System](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

## Inhalt der Ereignisbenachrichtigung

Eine Ereignis-Benachrichtigungs-E-Mail enthält Informationen zum stattgefundenen Ereignis sowie einen Link zu [!DNL Workfront], in dem Sie das Ereignis im System sehen können. Weitere Informationen zum Empfang von E-Mail-Benachrichtigungen finden Sie unter [Benachrichtigungen - Übersicht](../../workfront-basics/using-notifications/wf-notifications.md).

Ein [!DNL Workfront]-Administrator kann den Inhalt einer E-Mail-Benachrichtigung nicht ändern, da er von [!DNL Workfront] konfiguriert wurde. Er kann jedoch die Betreffzeilen der E-Mail-Benachrichtigung für Ereignisse ändern. Weitere Informationen finden Sie unter [Anpassen von E-Mail-Betreffen für Ereignisbenachrichtigungen](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

Eine Liste aller [!DNL Workfront] Ereignisbenachrichtigungen mit einer kurzen Beschreibung der einzelnen Ereignisse und ob sie standardmäßig aktiv oder inaktiv sind, finden Sie unter [Ereignistypen](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
