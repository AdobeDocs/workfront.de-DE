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
source-git-commit: 15aa025c9a35e30867f942047ec1989fdd6834e5
workflow-type: tm+mt
source-wordcount: '2517'
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
>* Die neue SharePoint-Integration erfordert keine Konfiguration durch einen Administrator und kann von einzelnen Benutzern eingerichtet werden. Um jedoch einen reibungslosen Übergang zur neuen SharePoint-Integration sicherzustellen, muss ein Workfront-Administrator einige kleine Änderungen an den Einstellungen im Workfront-Setup-Bereich vornehmen.
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


## Konfigurieren der alten SharePoint-Integration für den kontinuierlichen Zugriff auf Dokumente

Um sicherzustellen, dass Ihre Benutzer über die veraltete SharePoint-Integration weiterhin auf mit Workfront verknüpfte Dokumente zugreifen können, müssen Sie den Zugriff auf die veraltete SharePoint-Integration neu konfigurieren und den SharePoint-Client-Geheimnisschlüssel auf dem neuesten Stand halten.

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



## Anleitung zum Einrichten der alten SharePoint-Integration

>[!IMPORTANT]
>
>Diese Integration wird nicht mehr unterstützt. Die Anweisungen dienen nur zur Information und werden in naher Zukunft entfernt.


Workfront stellt Verbindungen her [!DNL SharePoint] Online mit OAuth 2.0, einem Standard, der von den meisten webbasierten Integrationen für die Authentifizierung und Autorisierung von Benutzern verwendet wird.

Um OAuth zu konfigurieren, müssen Sie eine [!DNL SharePoint] Site und eine Site-App in [!DNL SharePoint]. Dieser Vorgang wird in den folgenden Abschnitten beschrieben.

