---
content-type: overview;reference
navigation-topic: notifications
title: Benachrichtigungsübersicht
description: Adobe Workfront sendet E-Mail-Benachrichtigungen, In-App-Benachrichtigungen und Benachrichtigungen auf Ihrem Mobilgerät.
author: Lisa
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: 6d2144732e5f47b670c2281d042a2dc950a2928f
workflow-type: tm+mt
source-wordcount: '1395'
ht-degree: 0%

---

# Benachrichtigungsübersicht

<!--Audited: 12/2023-->

[!DNL Adobe Workfront] sendet E-Mail-Benachrichtigungen, In-App-Benachrichtigungen und Benachrichtigungen auf Ihrem Mobilgerät.

## E-Mail-Benachrichtigungen

[!DNL Workfront] sendet E-Mail-Benachrichtigungen, um Benutzer über Aktivitäten in Workfront zu warnen, und stellt nützliche Informationen und Links bereit.

Informationen zum Ändern der Voreinstellungen für Ihre E-Mail-Benachrichtigungen finden Sie unter [Ihre eigenen E-Mail-Benachrichtigungen ändern](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Wenn Sie E-Mail-Benachrichtigungen von der Sandbox-Umgebung erhalten möchten, müssen Sie E-Mails aus Ihrem Benutzerprofil in dieser Umgebung aktivieren.

Sie können die folgenden E-Mail-Benachrichtigungen von [!DNL Workfront]:

* [Ereignisbenachrichtigungen](#event-notifications)
* [Tägliche Digest-Benachrichtigungen](#daily-digest-notifications)
* [Mitteilung geposteter Kommentare](#notification-of-posted-comments)
* [Automatische Erinnerungen](#automatic-reminders)
* [Erinnerungsbenachrichtigungen](#reminder-notifications)
* [Pinnwandbenachrichtigungen](#boards-notifications)
* [Sonstiges [!DNL Workfront] E-Mail](#other-workfront-emails)

### Ereignisbenachrichtigungen

Ereignisbenachrichtigungen werden in der Regel durch bestimmte vordefinierte Ereignisse ausgelöst, z. B. durch Zuweisung einer Aufgabe an Sie oder durch Erhalten einer Antwort auf einen Kommentar.

Nach der Aktivierung von Ereignisbenachrichtigungen in Ihrer [!DNL Workfront] System von [!DNL Workfront] Administrator oder Gruppenadministrator können Sie auswählen, welche Sie erhalten möchten, indem Sie Ihre [!UICONTROL Benachrichtigungen] Voreinstellungen in Ihrem Benutzerprofil. Sie können auch auswählen, ob Sie Benachrichtigungen bei Ereignissen erhalten möchten oder ob Sie Ereignisse in einer täglichen Digest-E-Mail erhalten möchten.

Je nachdem, wie die [!DNL Workfront] -Administrator hat Ereignisbenachrichtigungen für Ihre [!DNL Workfront] System. Weitere Informationen finden Sie unter [Ereignisbenachrichtigungen für alle Benutzer im System konfigurieren](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Der Standardstatus zeigt an, welche Benachrichtigungen (täglich, unmittelbar oder beides) standardmäßig für neue Benutzer aktiviert sind, wenn Sie die neuen Benutzer erstellen.

Eine vollständige Liste der Ereignisbenachrichtigungen sowie Informationen darüber, wie sie auf System-, Gruppen- oder Benutzerebene aktiviert und konfiguriert werden, finden Sie unter [Verfügbare Ereignisbenachrichtigungen [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Informationen dazu, wie Sie auswählen, welche Ereignisbenachrichtigungen Sie erhalten möchten, finden Sie unter [Ihre eigenen E-Mail-Benachrichtigungen ändern](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Ereignisbenachrichtigungen sind die einzigen Benachrichtigungen, die für die Bereitstellung in täglichen Digest-Updates konfiguriert werden können.

### Tägliche Digest-Benachrichtigungen

Eine tägliche Digest-Benachrichtigung ist eine E-Mail, die alle Benachrichtigungen eines bestimmten Typs enthält, die Sie in den 24 Stunden vor der E-Mail erhalten haben.

Eine vollständige Liste der für einen täglichen Digest-E-Mail-Versand aktivierten E-Mail-Benachrichtigungen sowie Informationen zu allen Kategorien für E-Mail-Benachrichtigungen finden Sie unter [Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications).

>[!NOTE]
>
>[!UICONTROL Workfront] sendet keine täglichen Digest-Benachrichtigungen für die [!UICONTROL Sonstiges] und [!DNL Goals] Ereigniskategorien. Sie können die täglichen Benachrichtigungen für diese Kategorien nicht deaktivieren.

Beim Empfang täglicher Digest-Benachrichtigungen müssen Sie auf verschiedene Punkte achten:

* Jeder [!UICONTROL Benachrichtigungen] im Abschnitt **[!UICONTROL Meine Einstellungen]** erzeugt eine eigene tägliche Digest-E-Mail. Sie können täglich so viele Digest-E-Mails haben wie Benachrichtigungseinstellungen, die für tägliche Digest-E-Mails aktiviert sind.\
   Wenn Sie beispielsweise ausgewählt haben, eine tägliche Digest-E-Mail für mehrere Aktionen unter dem **[!UICONTROL Informationen über Projekte I] Eigene** Sie erhalten eine E-Mail-Benachrichtigung, in der alle für diesen Bereich durchgeführten Ereignisse aufgelistet werden.

* Benachrichtigungen in einer täglichen Digest-E-Mail sind nach verschiedenen Kriterien gruppiert. Beispiel: im Fall von **[!UICONTROL Informationen zu eigenen Projekten]** festgelegt ist, werden die Ereignisse nach dem Projektnamen gruppiert.

  Für **[!UICONTROL Kommunikation]** -Kategorie, werden die Benachrichtigungen nach dem Objekt gruppiert, an dem die Kommunikation stattgefunden hat.

  >[!NOTE]
  >
  >In der Kategorie Kommunikation können Sie einzelne Benachrichtigungen nur für den sofortigen Versand auswählen. Damit Benachrichtigungen täglich versendet werden können, müssen Sie alle Benachrichtigungen auswählen.

* Die tägliche Digest-E-Mail listet Ereignisse auf, die für Aktionen in einem bestimmten Bereich aufgetreten sind (z. B. **Angaben zu eigenen Projekten**) innerhalb von 24 Stunden vor der für die Auslieferung ausgewählten Zeit.
* Die Zeitzone für den täglichen Digest-Versand stimmt mit Ihrer Zeitzone überein, wie sie in Ihrem Browser konfiguriert ist.
* Die täglichen Digest-E-Mails haben den Namen des Abschnitts in der Betreffzeile sowie das Datum, an dem sie zugestellt werden.
* Mindestens ein Ereignis muss eine Benachrichtigung Trigger haben, damit die tägliche Zusammenfassung bereitgestellt werden kann. Tägliche Digest-Benachrichtigungen werden nicht gesendet, wenn keine für tägliche Digest-E-Mails markierten Ereignisse eintreten.

### Mitteilung geposteter Kommentare

Die Benachrichtigungen in der [!UICONTROL Kommunikation] Kategoriewarnung für Kommentare, die in der [!UICONTROL Aktualisieren] Stream eines bestimmten Elements.

Tägliche Digest-E-Mails für die [!UICONTROL Kommunikation] für alle verfügbaren Benachrichtigungen ausgewählt werden.

Die Informationen werden für das Objekt zusammengefasst, an dem die Kommunikation stattgefunden hat, und für jedes Objekt wird eine Gesamtzahl an Kommunikationsnachrichten angezeigt.

So beantworten Sie den Kommentar oder zeigen ihn in Workfront an:

1. Klicken Sie auf **[!UICONTROL Kommentar]** in der E-Mail.

   Die [!UICONTROL Updates] -Bereich des Objekts geöffnet, wobei der spezifische Kommentar blau dargestellt wird.

   Ein Antwortfeld ist geöffnet, mit dem Sie auf den Kommentar antworten können.

Weitere Informationen zum Konfigurieren von E-Mail-Benachrichtigungen, einschließlich der Aktivierung täglicher Digest-Benachrichtigungen, finden Sie unter [E-Mail-Benachrichtigungseinstellungen anzeigen und ändern](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view-and-modify-your-email-notification-settings) in [Ihre eigenen E-Mail-Benachrichtigungen ändern](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Automatische Erinnerungen

Automatische Erinnerungen werden durch Ihre [!DNL Workfront] Administrator , um Sie über Aufgaben und Probleme zu informieren, die fällig, spät oder in der Nähe des geplanten Fertigstellungsdatums sind. Bei verspäteten Benachrichtigungen wird die E-Mail nächtlich gesendet, bis die Aufgabe oder das Problem abgeschlossen ist. Nachdem der Administrator diese Konfigurationen vorgenommen hat, können Sie sie nicht mehr deaktivieren. Außerdem können Sie den Inhalt oder die Betreffzeile einer E-Mail, die durch eine automatische Erinnerung ausgelöst wird, nicht ändern.

Sie können an eine oder mehrere der folgenden Adressen gesendet werden:

* Benutzer, die einer Aufgabe oder einem Problem zugewiesen sind
* Der sofortige Manager des Benutzers
* Der Manager des unmittelbaren Geschäftsführers

Automatische Erinnerungsnachrichten werden von der E-Mail-Adresse gesendet, die Ihre [!DNL Workfront] Administrator ausgewählt, um ausgehende E-Mails zu verarbeiten.

Je nachdem, welche automatische Erinnerung aktiviert ist, stehen in der automatischen Erinnerungsemail die folgenden Informationen zur Verfügung:

* Das Datum der Erstellung der Aufgabe oder des Problems
* Aufgaben- oder Problemname
* Der Name des Projekts, in dem sich die Aufgabe oder das Problem befindet
* Beschreibung der Aufgabe oder des Problems
* Eine Liste der der Aufgabe oder dem Problem zugewiesenen Benutzer
* Der Name des Benutzers, der die Aufgabe oder das Problem eingegeben hat
* Die Priorität der Aufgabe oder des Problems
* Datum, an dem die Aufgabe oder das Problem überfällig wurde

Informationen zum Aktivieren automatischer Erinnerungen finden Sie unter [Automatische Erinnerungen einrichten](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

### Erinnerungsbenachrichtigungen

A [!DNL Workfront] Administrator (oder ein Benutzer mit [!UICONTROL Planen] Zugriffsstufe und administrativer Zugriff auf Erinnerungsbenachrichtigungen) können Erinnerungsbenachrichtigungen über nahende Termine erstellen und sie manuell mit Projekten, Aufgaben, Problemen und Zeitesheets verknüpfen.

>[!IMPORTANT]
>
>Wenn sich der Termin ändert, nachdem ein Benutzer eine Erinnerungsbenachrichtigung für eines der oben genannten Objekte erhält, erhält der Benutzer keine weitere Erinnerungsbenachrichtigung.

Erinnerungsbenachrichtigungen werden von der E-Mail-Adresse gesendet, die die [!DNL Workfront] Administrator ausgewählt, um ausgehende E-Mails zu verarbeiten.

Informationen zum Einrichten und Aktivieren von Erinnerungsbenachrichtigungen finden Sie unter [Einrichten von Erinnerungsbenachrichtigungen](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).

Informationen dazu, wie Sie den erforderlichen Administratorzugriff erhalten können, finden Sie unter [Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

### Pinnwandbenachrichtigungen

[!DNL Adobe Workfront] [!UICONTROL Pinnwände] sendet Ihnen eine E-Mail, wenn Sie einer Pinnwand hinzugefügt werden und wenn Ihnen eine Karte zugewiesen ist. In den Vorlieben Ihrer Pinnwände können Sie auswählen, welche E-Mails Sie erhalten möchten.

Weitere Informationen finden Sie unter [E-Mail-Benachrichtigungen und Voreinstellungen in Foren](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

### Sonstiges [!DNL Workfront] E-Mail

Es gibt weitere E-Mails, die Sie möglicherweise von erhalten [!DNL Workfront] die nicht konfiguriert werden können.

Die folgenden E-Mails werden automatisch von [!DNL Workfront] wenn diese Bedingungen erfüllt sind:

* Wiederherstellen eines Elements: Wenn das [!DNL Workfront] administrator stellt ein Objekt aus dem [!UICONTROL Recycle] Container, eine E-Mail an die [!DNL Workfront] Administrator.
* Fehlgeschlagene Wiederherstellung: Wenn die Variable [!DNL Workfront] Der Administrator versucht, ein Objekt aus dem Papierkorb wiederherzustellen. Wenn die Wiederherstellung fehlschlägt, wird eine E-Mail an die [!DNL Workfront] Administrator.

Die folgenden E-Mails können nur auf Benutzerprofilebene konfiguriert werden. Sie können nicht auf Systemebene aktiviert oder deaktiviert werden:

* Abschluss der persönlichen Aufgabe: Wenn eine persönliche Aufgabe, die Sie einer anderen Person zugewiesen haben, abgeschlossen ist, erhalten Sie eine E-Mail.
* Kommentar zum Benutzer hinzugefügt: Wenn jemand zu Ihrem Benutzerprofil einen Kommentar abgibt, erhalten Sie eine E-Mail.

## In-App-Benachrichtigungen

Sie können Benachrichtigungen in der [!DNL Workfront] Webanwendung, wenn bestimmte Ereignisse auftreten.

Weitere Informationen zu In-App-Benachrichtigungen finden Sie unter [Anzeigen und Verwalten von In-App-Benachrichtigungen](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## E-Mail-Benachrichtigungen in der mobilen E-Mail-App

Sie können [!DNL Workfront] E-Mail-Benachrichtigungen in Ihrer mobilen E-Mail-App auf Ihrem Mobilgerät.

Wenn Sie [!DNL Workfront] Die auf Ihrem Telefon installierte Mobile App öffnet sie durch Tippen auf die Links in der E-Mail im [!DNL Workfront] Mobile App. Dazu gehört das Tippen auf eine der folgenden Aktionsschaltflächen:

* [!UICONTROL Arbeiten daran]
* [!UICONTROL Kommentar]
* [!UICONTROL Genehmigungsentscheidung treffen]
* [!UICONTROL Alle Benachrichtigungen anzeigen]
* [!UICONTROL Hinzufügen]
* [!UICONTROL Erste Schritte]
* [!UICONTROL Siehe Weitere Details .]

Weitere Informationen zum [!DNL Workfront] Mobile App, siehe [Verwenden Sie die [!DNL Adobe Workfront] mobile App](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).
