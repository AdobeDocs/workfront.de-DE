---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Verbinden [!DNL Adobe Workfront Fusion] nach [!DNL Google Services] Verwenden eines benutzerdefinierten OAuth-Clients
description: Sie können [!DNL Adobe Workfront Fusion] zur Verbindung mit [!DNL Google Services] Verwendung eines benutzerdefinierten OAuth-Clients. Dieses Verfahren erfordert eine vorhandene [!DNL Google] -Konto.
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 0%

---

# Verbinden [!DNL Adobe Workfront Fusion] nach [!DNL Google Services] Verwenden eines benutzerdefinierten OAuth-Clients

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Sie benötigen eine vorhandene [!DNL Google] -Konto erstellen, um diese Verbindung herzustellen.

## Erstellen Sie ein Projekt auf [!DNL Google Cloud Platform]

Das folgende Verfahren ist vorgesehen:

* Persönliche Verwendung ([!DNL @gmail.com] und [!DNL @googlemail.com] Benutzer)
* Interne Verwendung ([!DNL G Suite] Benutzer, die lieber einen benutzerdefinierten OAuth-Client verwenden)

So erstellen Sie ein Projekt in [!DNL Google Cloud] Plattform:

1. Anmelden bei [[!DNL Google Cloud] Plattform](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) mit [!DNL Google] Anmeldedaten.
1. Klicken Sie im linken Bereich auf **[!UICONTROL Dashboard]**.
1. Klicken **[!UICONTROL Projekt erstellen]** in der oberen rechten Ecke des Bildschirms.
1. Geben Sie die **[!UICONTROL Projektname]** Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Klicken Sie auf **[!UICONTROL Aktivieren von APIs und Diensten]** -Registerkarte am oberen Bildschirmrand.
1. Im **[!UICONTROL Suchen nach APIs und Diensten]** Geben Sie oben im Bildschirm den Namen des zu verwendenden Dienstes ein (z. B. [!DNL Gmail] API oder [!DNL Google Drive] API).
1. Klicken Sie bei der Anzeige auf die API oder den Dienst, mit der/dem Sie eine Verbindung herstellen möchten [!DNL Workfront Fusion].
1. Klicken **[!UICONTROL Aktivieren]** , um die ausgewählte API zu aktivieren.
1. Wiederholen Sie die Schritte 6 bis 8 für jede API, die Sie aktivieren möchten.

   >[!NOTE]
   >
   >Sie müssen [!DNL Google Drive] API sowie die API aller [!DNL Google] Apps, die Sie verwenden möchten (z. B. [!DNL Google Sheets] API).

