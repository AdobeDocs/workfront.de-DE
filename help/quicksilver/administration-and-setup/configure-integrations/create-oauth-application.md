---
title: Erstellen von OAuth2-Anwendungen für [!DNL Workfront] Integrationen
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Als [!DNL Adobe Workfront] Administrator können Sie OAuth2-Anwendungen für Ihre Instanz von [!DNL Workfront], die anderen Anwendungen den Zugriff auf Workfront ermöglichen. Ihre Benutzer können dann anderen Anwendungen Berechtigungen für den Zugriff auf ihre Workfront-Daten erteilen. Auf diese Weise können Sie Workfront mit Anwendungen Ihrer Wahl integrieren, einschließlich Ihrer eigenen internen Anwendungen.
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: e13c7dda-8945-47ad-b6d3-4d6a62b368f5
source-git-commit: ff24fcc65791b6c18668a0dd3c58e033772a2def
workflow-type: tm+mt
source-wordcount: '1945'
ht-degree: 5%

---

# Erstellen von OAuth2-Anwendungen für [!DNL Workfront] Integrationen

Als [!DNL Adobe Workfront] Administrator können Sie OAuth2-Anwendungen für Ihre Instanz von [!DNL Workfront], die anderen Anwendungen den Zugriff erlauben [!DNL Workfront]. Ihre Benutzer können dann anderen Anwendungen Berechtigungen erteilen, um auf ihre [!DNL Workfront] Daten. Auf diese Weise können Sie mit Anwendungen Ihrer Wahl, einschließlich Ihrer eigenen internen Anwendungen, integrieren.

Wenn Sie eine [!UICONTROL OAuth2] -Anwendung verwenden, generieren Sie eine Client-ID und einen Client-Geheimnis. Ihre Benutzer können dann die Client-ID in API-Aufrufen verwenden, um sie in die von Ihnen erstellte Anwendung zu integrieren.

>[!NOTE]
>
>Im Kontext von OAuth2 bezieht sich &quot;Erstellen einer App&quot;auf den Prozess der Erstellung dieser Art von Zugriffsverknüpfung zwischen einer App und einem Server, z. B. [!DNL Workfront].

