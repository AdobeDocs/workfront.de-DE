---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Zugriff [!DNL Adobe Workfront] von  [!DNL Slack]
description: Durch die Integration von [!DNL Adobe Workfront] in [!DNL Slack] können Sie über Slack auf [!DNL Workfront] zugreifen oder bestimmte Aktionen in [!DNL Workfront] mit einem Schrägstrich-Befehl ausführen. Die Integration kann von jeder beliebigen [!DNL Slack] Umgebung aus verwendet werden, einschließlich der  [!DNL Slack] mobilen App.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '1077'
ht-degree: 1%

---

# Zugriff auf [!DNL Adobe Workfront] von [!DNL Slack]

Durch die Integration von [!DNL Adobe Workfront] mit [!DNL Slack] können Sie von [!DNL Slack] auf [!DNL Workfront] zugreifen oder bestimmte Aktionen in [!DNL Workfront] mit einem Schrägstrich ausführen. Die Integration kann von jeder beliebigen [!DNL Slack] -Umgebung aus verwendet werden, einschließlich der [!DNL Slack] mobilen App.

Ihr [!DNL Slack]-Administrator muss die [!DNL Workfront]-App in Ihrer [!DNL Slack]-Instanz installieren, bevor Sie [!DNL Workfront] von [!DNL Slack] verwenden können. Weitere Informationen finden Sie unter [Konfigurieren von Adobe Workfront für Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Über Schrägstrich-Befehle {#about-slash-commands}

Bei Verwendung von [!DNL Slack] geben Sie Meldungen in ein Meldungsfeld ein. Wenn Sie Ihre Nachricht mit einem Schrägstrich beginnen, wird sie zu einem Befehl und verhält sich anders als eine einfache Nachricht. Der Befehl weist [!DNL Slack] an, eine Aktion durchzuführen.

Sie können von [!DNL Slack] aus auf Ihre [!DNL Workfront]-Instanz zugreifen, indem Sie in einen beliebigen [!DNL Slack] -Kanal einen Schrägstrich eingeben.

Beachten Sie Folgendes bei Verwendung eines Schrägstrich-Befehls in [!DNL Slack] für den Zugriff auf [!DNL Workfront]:

* Bei Schrägstrichbefehlen wird zwischen Groß- und Kleinschreibung unterschieden.
* Die Befehle für [!DNL Workfront] sind nur für Sie sichtbar, unabhängig davon, in welchem Kanal Sie sie eingeben.
* Der Befehl sollte immer mit `/workfront` oder `/wf` beginnen, gefolgt von einem Leerzeichen und dem Namen einer Aktion, die Sie in [!DNL Workfront] ausführen möchten.

  Dies bedeutet, dass Ihr Befehl für die [!DNL Workfront]-App vorgesehen ist. Die Befehle für [!DNL Workfront] funktionieren nur, wenn Sie die [!DNL Workfront] -App bereits mit Ihrer [!DNL Slack] -Instanz konfiguriert haben.

Eine Liste aller Befehle, die Sie von Slack für [!DNL Workfront] ausführen können, finden Sie unter [Zugriff [!DNL Workfront] über einen Schrägstrich-Befehl in  [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack).

## Anmelden bei [!DNL Workfront] von [!DNL Slack] {#log-in-to-workfront-from-slack}

Wenn Sie einen Befehl in das Meldungsfeld unter Slack eingeben, werden Sie aufgefordert, sich zuerst bei [!DNL Workfront] anzumelden.\
Eine vollständige Liste der [!DNL Workfront]-Befehle von [!DNL Slack] finden Sie im Abschnitt [Zugriff [!DNL Workfront] von einem Schrägstrich-Befehl in  [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack) in diesem Artikel.

So melden Sie sich von [!DNL Slack] bei [!DNL Workfront] an:

1. Melden Sie sich bei Ihrer [!DNL Slack] -Instanz an.
1. Geben Sie in einem beliebigen Kanal einen der folgenden Befehle ein:\
   `/workfront log in`

   Oder

   `/wf log in`

1. Klicken Sie auf den in der Antwort angezeigten Link [!DNL Workfront] **[!UICONTROL Anmelden]** .\
   Eine neue Registerkarte mit Feldern für [!DNL Workfront]-Anmeldedaten wird geöffnet.

1. Befolgen Sie die Anweisungen zum Anmelden bei [!DNL Workfront] mithilfe von Enhanced Authentication, OAuth 2.0 oder Ihrer SAML-URL (Security Assertion Markup Language).

   >[!NOTE]
   >
   >* Wenn Sie aufgefordert werden, den Host Ihres [!DNL Workfront]-Kontos einzugeben, geben Sie ihn in folgendem Format ein: *sDomain.my.workfront.com* Ihres Unternehmens. Die Domäne Ihres Unternehmens ist normalerweise der Name Ihres Unternehmens.
   >* Die erweiterte Authentifizierung ist erst verfügbar, wenn ein [!DNL Workfront] -Administrator sie für diese Integration aktiviert hat.


   Die Konfigurationsseite für [!DNL Workfront] -Benachrichtigungen in [!DNL Slack] wird geöffnet.

1. (Optional) Deaktivieren Sie alle [!DNL Workfront]-Benachrichtigungen, die Sie in [!DNL Slack] nicht erhalten möchten.

   Informationen zum Konfigurieren von [!DNL Workfront]-Einstellungen für [!DNL Slack] finden Sie im Abschnitt [Einstellungen konfigurieren](#configure-settings-configure-settings) in diesem Artikel

1. Navigieren Sie zurück zu Ihrem [!DNL Slack] -Kanal.

   Sie sind von Ihrer [!DNL Slack] -Instanz bei [!DNL Workfront] angemeldet.

## Zugriff auf [!DNL Workfront] von [!DNL Slack]

* [Über Schrägstrich-Befehle](#about-slash-commands-about-slash-commands)
* [Zugriff auf [!DNL Workfront] über einen freigegebenen Link in  [!DNL Slack]](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## Zugriff auf [!DNL Workfront] über einen Schrägstrich-Befehl in [!DNL Slack] {#access-workfront-from-a-slash-command-in-slack}

1. Melden Sie sich bei Ihrer [!DNL Slack] -Instanz an und melden Sie sich von [!DNL Slack] bei [!DNL Workfront] an.\
   Weitere Informationen zum Anmelden bei [!DNL Workfront] von [!DNL Slack] finden Sie unter [Anmelden bei  [!DNL Workfront] von  [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack)

1. Geben Sie von jedem Kanal aus den folgenden Befehl in das Meldungsfeld ein:

   `/workfront help`

   Oder

   `/wf help`

1. Wählen Sie unter den folgenden Befehlen aus:

   * `/wf home`

     Zeigt Schaltflächen an, über die Sie auf Listen Ihrer Aufgaben, Probleme und Genehmigungen zugreifen können. Wenn Sie auf eine der Schaltflächen klicken, werden die ersten 20 Elemente jeder Liste in [!DNL Slack] angezeigt.

     Weitere Informationen zum Verwalten von [!DNL Workfront] Arbeitselementen aus [!DNL Slack] finden Sie unter [Verwalten Ihrer Arbeit und Genehmigungen aus  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf add task <TaskName>`

     Fügen Sie den Namen der Aufgabe so ein, wie er in der [!DNL Workfront] -Benutzeroberfläche angezeigt wird.

     Fügt eine Aufgabe zu [!DNL Workfront] hinzu.

     Weitere Informationen zum Hinzufügen von Aufgaben zu [!DNL Workfront] von Slack finden Sie im Abschnitt &quot;Erstellen von Aufgaben aus [!DNL Slack]&quot;in [Aufgaben und Probleme aus  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md) erstellen.

   * `/wf add issue <Issue Name>`

     Fügen Sie den Namen des Problems so ein, wie es in der Benutzeroberfläche von [!DNL Workfront] angezeigt wird.

     Fügt ein Problem zu [!DNL Workfront] hinzu

     Weitere Informationen zum Hinzufügen von Problemen zu [!DNL Workfront] aus [!DNL Slack] finden Sie im Abschnitt &quot;Erstellen von Problemen aus [!DNL Slack]&quot;in [Aufgaben und Probleme aus  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md) erstellen.

   * `/wf favorites`

     Zeigt die Liste Ihrer [!DNL Workfront] Favoriten an.

     Weitere Informationen zum Zugriff auf Ihre Favoriten über [!DNL Slack] finden Sie im Abschnitt [Zugreifen auf Ihre [!UICONTROL Favoriten]-Liste von  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites) im Artikel [Zugreifen auf Ihre Favoriten und aktuellen Elemente von  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) .

   * `/wf recent`

     Zeigt die Liste der zuletzt aufgerufenen Elemente in [!DNL Workfront] an.

     Weitere Informationen zum Zugriff auf die neuesten Elemente von [!DNL Slack] aus finden Sie im Artikel [Zugriff auf Ihre Liste der letzten Elemente [!UICONTROL 3} aus  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites]  und [!UICONTROL aktuelle Elemente aus  [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) .]

   * `wf tasks`

     Zeigt eine Liste Ihrer Aufgaben an.

     Weitere Informationen zum Verwalten Ihrer Aufgaben über [!DNL Slack] finden Sie im Abschnitt &quot;Verwalten Ihrer Aufgaben über [!DNL Slack]&quot;in [Verwalten Ihrer Arbeit und Genehmigungen von  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf issues`

     Zeigt eine Liste Ihrer Probleme an.

     Weitere Informationen zum Verwalten Ihrer Probleme über [!DNL Slack] finden Sie im Abschnitt &quot;Verwalten Ihrer Probleme über [!DNL Slack]&quot;in [Verwalten Ihrer Arbeit und Genehmigungen von  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf approvals` Zeigt Ihre [!DNL Workfront] Genehmigungen an.\

     Weitere Informationen zur Verwaltung Ihrer Genehmigungen über [!DNL Slack] finden Sie im Abschnitt &quot;Verwalten Ihrer Genehmigungen von [!DNL Slack]&quot;in [Verwalten Ihrer Arbeit und Genehmigungen von  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

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
      * Hinweis

        Weitere Informationen zum Suchen in [!DNL Slack] finden Sie unter [Suchen nach  [!DNL Adobe Workfront] Elementen von Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md).
   * `/wf log in`

     Protokolliert Sie bei [!DNL Slack] bei [!DNL Workfront].

   * `/wf log out `

     Protokolliert Sie von [!DNL Slack] aus von [!DNL Workfront]. Sie bleiben bei [!DNL Workfront] angemeldet, wenn Sie eine separate [!DNL Workfront] -Instanz in einer anderen Browser-Registerkarte in einer anderen Anwendung geöffnet haben.
   * `/wf settings`

     Ermöglicht Ihnen Zugriff auf die Konfiguration Ihrer [!DNL Workfront]-Einstellungen in [!DNL Slack].

     Informationen zum Konfigurieren von [!DNL Workfront]-Einstellungen unter Slack finden Sie unter [Einstellungen konfigurieren](#configure-settings-configure-settings).

   * `/wf help`
Zeigt eine vollständige Liste der Befehle für [!DNL Workfront] an.


   * `Visit Workfront Help`: Öffnet den Abschnitt [!UICONTROL Slack] auf der Hilfeseite [!DNL Workfront] in einer neuen Browserregisterkarte.


1. (Optional) Um die Meldung eines Befehls zu löschen, bewegen Sie den Mauszeiger über die rechte obere Ecke der Slack-Nachricht, die den Befehl enthält, und klicken Sie auf &#x200B;**[!UICONTROL Nachrichtenaktionen anzeigen]** und klicken Sie dann auf **[!UICONTROL Nachricht löschen]**.

1. (Optional und bedingt) Klicken Sie auf **[!UICONTROL Löschen]** , um zu bestätigen, dass Sie diese Nachricht löschen möchten.

### Zugriff auf [!DNL Workfront] über einen freigegebenen Link in [!DNL Slack] {#access-workfront-from-a-shared-link-in-slack}

Sie können von einem Link aus auf [!DNL Workfront] -Objekte zugreifen, die für Sie in [!DNL Slack] freigegeben sind.

Weitere Informationen zum Zugriff auf [!DNL Workfront] über einen freigegebenen Link finden Sie unter [Zugriff auf [!DNL Adobe Workfront] Objekte von einem freigegebenen Link in  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md).

## Einstellungen konfigurieren {#configure-settings}

1. Geben Sie in das Meldungsfeld [!DNL Slack] den folgenden Befehl ein:

   `/workfront settings`

   Oder

   `/wf settings`

   Alle Einstellungen sind standardmäßig aktiviert.

1. Deaktivieren Sie die Option aus den folgenden Optionen, um Ihre Einstellungen für Workfront zu deaktivieren:

   * Deaktivieren Sie im Bereich **[!UICONTROL Allgemeine Einstellungen]** die Einstellung **[!UICONTROL Wenn Sie eine [!DNL Workfront]-URL in einen [!DNL Slack]-Kanal einfügen, zeigen Sie zusätzliche Beschreibungen, Fälligkeitsdatum oder den Anfragennamen an]** &#x200B; wenn Sie nicht möchten, dass [!DNL Slack] zusätzliche Informationen zu Ihren [!DNL Workfront]-Objekten hinzufügt, wenn Sie eine URL in [!UICONTROL Slack] für das Objekt freigeben.

   * Deaktivieren Sie im Bereich **[!UICONTROL Benachrichtigungseinstellungen]** Benachrichtigungen, die Sie nicht mehr von Workfront erhalten möchten.\

     Informationen zum Empfang von [!DNL Workfront]-Benachrichtigungen in [!DNL Slack] finden Sie unter [Empfang von  [!DNL Adobe Workfront] Benachrichtigungen in  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Abmelden von [!DNL Workfront] von [!DNL Slack]

1. Geben Sie in das Meldungsfeld [!DNL Slack] den folgenden Befehl ein:\
   `/workfront log out` oder\
   `/wf log out`\
   Sie erhalten eine Bestätigung, dass Sie von [!DNL Workfront] abgemeldet wurden.\
   Sie bleiben bei [!DNL Workfront] angemeldet, wenn Sie eine separate [!DNL Workfront] -Instanz in einer anderen Browser-Registerkarte in einer anderen Anwendung geöffnet haben.