Weitere Informationen zu OAuth finden Sie unter [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>So können Sie Informationen einfach kopieren und einfügen zwischen [!DNL Workfront] und [!DNL SharePoint] In diesen Schritten wird empfohlen, beide Anwendungen in separaten Tabs offen zu halten.

* [Erstellen und konfigurieren Sie eine [!DNL SharePoint] site](#create-and-configure-a-sharepoint-site)
* [Schreibberechtigungen für die Site-App gewähren](#grant-write-permissions-to-the-site-app)
* [Erstellen Sie eine [!DNL Workfront] [!DNL SharePoint] Integrationsinstanz](#create-a-workfront-sharepoint-integration-instance)
* [Integration abschließen](#complete-your-integration)
* [Dokumente hinzufügen](#add-documents)

### Erstellen und konfigurieren Sie eine [!DNL SharePoint] site  {#create-and-configure-a-sharepoint-site}

Zur [!DNL Workfront] zum Authentifizieren mit [!DNL SharePoint], [!DNL Workfront] kann eine Übergeordnete Site verwenden, auf der Benutzer über die [!UICONTROL Vollständige Kontrolle] Berechtigungsebene oder spezifische Berechtigungen verwalten. Diese Übergeordnete Site dient als Authentifizierungs-Einstiegspunkt für [!DNL Workfront].

So erstellen und konfigurieren Sie eine [!DNL SharePoint] Site:

1. (Optional) Wenn Sie die Stammsite Ihres Unternehmens nicht verwenden möchten, können Sie eine Übergeordnete Site in [!DNL SharePoint].

   Anweisungen finden Sie unter [Erstellen einer Site](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) im [!DNL Microsoft] Dokumentation.

   * Wählen Sie die **[!UICONTROL Team-Site]** bei der Erstellung der Site.

1. (Bedingt) Wenn Sie in Schritt 1 eine Site erstellt haben, gehen Sie zur soeben erstellten Site.

   Oder

   Wenn Sie in Schritt 1 keine Site erstellt haben, gehen Sie zur Stammsite Ihres Unternehmens.

1. Hinzufügen `/_layouts/15/appregnew.aspx` an das Ende der URL in der Suchleiste am oberen Rand des Browser-Fensters.
1. Konfigurieren Sie die folgenden Felder:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client-ID]</p> </td> 
      <td> <p>Klicken <strong>[!UICONTROL Generate]</strong> , um eine Client-ID zu generieren. Kopieren Sie diese ID an einen sicheren Speicherort. Sie werden sie später bei der Einrichtung der [!DNL SharePoint] Integration in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client Secret]</p> </td> 
      <td> <p>Klicken <strong>[!UICONTROL Generate]</strong> , um ein Client-Geheimnis zu generieren. Kopieren Sie dieses Geheimnis an einen sicheren Speicherort. Sie werden sie später bei der Einrichtung der [!DNL SharePoint] Integration in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Titel</p> </td> 
      <td> <p>Geben Sie einen Titel ein, z. B. [!DNL Workfront] Site-App. Benutzer sehen diesen Titel beim Hinzufügen von Dokumenten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App Domain]</p> </td> 
      <td> <p><code>my.workfront.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Weiterleitungs-URI]</p> </td> 
      <td> <p><code>https://oauth.my.workfront.com/oauth2/redirect</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **[!UICONTROL Erstellen]**
1. Weiter zu [Schreibberechtigungen für die Site-App gewähren](#grant-write-permissions-to-the-site-app).

### Schreibberechtigungen für die Site-App gewähren  {#grant-write-permissions-to-the-site-app}

An dieser Stelle haben Sie erfolgreich eine Site-App erstellt und in [!DNL Workfront]. Diese Site-App wird auch als App-Prinzipal in [!DNL SharePoint]. Sie befindet sich in Ihrem Mandanten. Neue Site-Apps haben nicht automatisch Zugriff auf Site-Sammlungen innerhalb des Mandanten. Berechtigungen müssen explizit für jede Site-Sammlung erteilt werden. Die folgenden Schritte zeigen Ihnen, wie Sie der neuen Site-App eine Site-Sammlung Schreibberechtigung erteilen. Wiederholen Sie diese Schritte für die einzelnen Website-Sammlungen, die Sie unter [!UICONTROL Sichtbare Site-Sammlungen] in den obigen Schritten beschrieben.

Diese Site-App muss [!UICONTROL Schreiben] Zugriff auf alle Site-Sammlungen, auf die Benutzer über zugreifen müssen [!DNL Workfront].

1. Fügen Sie &quot;/_layouts/15/appinv.aspx&quot;zur URL in [!DNL Sharepoint].

   **Beispiel:**

   ```
   https://mycompany.sharepoint.com/sites/mysite/_layouts/15/appinv.aspx
   ```

1. Konfigurieren Sie die folgenden Felder

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL App ID]</td> 
      <td> <p>Fügen Sie die Client-ID hinzu, die Sie in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Erstellen und konfigurieren Sie eine [!DNL SharePoint] site </a>und klicken Sie auf <strong>[!UICONTROL Lookup]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client] / [!UICONTROL App Domain] / [!UICONTROL Weiterleitungs-URL]</p> </td> 
      <td> <p>Diese werden automatisch ausgefüllt, wenn Sie auf [!UICONTROL Lookup] klicken.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Berechtigungsanfrage XML]</td> 
      <td> <p>Kopieren Sie die folgende XML in das Feld [!UICONTROL Permission Request XML] . Stellen Sie sicher, dass sie genau so hinzugefügt wird, wie sie ohne zusätzliche Leerzeichen usw. angezeigt wird. um Fehler zu vermeiden.</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre></pre></div></div></td></tr></tbody></table>

