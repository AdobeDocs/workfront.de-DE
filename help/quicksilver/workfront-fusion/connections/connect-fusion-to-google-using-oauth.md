---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Verbinden von [!DNL Adobe Workfront Fusion] mit [!DNL Google Services] mithilfe eines benutzerdefinierten OAuth-Clients
description: Sie können  [!DNL Adobe Workfront Fusion] verwenden, um mithilfe eines benutzerdefinierten OAuth-Clients eine Verbindung zu  [!DNL Google Services]  herzustellen. Für dieses Verfahren ist ein vorhandenes [!DNL Google] Konto erforderlich.
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# Verbinden von [!DNL Adobe Workfront Fusion] mit [!DNL Google Services] mithilfe eines benutzerdefinierten OAuth-Clients

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: [!UICONTROL Standard]</p><p>Oder</p><p>Aktuell: [!UICONTROL Arbeit] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Aktuell: Keine [!DNL Workfront Fusion] Lizenzanforderung.</p>
   <p>Oder</p>
   <p>Veraltet: Beliebig </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Neu:</p> <ul><li>[!UICONTROL Select] oder [!UICONTROL Prime] [!DNL Workfront] Plan: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben.</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] ist enthalten.</li></ul>
   <p>Oder</p>
   <p>Aktuell: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] kaufen.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Sie benötigen ein vorhandenes [!DNL Google] -Konto, um diese Verbindung herzustellen.

## Verbinden von Fusion mit Google-Diensten mit einem benutzerdefinierten OAuth-Client

Um diese Verbindung herzustellen, müssen Sie ein Projekt auf der Google Cloud-Plattform erstellen und konfigurieren und dann die Verbindung in Fusion auf der Grundlage dieses Projekts konfigurieren.