* Anweisungen zum Konfigurieren und Verwenden der OAuth2-Anwendung mit Benutzeranmeldeinformationen (Autorisierungscode-Ablauf) finden Sie unter [Benutzerdefinierte OAuth 2-Anwendungen Ihres Unternehmens mithilfe des Autorisierungscode-Flusses konfigurieren und verwenden](../../wf-api/api/oauth-app-code-token-flow.md).
* Anweisungen zum Konfigurieren und Verwenden der OAuth2-Anwendung mithilfe der Serverauthentifizierung (JWT-Fluss) finden Sie unter [Benutzerdefinierte OAuth 2-Anwendungen Ihres Unternehmens mithilfe des JWT-Flusses konfigurieren und verwenden](../../wf-api/api/oauth-app-jwt-flow.md).
* Anweisungen zum Konfigurieren und Verwenden der OAuth2-Anwendung mit PKCE finden Sie unter [Benutzerdefinierte OAuth 2-Anwendungen Ihres Unternehmens mithilfe des PKCE-Flusses konfigurieren und verwenden](../../wf-api/api/oauth-app-pkce-flow.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>Neu: [!UICONTROL Standard]</p>
   Oder
   <p>Aktuell:[!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> Sie müssen [!DNL Workfront] Administrator. </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## OAuth2-Übersicht

Stellen Sie sich vor, eine Anwendung muss einige spezifische Informationen abrufen. [!DNL Workfront]. Eine Anwendung, die Informationen anfordert, wird als Client bezeichnet. In diesem Beispiel lautet der Client-Name ClientApp. ClientApp benötigt Zugriff auf die Informationen eines bestimmten Benutzers und muss daher auf [!DNL Workfront] als dieser Benutzer. Wenn Ihr Benutzer ClientApp seinen Benutzernamen und sein Kennwort gibt, kann ClientApp auf alle Daten zugreifen, auf die der Benutzer zugreifen kann. Dies ist ein Sicherheitsrisiko, da ClientApp nur einen kleinen, spezifischen Satz an Informationen benötigt.

Wenn Sie eine OAuth2-App für ClientApp erstellen, erzählen Sie im Grunde [!DNL Workfront] , auf die ClientApp zugreifen darf [!DNL Workfront], jedoch nur dann, wenn der Benutzer, auf dessen Konto ClientApp zugreift, die Berechtigung für den Zugriff erteilt.

## Erstellen einer OAuth2-Anwendung

Wählen Sie beim Erstellen einer OAuth2-Anwendung den Anwendungstyp aus, der den Anforderungen Ihrer Integration am besten entspricht.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Anwendungstyp</th> 
   <th>Best for</th> 
   <th>Authentifizierungsmethode</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Maschine-zu-Maschine-Anwendung</p> </td> 
   <td> <p>Best Practices für CLIs, Daemons oder Skripte, die auf Ihrem Server ausgeführt werden</p> <p>Beispiele:</p> 
    <ul> 
     <li> <p>[!DNL Shell] </p> </li> 
     <li> <p>[!DNL Python]</p> </li> 
    </ul> </td> 
   <td> <p>Authentifizierung mit JSON-Web-Token mit Verschlüsselung des öffentlichen/privaten Schlüsselpaares.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Single Page Application (einseitige Web-Anwendung)</p> </td> 
   <td> <p>Optimal für mobile oder einseitige Webanwendungen</p> <p>Beispiele:</p> 
    <ul> 
     <li> <p>[!DNL Javascript]</p> </li> 
     <li> <p>[!DNL Angular]</p> </li> 
     <li> <p>[!DNL React]</p> </li> 
     <li> <p>[!DNL Vue]</p> </li> 
    </ul> </td> 
   <td> <p>Authentifizierung durch OAuth 2.0 Authorization Code Flow mit Proof Key for Code Exchange (PKCE).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Web-Anwendung</p> </td> 
   <td> <p>Optimale Lösung für serverseitige Anwendungen, die Anmeldeinformationen und Tokens auf dem Server verarbeiten</p> <p>Beispiele:</p> 
    <ul> 
     <li> <p>[!DNL Go]</p> </li> 
     <li> <p>[!DNL Java]</p> </li> 
     <li> <p>[!DNL ASP.Net]</p> </li> 
     <li> <p>[!DNL Node.js]</p> </li> 
     <li> <p>[!DNL PHP]</p> </li> 
    </ul> </td> 
   <td> <p>Authentifizierung über OAuth 2.0 Authorization Code Flow.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Sie können bis zu zehn OAuth2-Anwendungen gleichzeitig haben.

* [Erstellen einer OAuth2-Anwendung mithilfe der Serverauthentifizierung (JWT-Fluss)](#create-an-oauth2-application-using-server-authentication-jwt-flow)
* [Erstellen einer OAuth2-Anwendung mit Benutzeranmeldeinformationen (Autorisierungscode-Fluss)](#create-an-oauth2-application-using-user-credentials-authorization-code-flow)
* [Erstellen einer OAuth2-Single-Page-Webanwendung mit PKCE](#create-an-oauth2-single-page-web-application-using-pkce)

### Erstellen einer OAuth2-Anwendung mithilfe der Serverauthentifizierung (JWT-Fluss) {#create-an-oauth2-application-using-server-authentication-jwt-flow}

{{step-1-to-setup}}

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]**, wählen Sie **[!UICONTROL OAuth2-Anwendungen]**.
1. Klicks **[!UICONTROL App-Integration erstellen]**.
Die **Neue OAuth2-Anwendung** angezeigt.
1. Im **Neue OAuth2-Anwendung** auswählen **[!UICONTROL Maschinelle Anwendung]**.
1. Geben Sie einen Namen für die neue Anwendung ein, beispielsweise &quot;[!DNL Workfront] für ClientApp.&quot;
1. Klicks **[!UICONTROL Erstellen]**.
1. Füllen Sie die Felder für die neue App aus.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client-ID]</td> 
      <td> <p>Dieses Feld wird automatisch generiert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client secret]</td> 
      <td> <p>Dieses Feld wird automatisch generiert</p> <p><b>WICHTIG</b>:  <p>Kopieren Sie den Inhalt dieses Felds in eine andere sichere Datei, bevor Sie diese Seite schließen. Sie werden diesen geheimen Schlüssel nicht mehr sehen können.</p> <p>Wenn Sie diesen Schlüssel verlieren, löschen Sie ihn und erstellen Sie ein Client-Geheimnis.</p> 
        <ol> 
         <li value="1"> <p>Klicken Sie auf <b>[!UICONTROL Löschen]</b> icon <img src="assets/delete.png"> , um das aktuelle Client-Geheimnis zu löschen.</p> </li> 
         <li value="2"> <p>Klicks <b>[!UICONTROL Client-Geheimnis hinzufügen]</b> , um ein neues Client-Geheimnis zu generieren.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Public Keys]</td> 
      <td> <p>Server-zu-Server-Apps verwenden öffentliche und private Schlüssel zur Authentifizierung. Führen Sie einen der folgenden Schritte aus:</p> 
       <ul> 
        <li> <p>Klicks <b>[!UICONTROL Öffentlichen Schlüssel hinzufügen]</b> und geben Sie den öffentlichen Schlüssel aus der anderen Anwendung ein.</p> </li> 
        <li> <p>Klicks <b>[!UICONTROL Generieren eines öffentlichen/privaten Keypairs]</b>, und geben Sie dann den öffentlichen Schlüssel für die andere Anwendung frei.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Dies ist der gleiche Name wie die App. Dieses Feld darf nicht leer sein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Beschreibung]</td> 
      <td>Geben Sie eine Beschreibung für die Integration ein.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Speichern]**.

