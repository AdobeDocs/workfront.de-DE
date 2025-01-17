---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Verbinden [!DNL Adobe Workfront Fusion] mit [!DNL Google Services] mithilfe eines benutzerdefinierten OAuth-Clients
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 0%

---

# Verbinden von [!DNL Adobe Workfront Fusion] mit [!DNL Google Services] mithilfe eines benutzerdefinierten OAuth-Clients

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Verbinden von Adobe Workfront Fusion mit Google Services mithilfe eines benutzerdefinierten OAuth-Clients](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/connect-fusion-to-google-using-oauth.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: [!UICONTROL Standard]</p><p>Oder</p><p>Aktuell: [!UICONTROL Work] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Lizenz **</td> 
   <td>
   <p>Aktuell: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy: Beliebig </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Neu:</p> <ul><li>[!UICONTROL Select] oder [!UICONTROL Prime] [!DNL Workfront] Plan: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] kaufen.</li><li>[!UICONTROL Ultimate] [!DNL Workfront]: [!DNL Workfront Fusion] ist enthalten.</li></ul>
   <p>Oder</p>
   <p>Aktuell: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Sie benötigen ein vorhandenes [!DNL Google]-Konto, um diese Verbindung herzustellen.

## Verbinden von Fusion mit Google-Services mithilfe eines benutzerdefinierten OAuth-Clients

Um diese Verbindung zu erstellen, müssen Sie ein Projekt auf Google Cloud Platform erstellen und konfigurieren und dann die Verbindung in Fusion basierend auf diesem Projekt konfigurieren.