* [Erstellen eines Projekts auf  [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform)
* [Konfigurieren von [!UICONTROL OAuth-Einverständniseinstellungen] Einstellungen](#configure-oauth-consent-settings)
* [OAuth-Anmeldedaten erstellen](#create-oauth-credentials)
* [Mit [!DNL Google] in [!DNL Workfront Fusion] verbinden](#connect-to-google-in-workfront-fusion)

>[!NOTE]
>
>Dieses Verfahren dient folgenden Zwecken:
>
>* Persönliche Nutzung ([!DNL `@gmail.com`] - und [!DNL `@googlemail.com`] -Benutzer)
>* Interne Verwendung ([!DNL Google Workspace] Benutzer, die einen benutzerdefinierten OAuth-Client bevorzugen)

### Erstellen eines Projekts auf [!DNL Google Cloud Platform]

So erstellen Sie ein Projekt auf der [!DNL Google Cloud]-Plattform:

1. Melden Sie sich mit Ihren [!DNL Google] -Anmeldedaten bei [[!DNL Google Cloud] Platform](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) an.
1. Klicken Sie im linken Bereich auf **[!UICONTROL Dashboard]**.
1. Klicken Sie oben rechts im Bildschirm auf **[!UICONTROL Projekt erstellen]** .
1. Geben Sie den **[!UICONTROL Projektnamen]** ein und klicken Sie dann auf **[!UICONTROL Erstellen]**.

1. Klicken Sie oben im Bildschirm auf die Registerkarte **[!UICONTROL APIs und Dienste aktivieren]** .
1. Geben Sie im Feld **[!UICONTROL Suche nach APIs und Services]** oben im Bildschirm den Namen des zu verwendenden Dienstes ein (z. B. [!DNL Gmail] API oder [!DNL Google Drive] API).
1. Klicken Sie beim Anzeigen auf die API oder den Dienst, mit der/dem Sie eine Verbindung herstellen möchten, mit [!DNL Workfront Fusion].
1. Klicken Sie auf **[!UICONTROL Aktivieren]** , um die ausgewählte API zu aktivieren.
1. Wiederholen Sie die Schritte 6 bis 8 für jede API, die Sie aktivieren möchten.

   >[!NOTE]
   >
   >Sie müssen die [!DNL Google Drive] -API sowie die API aller [!DNL Google]-Apps aktivieren, die Sie verwenden möchten (z. B. die [!DNL Google Sheets] -API).

1. Klicken Sie im angezeigten Bildschirm oben rechts auf **[!UICONTROL Anmeldeinformationen erstellen]** .
1. Fahren Sie mit dem Abschnitt [OAuth-Zustimmungseinstellungen konfigurieren](#configure-oauth-consent-settings) in diesem Artikel fort.

### Einstellungen für [!UICONTROL OAuth-Einverständnis] konfigurieren

1. Klicken Sie im linken Bereich auf den Bildschirm **[!UICONTROL OAuth-Einverständnisbildschirm]**.
1. Wählen Sie **[!UICONTROL External]** und klicken Sie dann auf **[!UICONTROL Erstellen]**.

   >[!NOTE]
   >
   >Bei Auswahl dieser Option werden Ihnen keine Gebühren berechnet. Weitere Informationen finden Sie in den Informationen von [!DNL Google] zu Ausnahmen von den Überprüfungsanforderungen.

1. Füllen Sie die erforderlichen Felder wie folgt aus:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App name]</p> </td> 
      <td> <p>Geben Sie den Namen der App ein, um die Zustimmung einzuholen.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL E-Mail zur Benutzerunterstützung]</td> 
      <td>Geben Sie eine E-Mail-Adresse ein, an die Benutzer Sie bei Fragen zur Einwilligung beim Herstellen einer Verbindung mit dieser App kontaktieren können.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL E-Mail-Adressen]</td> 
      <td>Geben Sie eine oder mehrere E-Mail-Adressen ein, über die Google Sie über Änderungen an Ihrem Projekt benachrichtigen kann.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie unter [!UICONTROL Autorisierte Domänen] auf **[!UICONTROL Domäne hinzufügen]** und geben Sie `workfrontfusion.com` ein.

1. Klicken Sie auf **[!UICONTROL Speichern und fortfahren]**.
1. Klicken Sie auf **[!UICONTROL Bereiche hinzufügen oder entfernen]**.
1. Aktivieren Sie im rechten Bereich die folgenden Bereiche:

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

Möglicherweise müssen Sie die Liste erweitern oder zur nächsten Seite der Liste wechseln, um alle anzuzeigen.

1. Klicken Sie auf **[!UICONTROL Aktualisieren]**.
1. Klicken Sie auf **[!UICONTROL Speichern und fortfahren]**.
1. (Optional) Fügen Sie dem Projekt beliebige Testbenutzer hinzu.
1. Klicken Sie auf **[!UICONTROL Speichern und fortfahren]**.
1. Überprüfen Sie Ihre Informationen auf ihre Richtigkeit und klicken Sie dann auf **[!UICONTROL Zurück zum Dashboard]**.

   >[!NOTE]
   >
   >Sie müssen Ihren Einverständnisbildschirm und den Antrag nicht zur Überprüfung durch [!DNL Google] einreichen.

1. Fahren Sie mit [OAuth-Anmeldedaten erstellen](#create-oauth-credentials) fort.

### OAuth-Anmeldedaten erstellen

1. Klicken Sie im linken Bereich auf **[!UICONTROL Anmeldedaten]**.

   >[!NOTE]
   >
   >Wenn dies nicht die erste API oder der erste Dienst ([!DNL Gmail] oder [!DNL Google Drive]) ist, die Sie aktiviert haben, müssen Sie keine neuen Anmeldeinformationen erstellen.

1. Klicken Sie oben im Bildschirm auf **[!UICONTROL Anmeldeinformationen erstellen]** und wählen Sie dann **[!UICONTROL OAuth-Client-ID]** aus dem Dropdown-Menü aus.

1. Füllen Sie die erforderlichen Felder wie folgt aus:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Anwendungstyp]</td> 
      <td> <p> [!UICONTROL Webanwendung]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>[!DNL Workfront Fusion] </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie unter &quot;[!UICONTROL Autorisierte Umleitungs-URIs]&quot;auf &quot;**[!UICONTROL URI hinzufügen]**&quot;und geben Sie &quot;**one**&quot;ein:

   * Für [!DNL Gmail] oder [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * Für andere [!DNL Google] -Apps: `https://app.workfrontfusion.com/oauth/cb/google`

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

   Die Anzeige [!UICONTROL Client-ID] und [!UICONTROL Client-Geheimnis] wird angezeigt.

1. Kopieren Sie die [!UICONTROL Client-ID] und den [!UICONTROL Client-Geheimnis] an einen sicheren Speicherort. Sie werden sie verwenden, um eine Verbindung in [!DNL Workfront Fusion] herzustellen.
1. Fahren Sie mit [Verbinden mit [!DNL Google] in [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion) fort.

### Mit [!DNL Google] in [!DNL Workfront Fusion] verbinden

Der Prozess der Erstellung einer Verbindung zu [!DNL Google] hängt davon ab, ob Sie ein Modul aus einem [!DNL Google] -Dienst (z. B. [!DNL Google Sheets] oder [!DNL Google Docs]) verwenden oder ob Sie eine Verbindung zu [!DNL Google] über das Anforderungsmodul [!UICONTROL HTTP] >[!UICONTROL Erstellen einer OAuth2.0] herstellen.

* [Verbindung zu [!DNL Google] in einem [!DNL Google] Dienst herstellen](#connect-to-google-in-a-google-service)
* [Stellen Sie eine Verbindung zu [!DNL Google] im Modul [!UICONTROL HTTP] > [!UICONTROL Erstellen einer OAuth2.0-Anfrage] her.](#connect-to-google-in-the-http--make-an-oauth20-request-module)

#### Mit [!DNL Google] in einem [!DNL Google]-Dienst verbinden

1. Suchen Sie in [!DNL Workfront Fusion] das Modul [!DNL Google], für das Sie eine Verbindung erstellen müssen.
1. Klicken Sie auf **[!UICONTROL Verbindung erstellen]** und dann auf **[!UICONTROL Erweiterte Einstellungen anzeigen]**.

1. Geben Sie die [!UICONTROL Client-ID] und den [!UICONTROL Client-Geheimnis] ein, die Sie in den Feldern unter [[!UICONTROL OAuth-Anmeldedaten erstellen]](#create-oauth-credentials) abgerufen haben, und klicken Sie dann auf **[!UICONTROL Weiter]**.

1. Melden Sie sich mit Ihrem [!DNL Google] -Konto an.

   Das Fenster **[!UICONTROL Diese App ist nicht verifiziert]** wird angezeigt. Beachten Sie, dass die im Fenstertitel erwähnte &quot;App&quot;der OAuth-Client ist, den Sie oben erstellt haben.

1. Klicken Sie auf **[!UICONTROL Erweitert]** und dann auf **[!UICONTROL Gehe zu [!DNL Workfront Fusion] (unsafe)]**, um den Zugriff über Ihren benutzerdefinierten OAuth-Client zu ermöglichen.

1. Klicken Sie auf **[!UICONTROL Zulassen]** , um [!DNL Workfront Fusion] Berechtigung zu erteilen.
1. Klicken Sie im sich öffnenden Fenster erneut auf **[!UICONTROL Zulassen]** , um Ihre Auswahl zu bestätigen.

   Die Verbindung zum gewünschten [!DNL Google]-Dienst mithilfe eines benutzerdefinierten OAuth-Clients wird hergestellt.

#### Stellen Sie eine Verbindung zu [!DNL Google] im Modul [!UICONTROL HTTP] > [!UICONTROL Erstellen einer OAuth2.0-Anfrage] her. {#connect-to-google-in-the-http--make-an-oauth20-request-module}

Anweisungen zum Herstellen einer Verbindung zu [!DNL Google] im Modul [!UICONTROL HTTP] > [!UICONTROL Erstellen einer OAuth2.0-Anforderung] finden Sie unter [Anweisungen zum Erstellen einer Verbindung zu  [!DNL Google] im Modul [!UICONTROL HTTP] > [!UICONTROL Erstellen einer OAuth 2.0-Anforderung] im Modul [[!UICONTROL HTTP] > 14}Erstellen Sie eine OAuth 2.0-Anfrage] -Modul](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module)[!UICONTROL 

## Mögliche Fehlermeldung:[!UICONTROL [403] Zugriff nicht konfiguriert]

Wenn die Fehlermeldung [!UICONTROL `403 Access Not Configured`] angezeigt wird, müssen Sie die entsprechende API in Ihrer Google Cloud-Plattform aktivieren. Um die API zu aktivieren, führen Sie die Schritte im Abschnitt [Projekt erstellen am [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) in diesem Artikel aus.
