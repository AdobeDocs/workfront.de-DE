---
title: Konfigurieren Sie die [!DNL SharePoint] Integration
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Sie können [!DNL Workfront] mit [!DNL SharePoint] Online, sodass Benutzer zu navigieren, eine Verknüpfung erstellen und [!DNL SharePoint] Dokumente in Workfront. Die bereitgestellten Funktionen ähneln denen anderer [!DNL Workfront] Integrationen wie Google Drive, Box und Dropbox.
author: Becky, Caroline
feature: System Setup and Administration, [!DNL Workfront] Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: e08b56b3bc212d49fd594912b6b28cd8e8f77b8b
workflow-type: tm+mt
source-wordcount: '1483'
ht-degree: 0%

---

# Ältere Version konfigurieren [!DNL SharePoint] Integration

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>Die neue [!DNL SharePoint] Die Integration wurde mit der Version 22.3 (Juli 2022) für die Produktion freigegeben. Auch wenn Ihre Benutzer weiterhin auf Dokumente zugreifen können, die über die veraltete [!DNL SharePoint] -Integration, müssen sie die neue [!DNL SharePoint] Integration, um Dokumente aus SharePoint zu verknüpfen.
>
>* Die neue SharePoint-Integration muss nicht von einem Administrator konfiguriert werden und kann von einzelnen Benutzern eingerichtet werden. Um jedoch einen reibungslosen Übergang zur neuen SharePoint-Integration sicherzustellen, muss ein Workfront-Administrator einige kleine Änderungen an den Einstellungen im Workfront-Setup-Bereich vornehmen.
>
>    Informationen und Anweisungen finden Sie unter [Konfigurieren der alten SharePoint-Integration für den kontinuierlichen Zugriff auf Dokumente](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents) in diesem Artikel.
>    
>* Es wird empfohlen, dass Benutzer Dokumente verknüpfen, die derzeit über die veraltete Version verknüpft sind [!DNL SharePoint] Integration durch die neue Integration.
>    
>    Anweisungen zum Verknüpfen von Dokumenten finden Sie unter [Verknüpfen von Dokumenten mit externen Anwendungen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Sie können [!DNL Workfront] mit [!DNL SharePoint Online], sodass Benutzer zu navigieren, eine Verknüpfung erstellen und [!DNL SharePoint] Dokumente in Workfront. Die bereitgestellten Funktionen ähneln denen anderer [!DNL Workfront] Integrationen, z. B. [!DNL Google Drive], [!DNL Box]und [!DNL Dropbox].

Diese Integration ist nur mit [!DNL SharePoint Online]. On-Premise-Instanzen von [!DNL SharePoint] werden nicht unterstützt.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Sie müssen [!DNL Workfront] Administrator. Informationen über [!DNL Workfront] Administratoren, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Voraussetzungen

Sie müssen über alle erforderlichen Zugriff oder Berechtigungen verfügen in [!DNL SharePoint] , um die [!DNL SharePoint].

## Verknüpfen von Dokumenten über die neue SharePoint-Integration

Einzelne Benutzer können Dokumente über die neue [!DNL SharePoint] Integration. Für die Integration ist keine Administratorkonfiguration erforderlich. Stattdessen meldet sich der Benutzer bei der [!DNL Microsoft] Konto beim Verknüpfen eines Dokuments, über das die Integration auf Dokumente zugreifen kann, die im [!DNL SharePoint].

Wenn ein Benutzer die [!DNL Workfront] [!DNL SharePoint] Integration [!DNL SharePoint] -Konto, sehen sie alle Berechtigungen, die [!DNL Workfront] bei der Interaktion mit ihren [!UICONTROL SharePoint] -Konto. Leseberechtigungen zulassen [!DNL Workfront] zum Anzeigen und Aufrufen von Dateien in [!DNL SharePoint]und Schreibberechtigungen ermöglichen es dem Benutzer, Dateien in hochzuladen. [!DNL SharePoint].

![Sharepoint-Berechtigungen](assets/sharepoint-permissions.png)

Anweisungen zum Verknüpfen von Dokumenten über die neue [!DNL SharePoint] Integration, siehe [Externes Dokument verknüpfen zu [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* A [!DNL SharePoint] Integration kann eine Verbindung zu einer [!DNL SharePoint] -Instanz. Daher kann ein Benutzer eine Integration für eine [!DNL SharePoint], kann jedoch keine Integration für eine Sekunde einrichten [!DNL SharePoint], auch wenn sie über Berechtigungen und Dokumente für die zweite verfügen [!DNL SharePoint].
>
>* Ein Benutzer hat Zugriff auf dieselben Sites, Sammlungen, Ordner, Unterordner und Dateien über die [!DNL Workfront] [!DNL SharePoint] -Integration, wie sie in ihren [!DNL SharePoint] -Konto.

## Sicherheits-, Zugriffs- und Autorisierungsinformationen für die [!DNL SharePoint] Integration

### Authentifizierung und Autorisierung

[!DNL Workfront] verwendet OAuth2, um ein Zugriffstoken und ein Aktualisierungstoken abzurufen. Dieses Zugriffstoken wird für die Autorisierung mit allen [!DNL SharePoint] Gebiete.

### Zugriff und Berechtigungen

Wenn ein Benutzer zum ersten Mal ein Dokument zu [!DNL Workfront] von [!DNL SharePoint], werden sie zu einem Bildschirm geleitet, der die folgenden Berechtigungen anfordert:

| Zugriff | Grund |
|---|---|
| Vollständigen Zugriff auf Ihre Dateien | Ermöglicht [!DNL Workfront] , um auf die Dateien eines Benutzers zuzugreifen und das Asset zu verknüpfen. Wann Dokumente gesendet werden von [!DNL Workfront] nach [!DNL SharePoint], [!DNL Workfront] erfordert Zugriff, um das Asset zu erstellen. |
| Elemente in allen Site-Sammlungen lesen | Ermöglicht [!DNL Workfront] , um Assets zu lesen und die Benutzernavigation zu aktivieren. |
| Bearbeiten oder Löschen von Elementen in allen Site-Sammlungen | Ermöglicht [!DNL Workfront] , um Assets in Sites und Site-Sammlung zu erstellen. Löschen wird nur bei Bereinigungen nach erfolglosen Linkversuchen verwendet. |
| Beibehalten des Zugriffs auf die Daten, auf die Sie Zugriff gewährt haben | Ermöglicht [!DNL Workfront] , um ein Aktualisierungstoken zu generieren. |
| Anmelden und Benutzerprofil lesen | Ermöglicht [!DNL Workfront] , um das Zugriffstoken zu verwenden, um im Namen des Benutzers über den OAuth2-Anmeldefluss zu handeln. |

Dieser Zugriff wird vom Benutzer beim ersten Verwenden der Integration gewährt und kann jederzeit widerrufen werden.

Beachten Sie Folgendes bezüglich des Zugriffs auf [!DNL SharePoint] durch [!DNL Workfront] [!DNL SharePoint] Integration:

* Die für diese Integration angeforderten Berechtigungen sind **delegiert** Berechtigungen.
* [!DNL Workfront] fordert den Mindestzugriff an, der für die Durchführung von Vorgängen in der Integration erforderlich ist.
* Zugriff auf das Anzeigen, Bearbeiten oder Löschen eines [!DNL Adobe Workfront] Dokument, das verknüpft ist mit [!DNL SharePoint] basiert auf dem Zugriff des Benutzers in [!DNL Workfront]. Allerdings können Navigations-, Download- oder Bearbeitungsvorgänge von [!DNL SharePoint] Datei oder Ordner erfordert Zugriff auf [!DNL SharePoint], und der Zugriff auf diese Aktionen wird durch [!DNL SharePoint].
* Benutzer können Miniaturansichten und Vorschaubilder anzeigen, die aus [!DNL SharePoint]und die Datei- und Ordnernamen in [!DNL SharePoint], ohne sich anzumelden [!DNL SharePoint].
* Das Zugriffstoken eines Benutzers wird nur verwendet, wenn der Benutzer offline ist, und ein anderer Benutzer sieht den Inhalt eines Ordners an, der mit [!DNL Workfront]. Das Zugriffstoken wird verwendet, um festzustellen, ob Dokumente im Ordner hinzugefügt, entfernt oder bearbeitet wurden.

### Sicherheit

Alle Kommunikation zwischen [!DNL Workfront] und [!DNL SharePoint] wird über HTTPS durchgeführt, das die Informationen verschlüsselt.

[!DNL Workfront] speichert, kopiert oder dupliziert keine Daten aus [!DNL SharePoint]. Die einzige Ausnahme ist, dass [!DNL Workfront] speichert Miniaturansichten aus [!DNL SharePoint] in der Listenansicht und in der Vorschau angezeigt.

Wenn ein Asset zum ersten Mal in hochgeladen wurde [!DNL Workfront]und anschließend an [!DNL SharePoint], [!DNL Workfront] speichert die Daten für die erste Datei, da Benutzer eine frühere Version eines [!DNL Workfront] Dokument. Wenn ein Dokument in [!DNL SharePoint], [!DNL Workfront] speichert diese Dateidaten nicht.

## Konfigurieren der alten [!DNL SharePoint] Integration für den kontinuierlichen Zugriff auf Dokumente

So stellen Sie sicher, dass Ihre Benutzer über die alte Version weiterhin Zugriff auf mit Workfront verknüpfte Dokumente haben [!DNL SharePoint] Integration, müssen Sie den Zugriff auf die veraltete [!DNL SharePoint] Integration und halten Sie das SharePoint Client Secret auf dem neuesten Stand.

* [Zugriff auf die alte Version neu konfigurieren [!DNL SharePoint] Integration](#reconfigure-access-to-the-legacy-dnl-sharepoint-integration)
* [Client-Geheimnis für kontinuierlichen Zugriff auf die alte Version konfigurieren [!DNL SharePoint] Integration](#configure-the-client-secret-for-continued-access-to-the-legacy-dnl-sharepoint-integration)

### Zugriff auf die alte Version neu konfigurieren [!DNL SharePoint] Integration

So stellen Sie sicher, dass Sie auf Dokumente zugreifen können, die über die veralteten [!DNL SharePoint] -Integration, wobei sichergestellt wird, dass Ihre Benutzer keine neuen Dokumente über diese Integration verknüpfen können, führen Sie das folgende Verfahren aus.

>[!NOTE]
>
> * Das Vermächtnis [!DNL SharePoint] Integration wird als[!DNL SharePoint].&quot;
> * Die neue [!DNL SharePoint] Integration wird als[!UICONTROL [!DNL SharePoint] (Graph-API)].&quot;

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **[!UICONTROL Einrichtung]** ![Einrichtung](../get-started-wf-administration/assets/gear-icon-settings.png).
1. Auswählen **[!UICONTROL Dokumente]** Wählen Sie im linken Navigationsbereich die Option **[!UICONTROL Cloud-Anbieter]**.
1. Stellen Sie sicher, dass die Variable **[!DNL SharePoint]** und **[!UICONTROL [!DNL SharePoint](Graph-API)]** beide aktiviert sind.
1. Klicken Sie auf **[!UICONTROL Speichern]**.
1. Auswählen **[!UICONTROL Dokumente]** Wählen Sie im linken Navigationsbereich die Option **[!UICONTROL [!DNL SharePoint]Integration]**.
1. Markieren Sie links neben der Liste das Kontrollkästchen für alle vorhandenen Integrationen und wählen Sie dann **[!UICONTROL Deaktivieren]**.


### Client-Geheimnis für kontinuierlichen Zugriff auf die alte Version konfigurieren [!DNL SharePoint] Integration

Ihre [!DNL SharePoint] Client Secret läuft einmal jährlich ab. Gewährleistung eines kontinuierlichen Zugriffs auf die Dokumente in Ihrer alten [!DNL SharePoint] Integration, müssen Sie die [!DNL SharePoint] Client Secret auf dem neuesten Stand.

>[!IMPORTANT]
>
> weil [!DNL SharePoint] Client-Geheimnisse werden von [!DNL Microsoft], können sich die Funktionen und Verfahren des Client-Geheimnisses basierend auf Aktualisierungen von [!DNL SharePoint] von [!DNL Microsoft]. Überprüfen Sie immer die [!DNL Microsoft] Dokumentation mit aktuellen Informationen zu Verfahren und Funktionen in [!DNL SharePoint].

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. Generieren Sie ein neues Client-Geheimnis, wie unter [Ersetzen eines ablaufenden Client-Geheimnisses in einer [!DNL SharePoint] Add-in](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret)
1. Kopieren Sie dieses Client-Geheimnis an einen sicheren Speicherort.
1. Anmelden [!DNL Workfront] als Administrator.
1. Klicken Sie in Workfront auf die **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).
1. Klicken Sie im linken Bereich auf **[!UICONTROL Dokumente]** > **[!UICONTROL [!DNL SharePoint]Integration]**.
1. Klicken Sie auf [!DNL SharePoint] Integration, die Sie aktualisieren möchten, und klicken Sie auf **[!UICONTROL Bearbeiten]**.
1. Geben Sie den neuen Client-Geheimnisschlüssel in das **[!UICONTROL Client Secret]** -Feld.
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
1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

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

1. In Workfront, Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Documents]** ![](assets/document-icon.png).
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

* [Problem: Benutzer erhalten bei der Verwendung der Variablen [!DNL SharePoint] Integration.](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [Problem: Beim Versuch zu durchsuchen [!DNL SharePoint] Dateien in [!DNL Workfront], sehe ich keine oder alle meiner Site-Sammlungen.](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [Problem: Ich kann nicht auf zuvor verknüpfte Ordner und Dokumente in [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### Problem: Benutzer erhalten bei der Verwendung der Variablen [!DNL SharePoint] Integration. {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

Lösungen:

Benutzer müssen über die entsprechenden Berechtigungen für die [!DNL SharePoint] Site.

Benutzer mit [!UICONTROL Vollständige Kontrolle] Zugriff haben alle erforderlichen Berechtigungen für Ihre [!DNL SharePoint] Integration. Wenn Sie Ihren Benutzern keinen Vollzugriff gewähren möchten, müssen Sie die folgenden Berechtigungen erteilen:

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
   <td> <p>Kann Listen hinzufügen, bearbeiten und löschen; Listenelemente und Dokumente anzeigen, hinzufügen, aktualisieren und löschen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contribute]</p> </td> 
   <td> <p>Listenelemente und Dokumente anzeigen, hinzufügen, aktualisieren und löschen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nur Ansicht]</p> </td> 
   <td> <p>Kann Seiten, Listenelemente und Dokumente anzeigen (Dokumenttypen mit serverseitigen Dateihandlern können im Browser angezeigt, aber nicht heruntergeladen werden)</p> </td> 
  </tr> 
 </tbody> 
</table>

Anweisungen zum Erstellen und Bearbeiten von Berechtigungsebenen finden Sie unter [So erstellen und bearbeiten Sie Berechtigungsebenen](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels) in der Microsoft-Dokumentation.

<!--

### Problem: As a [!DNL Workfront] user, I am unable to provision a new [!DNL SharePoint] instance. When I attempt to do I see an error. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Solutions:

This can be caused by a number of things, originating in either [!DNL Workfront] or [!DNL SharePoint]'s configuration. Verify that:

* The Client ID, Client Secret, return URL and other configuration fields are correctly mapped between the [!DNL Workfront] [!DNL SharePoint] Integration instance and the [!DNL SharePoint] Site App.
* The user has [!UICONTROL Full Control] permission to the Site Collection used for authentication.
* The Site App is listed under [!UICONTROL Site App Permissions] for the [!UICONTROL Site Collection] used for authentication.

-->

### Problem: Beim Versuch zu durchsuchen [!DNL SharePoint] Dateien in [!DNL Workfront], sehe ich keine oder alle meiner Site-Sammlungen. {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

Lösungen:

So zeigen Sie eine Site-Sammlung in [!DNL Workfront]müssen folgende Bedingungen erfüllt sein:

<!--

* The site collection must be registered in the [!DNL Workfront] [!DNL SharePoint] Integration instance.

  To verify this in [!DNL Workfront]:

   1. Go to [!UICONTROL Setup] > [!UICONTROL Documents] > [!UICONTROL [!DNL SharePoint] Integration].
   1. Edit the [!DNL SharePoint] Integration instance information.
   1. Verify that the site collection is listed under [!UICONTROL Visible Site Collections].
   -->

* Der Benutzer muss Zugriff auf die Site-Sammlung in der [!DNL SharePoint].

  So überprüfen Sie dies in [!DNL SharePoint], gehen Sie zu [!DNL SharePoint]und öffnen Sie die Site-Sammlung > [!UICONTROL Einstellungen] > [!UICONTROL Site-Berechtigungen].
<!--* The [!DNL SharePoint] Site App must have access to the site collection.

  To verify this in [!DNL SharePoint]:

   1. Go to the site collection > [!UICONTROL Settings] > [!UICONTROL Site app permissions].
   1. Ensure that the [!UICONTROL Site App] used by [!DNL Workfront] is listed here.
   1. (Conditional) If the Site App is not listed, add to the site collection using _layouts/15/appinv.aspx.

      For information about adding the site collection, see Granting Write Permissions To The Site App.
      
-->

### Problem: Ich kann nicht auf zuvor verknüpfte Ordner und Dokumente in [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

Lösung:

Wenn der Benutzer, der eine [!DNL SharePoint] -Ordner kann nicht mehr authentifiziert werden; [!DNL Workfront] kann nicht mehr auf den Inhalt des Ordners zugreifen. Dies kann beispielsweise der Fall sein, wenn der Benutzer, der den Ordner ursprünglich verknüpft hat, das Unternehmen verlässt.

Um einen kontinuierlichen Zugriff sicherzustellen, muss ein Benutzer mit Zugriff auf den Ordner den Ordner erneut verknüpfen.

Informationen zum Verknüpfen von Ordnern von externen Anbietern finden Sie unter [Verknüpfen von Dokumenten mit externen Anwendungen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<!--

### Problem: I see a "404 not found" error when attempting to add a document from [!DNL Sharepoint]

#### Solution:

This error might occur if one of the sites configured in the [!UICONTROL Visible Site Collections] list has been deleted in Sharepoint. Check the [!UICONTROL Visible Site Collections] list, and remove any sites that have been deleted in Sharepoint.-->