Anweisungen zum Konfigurieren und Verwenden der OAuth2-Anwendung mit Benutzeranmeldeinformationen (Autorisierungscode-Ablauf) finden Sie unter [Benutzerdefinierte OAuth 2-Anwendungen Ihres Unternehmens mithilfe des JWT-Flusses konfigurieren und verwenden](../../wf-api/api/oauth-app-jwt-flow.md).

### Erstellen einer OAuth2-Anwendung mit Benutzeranmeldeinformationen (Autorisierungscode-Fluss) {#create-an-oauth2-application-using-user-credentials-authorization-code-flow}

{{step-1-to-setup}}

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]**, wählen Sie **[!UICONTROL OAuth2-Anwendungen]**.
1. Klicks **[!UICONTROL App-Integration erstellen]**.

   Die **Neue OAuth2-Anwendung** angezeigt.
1. Im **Neue OAuth2-Anwendung** auswählen **[!UICONTROL Webanwendung]**.
1. Geben Sie einen Namen für die neue OAuth2-Anwendung ein, beispielsweise &quot;[!DNL Workfront] für ClientApp.&quot;
1. Klicks **[!UICONTROL Erstellen]**.
1. Füllen Sie die Felder für die neue App aus.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client-ID]</td> 
      <td> <p>Dieses Feld wird automatisch generiert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client secret]</td> 
      <td> <p>Dieses Feld wird automatisch generiert</p> <p><b>WICHTIG</b>:  <p>Kopieren Sie den Inhalt dieses Felds in eine andere sichere Datei, bevor Sie diese Seite schließen. Sie werden diesen geheimen Schlüssel nicht mehr sehen können.</p> <p>Wenn Sie diesen Schlüssel verlieren, löschen Sie ihn und erstellen Sie ein Client-Geheimnis.</p> 
        <ol> 
         <li value="1"> <p>Klicken Sie auf <b>[!UICONTROL Löschen]</b> icon <img src="assets/delete.png"> , um das aktuelle Client-Geheimnis zu löschen.</p> </li> 
         <li value="2"> <p>Klicks <b>[!UICONTROL Client-Geheimnis hinzufügen]</b> , um ein neues Client-Geheimnis zu generieren.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Umleitungs-URLs]</td> 
      <td>Benutzer werden nach der Authentifizierung mit diesem Pfad zu diesem Pfad umgeleitet [!DNL Workfront].</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Aktualisierung der Tokenrotation]</td> 
      <td>Aktivieren Sie diese Option, um jedes Mal, wenn ein Refresh-Token verwendet wird, ein neues Refresh-Token zu erstellen. Ihre Anwendung muss das neue Refresh-Token nach jeder Aktualisierung speichern.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Absoluter Aktualisierungstoken-Ablauf]</td> 
      <td> <p>Wählen Sie den Zeitraum aus, für den ein Aktualisierungstoken vorhanden sein soll, bevor es abläuft. Nach Ablauf dieser Frist müssen sich Ihre Benutzer erneut bei der Integration anmelden. Wählen Sie "[!UICONTROL No expiration]", wenn das Aktualisierungstoken nicht ablaufen soll.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Gültigkeit des Inaktivitätsaktualisierungs-Tokens</td> 
      <td> <p>Wählen Sie den Zeitraum aus, nach dem das Aktualisierungstoken abläuft, wenn der Benutzer nicht in Ihrem System aktiv war. </p> <p>Wenn beispielsweise die Gültigkeit des Inaktivitäts-Aktualisierungstokens 6 Monate beträgt und sich der Benutzer sechs Monate lang nicht anmeldet, läuft das Aktualisierungs-Token ab, auch wenn der absolute Ablauf des Aktualisierungstokens möglicherweise länger festgelegt ist.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Logo]</td> 
      <td>Sie können ein Logo hinzufügen, um diese App leichter identifizierbar zu machen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Dies ist der gleiche Name wie die App. Dieses Feld darf nicht leer sein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Beschreibung]</td> 
      <td>Geben Sie eine Beschreibung für die Integration ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL App Description URL]</td> 
      <td>Hierbei kann es sich um einen Link zu einer "Info"-Seite oder zu einer Seite mit weiteren Informationen zur Integration handeln.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Speichern]**.

