---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: Konfigurieren  [!DNL Adobe Workfront]  Slack
description: Durch die  [!DNL Adobe Workfront]  von mit Slack können Sie auf  [!DNL Workfront] , Genehmigungen, Favoriten und zuletzt verwendete Elemente aus Slack zugreifen und diese erstellen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Konfigurieren von [!DNL Adobe Workfront for Slack]

Durch die Integration von [!DNL Adobe Workfront] mit [!DNL Slack] haben Sie folgende Möglichkeiten:

* Greifen Sie über [!DNL Slack] auf Ihre [!DNL Workfront] Arbeitselemente, Genehmigungen, Favoriten und zuletzt verwendeten Elemente zu.
* Abonnieren, genehmigen, Arbeit von [!DNL Slack] zuweisen.
* Erstellen Sie Aufgaben und Probleme aus [!DNL Slack].
* Erhalten Sie einige [!DNL Workfront]-Benachrichtigungen in [!DNL Slack].

Je nachdem, wie Ihre [!DNL Slack] konfiguriert ist, können Sie [!DNL Workfront for Slack] selbst installieren und konfigurieren oder Ihr [!DNL Workfront] muss die Installation und Konfiguration zuerst durchführen, bevor Sie sie selbst konfigurieren können.

Wenn Sie Ihre [!DNL Slack]-Instanz mit integrieren, können [!DNL Workfront] Benutzer [!DNL Workfront] verwenden, während sie innerhalb ihrer [!DNL Slack] Kanäle zusammenarbeiten. Die Integration kann aus jeder [!DNL Slack]-Umgebung verwendet werden, einschließlich der [!DNL Slack] Mobile App.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/de/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront]]</a>*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.\

## Voraussetzungen für die Verwendung von [!DNL Workfront] mit [!DNL Slack]

* Sie müssen über eine [!DNL Slack] Instanz verfügen.
* Ihr [!DNL Slack]-Systemadministrator muss allen [!DNL Slack] Benutzern die Installation von [!DNL Workfront for Slack] erlauben.
* Sie müssen über eine [!DNL Workfront]-Lizenz verfügen, um die integrierten Funktionen in [!DNL Workfront] nutzen zu können.

  >[!NOTE]
  >
  >Benutzende mit einem beliebigen [!DNL Workfront] Lizenztyp können über [!DNL Slack] auf [!DNL Workfront] zugreifen. Die Aktionen, die Sie von [!DNL Slack] aus ausführen können, sind auf Ihre [!DNL Workfront]-Lizenz und -Berechtigungsebenen beschränkt.

Weitere Informationen zum Verwalten von Apps in [!DNL Slack] finden Sie unter [Verwalten von Apps für Ihre Workspace.](https://get.slack.help/hc/en-us/articles/222386767-Manage-apps-for-your-workspace)

## Installieren von [!DNL Workfront for Slack]

Jeder [!DNL Slack] muss die [!DNL Workfront]-App selbst installieren, um [!DNL Workfront] von [!DNL Slack] verwenden zu können.

Sie können die App wie folgt installieren:

* [Installieren Sie die  [!DNL Workfront] -App draußen [!DNL Slack]](#install-the-workfront-app-outside-slack-install-the-workfront-app-outside-slack)
* [Installieren Sie die  [!DNL Workfront] -App in [!DNL Slack]](#install-the-workfront-app-within-slack-install-the-workfront-app-within-slack)

### Installieren der [!DNL Workfront] außerhalb von [!DNL Slack] {#install-the-workfront-app-outside-slack}

Gehen Sie wie folgt vor, um den Installationsprozess auszuführen und [!DNL Workfront for Slack] auf Ihrer [!DNL Slack] zu autorisieren.

>[!IMPORTANT]
>
>Wenn eine neue Version von [!DNL Workfront] für Slack veröffentlicht wird, müssen Sie die App erneut autorisieren, um sie weiterhin verwenden zu können.

1. Suchen Sie das [!DNL Adobe Workfront]-Add-on im [[!DNL Slack] Store](https://workfront.slack.com/apps/A7CLAMVNW-adobe-workfront?tab=more_info).

1. Klicken Sie auf **[!UICONTROL In[!DNL Slack]]** öffnen.

1. Melden Sie sich bei Ihrem -Arbeitsbereich an, indem Sie Ihre [!DNL Slack]-URL angeben und auf **[!UICONTROL Weiter]** klicken.

1. Überprüfen Sie den von [!DNL Slack] angeforderten Zugriff. Wenn Sie diesem Zugriff zustimmen, klicken Sie auf **[!UICONTROL Zugriff zulassen]**, um die [!DNL Workfront] App zu autorisieren.

Sie können jetzt über [!DNL Slack] auf [!DNL Workfront] zugreifen, wie unter [Zugriff [!DNL Workfront] von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) beschrieben.

### Installieren der [!DNL Workfront] App in [!DNL Slack] {#install-the-workfront-app-within-slack}

Sie können die [!DNL Workfront] App direkt über die [!DNL Slack] App installieren:

1. Navigieren Sie zu Ihrer [!DNL Slack] URL.

   Beispiel: *`<YourTeamName>`.slack.com/apps*.

   Oder

   Klicken Sie auf **[!UICONTROL Symbol]** Apps hinzufügen“ in Ihrer [!DNL Slack].

1. Beginnen Sie, *[!DNL Workfront]* in das Suchfeld einzugeben.
1. Drücken Sie die Eingabetaste.
1. Wählen Sie die **[!DNL Workfront]** aus.
1. Klicken Sie **[!UICONTROL Einstellungen]**.

   Die Seite „App-Verzeichnis“ wird angezeigt.

1. Klicken Sie **[!UICONTROL Besuchen Sie die App-Site]**.
1. Klicken Sie auf **[!UICONTROL Zu[!DNL Slack]]** hinzufügen.
1. Führen Sie die Schritte aus, um die Installation abzuschließen.
1. Nach Abschluss der Installation können Sie von [!DNL Slack] aus auf [!DNL Workfront] zugreifen, wie in der [[!UICONTROL Access [!DNL Workfront] from [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) beschrieben.
