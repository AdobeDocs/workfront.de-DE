---
title: Erstellen von OAuth2-Anwendungen für [!DNL Workfront] Integrationen
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Als [!DNL Adobe Workfront] Administrator können Sie OAuth2-Anwendungen für Ihre Instanz von [!DNL Workfront] erstellen, die anderen Anwendungen den Zugriff auf Workfront ermöglichen. Ihre Benutzer können dann anderen Anwendungen Berechtigungen für den Zugriff auf ihre Workfront-Daten erteilen. Auf diese Weise können Sie Workfront mit Anwendungen Ihrer Wahl integrieren, einschließlich Ihrer eigenen internen Anwendungen.
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: e13c7dda-8945-47ad-b6d3-4d6a62b368f5
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '1957'
ht-degree: 6%

---

# Erstellen von OAuth2-Anwendungen für [!DNL Workfront] -Integrationen

Als [!DNL Adobe Workfront] -Administrator können Sie OAuth2-Anwendungen für Ihre Instanz von [!DNL Workfront] erstellen, die anderen Anwendungen den Zugriff auf [!DNL Workfront] ermöglichen. Ihre Benutzer können dann diesen anderen Anwendungen Berechtigungen für den Zugriff auf ihre [!DNL Workfront] -Daten erteilen. Auf diese Weise können Sie die   mit Anwendungen Ihrer Wahl, einschließlich Ihrer eigenen internen Anwendungen.

Wenn Sie eine [!UICONTROL OAuth2] -Anwendung erstellen, generieren Sie eine Client-ID und einen Client-Geheimnis. Ihre Benutzer können dann die Client-ID in API-Aufrufen verwenden, um sie in die von Ihnen erstellte Anwendung zu integrieren.

>[!NOTE]
>
>Im Kontext von OAuth2 bezieht sich &quot;Erstellen einer App&quot;auf den Prozess der Erstellung einer solchen Zugriffsverknüpfung zwischen einer App und einem Server wie [!DNL Workfront].

* Anweisungen zum Konfigurieren und Verwenden der OAuth2-Anwendung mit Benutzeranmeldeinformationen (Fluss des Autorisierungscodes) finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe des Autorisierungscodeflusses](../../wf-api/api/oauth-app-code-token-flow.md).
* Anweisungen zum Konfigurieren und Verwenden der OAuth2-Anwendung mithilfe der Serverauthentifizierung (JWT-Fluss) finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe des JWT-Flusses](../../wf-api/api/oauth-app-jwt-flow.md).
* Anweisungen zum Konfigurieren und Verwenden der OAuth2-Anwendung mit PKCE finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mit PKCE Flow](../../wf-api/api/oauth-app-pkce-flow.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>Neu: [!UICONTROL Standard]</p>
   Oder
   <p>Aktuell:[!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> Sie müssen ein [!DNL Workfront] -Administrator sein. </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## OAuth2-Übersicht

Stellen Sie sich vor, eine Anwendung muss einige spezifische Informationen aus [!DNL Workfront] abrufen. Eine Anwendung, die Informationen anfordert, wird als Client bezeichnet. In diesem Beispiel lautet der Client-Name ClientApp. ClientApp benötigt Zugriff auf die Informationen eines bestimmten Benutzers und muss daher auf [!DNL Workfront] als diesen Benutzer zugreifen. Wenn Ihr Benutzer ClientApp seinen Benutzernamen und sein Kennwort gibt, kann ClientApp auf alle Daten zugreifen, auf die der Benutzer zugreifen kann. Dies ist ein Sicherheitsrisiko, da ClientApp nur einen kleinen, spezifischen Satz an Informationen benötigt.

Wenn Sie eine OAuth2-App für ClientApp erstellen, teilen Sie [!DNL Workfront] im Wesentlichen mit, dass ClientApp auf [!DNL Workfront] zugreifen darf, allerdings nur, wenn der Benutzer, auf dessen Konto ClientApp zugreift, die Berechtigung für den Zugriff erteilt.

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

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]** und wählen Sie dann **[!UICONTROL OAuth2 Applications]** aus.
1. Klicken Sie auf **[!UICONTROL App-Integration erstellen]**.
Das Feld **Neue OAuth2-Anwendung** wird angezeigt.
1. Wählen Sie im Feld **Neue OAuth2-Anwendung** die Option **[!UICONTROL Machine to Machine Application]**.
1. Geben Sie einen Namen für die neue Anwendung ein, z. B. &quot;[!DNL Workfront] für ClientApp&quot;.
1. Klicken Sie auf **[!UICONTROL Erstellen]**.
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
         <li value="1"> <p>Klicken Sie auf das Symbol <b>[!UICONTROL Löschen]</b> <img src="assets/delete.png">, um den aktuellen Client-Geheimniswert zu löschen.</p> </li> 
         <li value="2"> <p>Klicken Sie auf <b>[!UICONTROL Client-Geheimnis hinzufügen]</b> , um ein neues Client-Geheimnis zu generieren.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Public Keys]</td> 
      <td> <p>Server-zu-Server-Apps verwenden öffentliche und private Schlüssel zur Authentifizierung. Führen Sie einen der folgenden Schritte aus:</p> 
       <ul> 
        <li> <p>Klicken Sie auf <b>[!UICONTROL Öffentlichen Schlüssel hinzufügen]</b> und geben Sie den öffentlichen Schlüssel aus der anderen Anwendung ein.</p> </li> 
        <li> <p>Klicken Sie auf <b>[!UICONTROL Generate a public/private keypair]</b> und geben Sie dann den öffentlichen Schlüssel für die andere Anwendung frei.</p> </li> 
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

