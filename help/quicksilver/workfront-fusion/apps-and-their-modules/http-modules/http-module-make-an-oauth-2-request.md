---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: http-modules
title: HTTP &gt; Erstellen eines OAuth 2.0-Anforderungsmoduls
description: Um eine  [!DNL Adobe Workfront Fusion] HTTP(S)-Anfrage an Server zu richten, für die eine OAuth 2.0-Autorisierung erforderlich ist, müssen Sie zunächst eine OAuth-Verbindung erstellen. [!DNL Adobe Workfront Fusion] stellt sicher, dass alle mit dieser Verbindung getätigten Aufrufe über die entsprechenden Autorisierungskopfzeilen verfügen und die zugehörigen Token bei Bedarf automatisch aktualisieren.
author: Becky
feature: Workfront Fusion
exl-id: 6c68c9b9-9f74-44a7-94ed-3785081b8331
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '2236'
ht-degree: 0%

---

# [!UICONTROL HTTP] > [!UICONTROL Erstellen eines OAuth 2.0-Anfrage-Moduls]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] erfordert zusätzlich zu einer [!DNL Adobe Workfront] -Lizenz eine [!DNL Adobe Workfront Fusion] -Lizenz.

Um eine [!DNL Adobe Workfront Fusion] HTTP(S)-Anfrage an Server zu richten, für die eine OAuth 2.0-Autorisierung erforderlich ist, müssen Sie zunächst eine OAuth-Verbindung erstellen. [!DNL Adobe Workfront Fusion] stellt sicher, dass alle mit dieser Verbindung getätigten Aufrufe über die entsprechenden Autorisierungskopfzeilen verfügen und die zugehörigen Token bei Bedarf automatisch aktualisieren.

[!DNL Workfront Fusion] unterstützt die folgenden OAuth 2.0-Authentifizierungsflüsse:

* Autorisierungscode-Fluss
* Impliziter Fluss

Andere Flüsse, wie &quot;Resource Owner Password Credentials Flow&quot;und &quot;Client Credentials Flow&quot;, werden von diesem Modul nicht automatisch unterstützt.

