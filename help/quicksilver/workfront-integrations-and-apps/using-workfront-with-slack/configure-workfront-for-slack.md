---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: Konfigurieren von [!DNL Adobe Workfront] für Slack
description: Durch die Integration von [!DNL Adobe Workfront] mit Slack können Sie auf [!DNL Workfront] Arbeitselemente, Genehmigungen, Favoriten und aktuelle Elemente von Slack zugreifen und diese erstellen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Konfigurieren von [!DNL Adobe Workfront for Slack]

Durch die Integration von [!DNL Adobe Workfront] mit [!DNL Slack] können Sie Folgendes tun:

* Greifen Sie auf Ihre [!DNL Workfront] Arbeitselemente, Genehmigungen, Favoriten und aktuelle Elemente aus [!DNL Slack] zu.
* Abonnieren, genehmigen, Arbeit von [!DNL Slack] zuweisen.
* Erstellen Sie Aufgaben und Probleme über [!DNL Slack].
* Empfangen Sie einige [!DNL Workfront]-Benachrichtigungen in [!DNL Slack].

Abhängig davon, wie Ihre [!DNL Slack] -Umgebung konfiguriert ist, können Sie [!DNL Workfront for Slack] selbst installieren und konfigurieren oder Ihr [!DNL Workfront] -Administrator muss diese zunächst installieren und konfigurieren, bevor Sie sie selbst konfigurieren können.

Wenn Sie Ihre [!DNL Slack] -Instanz mit [!DNL Workfront] integrieren, können Benutzer [!DNL Workfront] verwenden, während sie innerhalb ihrer [!DNL Slack]-Kanäle zusammenarbeiten. Die Integration kann von jeder beliebigen [!DNL Slack] -Umgebung aus verwendet werden, einschließlich der [!DNL Slack] mobilen App.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.\

## Voraussetzungen für die Verwendung von [!DNL Workfront] mit [!DNL Slack]

* Sie müssen über eine [!DNL Slack] -Instanz verfügen.
* Ihr [!DNL Slack] -Systemadministrator muss allen [!DNL Slack] -Benutzern die Installation von [!DNL Workfront for Slack] gestatten.
* Sie müssen über eine [!DNL Workfront] -Lizenz verfügen, um die integrierten Funktionen in [!DNL Workfront] verwenden zu können.

  >[!NOTE]
  >
  >Benutzer mit einem beliebigen [!DNL Workfront] -Lizenztyp können über [!DNL Slack] auf [!DNL Workfront] zugreifen. Die Aktionen, die Sie über [!DNL Slack] ausführen können, sind auf Ihre [!DNL Workfront] -Lizenz und -Berechtigungsstufen beschränkt.

Weitere Informationen zum Verwalten von Apps in [!DNL Slack] finden Sie unter [Verwalten von Apps für Ihre Workspace](https://get.slack.help/hc/en-us/articles/222386767-Manage-apps-for-your-workspace).

## Installieren Sie [!DNL Workfront for Slack]

Jeder [!DNL Slack] -Benutzer muss die [!DNL Workfront]-App selbst installieren, um [!DNL Workfront] von [!DNL Slack] zu verwenden.

Sie können das Programm wie folgt installieren:

* [Installieren Sie die [!DNL Workfront] App außerhalb von [!DNL Slack].](#install-the-workfront-app-outside-slack-install-the-workfront-app-outside-slack)
* [Installieren Sie die [!DNL Workfront] App in  [!DNL Slack]](#install-the-workfront-app-within-slack-install-the-workfront-app-within-slack)

### Installieren Sie die [!DNL Workfront]-App außerhalb von [!DNL Slack] {#install-the-workfront-app-outside-slack}

Führen Sie die folgenden Schritte aus, um den Installationsprozess auszuführen und [!DNL Workfront for Slack] für Ihre [!DNL Slack] -Instanz zu autorisieren.

>[!IMPORTANT]
>
>Wenn eine neue Version von [!DNL Workfront] für Slack veröffentlicht wird, müssen Sie die App neu autorisieren, um sie weiterhin verwenden zu können.

1. Suchen Sie das Add-on [!DNL Adobe Workfront] im [[!DNL Slack] store](https://workfront.slack.com/apps/A7CLAMVNW-adobe-workfront?tab=more_info).

1. Klicken Sie auf **[!UICONTROL Öffnen in[!DNL Slack]]**.

1. Melden Sie sich bei Ihrem Arbeitsbereich an, indem Sie Ihre [!DNL Slack]-URL angeben und auf **[!UICONTROL Weiter]** klicken.\

1. Überprüfen Sie den Zugriff, den [!DNL Slack] anfordert. Wenn Sie diesem Zugriff zustimmen, klicken Sie auf **[!UICONTROL Zugriff erlauben]** , um die [!DNL Workfront] -App zu autorisieren.

Sie können jetzt über [!DNL Slack] auf [!DNL Workfront] zugreifen, wie in [Zugriff [!DNL Workfront] von  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] aus [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) beschrieben.

### Installieren Sie die [!DNL Workfront]-App innerhalb von [!DNL Slack] {#install-the-workfront-app-within-slack}

Sie können die [!DNL Workfront]-App direkt über die [!DNL Slack]-Anwendung installieren:

1. Navigieren Sie zu Ihrer [!DNL Slack]-URL.

   Beispiel: *`<YourTeamName>`.slack.com/apps*.

   Oder

   Klicken Sie in Ihrer [!DNL Slack] -Instanz auf das Symbol **[!UICONTROL Apps hinzufügen]** .

1. Geben Sie im Suchfeld *[!DNL Workfront]* ein.
1. Drücken Sie die Eingabetaste.
1. Wählen Sie die **[!DNL Workfront]** -App aus.
1. Klicken Sie auf **[!UICONTROL Einstellungen]**.

   Die Seite App-Verzeichnis wird angezeigt.

1. Klicken Sie auf **[!UICONTROL Besuchen Sie die App-Site]**.
1. Klicken Sie auf **[!UICONTROL Zu[!DNL Slack]]** hinzufügen.
1. Führen Sie die Schritte aus, um die Installation abzuschließen.
1. Nach Abschluss der Installation können Sie über [!DNL Slack] auf [!DNL Workfront] zugreifen, wie in [[!UICONTROL Access [!DNL Workfront]  von  [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront]  aus  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) beschrieben.
