---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Zugriff [!DNL Adobe Workfront] von [!DNL Slack]
description: Durch die  [!DNL Adobe Workfront]  von  [!DNL Slack]  können Sie auf  [!DNL Workfront]  Slack zugreifen oder bestimmte Aktionen  [!DNL Workfront]  einem Schrägstrich durchführen. Die Integration kann in jeder beliebigen  [!DNL Slack]  verwendet werden, einschließlich der Mobile [!DNL Slack] App.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '1077'
ht-degree: 1%

---

# Zugriff auf [!DNL Adobe Workfront] von [!DNL Slack]

Durch die Integration von [!DNL Adobe Workfront] mit [!DNL Slack] können Sie von [!DNL Slack] aus auf [!DNL Workfront] zugreifen oder bestimmte Aktionen in [!DNL Workfront] mit einem Schrägstrich durchführen. Die Integration kann aus jeder [!DNL Slack]-Umgebung verwendet werden, einschließlich der [!DNL Slack] Mobile App.

Sie oder Ihr [!DNL Slack] müssen die [!DNL Workfront] App in Ihrer [!DNL Slack]-Instanz installieren, bevor Sie [!DNL Workfront] von [!DNL Slack] verwenden können. Weitere Informationen finden Sie unter [Konfigurieren von Adobe Workfront für Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Über Schrägstriche {#about-slash-commands}

Wenn Sie [!DNL Slack] verwenden, geben Sie Nachrichten in ein Nachrichtenfeld ein. Wenn Sie Ihre Nachricht mit einem Schrägstrich beginnen, wird sie zu einem Befehl und verhält sich anders als eine einfache Nachricht. Der Befehl weist [!DNL Slack] an, eine Aktion auszuführen.

Sie können auf Ihre [!DNL Workfront]-Instanz über [!DNL Slack] zugreifen, indem Sie einen Schrägstrich in einem beliebigen [!DNL Slack] eingeben.

Beachten Sie Folgendes, wenn Sie einen Schrägstrich in verwenden, [!DNL Slack] auf [!DNL Workfront] zuzugreifen:

* Bei Schrägstrichen wird zwischen Groß- und Kleinschreibung unterschieden.
* Die Befehle für [!DNL Workfront] sind nur für Sie sichtbar, unabhängig davon, in welchen Kanal Sie sie eingeben.
* Der Befehl sollte immer mit `/workfront` oder `/wf` beginnen, gefolgt von einem Leerzeichen und dem Namen einer Aktion, die Sie in [!DNL Workfront] ausführen möchten.

  Dies bedeutet, dass Ihr Befehl für die [!DNL Workfront] App vorgesehen ist. Die Befehle für [!DNL Workfront] funktionieren nur, wenn Sie die [!DNL Workfront] App bereits mit Ihrer [!DNL Slack]-Instanz konfiguriert haben.

Eine Liste aller Befehle, die Sie [!DNL Workfront] von Slack ausführen können, finden Sie unter [Zugriff [!DNL Workfront] von einem Schrägstrich in [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack).

## Anmelden bei [!DNL Workfront] von [!DNL Slack] {#log-in-to-workfront-from-slack}

Wenn Sie einen Befehl in das Nachrichtenfeld auf Slack eingeben, werden Sie aufgefordert, sich zuerst bei [!DNL Workfront] anzumelden.\
Eine vollständige Liste der [!DNL Workfront] Befehle aus [!DNL Slack] finden Sie [ Abschnitt Zugriff [!DNL Workfront] von einem Schrägstrich in  [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack) diesem Artikel.

So melden Sie sich von [!DNL Slack] aus bei [!DNL Workfront] an:

1. Melden Sie sich bei Ihrer [!DNL Slack] an.
1. Geben Sie in einem beliebigen Kanal einen der folgenden Befehle ein:\
   `/workfront log in`

   Oder

   `/wf log in`

1. Klicken Sie auf den [!DNL Workfront] **[!UICONTROL Anmelden]** Link, der in der Antwort angezeigt wird.\
   Eine neue Registerkarte mit Feldern für [!DNL Workfront] Anmeldeinformationen wird geöffnet.

1. Befolgen Sie die Anweisungen, um sich mit der erweiterten Authentifizierung, OAuth 2.0 oder Ihrer SAML-URL (Security Assertion Markup Language) bei [!DNL Workfront] anzumelden.

   >[!NOTE]
   >
   >* Wenn Sie aufgefordert werden, den Host Ihres [!DNL Workfront]-Kontos einzugeben, geben Sie ihn in folgendem Format ein: *yourCompany&#39;sDomain.my.workfront.com*. Die Domain Ihres Unternehmens ist normalerweise der Name Ihres Unternehmens.
   >* Die erweiterte Authentifizierung ist erst verfügbar, wenn sie von einem [!DNL Workfront]-Administrator für diese Integration aktiviert wurde.


   Die Konfigurationsseite für [!DNL Workfront]-Benachrichtigungen in [!DNL Slack] wird geöffnet.

1. (Optional) Deaktivieren Sie alle [!DNL Workfront], die Sie in [!DNL Slack] nicht erhalten möchten.

   Informationen zum Konfigurieren [!DNL Workfront] Einstellungen für [!DNL Slack] finden Sie [ Abschnitt „Konfigurieren ](#configure-settings-configure-settings)&quot; in diesem Artikel

1. Navigieren Sie zurück zu Ihrem [!DNL Slack].

   Sie sind von Ihrer [!DNL Slack]-Instanz aus bei [!DNL Workfront] angemeldet.

## Zugriff auf [!DNL Workfront] von [!DNL Slack]

* [Über Schrägstriche](#about-slash-commands-about-slash-commands)
* [Zugriff  [!DNL Workfront]  einem freigegebenen Link in [!DNL Slack]](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## Zugriff auf [!DNL Workfront] über einen Schrägstrich in [!DNL Slack] {#access-workfront-from-a-slash-command-in-slack}

1. Melden Sie sich bei Ihrer [!DNL Slack]-Instanz an und melden Sie sich von [!DNL Slack] aus bei [!DNL Workfront] an.\
   Weitere Informationen zur Anmeldung bei [!DNL Workfront] von [!DNL Slack] finden Sie unter [Anmelden bei [!DNL Workfront] von [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack)

1. Geben Sie in einem beliebigen Kanal den folgenden Befehl in das Feld Nachricht ein:

   `/workfront help`

   Oder

   `/wf help`

1. Wählen Sie aus den folgenden Befehlen aus:

   * `/wf home`

     Zeigt Schaltflächen an, über die Sie auf Listen Ihrer Aufgaben, Probleme und Genehmigungen zugreifen können. Durch Klicken auf eine der Schaltflächen werden die ersten 20 Elemente jeder Liste in [!DNL Slack] angezeigt.

     Weitere Informationen zum Verwalten [!DNL Workfront] Arbeitselemente von [!DNL Slack] finden Sie unter [Verwalten Ihrer Arbeit und Genehmigungen von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf add task <TaskName>`

     Fügen Sie den Namen der Aufgabe ein, wie er in der [!DNL Workfront] angezeigt wird.

     Fügt [!DNL Workfront] eine Aufgabe hinzu.

     Weitere Informationen zum Hinzufügen von Aufgaben zu [!DNL Workfront] von Slack finden Sie im Abschnitt „Erstellen von Aufgaben aus [!DNL Slack]&quot; in [Erstellen von Aufgaben und Problemen aus [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf add issue <Issue Name>`

     Binden Sie den Namen des Problems ein, wie er in der [!DNL Workfront] angezeigt wird.

     Fügt ein Problem zu [!DNL Workfront] hinzu

     Weitere Informationen zum Hinzufügen von Problemen zu [!DNL Workfront] aus [!DNL Slack] finden Sie im Abschnitt „Erstellen von Problemen aus [!DNL Slack]&quot; in [Erstellen von Aufgaben und Problemen aus [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf favorites`

     Zeigt die Liste Ihrer [!DNL Workfront] Favoriten an.

     Weitere Informationen zum Zugriff auf Ihre Favoriten aus [!DNL Slack] finden Sie im Abschnitt [Zugriff auf Ihre [!UICONTROL Favoriten] Liste aus [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites) im Artikel [Zugriff auf Ihre Favoriten und die letzten Elemente aus [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md).

   * `/wf recent`

     Zeigt die Liste der zuletzt in [!DNL Workfront] aufgerufenen Elemente an.

     Weitere Informationen zum Zugriff auf Ihre letzten Elemente aus [!DNL Slack] finden Sie im Artikel [Zugriff auf Ihre [!UICONTROL letzten Elemente] Liste aus [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites]  und [!UICONTROL letzte Elemente aus [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md).

   * `wf tasks`

     Zeigt eine Liste Ihrer Aufgaben an.

     Weitere Informationen zur Verwaltung Ihrer Aufgaben aus [!DNL Slack] finden Sie im Abschnitt „Verwalten Ihrer Aufgaben aus [!DNL Slack]&quot; in [Verwalten Ihrer Arbeit und Genehmigungen aus [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf issues`

     Zeigt eine Liste Ihrer Probleme an.

     Weitere Informationen zum Verwalten Ihrer Probleme von [!DNL Slack] aus finden Sie im Abschnitt „Verwalten Ihrer Probleme von [!DNL Slack] aus“ in [Verwalten Ihrer Arbeit und Genehmigungen von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf approvals` Zeigt Ihre [!DNL Workfront] Genehmigungen an.\

     Weitere Informationen zum Verwalten Ihrer Genehmigungen aus [!DNL Slack] finden Sie im Abschnitt „Verwalten Ihrer Genehmigungen aus [!DNL Slack]&quot; in [Verwalten Ihrer Arbeit und Genehmigungen aus [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf search <keyword>`

     Schlüsselwort einschließen.

     Suchen Sie nach einem bestimmten Keyword. Sie können nach den folgenden Objekttypen suchen:

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
      * Hinweis \

        Weitere Informationen zum Suchen in [!DNL Slack] finden Sie unter [Suchen nach [!DNL Adobe Workfront] Elementen auf Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md).
   * `/wf log in`

     Meldet Sie von [!DNL Slack] aus bei [!DNL Workfront] an.

   * `/wf log out `

     Sie werden von [!DNL Workfront] von [!DNL Slack] abgemeldet. Sie bleiben bei [!DNL Workfront] angemeldet, wenn in einer anderen Browser-Registerkarte in einer anderen Anwendung eine separate [!DNL Workfront]-Instanz geöffnet ist.
   * `/wf settings`

     Ermöglicht die Konfiguration der [!DNL Workfront] in [!DNL Slack].

     Informationen zum Konfigurieren der [!DNL Workfront] in Slack finden Sie unter [Konfigurieren von Einstellungen](#configure-settings-configure-settings).

   * `/wf help`
Zeigt eine vollständige Liste der Befehle für [!DNL Workfront] an.


   * `Visit Workfront Help`: Öffnet den Abschnitt [!UICONTROL Slack] auf der [!DNL Workfront]-Hilfeseite in einer neuen Browser-Registerkarte.


1. (Optional) Um die Nachricht eines beliebigen Befehls zu löschen, bewegen Sie die Maus über die obere rechte Ecke der Slack-Nachricht mit dem Befehl und klicken Sie auf &#x200B;**[!UICONTROL Nachrichtenaktionen anzeigen]** und klicken Sie dann auf **[!UICONTROL Nachricht löschen]**.

1. (Optional und bedingt) Klicken Sie auf **[!UICONTROL Löschen]** um zu bestätigen, dass Sie diese Nachricht löschen möchten.

### Zugriff auf [!DNL Workfront] über einen freigegebenen Link in [!DNL Slack] {#access-workfront-from-a-shared-link-in-slack}

Sie können auf [!DNL Workfront] Objekte über einen Link auf diese Objekte zugreifen, der für Sie in [!DNL Slack] freigegeben ist.

Weitere Informationen zum Zugriff auf [!DNL Workfront] über einen freigegebenen Link finden Sie unter [Zugriff [!DNL Adobe Workfront] Objekte über einen freigegebenen Link in [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md).

## Einstellungen konfigurieren {#configure-settings}

1. Geben Sie innerhalb eines [!DNL Slack]-Nachrichtenfelds den folgenden Befehl ein:

   `/workfront settings`

   Oder

   `/wf settings`

   Alle Einstellungen sind standardmäßig aktiviert.

1. Deaktivieren Sie die Auswahl aus den folgenden Optionen, um Ihre Einstellungen für Workfront zu deaktivieren:

   * Deaktivieren Sie im Bereich **[!UICONTROL Allgemeine Einstellungen]** die Einstellung **[!UICONTROL Beim Einfügen einer [!DNL Workfront]-URL in einen [!DNL Slack]-Kanal zusätzliche Beschreibung, Fälligkeitsdatum oder Anforderernamen anzeigen]**&#x200B;, wenn Sie nicht möchten, dass [!DNL Slack] zusätzliche Informationen zu Ihren [!DNL Workfront]-Objekten hinzufügen, wenn Sie eine URL für das Objekt in [!UICONTROL Slack&rbrace; &#x200B;].

   * Deaktivieren Sie **[!UICONTROL Bereich &quot;]**&quot; die Benachrichtigungen, die Sie nicht mehr von Workfront erhalten möchten.\

     Weitere Informationen zum Empfang [!DNL Workfront] Benachrichtigungen in [!DNL Slack] finden Sie unter [Empfangen [!DNL Adobe Workfront] Benachrichtigungen in [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Abmelden von [!DNL Workfront] von [!DNL Slack]

1. Geben Sie innerhalb eines [!DNL Slack]-Nachrichtenfelds den folgenden Befehl ein:\
   `/workfront log out` oder\
   `/wf log out`\
   Sie erhalten eine Bestätigung, dass Sie von [!DNL Workfront] abgemeldet wurden.\
   Sie bleiben bei [!DNL Workfront] angemeldet, wenn in einer anderen Browser-Registerkarte in einer anderen Anwendung eine separate [!DNL Workfront]-Instanz geöffnet ist.
