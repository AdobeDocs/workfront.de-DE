---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: Konfigurieren [!DNL Adobe Workfront] für Slack
description: Integration [!DNL Adobe Workfront] mit Slack können Sie auf [!DNL Workfront] Arbeitselemente, Genehmigungen, Favoriten, aktuelle Elemente aus dem Slack.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
source-git-commit: 09b4644a63241fa9e0a213bfa6f1a7e4264a1703
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# Konfigurieren [!DNL Adobe Workfront for Slack]

Integration [!DNL Adobe Workfront] mit [!DNL Slack] ermöglicht Ihnen Folgendes:

* Zugriff auf [!DNL Workfront] Arbeitselemente, Genehmigungen, Favoriten, aktuelle Elemente aus [!DNL Slack].
* Abonnieren, genehmigen, Arbeit zuweisen von [!DNL Slack].
* Erstellen von Aufgaben und Problemen aus [!DNL Slack].
* Einige erhalten [!DNL Workfront] Benachrichtigungen in [!DNL Slack].

Je nachdem, wie Ihre [!DNL Slack] -Umgebung konfiguriert ist, können Sie [!DNL Workfront for Slack] Sie selbst oder Ihre [!DNL Workfront] -Administrator muss sie zuerst installieren und konfigurieren, bevor Sie sie selbst konfigurieren können.

Wenn Sie Ihre [!DNL Slack] Instanz mit [!DNL Workfront] -Benutzer können [!DNL Workfront] bei der Zusammenarbeit innerhalb ihrer [!DNL Slack] Kanäle. Die Integration kann von jedem [!DNL Slack] Umgebung, einschließlich [!DNL Slack] mobile App.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] Plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] administrator.\

## Voraussetzungen für die Verwendung [!DNL Workfront] mit [!DNL Slack]

* Sie müssen über eine [!DNL Slack] -Instanz.
* Ihre [!DNL Slack] Systemadministrator muss alle [!DNL Slack] Benutzer zur Installation [!DNL Workfront for Slack].
* Sie müssen über eine [!DNL Workfront] -Lizenz, um die integrierten Funktionen in [!DNL Workfront].

   >[!NOTE]
   >
   >Benutzer mit [!DNL Workfront] Der Lizenztyp kann auf [!DNL Workfront] von [!DNL Slack]. Die Aktionen, die Sie ausführen können aus [!DNL Slack] sind auf Ihre [!DNL Workfront] Lizenzstufen und Berechtigungsebenen.

Weitere Informationen zum Verwalten von Apps finden Sie unter [!DNL Slack], siehe [Verwalten Sie Apps für Ihren Arbeitsbereich.](https://get.slack.help/hc/en-us/articles/222386767-Manage-apps-for-your-workspace)

## Installieren [!DNL Workfront for Slack]

Jeder [!DNL Slack] Der Benutzer muss die [!DNL Workfront] App verwenden, um [!DNL Workfront] von [!DNL Slack].

Sie können das Programm wie folgt installieren:

* [Installieren Sie die [!DNL Workfront] App außerhalb [!DNL Slack]](#install-the-workfront-app-outside-slack-install-the-workfront-app-outside-slack)
* [Installieren Sie die [!DNL Workfront] App innerhalb [!DNL Slack]](#install-the-workfront-app-within-slack-install-the-workfront-app-within-slack)

### Installieren Sie die [!DNL Workfront] App außerhalb [!DNL Slack] {#install-the-workfront-app-outside-slack}

Führen Sie die folgenden Schritte aus, um den Installationsprozess auszuführen und zu autorisieren [!DNL Workfront for Slack] auf [!DNL Slack] -Instanz.

>[!IMPORTANT]
>
>Wenn eine neue Version von [!DNL Workfront] Wenn Slack veröffentlicht wurde, müssen Sie die App erneut autorisieren, um sie weiterhin verwenden zu können.

1. Suchen Sie die [!DNL Adobe Workfront] -Add-on im [[!DNL Slack] store](https://workfront.slack.com/apps/A7CLAMVNW-adobe-workfront?tab=more_info).

1. Klicken **[!UICONTROL Öffnen in[!DNL Slack]]**.

1. Melden Sie sich bei Ihrem Arbeitsbereich an, indem Sie [!DNL Slack] URL und Klicken **[!UICONTROL Weiter]**.\
   ![screen_shot_2017-10-17_at_8.27.38_AM.png](assets/screen-shot-2017-10-17-at-8.27.38-am-350x432.png)

1. Untersuchen Sie den Zugriff, der [!DNL Slack] fordert. Wenn Sie diesem Zugriff zustimmen, klicken Sie auf **[!UICONTROL Zugriff erlauben]** die [!DNL Workfront] App.

   ![](assets/integrations-access-screen-350x429.png)

Sie können jetzt auf [!DNL Workfront] von [!DNL Slack], wie im Abschnitt [Zugriff [!DNL Workfront] von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

### Installieren Sie die [!DNL Workfront] App innerhalb [!DNL Slack] {#install-the-workfront-app-within-slack}

Sie können die [!DNL Workfront] App direkt über [!DNL Slack] application:

1. Navigieren Sie zu Ihrer [!DNL Slack] URL.

   Beispiel: *`<YourTeamName>`.slack.com/apps*.

   Oder

   Klicken Sie auf **[!UICONTROL Apps hinzufügen]** in der [!DNL Slack] -Instanz.

   ![add_apps_in_Slack.png](assets/add-apps-in-slack-350x112.png)

1. Typisierung beginnen *[!DNL Workfront]* im Suchfeld.
1. Drücken Sie die Eingabetaste.
1. Wählen Sie die **[!DNL Workfront]** App.
1. Klicken **[!UICONTROL Einstellungen]**.

   Die Seite App-Verzeichnis wird angezeigt.

1. Klicken **[!UICONTROL Besuchen der App-Site]**.
1. Klicken **[!UICONTROL Hinzufügen zu[!DNL Slack]]**.
1. Führen Sie die Schritte aus, um die Installation abzuschließen.
1. Nach Abschluss der Installation können Sie auf [!DNL Workfront] von [!DNL Slack], wie im Abschnitt [Zugriff auf [!UICONTROL [!DNL Workfront] von [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).