Anweisungen zum Konfigurieren und Verwenden der OAuth2-Anwendung mit Benutzeranmeldeinformationen (Autorisierungscode-Ablauf) finden Sie unter [Benutzerdefinierte OAuth 2-Anwendungen Ihres Unternehmens mithilfe des Autorisierungscode-Flusses konfigurieren und verwenden](../../wf-api/api/oauth-app-code-token-flow.md).

### Erstellen einer OAuth2-Single-Page-Webanwendung mit PKCE {#create-an-oauth2-single-page-web-application-using-pkce}

{{step-1-to-setup}}

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]**, wählen Sie **[!UICONTROL OAuth2-Anwendungen]**.
1. Klicks **[!UICONTROL App-Integration erstellen]**.

   Die **Neue OAuth2-Anwendung** angezeigt.
1. Im **Neue OAuth2-Anwendung** auswählen **[!UICONTROL Einzelseiten-Webanwendung]**.
1. Geben Sie einen Namen für die neue [!UICONTROL OAuth2] -Anwendung, z. B. &quot;[!DNL Workfront] für ClientApp.&quot;
1. Klicks **[!UICONTROL Erstellen]**.
1. Füllen Sie die Felder für die neue App aus.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client-ID]</td> 
      <td> <p>Dieses Feld wird automatisch generiert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Umleitungs-URLs]</td> 
      <td>Benutzer werden nach der Authentifizierung bei Workfront zu diesem Pfad umgeleitet.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Aktualisierungstoken bei jeder Verwendung drehen]</td> 
      <td>Aktivieren Sie diese Option, um jedes Mal, wenn ein Refresh-Token verwendet wird, ein neues Refresh-Token zu erstellen. Ihre Anwendung muss das neue Refresh-Token nach jeder Aktualisierung speichern.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Absoluter Ablauf]</td> 
      <td> <p>Wählen Sie den Zeitraum aus, für den ein Aktualisierungstoken vorhanden sein soll, bevor es abläuft. Nach Ablauf dieser Frist müssen sich Ihre Benutzer erneut bei der Integration anmelden. Wählen Sie "[!UICONTROL No expiration]", wenn das Aktualisierungstoken nicht ablaufen soll.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Inaktivitätsablauf]</td> 
      <td> <p>Wählen Sie den Zeitraum aus, nach dem das Aktualisierungstoken abläuft, wenn der Benutzer nicht in Ihrem System aktiv war. </p> <p>Wenn beispielsweise die Gültigkeit des Inaktivitäts-Aktualisierungstokens 6 Monate beträgt und sich der Benutzer sechs Monate lang nicht anmeldet, läuft das Aktualisierungs-Token ab, auch wenn der absolute Ablauf des Aktualisierungstokens möglicherweise länger festgelegt ist.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Logo]</td> 
      <td>Sie können ein Logo hinzufügen, um diese App leichter identifizierbar zu machen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Dies ist der gleiche Name wie die App. Dieses Feld darf nicht leer sein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Beschreibung]</td> 
      <td>Geben Sie eine Beschreibung für die Integration ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Entwicklername]</td> 
      <td>Dies ist der Name des Entwicklers, der die OAuth2-Anwendung eingerichtet hat.</td> 
     </tr> 
   <tr> 
      <td role="rowheader">[!UICONTROL Entwickler-E-Mail-Adresse]</td> 
      <td>Dies ist die E-Mail-Adresse des Entwicklers, der die OAuth2-Anwendung eingerichtet hat.</td> 
     </tr> 
   <tr> 
      <td role="rowheader">URL der [!UICONTROL Datenschutzrichtlinie]</td> 
      <td>Dies ist der Link zu dem Ort, an dem Ihre Organisation die Datenschutzrichtlinie speichert.</td> 
     </tr>


   </tbody> 
   </table>

   <!-- removed this from the table, and added "Developer name" and following rows:
   [!UICONTROL App Description URL]</td> 
      <td>This can be a link to an "About us" page or a page with more information about the integration.> -->