1. Klicken Sie auf **[!UICONTROL Erstellen]**.
1. Klicken Sie im angezeigten Dialogfeld auf **[!UICONTROL Vertrauen]**.
1. Stellen Sie sicher, dass die Site-App Zugriff auf die Site-Sammlung hat, indem Sie auf die **[!UICONTROL Berechtigungen für Site-Sammlungs-Apps]** Link in [!UICONTROL Site-Einstellungen].
1. Wiederholen Sie die obigen Schritte für die verbleibenden Site-Sammlungen und fahren Sie dann mit [Erstellen Sie eine [!DNL Workfront] [!DNL SharePoint] Integrationsinstanz](#create-a-workfront-sharepoint-integration-instance).

### Erstellen Sie eine [!DNL Workfront] [!DNL SharePoint] Integrationsinstanz {#create-a-workfront-sharepoint-integration-instance}

Wenn Sie eine Site-App in [!DNL SharePoint]können Sie jetzt Informationen aus der Site-App in [!DNL Workfront]. Die Site-App ist ein App-Prinzipal und fungiert als Kanal, über den OAuth-Anfragen für den Zugriff auf Dokumente in Site-Sammlungen gesendet werden.

1. Anmelden [!DNL Workfront] als Administrator.
1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **[!UICONTROL Dokumente]** > **[!UICONTROL [!DNL SharePoint]Integration]**.
1. Klicken **[!UICONTROL Hinzufügen[!DNL SharePoint]]**.
1. Konfigurieren Sie die folgenden Felder:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Name]</p> </td> 
      <td> <p>Geben Sie einen Namen für die [!DNL SharePoint] Integration. Benutzer sehen diesen Namen, wenn sie auf [!UICONTROL Hinzufügen] &gt; [!UICONTROL Aus] "Name der Integration"klicken. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] Host Instance]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] Zugriffsdomäne]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>Dies bezieht sich auf die Übergeordnete Site, über die sich Benutzer authentifizieren. Wahrscheinlich ist es dieselbe Domäne wie [!UICONTROL [!DNL SharePoint] Hostinstanz].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>Wichtig</b> Site-Sammlungen werden nur in der alten Version verwendet [!DNL SharePoint] Integration.
       <ul> 
        <li> <p><b>Wenn Sie die Stammsite Ihres Unternehmens verwenden</b><b>:</b> </p> <p>Eingabe <code>/</code></p> </li> 
        <li> <p><b>Wenn Sie eine Übergeordnete Site und Untersites verwenden:</b> </p> <p><b>WICHTIG</b>: [!DNL Microsoft SharePoint] empfiehlt nicht mehr die Verwendung von Subsites.</p> <p>Geben Sie den URL-Stamm für die Site-Sammlung ein, die Sie oben im Abschnitt erstellt haben.</p> <p>Dies ist der Abschnitt der URL nach .com.</p> <p>Beispiel: für die URL <code>https://mycompany.sharepoint.com/sites/mysite</code>, würde der Stamm <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Client-ID]</td> 
      <td>Geben Sie die Client-ID ein, die Sie in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Erstellen und konfigurieren Sie eine [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Client Secret]</td> 
      <td>Geben Sie den Client-Geheimnis ein, den Sie in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Erstellen und konfigurieren Sie eine [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Sichtbare Site-Sammlungen]</td> 
      <td> <b>Wichtig</b> Site-Sammlungen werden nur in der alten Version verwendet [!DNL SharePoint] Integration.
       <ul> 
        <li> <p><b> Wenn Sie die Stammsite Ihres Unternehmens verwenden</b><b>:</b> </p> <p>Eingabe <code>/</code></p> </li> 
        <li> <p><b>Wenn Sie eine Übergeordnete Site und Untersites verwenden:</b> </p> <p><b>WICHTIG</b>: [!DNL Microsoft SharePoint] empfiehlt nicht mehr die Verwendung von Subsites.</p> <p>Für jede Subsite, die Sie zu Ihrer [!DNL SharePoint] -Integration, geben Sie den Stamm der Subsite ein.</p> <p>Beispiel: für die URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, würde der Stamm <code>/sites/mysite/mysubsite</code>.</p> <p><b>NOTIZ</b>:   <p>Wenn Sie nur Ihre Konfiguration testen möchten (keine Unterseiten), geben Sie den Stamm der Übergeordneten Site ein. </p> <p>Beispiel: für die URL <code> https://mycompany.sharepoint.com/sites/mysite</code>, würde der Stamm <code>/sites/mysite</code>.</p> <p>Wenn Sie Ihre Konfiguration wie unter <a href="#complete-your-integration" class="MCXref xref">Integration abschließen</a>, müssen Sie die Übergeordnete Site entfernen und die Unterseiten eingeben.</p> 
          <ol> 
           <li value="1">Klicken Sie auf <strong>[!UICONTROL Hauptmenü]</strong> icon <img src="assets/main-menu-icon.png"> in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf <strong>[!UICONTROL Setup]</strong> <img src="assets/gear-icon-settings.png">.<li><p>Klicken Sie im linken Bereich auf <strong>[!UICONTROL Dokumente]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] Integration]</strong>.</p></li><li><p>Klicken Sie auf [!DNL SharePoint] Integration, die Sie einrichten, und klicken Sie dann auf Bearbeiten.</p></li><li><p>Löschen Sie den Stamm für die Übergeordnete Site aus dem Feld [!UICONTROL Sichtbare Site-Sammlungen] .</p></li><li><p>Für jede Subsite, die Sie zu Ihrer [!DNL SharePoint] -Integration, geben Sie den Stamm der Subsite ein.</p></li><p>Beispiel: für die URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, würde der Stamm <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Speichern]**