* [Erstellen Sie ein Projekt in [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform)
* [Konfigurieren der [!UICONTROL OAuth-Einverständnis]-Einstellungen](#configure-oauth-consent-settings)
* [OAuth-Anmeldedaten erstellen](#create-oauth-credentials)
* [Verbindung mit  [!DNL Google]  herstellen [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion)

>[!NOTE]
>
>Dieses Verfahren ist für Folgendes gedacht:
>
>* Persönlicher Gebrauch ([!DNL `@gmail.com`] und [!DNL `@googlemail.com`])
>* Interne Verwendung ([!DNL Google Workspace] Benutzer, die einen benutzerdefinierten OAuth-Client verwenden möchten)

### Erstellen eines Projekts in [!DNL Google Cloud Platform]

So erstellen Sie ein Projekt in [!DNL Google Cloud] Platform:

1. Melden Sie sich mit Ihren [!DNL Google] Anmeldeinformationen bei [[!DNL Google Cloud] Platform](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) an.
1. Klicken Sie im linken Bedienfeld auf **[!UICONTROL Dashboard]**.
1. Klicken **[!UICONTROL oben rechts]** Bildschirm auf „Projekt erstellen“.
1. Geben Sie den **[!UICONTROL Projektnamen]** ein und klicken Sie dann auf **[!UICONTROL Erstellen]**.

1. Klicken Sie auf **[!UICONTROL APIs und Services aktivieren]** oben im Bildschirm.
1. Geben **[!UICONTROL oben im Bildschirm im Feld „Nach APIs und]** suchen“ den Namen des Services ein, den Sie verwenden möchten (z. B. [!DNL Gmail] API oder [!DNL Google Drive] API).
1. Wenn sie angezeigt wird, klicken Sie auf die API oder den Service, mit der bzw. dem Sie eine Verbindung herstellen [!DNL Workfront Fusion].
1. Klicken Sie auf **[!UICONTROL Aktivieren]**, um die ausgewählte API zu aktivieren.
1. Wiederholen Sie die Schritte 6-8 für jede API, die Sie aktivieren möchten.

   >[!NOTE]
   >
   >Sie müssen [!DNL Google Drive] API sowie die API aller [!DNL Google] Apps aktivieren, die Sie verwenden möchten (z. B. [!DNL Google Sheets] API).

1. Klicken Sie auf dem angezeigten Bildschirm **[!UICONTROL Anmeldedaten erstellen]** in der oberen rechten Ecke.
1. Fahren Sie mit dem Abschnitt [Konfigurieren der OAuth-](#configure-oauth-consent-settings)&quot; in diesem Artikel fort.

### Konfigurieren der [!UICONTROL OAuth-]-Einstellungen

1. Klicken Sie im linken Bedienfeld auf **[!UICONTROL OAuth-Einverständnisbildschirm]**.
1. Wählen Sie **[!UICONTROL Extern]** aus und klicken Sie dann auf **[!UICONTROL Erstellen]**.

   >[!NOTE]
   >
   >Bei Auswahl dieser Option fallen keine Gebühren an. Weitere Informationen finden Sie in den [!DNL Google] zu Ausnahmen von den Prüfanforderungen.

1. Füllen Sie die erforderlichen Felder wie folgt aus:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App-Name]</p> </td> 
      <td> <p>Geben Sie den Namen der App ein, die um Zustimmung bittet.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL E-Mail zur Benutzerunterstützung]</td> 
      <td>Geben Sie eine E-Mail-Adresse ein, an die sich Benutzer bei Fragen zu ihrem Einverständnis wenden können, wenn sie eine Verbindung zu dieser App herstellen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL E-Mail-Adressen]</td> 
      <td>Geben Sie eine oder mehrere E-Mail-Adressen ein, die Google verwenden kann, um Sie über Änderungen an Ihrem Projekt zu informieren.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken [!UICONTROL  unter &quot;] Domains“ auf **[!UICONTROL Domain hinzufügen]** und geben Sie `workfrontfusion.com` ein.

1. Klicken Sie **[!UICONTROL Speichern und fortfahren]**.
1. Klicken Sie **[!UICONTROL Bereiche hinzufügen oder entfernen]**.
1. Aktivieren Sie im rechten Bedienfeld die folgenden Bereiche:

<table style="table-layout:auto">
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Service/API</th> 
      <th>Erforderliche Bereiche</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p>[!DNL Gmail]</p> </td> 
      <td> <p>https://mail.google.com/</p> <p>https://www.googleapis.com/auth/gmail.labels</p> <p>https://www.googleapis.com/auth/gmail.send</p> <p>https://www.googleapis.com/auth/gmail.readonly</p> <p>https://www.googleapis.com/auth/gmail.compose</p> <p>https://www.googleapis.com/auth/gmail.insert</p> <p>https://www.googleapis.com/auth/gmail.modify</p> <p>https://www.googleapis.com/auth/gmail.metadata</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!DNL Google Drive]</p> </td> 
      <td> <p>https://www.googleapis.com/auth/drive</p> <p>https://www.googleapis.com/auth/drive.readonly</p> </td> 
     </tr> 
    </tbody> 
   </table>

Möglicherweise müssen Sie die Liste erweitern oder zur nächsten Seite der Liste gehen, um alle Einträge anzuzeigen.

1. Klicken Sie auf **[!UICONTROL Aktualisieren]**.
1. Klicken Sie **[!UICONTROL Speichern und fortfahren]**.
1. (Optional) Fügen Sie dem Projekt Testbenutzer hinzu.
1. Klicken Sie **[!UICONTROL Speichern und fortfahren]**.
1. Überprüfen Sie Ihre Informationen auf Genauigkeit und klicken Sie dann auf **[!UICONTROL Zurück zum Dashboard]**.

   >[!NOTE]
   >
   >Sie müssen Ihren Einverständnisbildschirm und Ihren Antrag nicht zur Verifizierung durch [!DNL Google] einreichen.

1. Fahren Sie fort [OAuth-Anmeldeinformationen erstellen](#create-oauth-credentials).

### OAuth-Anmeldedaten erstellen

1. Klicken Sie im linken Bedienfeld auf **[!UICONTROL Anmeldedaten]**.

   >[!NOTE]
   >
   >Wenn dies nicht die erste API oder der erste Service ([!DNL Gmail] oder [!DNL Google Drive]) ist, die bzw. den Sie aktiviert haben, müssen Sie keine neuen Anmeldeinformationen erstellen.

1. Klicken Sie **[!UICONTROL oben]** Bildschirm auf „Anmeldeinformationen erstellen“ und wählen Sie dann **[!UICONTROL OAuth Client ID]** aus dem Dropdown-Menü aus.

1. Füllen Sie die erforderlichen Felder wie folgt aus:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Anwendungstyp]</td> 
      <td> <p> [!UICONTROL Web-Anwendung]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>[!DNL Workfront Fusion] </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken [!UICONTROL  unter „Autorisierte Umleitungs]URIs“ auf **[!UICONTROL URI hinzufügen]** und geben Sie **einen** der folgenden Werte ein:

   * Für [!DNL Gmail] oder [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * Für andere [!DNL Google] Apps: `https://app.workfrontfusion.com/oauth/cb/google`

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

   Die [!UICONTROL Client-ID] und [!UICONTROL Client-]) werden angezeigt.

1. Kopieren Sie [!UICONTROL Client-ID] und [!UICONTROL Client-Geheimnis] an einen sicheren Speicherort. Sie werden sie verwenden, um in [!DNL Workfront Fusion] eine Verbindung herzustellen.
1. Fahren Sie fort [Verbinden mit [!DNL Google] in [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

### Verbindung zu [!DNL Google] in [!DNL Workfront Fusion] herstellen

Der Prozess der Erstellung einer Verbindung zu [!DNL Google] unterscheidet sich, je nachdem, ob Sie ein Modul aus einem [!DNL Google]-Service (z. B. [!DNL Google Sheets] oder [!DNL Google Docs]) verwenden oder ob Sie eine Verbindung zu [!DNL Google] über das [!UICONTROL HTTP] >[!UICONTROL Erstellen eines OAuth2.0]-Anfragemoduls herstellen.

* [Verbindung mit  [!DNL Google] in einem [!DNL Google] Service herstellen](#connect-to-google-in-a-google-service)
* [Stellen Sie eine Verbindung  [!DNL Google]  dem Modul [!UICONTROL HTTP] > [!UICONTROL OAuth2.0-Anfrage ].](#connect-to-google-in-the-http--make-an-oauth20-request-module)

#### Herstellen einer Verbindung zu [!DNL Google] in einem [!DNL Google] Service

1. Suchen Sie in [!DNL Workfront Fusion] das [!DNL Google], für das Sie eine Verbindung erstellen müssen.
1. Klicken Sie **[!UICONTROL Verbindung erstellen]** und anschließend auf **[!UICONTROL Erweiterte Einstellungen anzeigen]**.

1. Geben Sie die [!UICONTROL Client-ID] und [!UICONTROL Client-Geheimnis], die Sie unter [[!UICONTROL OAuth-Anmeldeinformationen erstellen]](#create-oauth-credentials) in den entsprechenden Feldern abgerufen haben, und klicken Sie dann auf **[!UICONTROL Weiter]**.

1. Melden Sie sich mit Ihrem [!DNL Google] Konto an.

   Das Fenster **[!UICONTROL Diese App ist nicht verifiziert]** wird angezeigt. Beachten Sie, dass die im Fenstertitel erwähnte „App“ der OAuth-Client ist, den Sie oben erstellt haben.

1. Klicken Sie auf **[!UICONTROL Erweitert]** und dann auf **[!UICONTROL Wechseln zu [!DNL Workfront Fusion] (unsicher)]**, um den Zugriff mit Ihrem benutzerdefinierten OAuth-Client zu ermöglichen.

1. Klicken Sie **[!UICONTROL Zulassen]**, um [!DNL Workfront Fusion] Berechtigung zu erteilen.
1. Klicken Sie im angezeigten Fenster erneut auf **[!UICONTROL Zulassen]**, um Ihre Auswahl zu bestätigen.

   Die Verbindung zum gewünschten [!DNL Google]-Service mithilfe eines benutzerdefinierten OAuth-Clients wird hergestellt.

#### Stellen Sie eine Verbindung zu [!DNL Google] im Modul [!UICONTROL HTTP] > [!UICONTROL OAuth2.0-Anfrage] her {#connect-to-google-in-the-http--make-an-oauth20-request-module}

Anweisungen zum Herstellen einer Verbindung zu [!DNL Google] im Modul [!UICONTROL HTTP] > [!UICONTROL OAuth2.0-Anfrage ]erstellen, finden Sie [Anweisungen zum Erstellen einer Verbindung zu [!DNL Google]  im Modul [!UICONTROL HTTP] > [!UICONTROL Erstellen einer OAuth 2.0-Anfrage] [[!UICONTROL  im Modul ](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module)HTTP] > [!UICONTROL Erstellen einer OAuth 2.0-Anfrage]](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## Mögliche Fehlermeldung: [!UICONTROL [403] Zugriff nicht konfiguriert]

Wenn die [!UICONTROL `403 Access Not Configured`] Fehlermeldung angezeigt wird, müssen Sie die entsprechende API in Ihrer Google Cloud-Plattform aktivieren. Um die API zu aktivieren, führen Sie die Schritte im Abschnitt [Erstellen eines Projekts auf [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) in diesem Artikel aus.