1. Klicken Sie auf **[!UICONTROL Speichern]**.

## Konfigurieren und Verwenden der erstellten OAuth2-Anwendung

Die weitere Konfiguration und Verwendung der erstellten OAuth2-Anwendung erfordert einige technische Kenntnisse, einschließlich API-Aufrufen.

* Anweisungen zum Konfigurieren und Verwenden der OAuth2-Anwendung mit Benutzeranmeldeinformationen (Autorisierungscode-Ablauf) finden Sie unter [Benutzerdefinierte OAuth 2-Anwendungen Ihres Unternehmens mithilfe des Autorisierungscode-Flusses konfigurieren und verwenden](../../wf-api/api/oauth-app-code-token-flow.md).
* Anweisungen zum Konfigurieren und Verwenden der OAuth2-Anwendung mithilfe der Serverauthentifizierung (JWT-Fluss) finden Sie unter [Benutzerdefinierte OAuth 2-Anwendungen Ihres Unternehmens mithilfe des JWT-Flusses konfigurieren und verwenden](../../wf-api/api/oauth-app-jwt-flow.md).
* Anweisungen zum Konfigurieren und Verwenden der OAuth2-Anwendung mit PKCE finden Sie unter [Benutzerdefinierte OAuth 2-Anwendungen Ihres Unternehmens mithilfe des PKCE-Flusses konfigurieren und verwenden](../../wf-api/api/oauth-app-pkce-flow.md).

