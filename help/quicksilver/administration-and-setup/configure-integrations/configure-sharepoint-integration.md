---
title: Konfigurieren der  [!DNL SharePoint] -Integration
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Sie können  [!DNL Workfront] - [!DNL SharePoint] -Online integrieren und Benutzenden die Möglichkeit geben, innerhalb von Workfront zu  [!DNL SharePoint] -Dokumenten zu navigieren, sie zu verknüpfen und hinzuzufügen. Die bereitgestellte Funktionalität ist mit der anderer  [!DNL Workfront]  vergleichbar.
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '1711'
ht-degree: 0%

---

# [!DNL SharePoint] konfigurieren

<!--Audited: 12/2023-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>Die neue [!DNL SharePoint]-Integration wurde mit der Version 22.3 (Juli 2022) in die Produktion übernommen.
>
>* Obwohl Ihre Benutzer weiterhin auf Dokumente zugreifen können, die über die alte [!DNL SharePoint]-Integration verknüpft sind, können sie keine Dokumente über diese verknüpfen. Sie müssen die neue [!DNL SharePoint]-Integration verwenden, um Dokumente aus SharePoint zu verknüpfen.
>
>* Wenn Sie keine ältere SharePoint-Integration konfiguriert haben, können Sie sie nicht hinzufügen. Sie müssen die neue SharePoint-Integration verwenden, um Dokumente mit SharePoint zu verknüpfen.
>
>* Die neue SharePoint-Integration muss möglicherweise nicht von einem Administrator konfiguriert werden. Sie kann auch von einzelnen Benutzern eingerichtet werden. Um jedoch einen reibungslosen Übergang zur neuen SharePoint-Integration sicherzustellen, muss ein Workfront-Administrator einige kleine Änderungen an den Einstellungen im Bereich &quot;Workfront-Setup“ vornehmen.
>
>    Weitere Informationen und Anweisungen finden Sie unter [Konfigurieren der Legacy-SharePoint-Integration für den kontinuierlichen Zugriff auf ](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents) in diesem Artikel.
>    
>* Es wird empfohlen, dass Benutzer Dokumente verknüpfen, die derzeit über die alte [!DNL SharePoint]-Integration über die neue Integration verknüpft sind.
>    
>    Anweisungen zum Verknüpfen von Dokumenten finden Sie unter [Verknüpfen von Dokumenten aus externen Anwendungen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Sie können [!DNL Workfront] mit [!DNL SharePoint Online] integrieren und Benutzern die Möglichkeit geben, innerhalb von Workfront zu [!DNL SharePoint]-Dokumenten zu navigieren, sie zu verknüpfen und hinzuzufügen. Die bereitgestellte Funktionalität ist mit der anderer [!DNL Workfront]-Integrationen vergleichbar, z. B. [!DNL Google Drive], [!DNL Box] und [!DNL Dropbox].

Diese Integration ist nur mit [!DNL SharePoint Online] kompatibel. On-Premise-Instanzen von [!DNL SharePoint] werden nicht unterstützt.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Sie müssen ein Workfront-Administrator sein. </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Sie müssen über alle erforderlichen Zugriffsrechte in [!DNL SharePoint] verfügen, um Ihre [!DNL SharePoint]-Integration zu ändern oder zu konfigurieren.

## Verknüpfen von Dokumenten über die neue SharePoint-Integration

Einzelne Benutzer können Dokumente über die neue [!DNL SharePoint]-Integration verknüpfen. Für die Integration ist keine Administratorkonfiguration erforderlich. Stattdessen meldet sich der Benutzer beim Verknüpfen eines Dokuments bei seinem [!DNL Microsoft]-Konto an, wodurch die Integration auf Dokumente zugreifen kann, die im [!DNL SharePoint] des Benutzers verfügbar sind.

Wenn ein(e) Benutzende(r) zum ersten Mal die [!DNL Workfront] [!DNL SharePoint]-Integration mit seinem/ihrem [!DNL SharePoint] Konto verbindet, erkennt er/sie entweder alle Berechtigungen an, die [!DNL Workfront] bei der Interaktion mit seinem/ihrem [!UICONTROL SharePoint]-Konto verwendet, und stimmt ihnen zu, oder er/sie kann Berechtigungen von seinem/ihrem Microsoft-Administrator(in) anfordern. Mit Leseberechtigungen können [!DNL Workfront] Dateien auf [!DNL SharePoint] anzeigen und darauf zugreifen, und mit Schreibberechtigungen kann der Benutzer Dateien in [!DNL SharePoint] hochladen.

![SharePoint-Berechtigungen](assets/sharepoint-permissions.png)

Anweisungen zum Verknüpfen von Dokumenten über die neue [!DNL SharePoint] finden Sie unter [Verknüpfen eines externen Dokuments mit [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* Je nach Microsoft-Konfiguration des Unternehmens wird Benutzenden möglicherweise eine Seite „Genehmigung erforderlich“ anstelle einer Seite „Berechtigungen angefordert“ angezeigt. In diesem Fall können die Benutzer diese Seite verwenden, um anzufordern, dass der Microsoft-Administrator des Unternehmens Berechtigungen für die SharePoint-Integration erteilt.
>
>* Eine [!DNL SharePoint]-Integration kann eine Verbindung zu einer einzelnen [!DNL SharePoint]-Instanz herstellen. Daher kann ein Benutzer eine Integration für eine [!DNL SharePoint] einrichten, aber keine Integration für eine zweite [!DNL SharePoint] einrichten, selbst wenn er über Berechtigungen für und Dokumente auf der zweiten [!DNL SharePoint] verfügt.
>
>* Ein Benutzer hat über die [!DNL Workfront] [!DNL SharePoint]-Integration Zugriff auf dieselben Sites, Sammlungen, Ordner, Unterordner und Dateien wie in seinem [!DNL SharePoint].

### Dokumente aus SharePoint verknüpfen

Anweisungen zum Verknüpfen von Dokumenten in SharePoint über die neue [!DNL SharePoint] finden Sie unter [Verknüpfen eines externen Dokuments mit [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront).

### Senden von Dokumenten an SharePoint

So senden Sie ein Dokument an SharePoint:

1. Klicken Sie auf das **Senden an**-Symbol ![Senden an](assets/send-to-icon.png) und wählen Sie SharePoint (Graph API) aus.
1. (Optional) Suchen Sie in der Suchleiste nach der Site oder dem Ordner, an die bzw. den Sie das Dokument senden möchten.
1. Wählen Sie die Site oder den Ordner aus der Liste aus.

   * Websites sind mit dem Symbol ![Site](assets/site-icon.png) gekennzeichnet.

   * Ordner werden mit ![Ordnersymbol](assets/folder-icon.png) gekennzeichnet.

   * Dateien sind nicht mit einem Symbol gekennzeichnet.

1. Klicken Sie auf **Speichern**.


## Informationen zu Sicherheit, Zugriff und Autorisierung für die [!DNL SharePoint] Integration

### Authentifizierung und Autorisierung

[!DNL Workfront] verwendet OAuth2, um ein Zugriffstoken und ein Aktualisierungstoken abzurufen. Dieses Zugriffstoken wird für die Autorisierung in allen [!DNL SharePoint] Bereichen verwendet.

### Zugriff und Berechtigungen

Wenn ein(e) Benutzende(r) zum ersten Mal ein Dokument zu [!DNL Workfront] von [!DNL SharePoint] hinzufügt, wird er/sie auf die Seite Angeforderte Berechtigungen weitergeleitet, wo er/sie Berechtigungen für seine/ihre SharePoint-Integration erteilen kann.

>[!NOTE]
>
>Je nach Microsoft-Konfiguration des Unternehmens wird Benutzenden möglicherweise eine Seite „Genehmigung erforderlich“ anstelle einer Seite „Berechtigungen angefordert“ angezeigt. In diesem Fall können die Benutzer diese Seite verwenden, um anzufordern, dass der Microsoft-Administrator des Unternehmens Berechtigungen für die SharePoint-Integration erteilt.

Die folgenden Berechtigungen werden angefordert:

| Zugriff | Grund |
|---|---|
| Vollständiger Zugriff auf Ihre Dateien | Ermöglicht [!DNL Workfront] den Zugriff auf die Dateien eines Benutzers, um Assets zu verknüpfen. Wenn Dokumente von [!DNL Workfront] an [!DNL SharePoint] gesendet werden, benötigt [!DNL Workfront] Zugriff, um das Asset zu erstellen. |
| Elemente in allen Websitesammlungen lesen | Ermöglicht [!DNL Workfront] das Lesen von Assets, um die Benutzernavigation zu aktivieren. |
| Bearbeiten oder Löschen von Elementen in allen Websitesammlungen | Ermöglicht [!DNL Workfront] das Erstellen von Assets in Sites und Websitesammlungen. Der Löschvorgang wird nur verwendet, wenn nach erfolglosen Verknüpfungsversuchen eine Bereinigung durchgeführt wird. |
| Beibehalten des Zugriffs auf Daten, auf die Sie Zugriff erteilt haben | Ermöglicht [!DNL Workfront] das Generieren eines Aktualisierungs-Tokens. |
| Anmelden und Benutzerprofil lesen | Ermöglicht [!DNL Workfront] die Verwendung des Zugriffstokens für das Handeln des Benutzers über den OAuth2-Anmeldefluss. |

* Dieser Zugriff wird vom Benutzer bei der ersten Verwendung der Integration gewährt und kann jederzeit widerrufen werden.
* Die für diese Integration angeforderten Berechtigungen sind **delegiert** Berechtigungen.
* [!DNL Workfront] fordert den Mindestzugriff an, der zum Ausführen von Vorgängen in der Integration erforderlich ist.
* Der Zugriff auf das Anzeigen, Bearbeiten oder Löschen eines mit [!DNL Adobe Workfront] verknüpften [!DNL SharePoint]-Dokuments basiert auf dem Zugriff des Benutzers in [!DNL Workfront]. Allerdings erfordert jedes Navigieren, Herunterladen oder Bearbeiten einer [!DNL SharePoint] Datei oder eines Ordners Zugriff auf [!DNL SharePoint], und der Zugriff auf diese Aktionen wird von [!DNL SharePoint] gesteuert.
* Benutzer können Miniaturansichten anzeigen und eine Vorschau von Bildern anzeigen, die aus [!DNL SharePoint] bezogen wurden, und können Datei- und Ordnernamen in [!DNL SharePoint] sehen, ohne sich bei [!DNL SharePoint] anzumelden.
* Das Zugriffstoken eines Benutzers wird nur verwendet, wenn der Benutzer offline ist und ein anderer Benutzer den Inhalt eines Ordners anzeigt, der mit [!DNL Workfront] verknüpft ist. Mit dem Zugriffstoken wird ermittelt, ob Dokumente im Ordner hinzugefügt, entfernt oder bearbeitet wurden.

### Sicherheit

Die gesamte Kommunikation zwischen [!DNL Workfront] und [!DNL SharePoint] erfolgt über HTTPS, wodurch die Informationen verschlüsselt werden.

[!DNL Workfront] speichert, kopiert oder dupliziert keine Daten aus [!DNL SharePoint]. Die einzige Ausnahme besteht darin, dass [!DNL Workfront] Miniaturansichten aus [!DNL SharePoint] speichert, die in der Listenansicht und in der Vorschau angezeigt werden sollen.

Wenn ein Asset zuerst in [!DNL Workfront] hochgeladen und dann an [!DNL SharePoint] gesendet wurde, behält [!DNL Workfront] die Daten für die erste Datei bei, da Benutzer eine frühere Version eines [!DNL Workfront]-Dokuments herunterladen können. Wenn ein Dokument in [!DNL SharePoint] erstellt wurde, speichert [!DNL Workfront] diese Dateidaten nicht.

## Konfigurieren der Legacy [!DNL SharePoint]-Integration für den kontinuierlichen Zugriff auf Dokumente

Um sicherzustellen, dass Ihre Benutzerinnen und Benutzer weiterhin über die alte [!DNL SharePoint]-Integration Zugriff auf Dokumente haben, die mit Workfront verknüpft sind, müssen Sie den Zugriff auf die alte [!DNL SharePoint]-Integration neu konfigurieren und den SharePoint-Client-Geheim-Code auf dem neuesten Stand halten.

* [Zugriff auf die Legacy- [!DNL SharePoint]  neu konfigurieren](#reconfigure-access-to-the-legacy-sharepoint-integration)
* [Konfigurieren des Client-Geheimnisses für den kontinuierlichen Zugriff auf die Legacy- [!DNL SharePoint] ](#configure-the-client-secret-for-continued-access-to-the-legacy-sharepoint-integration)

### Zugriff auf die alte [!DNL SharePoint]-Integration neu konfigurieren

Durch die Neukonfiguration der Legacy-[!DNL SharePoint]-Integration können Ihre Benutzer auf Dokumente zugreifen, die über die Legacy-[!DNL SharePoint]-Integration verknüpft sind, während gleichzeitig sichergestellt wird, dass Ihre Benutzer keine neuen Dokumente über diese Integration verknüpfen können.

>[!NOTE]
>
> * Die alte [!DNL SharePoint]-Integration trägt die Bezeichnung &quot;[!DNL SharePoint]&quot;.
> * Die neue [!DNL SharePoint]-Integration trägt die Bezeichnung &quot;[!UICONTROL [!DNL SharePoint] (Graph API)].

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **** Setup![Setup-Symbol](/help/_includes/assets/gear-icon-setup.png).
1. Wählen Sie **[!UICONTROL linken Navigationsbereich]** Dokumente“ und dann **[!UICONTROL Cloud-Anbieter]** aus.
1. Stellen Sie sicher, dass die Optionen **[!DNL SharePoint]** und **[!UICONTROL [!DNL SharePoint](Graph API)]** beide aktiviert sind.
1. Klicken Sie auf **[!UICONTROL Speichern]**.
1. Wählen Sie **[!UICONTROL linken Navigationsbereich]** Dokumente“ und dann **[!UICONTROL [!DNL SharePoint]Integration aus]**.
1. Aktivieren Sie das Kontrollkästchen links in der Liste für alle vorhandenen Integrationen und klicken Sie dann auf **[!UICONTROL Deaktivieren]**.



### Konfigurieren des Client-Geheimnisses für den kontinuierlichen Zugriff auf die alte [!DNL SharePoint]-Integration

Ihr [!DNL SharePoint]-Client-Geheimnis läuft einmal im Jahr ab. Um den kontinuierlichen Zugriff auf die Dokumente in Ihrer alten [!DNL SharePoint]-Integration sicherzustellen, müssen Sie das [!DNL SharePoint]-Client-Geheimnis auf dem neuesten Stand halten.

>[!IMPORTANT]
>
> Da [!DNL SharePoint] Client-Geheimnisse von [!DNL Microsoft] verarbeitet werden, können sich Funktionen und Verfahren des Client-Geheimnisses je nach Aktualisierungen der von [!DNL SharePoint] vorgenommenen [!DNL Microsoft] ändern. In der [!DNL Microsoft] Dokumentation finden Sie immer die neuesten Informationen zu Verfahren und Funktionen in [!DNL SharePoint].

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. Generieren Sie ein neues Client-Geheimnis, wie unter [Ersetzen eines ablaufenden Client-Geheimnisses in einem Add [!DNL SharePoint] In“ ](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret).
1. Kopieren Sie dieses Client-Geheimnis an einen sicheren Speicherort.
1. Melden Sie sich bei [!DNL Workfront] als Administrator an.
1. Klicken Sie in Workfront auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und dann auf **[!UICONTROL Setup]**![Setup](/help/_includes/assets/gear-icon-setup.png).
1. Klicken Sie im linken Bedienfeld auf **[!UICONTROL Dokumente]** > **[!UICONTROL [!DNL SharePoint]-Integration]**.
1. Klicken Sie auf die [!DNL SharePoint] Integration, die Sie aktualisieren möchten, und dann auf **[!UICONTROL Bearbeiten]**.
1. Suchen Sie im Bearbeitungsfenster den **Verbindungsinformationen** und geben Sie dann das neue Client-Geheimnis in das Feld **[!UICONTROL SharePoint-Client-Geheimnis]** ein.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

<!--

## Instructions for setting up the legacy SharePoint integration

>[!IMPORTANT]
>
>This integration has been deprecated. The instructions here are for information only and will be removed in the near future.


Workfront connects to [!DNL SharePoint] Online using OAuth 2.0, a standard used by most web-based integrations for the authentication and authorization of users.

To configure OAuth, you need to create a [!DNL SharePoint] site and a Site App within [!DNL SharePoint]. This process is described in the following sections.

For more information about OAuth, see [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>To make it easy to copy and paste information between [!DNL Workfront] and [!DNL SharePoint] in these steps, we recommend keeping both applications open in separate tabs.

* [Create and configure a [!DNL SharePoint] site](#create-and-configure-a-sharepoint-site) 
* [Grant write permissions to the site app](#grant-write-permissions-to-the-site-app) 
* [Create a [!DNL Workfront] [!DNL SharePoint] integration instance](#create-a-workfront-sharepoint-integration-instance) 
* [Complete your integration](#complete-your-integration) 
* [Add documents](#add-documents)

### Create and configure a [!DNL SharePoint] site  {#create-and-configure-a-sharepoint-site}

In order for [!DNL Workfront] to authenticate with [!DNL SharePoint], [!DNL Workfront] ca use a master site where users have the [!UICONTROL Full Control] permission level or specific Manage permissions. This master site acts as an Authentication Entry Point for [!DNL Workfront].

To create and configure a [!DNL SharePoint] Site:

1. (Optional) If you do not want to use your organization's root site, you can create a master site in [!DNL SharePoint].

   For instructions, visit [Create a site](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) in the [!DNL Microsoft] Documentation.

   * Select the **[!UICONTROL Team Site]** option when creating the site.

1. (Conditional) If you created a site in step 1, go to the site you just created.

   Or

   If you did not create a site in step 1, go to your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.
1. Configure the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client ID]</p> </td> 
      <td> <p>Click <strong>[!UICONTROL Generate]</strong> to generate a Client ID. Copy this ID to a secure location. You will use it later when you set up the [!DNL SharePoint] integration in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client Secret]</p> </td> 
      <td> <p>Click <strong>[!UICONTROL Generate]</strong> to generate a Client Secret. Copy this Secret to a secure location. You will use it later when you set up the [!DNL SharePoint] integration in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Title</p> </td> 
      <td> <p>Enter a title, such as [!DNL Workfront] Site App. Users see this title when adding documents..</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App Domain]</p> </td> 
      <td> <p><code>my.workfront.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Redirect URI]</p> </td> 
      <td> <p><code>https://oauth.my.workfront.com/oauth2/redirect</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create]**
1. Continue to [Grant write permissions to the site app](#grant-write-permissions-to-the-site-app).

### Grant write permissions to the site app  {#grant-write-permissions-to-the-site-app}

At this point, you have successfully created a Site App and registered it within [!DNL Workfront]. This site app is also known as an app principal in [!DNL SharePoint]. It resides within your tenant. New site apps do not automatically have access to site collections within the tenant. Permissions must be granted explicitly, for each site collection. The steps below will show you how to grant Write permission to the new Site App a site collection. Repeat these steps for each of the site collections you added under [!UICONTROL Visible Site Collections] in the steps above.

This site app must have [!UICONTROL Write] permission to any site collections that users need to access through [!DNL Workfront].

1. Add '/_layouts/15/appinv.aspx' to the URL in [!DNL Sharepoint].

   **Example:**

   ```
   https://mycompany.sharepoint.com/sites/mysite/_layouts/15/appinv.aspx
   ```

1. Configure the following fields

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL App ID]</td> 
      <td> <p>Add the Client ID that you created in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>and click <strong>[!UICONTROL Lookup]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client] / [!UICONTROL App Domain] / [!UICONTROL Redirect URL]</p> </td> 
      <td> <p>These automatically fill when you click [!UICONTROL Lookup].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Permission Request XML]</td> 
      <td> <p>Copy the following XML to the [!UICONTROL Permission Request XML] field. Make sure that it is added exactly as shown without additional spaces etc. in order to avoid errors.</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre><code><span style="color: #63a35c; ">&lt;AppPermissionRequests&gt;</span><br><span style="color: #63a35c; ">&lt;AppPermissionRequest <span style="color: #795da3; ">Scope</span><span style="color: #df5000; ">="http://sharepoint/content/sitecollection/web"</span> <span style="color: #795da3; ">Right</span><span style="color: #df5000; ">="Write"</span>/&gt;</span><br><span style="color: #63a35c; ">&lt;/AppPermissionRequests&gt;</span></code></pre> 
      </div> 
      </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create]**. 
1. In the dialog that appears, click **[!UICONTROL Trust it]**.
1. Verify that the site app has access to the site collection by clicking the **[!UICONTROL Site collection app permissions]** link in [!UICONTROL Site Settings].
1. Repeat the steps above for the remaining site collections, then continue with [Create a [!DNL Workfront] [!DNL SharePoint] integration instance](#create-a-workfront-sharepoint-integration-instance).

### Create a [!DNL Workfront] [!DNL SharePoint] integration instance {#create-a-workfront-sharepoint-integration-instance}

When you have created a site app in [!DNL SharePoint], you can now copy information from the site app into [!DNL Workfront]. The site app is an app principal and acts as the conduit through which OAuth requests are made to access documents within site collections.

1. Log into [!DNL Workfront] as an administrator.
1. Click the **[!UICONTROL Main Menu]** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Setup]** ![Gear settings icon](assets/gear-icon-settings.png).

1. In the left panel, click **[!UICONTROL Documents]** > **[!UICONTROL [!DNL SharePoint] Integration]**.
1. Click **[!UICONTROL Add [!DNL SharePoint]]**.
1. Configure the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Name]</p> </td> 
      <td> <p>Enter a name for the [!DNL SharePoint] integration. Users see this name when they click [!UICONTROL Add] &gt; [!UICONTROL From] 'name of integration'. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] Host Instance]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] Access Domain]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>This refers to the Master Site that users will use to authenticate through. It is likely the same domain as the [!UICONTROL [!DNL SharePoint] Host Instance].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>Important</b> Site collections are used only in the Legacy [!DNL SharePoint] Integration.
       <ul> 
        <li> <p><b>If you are using your organization's root site</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>If you are using a master site and subsites:</b> </p> <p><b>IMPORTANT</b>: [!DNL Microsoft SharePoint] no longer recommends the use of subsites.</p> <p>Enter the URL stem for the site collection that you created in the section above.</p> <p>This is the section of the URL after .com.</p> <p>Example: for the URL <code>https://mycompany.sharepoint.com/sites/mysite</code>, the stem would be <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Client ID]</td> 
      <td>Enter the Client ID that you generated in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Client Secret]</td> 
      <td>Enter the Client Secret that you generated in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Visible Site Collections]</td> 
      <td> <b>Important</b> Site collections are used only in the Legacy [!DNL SharePoint] integration.
       <ul> 
        <li> <p><b> If you are using your organization's root site</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>If you are using a master site and subsites:</b> </p> <p><b>IMPORTANT</b>: [!DNL Microsoft SharePoint] no longer recommends the use of subsites.</p> <p>For each subsite you want to add to your [!DNL SharePoint] integration, enter the stem of the subsite.</p> <p>Example: for the URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, the stem would be <code>/sites/mysite/mysubsite</code>.</p> <p><b>NOTE</b>:   <p>If you want to test your configuration only (no subsites), enter the stem of the master site. </p> <p>Example: for the URL <code> https://mycompany.sharepoint.com/sites/mysite</code>, the stem would be <code>/sites/mysite</code>.</p> <p>When you have tested your configuration as described in <a href="#complete-your-integration" class="MCXref xref">Complete your integration</a>, you must remove the master site and enter the subsites.</p> 
          <ol> 
           <li value="1">Click the <strong>[!UICONTROL Main Menu]</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of [!DNL Adobe Workfront], then click <strong>[!UICONTROL Setup]</strong> <img src="assets/gear-icon-settings.png">.<li><p>In the left panel, click <strong>[!UICONTROL Documents]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] Integration]</strong>.</p></li><li><p>Click the [!DNL SharePoint] integration you are setting up, then click Edit.</p></li><li><p>Delete the stem for the master site from the [!UICONTROL Visible Site Collections] field.</p></li><li><p>For each subsite you want to add to your [!DNL SharePoint] integration, enter the stem of the subsite.</p></li><p>Example: for the URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, the stem would be <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Save]**