Anweisungen zum Konfigurieren und Verwenden der OAuth2-Anwendung mit Benutzeranmeldeinformationen (Fluss des Autorisierungscodes) finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe des JWT-Flusses](../../wf-api/api/oauth-app-jwt-flow.md).

### Erstellen einer OAuth2-Anwendung mit Benutzeranmeldeinformationen (Autorisierungscode-Fluss) {#create-an-oauth2-application-using-user-credentials-authorization-code-flow}

{{step-1-to-setup}}

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]** und wählen Sie dann **[!UICONTROL OAuth2 Applications]** aus.
1. Klicken Sie auf **[!UICONTROL App-Integration erstellen]**.

   Die neue OAuth2-Anwendung **wird angezeigt.**
1. Wählen Sie im Feld **Neue OAuth2-Anwendung** die Option **[!UICONTROL Webanwendung]** aus.
1. Geben Sie einen Namen für die neue OAuth2-Anwendung ein, z. B. &quot;[!DNL Workfront] für ClientApp&quot;.
1. Klicken Sie auf **[!UICONTROL Erstellen]**.
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
         <li value="1"> <p>Klicken Sie auf das Symbol <b>[!UICONTROL Löschen]</b> <img src="assets/delete.png">, um den aktuellen Client-Geheimniswert zu löschen.</p> </li> 
         <li value="2"> <p>Klicken Sie auf <b>[!UICONTROL Client-Geheimnis hinzufügen]</b> , um ein neues Client-Geheimnis zu generieren.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Umleitungs-URLs]</td> 
      <td>Benutzer werden nach der Authentifizierung mit [!DNL Workfront] zu diesem Pfad umgeleitet.</td> 
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

Anweisungen zum Konfigurieren und Verwenden der OAuth2-Anwendung mit Benutzeranmeldeinformationen (Fluss des Autorisierungscodes) finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe des Autorisierungscodeflusses](../../wf-api/api/oauth-app-code-token-flow.md).

### Erstellen einer OAuth2-Single-Page-Webanwendung mit PKCE {#create-an-oauth2-single-page-web-application-using-pkce}

{{step-1-to-setup}}

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]** und wählen Sie dann **[!UICONTROL OAuth2 Applications]** aus.
1. Klicken Sie auf **[!UICONTROL App-Integration erstellen]**.

   Das Feld **Neue OAuth2-Anwendung** wird angezeigt.
1. Wählen Sie im Feld **Neue OAuth2-Anwendung** die Option **[!UICONTROL Single Page Web Application]**.
1. Geben Sie einen Namen für die neue Anwendung [!UICONTROL OAuth2] ein, z. B. &quot;[!DNL Workfront] für ClientApp&quot;.
1. Klicken Sie auf **[!UICONTROL Erstellen]**.
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