Weitere Informationen zur OAuth 2.0-Authentifizierung finden Sie unter [OAuth 2.0 Authorization Framework](https://tools.ietf.org/html/rfc6749).

>[!NOTE]
>
>Wenn Sie eine Verbindung zu einem Adobe-Produkt herstellen, das derzeit über keinen dedizierten Connector verfügt, empfehlen wir die Verwendung des Adobe Authenticator-Moduls.
>
>Weitere Informationen finden Sie unter [Adobe Authenticator-Modul](/help/quicksilver/workfront-fusion/apps-and-their-modules/adobe-authenticator-modules.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebene Funktionalität nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Herstellen einer Verbindung für eine [!DNL OAuth] -Anfrage

* [Allgemeine Anweisungen zum Erstellen einer Verbindung im HTTP > Erstellen eines OAuth 2.0-Anfragemoduls](#general-instructions-for-creating-a-connection-in-the-http--make-an-oauth-20-request-module)
* [Anweisungen zum Erstellen einer Verbindung zu Google im HTTP >[!UICONTROL Make] an OAuth 2.0-Anfragemodul](#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module)
* [Anleitung zum Herstellen einer Verbindung zur Microsoft Graph-API über HTTP > Erstellen eines OAuth 2.0-Anfragemoduls](#instructions-for-connecting-to-microsoft-graph-api-via-the-http--make-an-oauth-20-request-module)

### Allgemeine Anweisungen zum Erstellen einer Verbindung im Modul [!UICONTROL HTTP] > [!UICONTROL Erstellen einer OAuth 2.0-Anfrage]

1. Erstellen Sie einen OAuth-Client im [!DNL target]-Dienst, mit dem [!DNL Adobe Workfront Fusion] kommunizieren soll. Diese Option befindet sich höchstwahrscheinlich im Abschnitt [!UICONTROL Entwickler] des angegebenen Dienstes.

   1. Geben Sie beim Erstellen eines Clients die entsprechende URL in das Feld `[!UICONTROL Redirect URL]` oder `[!UICONTROL Callback URL]` ein:

      | Amerika/APAC | https://app.workfrontfusion.com/oauth/cb/oauth2 |
      |---|---|
      | EMEA | https://app-eu.workfrontfusion.com/oauth/cb/oauth2 |

   1. Nachdem Sie den Client erstellt haben, zeigt der angegebene Dienst zwei Schlüssel an: `[!UICONTROL Client ID]` und `[!UICONTROL Client Secret]`. Einige Dienste rufen diese `[!UICONTROL App Key]` und `[!UICONTROL App Secret]` auf. Speichern Sie den Schlüssel und das Geheimnis an einem sicheren Speicherort, damit Sie sie beim Erstellen der Verbindung in Workfront Fusion bereitstellen können.

1. Suchen Sie die `[!UICONTROL Authorize URI]` und `[!UICONTROL Token URI]` in der API-Dokumentation des angegebenen Dienstes. Dies sind URL-Adressen, über die [!DNL Workfront Fusion] mit dem [!DNL target]-Dienst kommuniziert. Die Adressen dienen der OAuth-Autorisierung.

   >[!NOTE]
   >
   >Wenn der Dienst den impliziten Fluss verwendet, benötigen Sie nur den `[!UICONTROL Authorize URI]`.

   >[!INFO]
   >
   >**Beispiel:** Yahoo-Adressen:
   >
   >* URI autorisieren:
   >
   >`https://api.login.yahoo.com/oauth2/request_auth`
   >
   >* Token-URI:
   >
   >`https://api.login.yahoo.com/oauth2/get_token`

1. (Bedingt) Wenn der Zieldienst Bereiche verwendet (Zugriffsberechtigungen), überprüfen Sie, wie der Dienst einzelne Bereiche trennt, und stellen Sie sicher, dass Sie das Trennzeichen in den erweiterten Einstellungen entsprechend festlegen. Wenn das Trennzeichen nicht korrekt festgelegt ist, kann [!DNL Workfront Fusion] die Verbindung nicht erstellen und Sie erhalten einen Fehler wegen ungültigen Umfangs.
1. Nachdem Sie die oben genannten Schritte ausgeführt haben, können Sie mit der Erstellung der OAuth-Verbindung in [!DNL Workfront Fusion] beginnen. Fügen Sie Ihrem Szenario das OAuth 2.0-HTTP(S)-Anfrage- und Antwortverarbeitungsmodul hinzu.
1. Klicken Sie im Feld Verbindung des Moduls auf **[!UICONTROL Hinzufügen]**.

1. Füllen Sie die folgenden Felder aus, um eine Verbindung zu erstellen:

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Verbindungsname] </td> 
      <td> <p>Geben Sie den Namen der Verbindung ein.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Flusstyp]</p> </td> 
      <td> <p>Wählen Sie den Fluss zum Abrufen von Token aus.</p> 
       <ul> 
        <li><strong>[!UICONTROL Autorisierungscode]</strong>: Geben Sie die <code>[!UICONTROL Authorize URI]</code> und die <code>[!UICONTROL Token URI]</code> aus der API-Dokumentation des Dienstes ein.</li> 
        <li><strong>[!UICONTROL Implicit]</strong>: Geben Sie die <code>[!UICONTROL Authorize URI]</code> in der API-Dokumentation des Dienstes ein.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Umfang] </td> 
      <td> <p>Einzelne Bereiche hinzufügen. Diese Informationen finden Sie in der Entwicklerdokumentation (API) des jeweiligen Dienstes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope separator] </td> 
      <td> <p>Wählen Sie aus, durch welche Bereiche die zuvor eingegebenen Bereiche getrennt werden sollen. Diese Informationen finden Sie in der Entwicklerdokumentation (API) des jeweiligen Dienstes.</p> <p>Warnung: Wenn das Trennzeichen nicht korrekt festgelegt ist, kann [!DNL Workfront Fusion] die Verbindung nicht erstellen und Sie erhalten einen Fehler wegen ungültigen Umfangs.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client-ID] </td> 
      <td> <p>Geben Sie die Client-ID ein. Sie haben die Client-ID erhalten, als Sie im Dienst, den Sie verbinden möchten, einen OAuth-Client erstellt haben.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td> <p> Geben Sie den Client-Geheimnis ein. Sie haben das Client-Geheimnis erhalten, als Sie einen OAuth-Client in dem Dienst erstellt haben, den Sie verbinden möchten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Autorisierungsparameter]</p> </td> 
      <td> <p>Fügen Sie alle Parameter hinzu, die Sie in den Autorisierungsaufruf einbeziehen möchten. Die folgenden Standardparameter werden immer automatisch eingeschlossen und müssen nicht hinzugefügt werden.</p> <p>Standardparameter:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL response_type]</strong> </p> <p> <code>code </code>für [!UICONTROL Autorisierungscode-Fluss] und <code>token </code>für [!UICONTROL Impliziter Fluss]</p> </li> 
        <li> <p><strong>[!UICONTROL redirect_uri]</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">Amerika/APAC</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">EMEA </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li> <p><strong>[!UICONTROL client_id]</strong> </p> <p> Die Client-ID, die Sie beim Erstellen des Kontos erhalten haben</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Zugriffstoken-Parameter]</p> </td> 
      <td> <p>Fügen Sie alle Parameter hinzu, die Sie in den Token-Aufruf aufnehmen möchten. Die folgenden Standardparameter werden immer automatisch eingeschlossen und müssen nicht hinzugefügt werden.</p> <p>Standardparameter:</p> 
       <ul> 
        <li><strong>[!UICONTROL grant_type]</strong>: <code>authorization_code</code></li> 
        <li> <p><strong>[!UICONTROL redirect_uri]:</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">Amerika/APAC</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">EMEA </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li><strong>[!UICONTROL client_id]</strong>: Die Client-ID, die Sie beim Erstellen des Kontos erhalten haben, wird automatisch im Anfragetext enthalten</li> 
        <li><strong>client_secret</strong>: Das Client-Geheimnis, das Sie beim Erstellen des Kontos erhalten haben, wird automatisch im Anfragetext enthalten</li> 
        <li><strong>code</strong>: Der von der Autorisierungsanfrage zurückgegebene Code</li> 
       </ul> <p>Hinweis:  <p>Der OAuth 2.0-Standard unterstützt mindestens 2 Methoden der Client-Authentifizierung während dieses Schritts (<code>[!UICONTROL client_secret_basic]</code> und <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] sendet automatisch die angegebene Client-ID und das Geheimnis über die Methode <code>[!UICONTROL client_secret_post]</code>. Daher werden diese Parameter automatisch als Teil des Token-Anforderungstextes einbezogen. </p> <p>Weitere Informationen zur OAuth 2.0-Authentifizierung finden Sie unter <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0 Authorization Framework</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Parameter des Aktualisierungstokens]</p> </td> 
      <td> <p>Fügen Sie alle Parameter hinzu, die Sie in den Token-Aufruf aufnehmen möchten. Die folgenden Standardparameter werden immer automatisch eingeschlossen und müssen nicht hinzugefügt werden.</p> <p>Standardparameter:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL grant_type]</strong>: <code>refresh_token</code></p> </li> 
        <li> <p><strong>[!UICONTROL refresh_token]</strong>: Das neueste Aktualisierungstoken, das vom Dienst abgerufen wurde, mit dem Sie eine Verbindung herstellen</p> </li> 
        <li> <p><strong>[!UICONTROL client_id]</strong>: Die Client-ID, die Sie beim Erstellen des Kontos erhalten haben, wird automatisch im Anfragetext enthalten</p> </li> 
        <li> <p><strong>[!UICONTROL client_secret]</strong>: Das Client-Geheimnis, das Sie beim Erstellen des Kontos erhalten haben, wird automatisch im Anfragetext enthalten</p> </li> 
       </ul> <p>Hinweis:  <p>Der OAuth 2.0-Standard unterstützt mindestens 2 Methoden der Client-Authentifizierung während dieses Schritts (<code>[!UICONTROL client_secret_basic]</code> und <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] sendet automatisch die angegebene Client-ID und das Geheimnis über die Methode <code>[!UICONTROL client_secret_post]</code>. Daher werden diese Parameter automatisch als Teil des Token-Anforderungstextes einbezogen. </p> <p>Weitere Informationen zur OAuth 2.0-Authentifizierung finden Sie unter <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0 Authorization Framework</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Benutzerdefinierte Kopfzeilen]</p> </td> 
      <td> <p>Geben Sie zusätzliche Schlüssel und Werte an, die in die Kopfzeile der Schritte [!UICONTROL Token] und R[!UICONTROL Aktualisierungstoken] aufgenommen werden sollen.</p> <p>Hinweis:  <p>Der OAuth 2.0-Standard unterstützt mindestens 2 Methoden der Client-Authentifizierung während dieses Schritts (<code>[!UICONTROL client_secret_basic]</code> und <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] unterstützt nicht automatisch die <code>[!UICONTROL client_secret_basic]</code> -Methode. Wenn der Dienst, mit dem Sie eine Verbindung herstellen möchten, erwartet, dass die Client-ID und das Client-Geheimnis zu einer einzelnen Zeichenfolge kombiniert und dann base64-kodiert in der Autorisierungskopfzeile werden, sollten Sie diese Kopfzeile und diesen Schlüsselwert hier hinzufügen.</p> <p> Weitere Informationen zur OAuth 2.0-Authentifizierung finden Sie unter <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0 Authorization Framework</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Token placement]</p> </td> 
      <td> <p>Wählen Sie aus, ob das Token im [!UICONTROL Header], in der [!UICONTROL Abfragezeichenfolge] oder in beiden beim Herstellen einer Verbindung zur angegebenen URL gesendet werden soll.</p> <p>Token werden meist im Anfrageheader gesendet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Header-Token-Name] </td> 
      <td> <p>Geben Sie den Namen des Autorisierungstokens in die Kopfzeile ein. Standard: <code>[!UICONTROL Bearer]</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Parametername der Abfragezeichenfolge] </td> 
      <td> <p>Geben Sie den Namen des Autorisierungstokens in die Abfragezeichenfolge ein. Standard: <code>[!UICONTROL access_token]</code>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindungseinstellungen zu speichern.