1. Continue to [Complete your integration](#complete-your-integration).

### Complete your integration {#complete-your-integration}

The basic configuration is almost complete.

1. In Workfront, Click the **[!UICONTROL Main Menu]** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Documents]** ![Document icon](assets/document-icon.png).
1. Click **[!UICONTROL Add new]**.
1. Click **[!UICONTROL From] `<title of your [!DNL SharePoint] site>`** in the dropdown.

   A dialog that invites you to Trust this site appears.

   >[!NOTE]
   >
   >If this dialog does not appear, your [!DNL SharePoint] integration is not configured correctly.

1. Click **[!UICONTROL Trust it]**.

### Add documents {#add-documents}

You can now add documents from your [!DNL SharePoint] site.

For instructions, see [Link an external document to [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) in [Link documents from external applications](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>If the user who linked a folder no longer has access to the external application, [!DNL Workfront] can no longer access the contents of the folder. This may happen, for example, if the user who originally linked the folder leaves the company. To ensure continued access, a user with access to the folder must re-link the folder.
> 

-->

## Fehlerbehebung

* [Problem: Bei der Verwendung der Integration tritt bei  [!DNL SharePoint]  Benutzern ein authentifizierungsbasierter Fehler auf](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [Problem: Beim Versuch, Dateien  [!DNL SharePoint]  durchsuchen [!DNL Workfront] werden keine oder alle meine Websitesammlungen angezeigt.](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [Problem: Ich kann auf zuvor verknüpfte Ordner und Dokumente in nicht zugreifen [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### Problem: Bei Verwendung der [!DNL SharePoint]-Integration treten authentifizierungsbasierte Fehler auf. {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

Lösungen:

Benutzer müssen über die entsprechenden Berechtigungen für die [!DNL SharePoint]-Site verfügen.

Benutzer mit [!UICONTROL Vollzugriff] verfügen über alle erforderlichen Berechtigungen für Ihre [!DNL SharePoint]. Wenn Sie den Benutzern keinen Vollzugriff gewähren möchten, müssen Sie die folgenden Berechtigungen gewähren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Design]</p> </td> 
   <td> <p>Kann anzeigen, hinzufügen, aktualisieren, löschen, genehmigen und anpassen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Bearbeiten]</p> </td> 
   <td> <p>Kann Listen hinzufügen, bearbeiten und löschen; kann Listenelemente und Dokumente anzeigen, hinzufügen, aktualisieren und löschen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contribute]</p> </td> 
   <td> <p>Kann Listenelemente und Dokumente anzeigen, hinzufügen, aktualisieren und löschen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!Nur UICONTROL-Ansicht]</p> </td> 
   <td> <p>Kann Seiten, Listenelemente und Dokumente anzeigen (Dokumenttypen mit Server-seitigen Datei-Handlern können im Browser angezeigt, aber nicht heruntergeladen werden)</p> </td> 
  </tr> 
 </tbody> 
</table>

Anweisungen zum Erstellen und Bearbeiten von Berechtigungsebenen finden Sie unter [Erstellen und Bearbeiten von Berechtigungsebenen](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels) in der Dokumentation zu Microsoft.

<!--

### Problem: As a [!DNL Workfront] user, I am unable to provision a new [!DNL SharePoint] instance. When I attempt to do I see an error. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Solutions:

This can be caused by a number of things, originating in either [!DNL Workfront] or [!DNL SharePoint]'s configuration. Verify that:

* The Client ID, Client Secret, return URL and other configuration fields are correctly mapped between the [!DNL Workfront] [!DNL SharePoint] Integration instance and the [!DNL SharePoint] Site App.
* The user has [!UICONTROL Full Control] permission to the Site Collection used for authentication.
* The Site App is listed under [!UICONTROL Site App Permissions] for the [!UICONTROL Site Collection] used for authentication.

-->

### Problem: Beim Versuch, [!DNL SharePoint] Dateien in [!DNL Workfront] zu durchsuchen, sehe ich keine oder alle meine Websitesammlungen. {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

Lösungen:

Um eine Websitesammlung in [!DNL Workfront] anzuzeigen, müssen die folgenden Bedingungen erfüllt sein:

<!--

* The site collection must be registered in the [!DNL Workfront] [!DNL SharePoint] Integration instance.

  To verify this in [!DNL Workfront]:

   1. Go to [!UICONTROL Setup] > [!UICONTROL Documents] > [!UICONTROL [!DNL SharePoint] Integration].
   1. Edit the [!DNL SharePoint] Integration instance information.
   1. Verify that the site collection is listed under [!UICONTROL Visible Site Collections].
   -->

* Der Benutzer muss Ansichtszugriff auf die Websitesammlung in [!DNL SharePoint] haben.

  Um dies in [!DNL SharePoint] zu überprüfen, überprüfen Sie die Berechtigungen der Websitesammlung in SharePoint.

<!--* The [!DNL SharePoint] Site App must have access to the site collection.

  To verify this in [!DNL SharePoint]:

   1. Go to the site collection > [!UICONTROL Settings] > [!UICONTROL Site app permissions].
   1. Ensure that the [!UICONTROL Site App] used by [!DNL Workfront] is listed here.
   1. (Conditional) If the Site App is not listed, add to the site collection using _layouts/15/appinv.aspx.

      For information about adding the site collection, see Granting Write Permissions To The Site App.
      
-->

### Problem: Ich kann nicht auf zuvor verknüpfte Ordner und Dokumente in [!DNL SharePoint] zugreifen. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

Lösung:

Wenn sich der Benutzer, der einen [!DNL SharePoint] Ordner verknüpft hat, nicht mehr authentifizieren kann, kann [!DNL Workfront] nicht mehr auf den Inhalt des Ordners zugreifen. Dies kann beispielsweise vorkommen, wenn der Benutzer, der den Ordner ursprünglich verknüpft hat, das Unternehmen verlässt.

Um den kontinuierlichen Zugriff sicherzustellen, muss ein Benutzer mit Zugriff auf den Ordner den Ordner erneut verknüpfen.

Informationen zum Verknüpfen von Ordnern von externen Anbietern finden Sie unter [Verknüpfen von Dokumenten aus externen Anwendungen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<!--

### Problem: I see a "404 not found" error when attempting to add a document from [!DNL Sharepoint]

#### Solution:

This error might occur if one of the sites configured in the [!UICONTROL Visible Site Collections] list has been deleted in Sharepoint. Check the [!UICONTROL Visible Site Collections] list, and remove any sites that have been deleted in Sharepoint.-->
