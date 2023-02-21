---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Zugriff [!DNL Adobe Workfront] von [!DNL Slack]
description: Integration [!DNL Adobe Workfront] mit [!DNL Slack] ermöglicht Ihnen den Zugriff auf [!DNL Workfront] von Slack aus oder führen bestimmte Aktionen in [!DNL Workfront] mit einem Schrägstrich. Die Integration kann von jedem [!DNL Slack] Umgebung, einschließlich [!DNL Slack] mobile App.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '1075'
ht-degree: 1%

---

# Zugriff [!DNL Adobe Workfront] von [!DNL Slack]

Integration [!DNL Adobe Workfront] mit [!DNL Slack] ermöglicht Ihnen den Zugriff auf [!DNL Workfront] von [!DNL Slack]oder bestimmte Aktionen in [!DNL Workfront] mit einem Schrägstrich. Die Integration kann von jedem [!DNL Slack] Umgebung, einschließlich [!DNL Slack] mobile App.

Sie oder Ihr [!DNL Slack] -Administrator muss die [!DNL Workfront] App in Ihrer [!DNL Slack] -Instanz, bevor Sie [!DNL Workfront] von [!DNL Slack]. Weitere Informationen finden Sie unter [Adobe Workfront für Slack konfigurieren](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Über Schrägstrich-Befehle {#about-slash-commands}

Bei Verwendung von [!DNL Slack], geben Sie Nachrichten in ein Meldungsfeld ein. Wenn Sie Ihre Nachricht mit einem Schrägstrich beginnen, wird sie zu einem Befehl und verhält sich anders als eine einfache Nachricht. Der Befehl gibt [!DNL Slack] , um eine Aktion durchzuführen.

Sie können auf Ihre [!DNL Workfront] Instanz von [!DNL Slack] durch Eingabe eines Schrägstrich-Befehls in eine beliebige [!DNL Slack] -Kanal.

Beachten Sie Folgendes bei Verwendung eines Schrägstrich-Befehls in [!DNL Slack] für den Zugriff [!DNL Workfront]:

* Bei Schrägstrichbefehlen wird zwischen Groß- und Kleinschreibung unterschieden.
* Die Befehle für [!DNL Workfront] sind nur für Sie sichtbar, unabhängig davon, in welchem Kanal Sie sie eingeben.
* Der Befehl sollte immer mit `/workfront` oder `/wf`, gefolgt von einem Leerzeichen und dem Namen einer Aktion, die Sie ausführen möchten [!DNL Workfront].

   Dies bedeutet, dass Ihr Befehl für die [!DNL Workfront] App. Die Befehle für [!DNL Workfront] funktioniert nur, wenn Sie die [!DNL Workfront] App mit [!DNL Slack] -Instanz.

Für eine Liste aller Befehle, die Sie von Slack ausführen können. [!DNL Workfront], siehe [Zugriff [!DNL Workfront] von einem Schrägstrich-Befehl in [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack).

## Anmelden bei [!DNL Workfront] von [!DNL Slack] {#log-in-to-workfront-from-slack}

Wenn Sie einen Befehl in das Meldungsfeld in Slack eingeben, werden Sie aufgefordert, sich bei [!DNL Workfront] zuerst.\
Eine vollständige Liste der [!DNL Workfront] Befehle von [!DNL Slack], siehe [Zugriff [!DNL Workfront] von einem Schrägstrich-Befehl in [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack) in diesem Artikel.

So melden Sie sich bei an [!DNL Workfront] von [!DNL Slack]:

1. Melden Sie sich bei Ihrer [!DNL Slack] -Instanz.
1. Geben Sie in einem beliebigen Kanal einen der folgenden Befehle ein:\
   `/workfront log in`

   Oder

   `/wf log in`

1. Klicken Sie auf [!DNL Workfront] **[!UICONTROL Anmelden]** in der Antwort angezeigt.\
   Eine neue Registerkarte mit Feldern für [!DNL Workfront] Anmeldedaten.

1. Befolgen Sie die Anweisungen zum Anmelden bei [!DNL Workfront] unter Verwendung der erweiterten Authentifizierung, OAuth 2.0 oder Ihrer SAML-URL (Security Assertion Markup Language).

   >[!NOTE]
   >
   >* Wenn Sie aufgefordert werden, den Host Ihrer [!DNL Workfront] -Konto angeben, geben Sie es in folgendem Format ein: *yourCompany&#39;sDomain.my.workfront.com*. Die Domäne Ihres Unternehmens ist normalerweise der Name Ihres Unternehmens.
   >* Die erweiterte Authentifizierung ist erst verfügbar, wenn eine [!DNL Workfront] -Administrator aktiviert sie für diese Integration.



   Die Konfigurationsseite für [!DNL Workfront] Benachrichtigungen in [!DNL Slack] geöffnet.

1. (Optional) Deaktivieren Sie alle [!DNL Workfront] Benachrichtigungen, die Sie nicht empfangen möchten [!DNL Slack].

   Informationen zur Konfiguration [!DNL Workfront] Einstellungen für [!DNL Slack], siehe [Einstellungen konfigurieren](#configure-settings-configure-settings) in diesem Artikel

1. Navigieren Sie zurück zu Ihrer [!DNL Slack] -Kanal.

   Sie sind bei angemeldet. [!DNL Workfront] von [!DNL Slack] -Instanz.

## Zugriff [!DNL Workfront] von [!DNL Slack]

* [Über Schrägstrich-Befehle](#about-slash-commands-about-slash-commands)
* [Zugriff [!DNL Workfront] über einen freigegebenen Link in [!DNL Slack]](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## Zugriff [!DNL Workfront] von einem Schrägstrich-Befehl in [!DNL Slack] {#access-workfront-from-a-slash-command-in-slack}

1. Melden Sie sich bei Ihrer [!DNL Slack] -Instanz und melden Sie sich bei [!DNL Workfront] von [!DNL Slack].\
   Weitere Informationen zur Anmeldung bei [!DNL Workfront] von [!DNL Slack], siehe [Anmelden bei [!DNL Workfront] von [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack)

1. Geben Sie von jedem Kanal aus den folgenden Befehl in das Meldungsfeld ein:

   `/workfront help`

   Oder

   `/wf help`

1. Wählen Sie unter den folgenden Befehlen aus:

   * `/wf home`

      Zeigt Schaltflächen an, über die Sie auf Listen Ihrer Aufgaben, Probleme und Genehmigungen zugreifen können. Wenn Sie auf eine der Schaltflächen klicken, werden die ersten 20 Elemente jeder Liste in [!DNL Slack].

      Weitere Informationen zur Verwaltung von [!DNL Workfront] Arbeitselemente aus [!DNL Slack], siehe [Verwalten Sie Ihre Arbeit und Ihre Genehmigungen über [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf add task <TaskName>`

      Fügen Sie den Namen der Aufgabe so ein, wie er im [!DNL Workfront] -Schnittstelle.

      Fügt eine Aufgabe zu [!DNL Workfront].

      Weitere Informationen zum Hinzufügen von Aufgaben zu [!DNL Workfront] aus dem Slack &quot;Erstellen von Aufgaben aus [!DNL Slack]&quot; Abschnitt in [Erstellen von Aufgaben und Problemen aus [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf add issue <Issue Name>`

      Fügen Sie den Namen des Problems so ein, wie es im [!DNL Workfront] -Schnittstelle.

      Fügt ein Problem zu [!DNL Workfront]

      Weitere Informationen zum Hinzufügen von Problemen zu [!DNL Workfront] von [!DNL Slack]finden Sie unter &quot;Erstellen von Problemen aus [!DNL Slack]&quot; Abschnitt in [Erstellen von Aufgaben und Problemen aus [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf favorites`

      Zeigt die Liste Ihrer [!DNL Workfront] Favoriten.

      Weitere Informationen zum Zugriff auf Ihre Favoriten finden Sie unter [!DNL Slack], siehe [Zugriff auf Ihre [!UICONTROL Favoriten] Liste aus [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites) im Abschnitt [Zugriff auf Ihre Favoriten und aktuellen Elemente über [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) Artikel.

   * `/wf recent`

      Zeigt die Liste der zuletzt aufgerufenen Artikel unter [!DNL Workfront].

      Weitere Informationen zum Zugriff auf die neuesten Elemente finden Sie unter [!DNL Slack], siehe [Zugriff auf Ihre [!UICONTROL Letzte Elemente] Liste aus [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites] und [!UICONTROL aktuelle Artikel aus [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) Artikel.

   * `wf tasks`

      Zeigt eine Liste Ihrer Aufgaben an.

      Weitere Informationen zur Verwaltung Ihrer Aufgaben finden Sie unter [!DNL Slack]finden Sie unter &quot;Verwalten Ihrer Aufgaben von [!DNL Slack]&quot; Abschnitt in [Verwalten Ihrer Arbeit und Genehmigungen über [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf issues`

      Zeigt eine Liste Ihrer Probleme an.

      Weitere Informationen zur Verwaltung Ihrer Probleme finden Sie unter [!DNL Slack]finden Sie unter &quot;Verwalten Ihrer Probleme von [!DNL Slack]&quot; Abschnitt in [Verwalten Ihrer Arbeit und Genehmigungen über [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf approvals` Zeigt Ihre [!DNL Workfront] Genehmigungen.\

      Weitere Informationen zur Verwaltung Ihrer Genehmigungen erhalten Sie unter [!DNL Slack]finden Sie unter &quot;Verwalten Ihrer Genehmigungen&quot;von [!DNL Slack]&quot; Abschnitt in [Verwalten Sie Ihre Arbeit und Ihre Genehmigungen über [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf search <keyword>`

      Suchbegriff einschließen.

      Suchen Sie nach einem bestimmten Suchbegriff. Sie können nach den folgenden Typen von Objekten suchen:

      * Projekt
      * Aufgabe
      * Problem
      * Bericht
      * Personen
      * Vorlage
      * Dokument
      * Portfolio
      * Programm
      * Dashboard
      * Firma
      * Notiz  \

         Weitere Informationen zur Suche in [!DNL Slack], siehe [Suchen Sie nach [!DNL Adobe Workfront] Elemente aus dem Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md).
   * `/wf log in`

      Meldet Sie sich bei [!DNL Workfront] von [!DNL Slack].

   * `/wf log out `

      Protokolliert Sie von [!DNL Workfront] von [!DNL Slack]. Sie bleiben bei [!DNL Workfront] wenn Sie über eine separate [!DNL Workfront] -Instanz in einer anderen Browser-Registerkarte in einer anderen Anwendung geöffnet.
   * `/wf settings`

      Ermöglicht Ihnen Zugriff auf die Konfiguration Ihrer [!DNL Workfront] Einstellungen in [!DNL Slack].

      Informationen zur Konfiguration [!DNL Workfront] -Einstellungen in Slack finden Sie unter [Einstellungen konfigurieren](#configure-settings-configure-settings).

   * `/wf help`
Zeigt eine vollständige Liste der Befehle für [!DNL Workfront].


   * `Visit Workfront Help`: Öffnet die [!UICONTROL Slack] im Abschnitt [!DNL Workfront] Hilfe-Site in einem neuen Browser-Tab.


1. (Optional) Um die Nachricht eines Befehls zu löschen, bewegen Sie den Mauszeiger über die rechte obere Ecke der Slack-Nachricht mit dem Befehl und klicken Sie auf &#x200B;**[!UICONTROL Nachrichtenaktionen anzeigen]** Klicken Sie auf **[!UICONTROL Nachricht löschen]**.

1. (Optional und bedingt) Klicken Sie auf **[!UICONTROL Löschen]** um zu bestätigen, dass Sie diese Nachricht löschen möchten.

### Zugriff [!DNL Workfront] über einen freigegebenen Link in [!DNL Slack] {#access-workfront-from-a-shared-link-in-slack}

Sie können [!DNL Workfront] Objekte aus einem Link zu den Objekten, die für Sie in [!DNL Slack].

Weitere Informationen zum Zugriff auf [!DNL Workfront] über einen freigegebenen Link, siehe [Zugriff [!DNL Adobe Workfront] Objekte aus einem freigegebenen Link in [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md).

## Einstellungen konfigurieren {#configure-settings}

1. Innerhalb eines [!DNL Slack] Meldungsfeld, geben Sie den folgenden Befehl ein:

   `/workfront settings`

   Oder

   `/wf settings`

   Alle Einstellungen sind standardmäßig aktiviert.

1. Deaktivieren Sie die Option aus den folgenden Optionen, um Ihre Einstellungen für Workfront zu deaktivieren:

   * Im **[!UICONTROL Allgemeine Einstellungen]** Bereich, deaktivieren Sie die **[!UICONTROL Beim Einfügen einer [!DNL Workfront] URL in einer [!DNL Slack] Kanal, zusätzliche Beschreibung, Fälligkeitsdatum oder Anfragenname anzeigen]**&#x200B; Einstellung, wenn Sie nicht möchten [!DNL Slack] um zusätzliche Informationen zu Ihrer [!DNL Workfront] Objekte beim Freigeben einer URL für das Objekt in [!UICONTROL Slack].

   * Im **[!UICONTROL Benachrichtigungseinstellungen]** deaktivieren Sie Benachrichtigungen, die Sie nicht mehr von Workfront erhalten möchten.\

      Informationen zum Empfang von [!DNL Workfront] Benachrichtigungen in [!DNL Slack], siehe [Empfangen [!DNL Adobe Workfront] Benachrichtigungen in [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Abmelden von [!DNL Workfront] von [!DNL Slack]

1. Innerhalb eines [!DNL Slack] Meldungsfeld, geben Sie den folgenden Befehl ein:\
   `/workfront log out` Oder\
   `/wf log out`\
   Sie erhalten eine Bestätigung, dass Sie von [!DNL Workfront].\
   Sie bleiben bei [!DNL Workfront] wenn Sie über eine separate [!DNL Workfront] -Instanz in einer anderen Browser-Registerkarte in einer anderen Anwendung geöffnet.