## OAuth2-Prozesse für den Autorisierungscode-Fluss

>[!NOTE]
>
>Ihre Benutzer greifen auf die [!UICONTROL OAuth2] -Anwendung über die -API. In diesem Abschnitt wird die Funktionalität allgemein beschrieben und nur zu Informationszwecken bereitgestellt.
>
>Spezifische Anweisungen zur Verwendung der OAuth2-Anwendung, einschließlich spezifischer API-Aufrufe, finden Sie unter [Benutzerdefinierte OAuth 2-Anwendungen Ihres Unternehmens mithilfe des Autorisierungscode-Flusses konfigurieren und verwenden](../../wf-api/api/oauth-app-code-token-flow.md).

### Autorisierung mit einem Autorisierungscode und Zugriffstoken {#authorizing-with-an-authorization-code-and-access-token}

1. ClientApp benötigt einige Informationen von [!DNL Workfront], sendet also eine Anfrage an die [!DNL Workfront] API `/authorize` -Endpunkt. Die Anfrage umfasst die [!UICONTROL response_type] `code`, der angibt, dass die Anfrage einen Autorisierungscode zurückgeben sollte.
1. Diese Trigger [!DNL Workfront] , um eine Authentifizierungsaufforderung an den Benutzer zu senden. Der Benutzer kann seine Anmeldedaten in die Eingabeaufforderung eingeben, die [!DNL Workfront] Berechtigung zur Kommunikation mit ClientApp. Wenn der Benutzer bereits angemeldet ist [!DNL Workfront]festgelegt ist, kann dieser Schritt übersprungen werden.
1. Die [!DNL Workfront] API sendet einen Autorisierungscode an ClientApp.
1. ClientApp sendet die folgenden Informationen in einer Anfrage an die [!DNL Workfront] API `/token`   Endpunkt:

   * Der Autorisierungscode, der in Schritt 3 an ClientApp gesendet wurde. Damit wird die spezifische Instanz der Benutzerberechtigungen identifiziert.
   * Das Client-Geheimnis, das beim Einrichten der ClientApp OAuth2-App in generiert wurde [!DNL Workfront]. Dies ermöglicht Folgendes [!DNL Workfront] , um zu erfahren, dass die Anfrage von ClientApp stammt.

1. Wenn der Autorisierungscode und das Client-Geheimnis korrekt sind, [!DNL Workfront] sendet ein Zugriffstoken an ClientApp. Dieses Zugriffstoken wird direkt von [!DNL Workfront] in ClientApp gespeichert ist und von keinem anderen Benutzer oder Client-Programm angezeigt, kopiert oder verwendet werden kann.
1. ClientApp sendet das Zugriffstoken an [!DNL Workfront] zusammen mit der spezifischen Informationsanfrage.
1. Da das Zugriffstoken korrekt ist, [!DNL Workfront] sendet die Informationen an ClientApp.

#### Aktualisieren von Zugriffstoken

Aus Sicherheitsgründen laufen Zugriffstoken nach kurzer Zeit ab. Um neue Zugriffstoken zu erhalten, ohne jedes Mal Anmeldeinformationen eingeben zu müssen, müssen Sie [!DNL OAuth2] verwendet Aktualisierungstoken. Aktualisierungs-Token werden vom Client gespeichert.

Der Prozess zum Erwerb eines Aktualisierungstokens entspricht dem im Abschnitt beschriebenen Verfahren [Autorisierung mit einem Autorisierungscode und Zugriffstoken](#authorizing-with-an-authorization-code-and-access-token). Der Antrag auf den Autorisierungscode umfasst den Geltungsbereich `offline_access`, der angibt, dass die Anfrage ein Anfrage-Token zusammen mit dem Autorisierungscode zurückgeben soll.