1. Klicken Sie im angezeigten Bildschirm auf **[!UICONTROL Erstellen von Anmeldeinformationen]** in der oberen rechten Ecke.
1. Fahren Sie mit dem Abschnitt fort. [OAuth-Zustimmungseinstellungen konfigurieren](#configure-oauth-consent-settings) in diesem Artikel.

## Konfigurieren [!UICONTROL OAuth-Zustimmung] settings

1. Klicken Sie im linken Bereich auf **[!UICONTROL OAuth-Einverständnisbildschirm]**.
1. Auswählen **[!UICONTROL Externe]** Klicken Sie auf **[!UICONTROL Erstellen]**.

   >[!NOTE]
   >
   >Bei Auswahl dieser Option werden Ihnen keine Gebühren berechnet. Weitere Informationen finden Sie unter [!DNL Google]Informationen über Ausnahmen von den Prüfanforderungen.

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

1. under [!UICONTROL Autorisierte Domänen]klicken **[!UICONTROL Domain hinzufügen]** und geben Sie `workfrontfusion.com`.

1. Klicken **[!UICONTROL Speichern und fortfahren]**.
1. Klicken **[!UICONTROL Bereiche hinzufügen oder entfernen]**.
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

1. Klicken **[!UICONTROL Aktualisieren]**.
1. Klicken **[!UICONTROL Speichern und fortfahren]**.
1. (Optional) Fügen Sie dem Projekt beliebige Testbenutzer hinzu.
1. Klicken **[!UICONTROL Speichern und fortfahren]**.
1. Überprüfen Sie Ihre Informationen auf ihre Richtigkeit und klicken Sie dann auf **[!UICONTROL Zurück zum Dashboard]**.

   >[!NOTE]
   >
   >Sie müssen Ihren Einverständnisbildschirm und Ihren Antrag nicht zur Überprüfung einreichen durch [!DNL Google].

1. Weiter zu [OAuth-Anmeldedaten erstellen](#create-oauth-credentials).

## OAuth-Anmeldedaten erstellen

1. Klicken Sie im linken Bereich auf **[!UICONTROL Anmeldeinformationen]**.

   >[!NOTE]
   >
   >Wenn dies nicht die erste API oder der erste Dienst ist ([!DNL Gmail] oder [!DNL Google Drive]), die Sie aktiviert haben, müssen Sie keine neuen Anmeldedaten erstellen.

1. Klicken **[!UICONTROL Erstellen von Anmeldeinformationen]** Wählen Sie oben im Bildschirm die Option **[!UICONTROL OAuth-Client-ID]** aus dem Dropdown-Menü.

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

1. under [!UICONTROL Autorisierte Umleitungs-URIs]klicken **[!UICONTROL URI hinzufügen]** und eingeben **one** des Folgenden:

   * Für [!DNL Gmail] oder [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * Für andere [!DNL Google] apps: `https://app.workfrontfusion.com/oauth/cb/google`

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

   Die [!UICONTROL Client-ID] und [!UICONTROL Client Secret] angezeigt.

1. Kopieren Sie die [!UICONTROL Client-ID] und [!UICONTROL Client Secret] an einen sicheren Ort. Sie werden sie verwenden, um eine Verbindung mit [!DNL Workfront Fusion].
1. Weiter zu [Verbinden mit [!DNL Google] in [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

## Verbinden mit [!DNL Google] in [!DNL Workfront Fusion]

Der Prozess der Erstellung einer Verbindung zu [!DNL Google] unterscheidet sich je nachdem, ob Sie ein Modul aus einem [!DNL Google] -Dienst(z. B. [!DNL Google Sheets] oder [!DNL Google Docs]) oder wenn Sie eine Verbindung zu [!DNL Google] über die [!UICONTROL HTTP] >[!UICONTROL Erstellen einer OAuth2.0] -Anfragemodul.

* [Verbinden mit [!DNL Google] in [!DNL Google] service](#connect-to-google-in-a-google-service)
* [Verbinden mit [!DNL Google] im [!UICONTROL HTTP] > [!UICONTROL OAuth2.0-Anfrage stellen] Modul](#connect-to-google-in-the-http--make-an-oauth20-request-module)

### Verbinden mit [!DNL Google] in [!DNL Google] service

1. In [!DNL Workfront Fusion], suchen Sie die [!DNL Google] -Modul, für das Sie eine Verbindung erstellen müssen.
1. Klicken **[!UICONTROL Verbindung erstellen]** Klicken Sie auf **[!UICONTROL Erweiterte Einstellungen anzeigen]**.

1. Geben Sie die [!UICONTROL Client-ID] und [!UICONTROL Client Secret] Sie haben abgerufen in [[!UICONTROL OAuth-Anmeldedaten erstellen]](#create-oauth-credentials) Klicken Sie in den entsprechenden Feldern auf **[!UICONTROL Weiter]**.

1. Melden Sie sich bei Ihrer [!DNL Google] -Konto.

   Die **[!UICONTROL Diese App ist nicht verifiziert]** angezeigt. Beachten Sie, dass die im Fenstertitel erwähnte &quot;App&quot;der OAuth-Client ist, den Sie oben erstellt haben.

1. Klicken **[!UICONTROL Erweitert]** Klicken Sie auf **[!UICONTROL Navigieren Sie zu [!DNL Workfront Fusion] (unsicher)]** , um den Zugriff über Ihren benutzerdefinierten OAuth-Client zu ermöglichen.

1. Klicken **[!UICONTROL Zulassen]** zu gewähren [!DNL Workfront Fusion] Berechtigung.
1. Klicken Sie im sich öffnenden Fenster auf **[!UICONTROL Zulassen]** erneut, um Ihre Auswahl zu bestätigen.

   Die Verbindung zum gewünschten [!DNL Google] -Dienst, der einen benutzerdefinierten OAuth-Client verwendet, eingerichtet ist.

### Verbinden mit [!DNL Google] im [!UICONTROL HTTP] > [!UICONTROL OAuth2.0-Anfrage stellen] Modul {#connect-to-google-in-the-http--make-an-oauth20-request-module}

Anweisungen zum Verbinden mit [!DNL Google] im [!UICONTROL HTTP] > [!UICONTROL OAuth2.0-Anfrage stellen] -Modul, siehe [Anleitung zum Erstellen einer Verbindung zu [!DNL Google] im [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0-Anfrage stellen] Modul](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instruct) in [[!UICONTROL HTTP] > [!UICONTROL OAuth 2.0-Anfrage stellen] Modul](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## Mögliche Fehlermeldung:[!UICONTROL [403] Zugriff nicht konfiguriert]

Wenn die Variable [!UICONTROL [403] Zugriff nicht konfiguriert] angezeigt wird, müssen Sie die entsprechende API in Ihrer Google Cloud-Plattform aktivieren. Gehen Sie wie im Abschnitt beschrieben vor, um die API zu aktivieren [Erstellen Sie ein Projekt auf [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) in diesem Artikel.