* Anweisungen zum Konfigurieren und Verwenden der OAuth2-Anwendung mit Benutzeranmeldeinformationen (Fluss des Autorisierungscodes) finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe des Autorisierungscodeflusses](../../wf-api/api/oauth-app-code-token-flow.md).
* Anweisungen zum Konfigurieren und Verwenden der OAuth2-Anwendung mithilfe der Serverauthentifizierung (JWT-Fluss) finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe des JWT-Flusses](../../wf-api/api/oauth-app-jwt-flow.md).
* Anweisungen zum Konfigurieren und Verwenden der OAuth2-Anwendung mit PKCE finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mit PKCE Flow](../../wf-api/api/oauth-app-pkce-flow.md).

## OAuth2-Prozesse für den Autorisierungscode-Fluss

>[!NOTE]
>
>Ihre Benutzer greifen über die API auf die Anwendung [!UICONTROL OAuth2] zu. In diesem Abschnitt wird die Funktionalität allgemein beschrieben und nur zu Informationszwecken bereitgestellt.
>
>Spezifische Anweisungen zur Verwendung der OAuth2-Anwendung, einschließlich spezifischer API-Aufrufe, finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe des Autorisierungscodeflusses](../../wf-api/api/oauth-app-code-token-flow.md).

### Autorisierung mit einem Autorisierungscode und Zugriffstoken {#authorizing-with-an-authorization-code-and-access-token}

1. ClientApp benötigt einige Informationen von [!DNL Workfront], daher wird eine Anfrage an den Endpunkt [!DNL Workfront] API `/authorize` gesendet. Die Anfrage enthält den [!UICONTROL response_type] `code` , der angibt, dass die Anfrage einen Autorisierungscode zurückgeben soll.
1. Dieser Trigger [!DNL Workfront] sendet eine Authentifizierungsaufforderung an den Benutzer. Der Benutzer kann seine Anmeldedaten in die Eingabeaufforderung eingeben, wodurch [!DNL Workfront] die Berechtigung zur Kommunikation mit ClientApp erhält. Wenn der Benutzer bereits bei [!DNL Workfront] angemeldet ist, kann dieser Schritt übersprungen werden.
1. Die [!DNL Workfront] -API sendet einen Autorisierungscode an ClientApp.
1. ClientApp sendet die folgenden Informationen in einer Anfrage an die [!DNL Workfront] API `/token`   Endpunkt:

   * Der Autorisierungscode, der in Schritt 3 an ClientApp gesendet wurde. Damit wird die spezifische Instanz der Benutzerberechtigungen identifiziert.
   * Das Client-Geheimnis, das beim Einrichten der ClientApp OAuth2-App in [!DNL Workfront] generiert wurde. Dadurch kann [!DNL Workfront] erkennen, dass die Anfrage von ClientApp stammt.

1. Wenn der Autorisierungscode und das Client-Geheimnis korrekt sind, sendet [!DNL Workfront] ein Zugriffstoken an ClientApp. Dieses Zugriffstoken wird direkt von [!DNL Workfront] an ClientApp gesendet und kann von keinem anderen Benutzer oder von keiner Client-Anwendung angezeigt, kopiert oder verwendet werden.
1. ClientApp sendet das Zugriffstoken zusammen mit der spezifischen Informationsanfrage an [!DNL Workfront].
1. Da das Zugriffstoken korrekt ist, sendet [!DNL Workfront] die Informationen an ClientApp.

#### Aktualisieren von Zugriffstoken

Aus Sicherheitsgründen laufen Zugriffstoken nach kurzer Zeit ab. Um neue Zugriffstoken zu erhalten, ohne jedes Mal Anmeldeinformationen eingeben zu müssen, verwendet [!DNL OAuth2] Aktualisierungstoken. Aktualisierungs-Token werden vom Client gespeichert.

Der Prozess für das Abrufen eines Aktualisierungstokens entspricht dem im Abschnitt [Autorisierung mit einem Autorisierungs-Code und Zugriffstoken](#authorizing-with-an-authorization-code-and-access-token) beschriebenen Verfahren. Die Anfrage für den Autorisierungscode enthält den Gültigkeitsbereich &quot;`offline_access`&quot;, der angibt, dass die Anfrage ein Anfrage-Token zusammen mit dem Autorisierungscode zurückgeben soll.
