---
content-type: overview;reference
navigation-topic: notifications
title: Benachrichtigungen - Übersicht
description: Adobe Workfront sendet E-Mail-Benachrichtigungen, In-App-Benachrichtigungen und Benachrichtigungen auf Ihrem Mobilgerät.
author: Lisa
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: 6d2144732e5f47b670c2281d042a2dc950a2928f
workflow-type: tm+mt
source-wordcount: '1395'
ht-degree: 1%

---

# Benachrichtigungen - Übersicht

<!--Audited: 12/2023-->

[!DNL Adobe Workfront] sendet E-Mail-Benachrichtigungen, In-App-Benachrichtigungen und Benachrichtigungen auf Ihrem Mobilgerät.

## E-Mail-Benachrichtigungen

[!DNL Workfront] sendet E-Mail-Benachrichtigungen, um Benutzende über Aktivitäten in Workfront zu informieren und nützliche Informationen und Links bereitzustellen.

Informationen zum Ändern der Voreinstellungen für Ihre E-Mail-Benachrichtigungen finden Sie unter [Ändern Ihrer eigenen E-Mail-Benachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Wenn Sie E-Mail-Benachrichtigungen von der Sandbox-Umgebung erhalten möchten, müssen Sie E-Mails aus Ihrem Benutzerprofil in dieser Umgebung aktivieren.

Sie können die folgenden E-Mail-Benachrichtigungen von [!DNL Workfront] erhalten:

* [Ereignisbenachrichtigungen](#event-notifications)
* [Tägliche Digest-Benachrichtigungen](#daily-digest-notifications)
* [Benachrichtigung über gepostete Kommentare](#notification-of-posted-comments)
* [Automatische Erinnerungen](#automatic-reminders)
* [Erinnerungsbenachrichtigungen](#reminder-notifications)
* [Pinnwand-Benachrichtigungen](#boards-notifications)
* [Other [!DNL Workfront] Emails](#other-workfront-emails)

### Ereignisbenachrichtigungen

Ereignisbenachrichtigungen werden in der Regel durch bestimmte vordefinierte Ereignisse ausgelöst, z. B. wenn Ihnen eine Aufgabe zugewiesen ist oder Sie eine Antwort auf einen von Ihnen abgegebenen Kommentar erhalten.

Nachdem Ereignisbenachrichtigungen in Ihrem [!DNL Workfront] von Ihrem [!DNL Workfront] oder Gruppenadministrator aktiviert wurden, können Sie auswählen, welche Benachrichtigungen Sie erhalten möchten, indem Sie Ihre [!UICONTROL Benachrichtigungen] in Ihrem Benutzerprofil bearbeiten. Sie können auch auswählen, ob Sie Benachrichtigungen über Ereignisse erhalten möchten oder ob Sie Ereignisse erhalten möchten, die in einer täglichen Digest-E-Mail zusammengefasst werden.

Je nachdem, wie der [!DNL Workfront]-Administrator Ereignisbenachrichtigungen für Ihr [!DNL Workfront] konfiguriert hat, wird in Ihren Einstellungen möglicherweise nur eine Teilmenge dieser Benachrichtigungen angezeigt. Weitere Informationen finden Sie unter [Konfigurieren von Ereignisbenachrichtigungen für alle Personen im System](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Der Standardstatus zeigt an, welche Benachrichtigungen (täglich, sofort oder beides) bei der Erstellung von neuen Benutzern standardmäßig für neue Benutzer aktiviert sind.

Eine vollständige Liste der Ereignisbenachrichtigungen und Informationen darüber, wie sie auf System-, Gruppen- oder Benutzerebene aktiviert und konfiguriert werden, finden Sie unter [Ereignisbenachrichtigungen verfügbar in [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Informationen zum Auswählen der Ereignisbenachrichtigungen, die Sie erhalten möchten, finden Sie unter [Ändern Ihrer eigenen E-Mail-Benachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Ereignisbenachrichtigungen sind die einzigen Benachrichtigungen, die konfiguriert werden können, um in täglichen Digest-Aktualisierungen gesendet zu werden.

### Tägliche Digest-Benachrichtigungen

Eine Daily Digest -Benachrichtigung ist eine E-Mail mit allen Benachrichtigungen eines bestimmten Typs, die Sie in den 24 Stunden vor der E-Mail erhalten haben.

Eine vollständige Liste der E-Mail-Benachrichtigungen, die für einen täglichen Digest-E-Mail-Versand aktiviert wurden, sowie Informationen zu allen Kategorien für E-Mail-Benachrichtigungen finden Sie unter [Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications).

>[!NOTE]
>
>[!UICONTROL Workfront] sendet keine täglichen Digest-Benachrichtigungen für die [!UICONTROL Verschiedene] und [!DNL Goals] Ereigniskategorien. Sie können die täglichen Benachrichtigungen für diese Kategorien nicht deaktivieren.

Es gibt mehrere Dinge, die Sie beachten sollten, wenn Sie tägliche Digest-Benachrichtigungen erhalten:

* Jeder [!UICONTROL Benachrichtigungs]-Abschnitt in Ihrem Bedienfeld **[!UICONTROL Meine Einstellungen]** generiert eine eigene tägliche Digest-E-Mail. Täglich können so viele Digest-E-Mails wie Benachrichtigungseinstellungen verwendet werden, die für Daily Digest-E-Mails aktiviert sind.\
   Wenn Sie beispielsweise ausgewählt haben, eine E-Mail mit einer täglichen Zusammenfassung für mehrere Aktionen unter **[!UICONTROL Informationen zu Projekten, deren Inhaber ich bin] zu erhalten,** erhalten Sie eine E-Mail-Benachrichtigung, in der alle für diesen Bereich getroffenen Ereignisse aufgelistet sind.

* Benachrichtigungen in einer täglichen Digest-E-Mail sind nach verschiedenen Kriterien gruppiert. Beispiel: Bei &quot;**[!UICONTROL über Projekte in meinem Besitz]** werden die Ereignisse nach Projektname gruppiert.

  Für die Kategorie **[!UICONTROL Kommunikation]** werden die Benachrichtigungen nach dem Objekt gruppiert, an dem die Kommunikation stattgefunden hat.

  >[!NOTE]
  >
  >Für die Kategorie Kommunikation können Sie einzelne Benachrichtigungen nur für den sofortigen Versand auswählen. Um Benachrichtigungen in einer täglichen Zusammenfassung bereitzustellen, müssen Sie alle auswählen.

* Die Daily Digest -E-Mail listet Ereignisse auf, die innerhalb der letzten 24 Stunden vor der gewählten Versandzeit für die Aktionen in einem bestimmten Bereich aufgetreten sind (z **B. Informationen zu Projekten, deren** ich besitze).
* Die Zeitzone der für den täglichen Digest-Versand ausgewählten Zeit entspricht Ihrer Zeitzone, wie in Ihrem Browser konfiguriert.
* Die Daily Digest -E-Mails enthalten den Namen des Abschnitts in der Betreffzeile sowie das Datum, an dem sie zugestellt werden.
* Mindestens ein Ereignis muss eine Benachrichtigung per Trigger senden, damit der tägliche Digest bereitgestellt werden kann. Tägliche Auszüge werden nicht gesendet, wenn keine Ereignisse für Tägliche Auszüge -E-Mails markiert sind.

### Benachrichtigung über gepostete Kommentare

Die Benachrichtigungen in der Kategorie [!UICONTROL Kommunikation] warnen Sie vor Kommentaren, die im [!UICONTROL Update]-Stream eines bestimmten Elements veröffentlicht wurden.

Für alle verfügbaren Benachrichtigungen werden tägliche Digest[!UICONTROL E-Mails für die &#x200B;] „Kommunikation“ ausgewählt.

Die Informationen werden für das Objekt zusammengefasst, in dem die Kommunikation stattgefunden hat, und für jedes Objekt wird eine Gesamtzahl von Kommunikationsnachrichten angezeigt.

So antworten Sie auf den Kommentar oder zeigen ihn in Workfront an:

1. Klicken Sie auf **[!UICONTROL Kommentar]** in der E-Mail.

   Der [!UICONTROL Aktualisierungen] des Objekts wird geöffnet, wobei der spezifische Kommentar blau dargestellt wird.

   Es öffnet sich ein Antwortfeld, mit dem Sie auf den Kommentar antworten können.

Weitere Informationen zum Konfigurieren von E-Mail-Benachrichtigungen, einschließlich der Aktivierung täglicher Digest-Benachrichtigungen, finden Sie unter [Anzeigen und Ändern Ihrer E-Mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view-and-modify-your-email-notification-settings)Benachrichtigungseinstellungen in [Ändern Ihrer eigenen E-Mail-Benachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Automatische Erinnerungen

Automatische Erinnerungen werden von Ihrem [!DNL Workfront] Admin aktiviert, um Sie über Aufgaben und Probleme zu informieren, die fällig oder verspätet sind oder sich dem geplanten Abschlussdatum nähern. Bei verspäteten Benachrichtigungen wird die E-Mail jede Nacht gesendet, bis die Aufgabe oder das Problem abgeschlossen ist. Nachdem der Administrator diese konfiguriert hat, können Sie sie nicht mehr deaktivieren. Außerdem können Sie weder den Inhalt noch die Betreffzeile einer E-Mail ändern, die durch eine automatische Erinnerung ausgelöst wird.

Sie können an eine oder mehrere der folgenden Personen gesendet werden:

* Die einer Aufgabe oder einem Problem zugewiesenen Benutzer
* Der unmittelbare Manager des Benutzers
* Der Manager des direkten Managers

Automatische Erinnerungs-E-Mails werden von der E-Mail-Adresse gesendet, die Ihr [!DNL Workfront] für die Verarbeitung ausgehender E-Mails ausgewählt hat.

Je nachdem, welche automatische Erinnerung aktiviert ist, sind die folgenden Arten von Informationen in der E-Mail mit der automatischen Erinnerung verfügbar:

* Das Datum, an dem die Aufgabe oder das Problem erstellt wurde
* Name der Aufgabe oder des Problems
* Der Name des Projekts, in dem sich die Aufgabe oder das Problem befindet
* Beschreibung der Aufgabe oder des Problems
* Eine Liste der Benutzer, die der Aufgabe oder dem Problem zugewiesen sind
* Der Name des Benutzers, der die Aufgabe oder das Problem eingegeben hat
* Die Priorität der Aufgabe oder des Problems
* Datum, an dem die Aufgabe oder das Problem überfällig wurde

Informationen zum Aktivieren automatischer Erinnerungen finden Sie unter [Einrichten automatischer Erinnerungen](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

### Erinnerungsbenachrichtigungen

Ein [!DNL Workfront] (oder ein Benutzer mit [!UICONTROL &#x200B; Zugriffsebene „Planer] und administrativem Zugriff auf Erinnerungsbenachrichtigungen) kann Erinnerungsbenachrichtigungen über bald ablaufende Fristen entwerfen und manuell mit Projekten, Aufgaben, Problemen und Arbeitszeittabellen verknüpfen.

>[!IMPORTANT]
>
>Wenn sich die Frist ändert, nachdem ein Benutzer eine Erinnerungsnachricht für eines der oben genannten Objekte erhalten hat, erhält er keine weitere Erinnerungsnachricht.

Erinnerungsbenachrichtigungen werden von der E-Mail-Adresse gesendet, die der [!DNL Workfront]-Administrator für die Verarbeitung ausgehender E-Mails ausgewählt hat.

Informationen zum Einrichten und Aktivieren von Erinnerungsbenachrichtigungen finden Sie unter [Einrichten von Erinnerungsbenachrichtigungen](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).

Informationen dazu, wie Sie den erforderlichen Administratorzugriff erhalten, finden Sie unter [Gewähren von Administratorzugriff für bestimmte Bereiche](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

### Pinnwand-Benachrichtigungen

[!DNL Adobe Workfront] [!UICONTROL Pinnwände] sendet Ihnen eine E-Mail, wenn Sie zu einer Pinnwand hinzugefügt werden und wenn Ihnen eine Karte zugewiesen wird. Sie können in den Voreinstellungen für Pinnwände auswählen, welche E-Mails Sie erhalten möchten.

Weitere Informationen finden Sie unter [Pinnwände - E-Mail-Benachrichtigungen und -Voreinstellungen](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

### Andere [!DNL Workfront] E-Mails

Es gibt weitere E-Mails, die Sie möglicherweise von [!DNL Workfront] erhalten, die nicht konfiguriert werden können.

Die folgenden E-Mails werden von [!DNL Workfront] automatisch gesendet, wenn diese Bedingungen erfüllt sind:

* Element wiederherstellen: Wenn der [!DNL Workfront] ein Objekt aus dem [!UICONTROL Papierkorb] wiederherstellt, wird eine E-Mail an den [!DNL Workfront] gesendet.
* Fehler beim Wiederherstellen: Wenn der [!DNL Workfront] versucht, ein Objekt aus dem Papierkorb wiederherzustellen und die Wiederherstellung fehlschlägt, wird eine E-Mail an den [!DNL Workfront] gesendet.

Die folgenden E-Mails können nur auf Benutzerprofilebene konfiguriert werden. Sie können nicht auf Systemebene aktiviert oder deaktiviert werden:

* Abschluss einer persönlichen Aufgabe: Wenn eine persönliche Aufgabe, die Sie einer anderen Person zugewiesen haben, abgeschlossen ist, erhalten Sie eine E-Mail.
* Kommentar hinzugefügt zu Benutzer: Wenn jemand einen Kommentar zu Ihrem Benutzerprofil abgibt, erhalten Sie eine E-Mail.

## In-App-Benachrichtigungen

Sie können Benachrichtigungen innerhalb der [!DNL Workfront]-Web-Anwendung erhalten, wenn bestimmte Ereignisse eintreten.

Weitere Informationen zu In-App-Benachrichtigungen finden Sie unter [Anzeigen und Verwalten von In-App-Benachrichtigungen](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## E-Mail-Benachrichtigungen in der Mobile App

Sie können [!DNL Workfront] E-Mail-Benachrichtigungen in Ihrer mobilen E-Mail-App auf Ihrem Mobilgerät erhalten.

Wenn die [!DNL Workfront] Mobile App auf Ihrem Mobiltelefon installiert ist, werden sie durch Tippen auf die Links in der E-Mail in der [!DNL Workfront] Mobile App geöffnet. Dazu gehört das Tippen auf eine der folgenden Aktionsschaltflächen:

* [!UICONTROL Bearbeiten Sie es]
* [!UICONTROL Kommentar]
* [!UICONTROL Genehmigungsentscheidung treffen]
* [!UICONTROL Alle Benachrichtigungen anzeigen]
* [!UICONTROL Hinzufügen]
* [!UICONTROL Erste Schritte]
* [!UICONTROL Weitere Details anzeigen]

Weitere Informationen zur [!DNL Workfront] Mobile App finden Sie unter [Verwenden der  [!DNL Adobe Workfront]  Mobile App](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).
