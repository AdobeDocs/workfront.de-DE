---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: Konfigurieren  [!DNL Adobe Workfront]  Slack
description: Durch die  [!DNL Adobe Workfront]  von mit Slack können Sie auf  [!DNL Workfront] , Genehmigungen, Favoriten und zuletzt verwendete Elemente aus Slack zugreifen und diese erstellen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 1%

---

# Konfigurieren von [!DNL Adobe Workfront for Slack]

Durch die Integration von [!DNL Adobe Workfront] mit [!DNL Slack] haben Sie folgende Möglichkeiten:

* Greifen Sie über [!DNL Workfront] auf Ihre [!DNL Slack] Arbeitselemente, Genehmigungen, Favoriten und zuletzt verwendeten Elemente zu.
* Abonnieren, genehmigen, Arbeit von [!DNL Slack] zuweisen.
* Erstellen Sie Aufgaben und Probleme aus [!DNL Slack].
* Erhalten Sie einige [!DNL Workfront]-Benachrichtigungen in [!DNL Slack].

Je nachdem, wie Ihre [!DNL Slack] konfiguriert ist, können Sie [!DNL Workfront for Slack] selbst installieren und konfigurieren oder Ihr [!DNL Workfront] muss die Installation und Konfiguration zuerst durchführen, bevor Sie sie selbst konfigurieren können.

Wenn Sie Ihre [!DNL Slack]-Instanz mit integrieren, können [!DNL Workfront] Benutzer [!DNL Workfront] verwenden, während sie innerhalb ihrer [!DNL Slack] Kanäle zusammenarbeiten. Die Integration kann aus jeder [!DNL Slack]-Umgebung verwendet werden, einschließlich der [!DNL Slack] Mobile App. ## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Beliebig</p>
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen für die Verwendung von [!DNL Workfront] mit [!DNL Slack]

* Sie müssen über eine [!DNL Slack] Instanz verfügen.
* Ihr [!DNL Slack]-Systemadministrator muss allen [!DNL Slack] Benutzern die Installation von [!DNL Workfront for Slack] erlauben.
* Sie müssen über eine [!DNL Workfront]-Lizenz verfügen, um die integrierten Funktionen in [!DNL Workfront] nutzen zu können.

  >[!NOTE]
  >
  >Benutzende mit einem beliebigen [!DNL Workfront] Lizenztyp können über [!DNL Workfront] auf [!DNL Slack] zugreifen. Die Aktionen, die Sie von [!DNL Slack] aus ausführen können, sind auf Ihre [!DNL Workfront]-Lizenz und -Berechtigungsebenen beschränkt.

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

Sie können jetzt über [!DNL Workfront] auf [!DNL Slack] zugreifen, wie unter [Zugriff [!DNL Workfront] von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) beschrieben.

### Installieren der [!DNL Workfront] App in [!DNL Slack] {#install-the-workfront-app-within-slack}

Sie können die [!DNL Workfront] App direkt über die [!DNL Slack] App installieren:

1. Navigieren Sie zu Ihrer [!DNL Slack] URL.

   Beispiel: *`<YourTeamName>`.slack.com/apps*.

   Oder

   Klicken Sie auf **[!UICONTROL Symbol]** Apps hinzufügen“ in Ihrer [!DNL Slack].

1. Beginnen Sie, *[!DNL Workfront]* in das Suchfeld einzugeben.
1. Drücken Sie die Eingabetaste.
1. Wählen Sie die **[!DNL Workfront]** aus.
1. Klicken Sie auf **[!UICONTROL Einstellungen]**.

   Die Seite „App-Verzeichnis“ wird angezeigt.

1. Klicken Sie **[!UICONTROL Besuchen Sie die App-Site]**.
1. Klicken Sie auf **[!UICONTROL Zu[!DNL Slack]]** hinzufügen.
1. Führen Sie die Schritte aus, um die Installation abzuschließen.
1. Nach Abschluss der Installation können Sie von [!DNL Workfront] aus auf [!DNL Slack] zugreifen, wie in der [[!UICONTROL Access [!DNL Workfront] from [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) beschrieben.