1. Fahren Sie mit [OAuth 2.0 request module setup](#oauth-20-request-module-setup) fort.

### Anweisungen zum Erstellen einer Verbindung zu [!DNL Google] im [!UICONTROL HTTP] >[!UICONTROL Erstellen eines OAuth 2.0-Anfragemoduls]

Das folgende Beispiel zeigt, wie Sie das Anfragemodul [!UICONTROL HTTP] > [!UICONTROL Erstellen eines OAuth 2.0] verwenden, um eine Verbindung zu [!DNL Google] herzustellen.

1. Stellen Sie sicher, dass Sie ein Projekt erstellt, OAuth-Einstellungen konfiguriert und Ihre Anmeldedaten generiert haben, wie in [Verbinden [!DNL Adobe Workfront Fusion] mit [!DNL Google Services] unter Verwendung eines benutzerdefinierten OAuth-Clients](../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md) beschrieben.
1. Öffnen Sie das Modul [!UICONTROL HTTP] >[!UICONTROL Erstellen einer OAuth 2.0-Anfrage] .
1. Klicken Sie neben dem Verbindungsfeld auf **[!UICONTROL Hinzufügen]** .
1. Geben Sie die folgenden Werte ein:

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Verbindungsname] </td> 
      <td> <p>Geben Sie den Namen der Verbindung ein.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Flusstyp]</p> </td> 
      <td> <p>[!UICONTROL Autorisierungscode]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Autorisierungs-URI]</td> 
      <td><code>https://accounts.google.com/o/oauth2/v2/auth</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token URI]</td> 
      <td><code>https://www.googleapis.com/oauth2/v4/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Umfang] </td> 
      <td> <p>Einzelne Bereiche hinzufügen. Weitere Informationen zu Bereichen finden Sie unter <a href="https://developers.google.com/identity/protocols/oauth2/scopes">OAuth 2.O-Bereiche für [!DNL Google] APIs</a> in der Dokumentation zu [!DNL Google].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope separator] </td> 
      <td> <p>[!UICONTROL SPACE]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client-ID] </td> 
      <td> <p>Geben Sie Ihre [!DNL Google] Client-ID ein. </p> <p>Informationen zum Erstellen einer Client-ID finden Sie unter <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">OAuth-Anmeldedaten erstellen</a> in <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] bis [!DNL Google Services] unter Verwendung eines benutzerdefinierten OAuth-Clients</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td> <p>Geben Sie Ihr [!DNL Google] Client-Geheimnis ein. </p> <p>Informationen zum Erstellen eines Client-Geheimnisses finden Sie unter <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">OAuth-Anmeldedaten erstellen</a> in <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] in [!DNL Google] Dienste mit einem benutzerdefinierten OAuth-Client</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Autorisierungsparameter]</p> </td> 
      <td> <p>Fügen Sie das Schlüssel-Wert-Paar <code>[!UICONTROL access_type]</code> - <code>[!UICONTROL offline] </code>hinzu.</p> <p> <img src="assets/google-authentication-http.png"> </p> <p>Hinweis: Wenn Authentifizierungsprobleme auftreten, z. B. beim Aktualisieren von Token, versuchen Sie, das Schlüssel-Wert-Paar <code>[!UICONTROL prompt] </code> - <code>[!UICONTROL consent] </code>hinzuzufügen.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindungseinstellungen zu speichern.