1. Weiter zu [Integration abschließen](#complete-your-integration).

### Integration abschließen {#complete-your-integration}

Die grundlegende Konfiguration ist fast abgeschlossen.

1. Klicken Sie in Workfront auf die **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **[!UICONTROL Dokumente]** ![](assets/document-icon.png).
1. Klicken **[!UICONTROL Neu hinzufügen]**.
1. Klicken **[!UICONTROL Von]`<title of your [!DNL SharePoint] site>`** in der Dropdown-Liste.

   Ein Dialogfeld, in dem Sie aufgefordert werden, dieser Site zu vertrauen, wird angezeigt.

   >[!NOTE]
   >
   >Wenn dieses Dialogfeld nicht angezeigt wird, wird Ihr [!DNL SharePoint] -Integration nicht korrekt konfiguriert ist.

1. Klicken **[!UICONTROL Vertrauen]**.

### Dokumente hinzufügen {#add-documents}

Sie können jetzt Dokumente aus Ihrem [!DNL SharePoint] Site.

Anweisungen finden Sie unter [Externes Dokument verknüpfen zu [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) in [Verknüpfen von Dokumenten mit externen Anwendungen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>Wenn der Benutzer, der einen Ordner verknüpft hat, keinen Zugriff mehr auf die externe Anwendung hat, [!DNL Workfront] kann nicht mehr auf den Inhalt des Ordners zugreifen. Dies kann beispielsweise der Fall sein, wenn der Benutzer, der den Ordner ursprünglich verknüpft hat, das Unternehmen verlässt. Um einen kontinuierlichen Zugriff sicherzustellen, muss ein Benutzer mit Zugriff auf den Ordner den Ordner erneut verknüpfen.

## Fehlerbehebung

* [Problem: Benutzer erhalten bei der Verwendung der Variablen [!DNL SharePoint] Integration.](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [Problem: Als [!DNL Workfront] Benutzer, kann ich keine neue [!DNL SharePoint] -Instanz. Wenn ich versuche, sehe ich einen Fehler.](#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error)
* [Problem: Beim Versuch zu durchsuchen [!DNL SharePoint] Dateien in [!DNL Workfront], sehe ich keine oder alle meiner Site-Sammlungen.](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [Problem: Ich kann nicht auf zuvor verknüpfte Ordner und Dokumente in [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### Problem: Benutzer erhalten bei der Verwendung der Variablen [!DNL SharePoint] Integration. {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

Lösungen:

Benutzer müssen Mitglied einer Gruppe sein, die über die entsprechenden Berechtigungen für die [!DNL SharePoint] Site.

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

### Problem: Als [!DNL Workfront] Benutzer, kann ich keine neue [!DNL SharePoint] -Instanz. Wenn ich versuche, sehe ich einen Fehler. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Lösungen:

Dies kann durch eine Reihe von Dingen verursacht werden, die aus [!DNL Workfront] oder [!DNL SharePoint]-Konfiguration. Stellen Sie sicher, dass:

* Die Felder Client-ID, Client-Geheimnis, URL-Rückgabe und andere Konfigurationsfelder werden zwischen der [!DNL Workfront] [!DNL SharePoint] Integrationsinstanz und [!DNL SharePoint] Site-App.
* Der Benutzer hat [!UICONTROL Vollständige Kontrolle] Zugriff auf die für die Authentifizierung verwendete Site-Sammlung.
* Die Site-App ist unter [!UICONTROL Site-App-Berechtigungen] für [!UICONTROL Site-Sammlung] zur Authentifizierung verwendet.

### Problem: Beim Versuch zu durchsuchen [!DNL SharePoint] Dateien in [!DNL Workfront], sehe ich keine oder alle meiner Site-Sammlungen. {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

Lösungen:

So zeigen Sie eine Site-Sammlung in [!DNL Workfront]müssen folgende Bedingungen erfüllt sein:

* Die Site-Sammlung muss im [!DNL Workfront] [!DNL SharePoint] Integrationsinstanz.

   So überprüfen Sie dies in [!DNL Workfront]:

   1. Navigieren Sie zu [!UICONTROL Einrichtung] > [!UICONTROL Dokumente] > [!UICONTROL [!DNL SharePoint] Integration].
   1. Bearbeiten Sie die [!DNL SharePoint] Informationen zur Integrationsinstanz.
   1. Stellen Sie sicher, dass die Site-Sammlung unter [!UICONTROL Sichtbare Site-Sammlungen].

* Der Benutzer muss Zugriff auf die Site-Sammlung in der [!DNL SharePoint].
* So überprüfen Sie dies in [!DNL SharePoint], gehen Sie zu [!DNL SharePoint]und öffnen Sie die Site-Sammlung > [!UICONTROL Einstellungen] > [!UICONTROL Site-Berechtigungen].
* Die [!DNL SharePoint] Die Site-App muss Zugriff auf die Site-Sammlung haben.

   So überprüfen Sie dies in [!DNL SharePoint]:

   1. Navigieren Sie zur Site-Sammlung > [!UICONTROL Einstellungen] > [!UICONTROL Berechtigungen für Site-Apps].
   1. Stellen Sie sicher, dass [!UICONTROL Site-App] verwendet von [!DNL Workfront] ist hier aufgeführt.
   1. (Bedingt) Wenn die Site-App nicht aufgeführt ist, fügen Sie die Site-Sammlung mit _layouts/15/appinv.aspx hinzu.

      Weitere Informationen zum Hinzufügen der Site-Sammlung finden Sie unter Erteilen von Schreibberechtigungen für die Site-App.

### Problem: Ich kann nicht auf zuvor verknüpfte Ordner und Dokumente in [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

Lösung:

Wenn der Benutzer, der eine [!DNL SharePoint] -Ordner kann nicht mehr authentifiziert werden; [!DNL Workfront] kann nicht mehr auf den Inhalt des Ordners zugreifen. Dies kann beispielsweise der Fall sein, wenn der Benutzer, der den Ordner ursprünglich verknüpft hat, das Unternehmen verlässt.

Um einen kontinuierlichen Zugriff sicherzustellen, muss ein Benutzer mit Zugriff auf den Ordner den Ordner erneut verknüpfen.

Informationen zum Verknüpfen von Ordnern von externen Anbietern finden Sie unter [Verknüpfen von Dokumenten mit externen Anwendungen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Problem: Beim Versuch, ein Dokument hinzuzufügen, wird der Fehler &quot;404 nicht gefunden&quot;angezeigt. [!DNL Sharepoint]

#### Lösung:

Dieser Fehler kann auftreten, wenn eine der im [!UICONTROL Sichtbare Site-Sammlungen] wurde in Sharepoint gelöscht. Überprüfen Sie die [!UICONTROL Sichtbare Site-Sammlungen] und entfernen Sie alle Sites, die in Sharepoint gelöscht wurden.