1. Fahren Sie mit [OAuth 2.0 request module setup](#oauth-20-request-module-setup) fort.

### Anweisungen zum Herstellen einer Verbindung zu [!DNL Microsoft Graph API] über das Modul [!UICONTROL HTTP] > [!UICONTROL Erstellen einer OAuth 2.0-Anforderung]

Anweisungen zu [!DNL Microsoft Graph API] finden Sie unter [Aufrufen der  [!DNL MS Graph REST API] über das Modul [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Erstellen einer OAuth 2.0-Anforderung]](../../../workfront-fusion/connections/call-the-ms-graph-rest-api.md).

## Einrichten des OAuth 2.0-Anforderungsmoduls

Wenn Sie eine [!DNL Oauth 2].0-Verbindung hergestellt haben, wie in [Erstellen einer Verbindung für eine [!DNL OAuth] Anfrage](#creating-a-connection-for-an-oauth-request) beschrieben, fahren Sie mit der Einrichtung des Moduls wie gewünscht fort. Alle Autorisierungstoken werden automatisch in diese Anfrage und in jede andere Anfrage einbezogen, die dieselbe Verbindung verwendet.

Wenn Sie das Modul [!UICONTROL HTTP] >[!UICONTROL Erstellen einer OAuth 2.0-Anfrage] konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

<!--
<img src="assets/map-toggle-350x74.png" style="width: 350;height: 74;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Informationen zum Einrichten einer Verbindung finden Sie unter <a href="#creating-a-connection-for-an-oauth-request" class="MCXref xref">Erstellen einer Verbindung für eine OAuth-Anforderung</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Alle Status als Fehler auswerten (mit Ausnahme von 2xx und 3xx]) </td> 
   <td> <p>Verwenden Sie diese Option, um die Fehlerbehandlung einzurichten.</p> <p>Weitere Informationen finden Sie unter <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">Umgang mit Fehlern in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Geben Sie die URL ein, an die Sie eine Anfrage senden möchten, z. B. einen API-Endpunkt, eine Website usw.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Methode]</p> </td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header] </td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu. Beispiel: <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p> Geben Sie die gewünschten Schlüssel-Wert-Paare für die Abfrage ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Textkörper]</p> </td> 
   <td> <p>Der HTTP-Hauptteil sind die Daten-Bytes, die in einer HTTP-Transaktionsnachricht unmittelbar auf die Header übertragen werden, sofern welche verwendet werden sollen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>Der Rohkörpertyp eignet sich im Allgemeinen für die meisten HTTP-Textkörperanforderungen, selbst wenn in der Entwicklerdokumentation keine zu sendenden Daten angegeben sind.</p> <p>Geben Sie im Feld [!UICONTROL Inhaltstyp] eine Form zum Analysieren der Daten an.</p> <p>Trotz des ausgewählten Inhaltstyps werden die Daten in einem beliebigen Format eingegeben, das in der Entwicklerdokumentation festgelegt oder benötigt wird.</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>Dieser Nachrichtentyp dient der POST von Daten mit <code>[!UICONTROL application/x-www-form-urlencoded]</code>.</p> <p>Bei <code>[!UICONTROL application/x-www-form-urlencoded]</code> ist der Hauptteil der an den Server gesendeten HTTP-Nachricht im Wesentlichen eine Abfragezeichenfolge. Die Schlüssel und Werte werden in Schlüssel-Wert-Paaren kodiert, die durch <code>&amp;</code> getrennt sind, und in einem <code>=</code> zwischen Schlüssel und Wert. </p> <p>Für Binärdaten ist stattdessen <code>use [!UICONTROL multipart/form-data]</code> erforderlich.</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>Beispiel: </b></span></span> 
       <p>Beispiel für das resultierende HTTP-Anforderungsformat:</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL Multipart/form-data]</strong> </p> <p>[!UICONTROL Multipart/form-data] ist eine HTTP-Multipart-Anfrage zum Senden von Dateien und Daten. Sie wird häufig zum Hochladen von Dateien auf den Server verwendet.</p> <p>Fügen Sie Felder hinzu, die in der Anfrage gesendet werden sollen. Jedes Feld muss ein Schlüssel-Wert-Paar enthalten.</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Text]</strong> </p> <p>Geben Sie den Schlüssel und den Wert ein, die im Anfrageinhalt gesendet werden sollen.</p> </li> 
       <li> <p><strong>[!UICONTROL Datei]</strong> </p> <p>Geben Sie den Schlüssel ein und geben Sie im Anfragetext die Quelldatei an, die Sie senden möchten.</p> <p>Ordnen Sie die Datei zu, die Sie vom vorherigen Modul hochladen möchten (z. B. [!UICONTROL HTTP] &gt;[!UICONTROL Datei abrufen] oder [!UICONTROL Google Drive] &gt;[!UICONTROL Datei herunterladen), oder geben Sie den Dateinamen und die Dateidaten manuell ein.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Parse response]</p> </td> 
   <td> <p>Aktivieren Sie diese Option, um Antworten automatisch zu analysieren und JSON- und XML-Antworten zu konvertieren, sodass Sie nicht [!UICONTROL JSON] &gt; [!UICONTROL Parse JSON] oder [!UICONTROL XML] &gt; [!UICONTROL Parse XML] Module verwenden müssen.</p> <p>Bevor Sie geparsten JSON- oder XML-Inhalt verwenden können, führen Sie das Modul einmal manuell aus, damit das Modul den Antwortinhalt erkennen und ihn in nachfolgenden Modulen zuordnen kann.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timeout] </td> 
   <td> <p>Geben Sie den Anforderungstimeout in Sekunden (1-300) ein. Der Standardwert beträgt 40 Sekunden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cookies mit anderen HTTP-Modulen teilen]</td> 
   <td> <p> Aktivieren Sie diese Option, um Cookies vom Server für alle HTTP-Module in Ihrem Szenario freizugeben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Selbstsigniertes Zertifikat]</td> 
   <td> <p> Laden Sie das Zertifikat hoch, wenn Sie TLS mit Ihrem selbst signierten Zertifikat verwenden möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ablehnen von Verbindungen, die nicht überprüfte (selbstsignierte) Zertifikate verwenden] </td> 
   <td> <p>Aktivieren Sie diese Option, um Verbindungen abzulehnen, die nicht überprüfte TLS-Zertifikate verwenden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Weiterleitung]</td> 
   <td> <p> Aktivieren Sie diese Option, um URL-Umleitungen mit 3xx-Antworten zu folgen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Alle Umleitungen folgen] </td> 
   <td> <p>Aktivieren Sie diese Option, um den URL-Umleitungen mit allen Antwort-Codes zu folgen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Deaktivieren der Serialisierung mehrerer Abfragezeichenfolgenschlüssel als Arrays]</p> </td> 
   <td> <p>Standardmäßig verarbeitet [!DNL Workfront Fusion] mehrere Werte für denselben URL-Abfragezeichenfolgen-Parameterschlüssel wie Arrays. Beispielsweise wird <code>www.test.com?foo=bar&amp;foo=baz</code> in <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code> umgewandelt. Aktivieren Sie diese Option, um diese Funktion zu deaktivieren. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Komprimierten Inhalt anfordern]</td> 
   <td> <p> Aktivieren Sie diese Option, um eine komprimierte Version der Website anzufordern.</p> <p>Dadurch wird ein <code>[!UICONTROL Accept-Encoding]</code> -Header hinzugefügt, um komprimierten Inhalt anzufordern.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Gegenseitige TLS verwenden]</td> 
   <td> <p>Aktivieren Sie diese Option, um in der HTTP-Anforderung die Verwendung von TLS mit Gegenseitigkeit vorzunehmen.</p> <p>Weitere Informationen zu TLS auf Gegenseitige Basis finden Sie unter <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">Verwenden von TLS auf Gegenseitiger Basis in HTTP-Modulen in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
