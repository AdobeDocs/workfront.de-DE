---
title: Erstellen von OAuth2-Anwendungen für  [!DNL Workfront] -Integrationen
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Als Administrator  [!DNL Adobe Workfront]  Sie OAuth2-Programme für Ihre Instanz von erstellen [!DNL Workfront] die anderen Programmen den Zugriff auf Workfront ermöglichen. Ihre Benutzer können dann diesen anderen Anwendungen die Berechtigung erteilen, auf ihre Workfront-Daten zuzugreifen. Auf diese Weise können Sie Workfront mit Anwendungen Ihrer Wahl integrieren, einschließlich Ihrer eigenen internen Anwendungen.
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: e13c7dda-8945-47ad-b6d3-4d6a62b368f5
source-git-commit: 711812d9fd4bf48bb7612c0339cee2cdbe08ef10
workflow-type: tm+mt
source-wordcount: '1960'
ht-degree: 6%

---

# Erstellen von OAuth2-Programmen für [!DNL Workfront] Integrationen

Als [!DNL Adobe Workfront] können Sie OAuth2-Programme für Ihre Instanz von [!DNL Workfront] erstellen, die anderen Programmen den Zugriff auf [!DNL Workfront] ermöglichen. Ihre Benutzer können dann diesen anderen Anwendungen die Berechtigung erteilen, auf ihre [!DNL Workfront] Daten zuzugreifen. Auf diese Weise können Sie integrieren   Mit Anwendungen Ihrer Wahl, einschließlich eigener Anwendungen.

Beim Erstellen einer [!UICONTROL OAuth2]-Anwendung generieren Sie eine Client-ID und ein Client-Geheimnis. Ihre Benutzer können dann die Client-ID in API-Aufrufen verwenden, um sie in die von Ihnen erstellte Anwendung zu integrieren.

>[!NOTE]
>
>Im Kontext von OAuth2 bezieht sich „Erstellen einer App“ auf den Prozess der Erstellung einer solchen Art von Zugriffs-Link zwischen einer App und einem Server wie [!DNL Workfront].

* Anweisungen zur Konfiguration und Verwendung der OAuth2-Anwendung mit Benutzeranmeldeinformationen (Autorisierungs-Code-Fluss) finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe eines Autorisierungs-Code-Flusses](../../wf-api/api/oauth-app-code-token-flow.md).
* Anweisungen zur Konfiguration und Verwendung der OAuth2-Anwendung mithilfe der Server-Authentifizierung (JWT-Fluss) finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe des JWT-Flusses](../../wf-api/api/oauth-app-jwt-flow.md).
* Anweisungen zur Konfiguration und Verwendung der OAuth2-Anwendung mithilfe von PKCE finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe von PKCE-Fluss](../../wf-api/api/oauth-app-pkce-flow.md).

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

## OAuth2 - Übersicht

Angenommen, eine Anwendung muss bestimmte Informationen aus [!DNL Workfront] abrufen. Eine Anwendung, die Informationen anfordert, wird als Client bezeichnet. In diesem Beispiel lautet der Client-Name ClientApp. ClientApp benötigt Zugriff auf die Informationen eines bestimmten Benutzers und muss daher als dieser Benutzer auf [!DNL Workfront] zugreifen. Wenn Ihr Benutzer ClientApp den Benutzernamen und das Passwort gibt, kann ClientApp auf alle Daten zugreifen, auf die der Benutzer zugreifen kann. Dies ist ein Sicherheitsrisiko, da ClientApp nur einen kleinen, spezifischen Satz von Informationen benötigt.

Wenn Sie eine OAuth2-App für ClientApp erstellen, geben Sie im Wesentlichen an, [!DNL Workfront] ClientApp berechtigt ist, auf [!DNL Workfront] zuzugreifen, jedoch nur, wenn der Benutzer, auf dessen Konto ClientApp zugreift, die Berechtigung für den Zugriff erteilt.

## Erstellen eines OAuth2-Programms

Wählen Sie beim Erstellen eines OAuth2-Programms den Anwendungstyp aus, der den Anforderungen Ihrer Integration am besten entspricht.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Anwendungstyp</th> 
   <th>Am besten geeignet für</th> 
   <th>Authentifizierungsmethode</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Maschine-zu-Maschine-Anwendung</p> </td> 
   <td> <p>Optimiert für CLIs, Daemons oder Skripte, die auf Ihrem Server ausgeführt werden</p> <p>Beispiele:</p> 
    <ul> 
     <li> <p>[!DNL Shell] </p> </li> 
     <li> <p>[!DNL Python]</p> </li> 
    </ul> </td> 
   <td> <p>Authentifizierung mit JSON-Web-Token mit Verschlüsselung des öffentlichen/privaten Schlüsselpaares.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Single Page Application (einseitige Web-Anwendung)</p> </td> 
   <td> <p>Optimiert für mobile oder Single Page Applications (SPAs)</p> <p>Beispiele:</p> 
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
   <td> <p>Optimiert für Server-seitige Anwendungen, die Anmeldeinformationen und Token auf dem Server verarbeiten</p> <p>Beispiele:</p> 
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

* [Erstellen einer OAuth2-Anwendung mit Server-Authentifizierung (JWT-Fluss)](#create-an-oauth2-application-using-server-authentication-jwt-flow)
* [Erstellen einer OAuth2-Anwendung mit Benutzeranmeldeinformationen (Autorisierungs-Code-Fluss)](#create-an-oauth2-application-using-user-credentials-authorization-code-flow)
* [Erstellen einer einseitigen OAuth2-Webanwendung mit PKCE](#create-an-oauth2-single-page-web-application-using-pkce)

### Erstellen einer OAuth2-Anwendung mit Server-Authentifizierung (JWT-Fluss) {#create-an-oauth2-application-using-server-authentication-jwt-flow}

{{step-1-to-setup}}

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]** und wählen Sie dann **[!UICONTROL OAuth2-Anwendungen]**.
1. Klicken Sie **[!UICONTROL App-Integration erstellen]**.
Das **Neue OAuth2-Anwendung** wird angezeigt.
1. Wählen Sie im Feld **Neue OAuth2** die Option **[!UICONTROL Anwendung von Computer zu Computer]** aus.
1. Geben Sie einen Namen für das neue Programm ein, z. B. &quot;[!DNL Workfront] for ClientApp“.
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
      <td role="rowheader">[!UICONTROL Client-Geheimnis]</td> 
      <td> <p>Dieses Feld wird automatisch generiert</p> <p><b>WICHTIG</b>:  <p>Kopieren Sie den Inhalt dieses Felds in eine andere sichere Datei, bevor Sie diese Seite schließen. Dieser geheime Schlüssel wird nicht mehr angezeigt.</p> <p>Wenn Sie diesen Schlüssel verlieren, löschen Sie ihn und erstellen Sie ein Client-Geheimnis.</p> 
        <ol> 
         <li value="1"> <p>Klicken Sie auf das Symbol <b>[!UICONTROL Löschen]</b>, <img src="assets/delete.png"> das aktuelle Client-Geheimnis zu löschen.</p> </li> 
         <li value="2"> <p>Klicken Sie auf <b>[!UICONTROL Client-Geheimnis hinzufügen]</b>, um ein neues Client-Geheimnis zu generieren.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Öffentliche Schlüssel]</td> 
      <td> <p>Server-zu-Server-Apps verwenden öffentliche und private Schlüssel für die Authentifizierung. Führen Sie einen der folgenden Schritte aus:</p> 
       <ul> 
        <li> <p>Klicken Sie auf <b>[!UICONTROL Öffentlichen Schlüssel hinzufügen]</b> und geben Sie den öffentlichen Schlüssel aus der anderen Anwendung ein.</p> </li> 
        <li> <p>Klicken Sie auf <b>[!UICONTROL Schlüsselpaar aus öffentlichem/privatem Schlüssel generieren]</b> und geben Sie dann den öffentlichen Schlüssel für die andere Anwendung frei.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Dies ist der gleiche Name, den Sie der App gegeben haben. Dieses Feld darf nicht leer sein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Beschreibung]</td> 
      <td>Geben Sie eine Beschreibung für die Integration ein.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Speichern]**.

Anweisungen zur Konfiguration und Verwendung der OAuth2-Anwendung mit Benutzeranmeldeinformationen (Autorisierungs-Code-Fluss) finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe von JWT-Fluss](../../wf-api/api/oauth-app-jwt-flow.md).

### Erstellen einer OAuth2-Anwendung mit Benutzeranmeldeinformationen (Autorisierungs-Code-Fluss) {#create-an-oauth2-application-using-user-credentials-authorization-code-flow}

>[!NOTE]
>
>Wenn Sie eine Anwendung erstellen, um eine Verbindung zu Workfront Fusion herzustellen, verwenden Sie eine der folgenden Umleitungs-URLs:
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-workfront`
>* `https://app-eu.workfrontfusion.com/oauth/cb/workfront-workfront` (EU-Rechenzentrum)
>* `https://app-az.workfrontfusion.com/oauth/cb/workfront-workfront` (Azure Data Center)

{{step-1-to-setup}}

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]** und wählen Sie dann **[!UICONTROL OAuth2-Anwendungen]**.
1. Klicken Sie **[!UICONTROL App-Integration erstellen]**.

   Die **Neue OAuth2-Anwendung** wird angezeigt.
1. Wählen Sie im **Neue OAuth2** Anwendung) die Option **[!UICONTROL Webanwendung]** aus.
1. Geben Sie einen Namen für das neue OAuth2-Programm ein, z. B. &quot;[!DNL Workfront] for ClientApp“.
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
      <td role="rowheader">[!UICONTROL Client-Geheimnis]</td> 
      <td> <p>Dieses Feld wird automatisch generiert</p> <p><b>WICHTIG</b>:  <p>Kopieren Sie den Inhalt dieses Felds in eine andere sichere Datei, bevor Sie diese Seite schließen. Dieser geheime Schlüssel wird nicht mehr angezeigt.</p> <p>Wenn Sie diesen Schlüssel verlieren, löschen Sie ihn und erstellen Sie ein Client-Geheimnis.</p> 
        <ol> 
         <li value="1"> <p>Klicken Sie auf das Symbol <b>[!UICONTROL Löschen]</b>, <img src="assets/delete.png"> das aktuelle Client-Geheimnis zu löschen.</p> </li> 
         <li value="2"> <p>Klicken Sie auf <b>[!UICONTROL Client-Geheimnis hinzufügen]</b>, um ein neues Client-Geheimnis zu generieren.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Umleitungs-URLs]</td> 
      <td>Benutzer werden zu diesem Pfad weitergeleitet, nachdem sie sich bei [!DNL Workfront] authentifiziert haben.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Token-Rotation aktualisieren]</td> 
      <td>Aktivieren Sie diese Option, um jedes Mal, wenn ein Refresh-Token verwendet wird, ein neues Refresh-Token zu erstellen. Ihre Anwendung muss das neue Refresh-Token nach jeder Aktualisierung speichern.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Absolute Aktualisierungstoken-Gültigkeit]</td> 
      <td> <p>Wählen Sie die Zeitspanne aus, für die ein Aktualisierungstoken vorhanden sein soll, bevor es abläuft. Nach Ablauf müssen sich Ihre Benutzer erneut bei der Integration anmelden. Wählen Sie "[!UICONTROL Kein Ablauf]", wenn das Aktualisierungstoken nicht ablaufen soll.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Gültigkeit des Inaktivitätsaktualisierungs-Tokens</td> 
      <td> <p>Wählen Sie die Zeitspanne aus, nach der das Aktualisierungstoken abläuft, wenn der Benutzer in Ihrem System nicht aktiv war. </p> <p>Wenn beispielsweise die Gültigkeit des Inaktivitäts-Aktualisierungstokens 6 Monate beträgt und sich der Benutzer sechs Monate lang nicht anmeldet, läuft das Aktualisierungstoken ab, obwohl die absolute Gültigkeit des Aktualisierungstokens möglicherweise länger eingestellt ist.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Logo]</td> 
      <td>Sie können ein Logo hinzufügen, um diese App leichter identifizierbar zu machen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Dies ist der gleiche Name, den Sie der App gegeben haben. Dieses Feld darf nicht leer sein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Beschreibung]</td> 
      <td>Geben Sie eine Beschreibung für die Integration ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL App Description URL]</td> 
      <td>Dabei kann es sich um einen Link zu einer „Über uns“-Seite oder um eine Seite mit weiteren Informationen zur Integration handeln.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Speichern]**.

Anweisungen zur Konfiguration und Verwendung der OAuth2-Anwendung mit Benutzeranmeldeinformationen (Autorisierungs-Code-Fluss) finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe eines Autorisierungs-Code-Flusses](../../wf-api/api/oauth-app-code-token-flow.md).

### Erstellen einer einseitigen OAuth2-Webanwendung mit PKCE {#create-an-oauth2-single-page-web-application-using-pkce}

{{step-1-to-setup}}

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]** und wählen Sie dann **[!UICONTROL OAuth2-Anwendungen]**.
1. Klicken Sie **[!UICONTROL App-Integration erstellen]**.

   Das **Neue OAuth2-Anwendung** wird angezeigt.
1. Wählen Sie im **Neue OAuth2** Anwendung) die Option **[!UICONTROL Einzelseiten-Webanwendung]** aus.
1. Geben Sie einen Namen für das neue [!UICONTROL OAuth2]-Programm ein, z. B. &quot;[!DNL Workfront] für ClientApp“.
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
      <td>Benutzer werden zu diesem Pfad weitergeleitet, nachdem sie sich bei Workfront authentifiziert haben.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Aktualisierungstoken jedes Mal drehen, wenn es verwendet wird]</td> 
      <td>Aktivieren Sie diese Option, um jedes Mal, wenn ein Refresh-Token verwendet wird, ein neues Refresh-Token zu erstellen. Ihre Anwendung muss das neue Refresh-Token nach jeder Aktualisierung speichern.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Absolute Gültigkeit]</td> 
      <td> <p>Wählen Sie die Zeitspanne aus, für die ein Aktualisierungstoken vorhanden sein soll, bevor es abläuft. Nach Ablauf müssen sich Ihre Benutzer erneut bei der Integration anmelden. Wählen Sie "[!UICONTROL Kein Ablauf]", wenn das Aktualisierungstoken nicht ablaufen soll.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Gültigkeit bei Inaktivität]</td> 
      <td> <p>Wählen Sie die Zeitspanne aus, nach der das Aktualisierungstoken abläuft, wenn der Benutzer in Ihrem System nicht aktiv war. </p> <p>Wenn beispielsweise die Gültigkeit des Inaktivitäts-Aktualisierungstokens 6 Monate beträgt und sich der Benutzer sechs Monate lang nicht anmeldet, läuft das Aktualisierungstoken ab, obwohl die absolute Gültigkeit des Aktualisierungstokens möglicherweise länger eingestellt ist.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Logo]</td> 
      <td>Sie können ein Logo hinzufügen, um diese App leichter identifizierbar zu machen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Dies ist der gleiche Name, den Sie der App gegeben haben. Dieses Feld darf nicht leer sein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Beschreibung]</td> 
      <td>Geben Sie eine Beschreibung für die Integration ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name des Entwicklers]</td> 
      <td>Dies ist der Name des Entwicklers, der die OAuth2-Anwendung einrichtet.</td> 
     </tr> 
   <tr> 
      <td role="rowheader">[!UICONTROL E-Mail-Adresse des Entwicklers]</td> 
      <td>Dies ist die E-Mail-Adresse des Entwicklers, der die OAuth2-Anwendung einrichtet.</td> 
     </tr> 
   <tr> 
      <td role="rowheader">[!UICONTROL URL der Datenschutzrichtlinie]</td> 
      <td>Dies ist der Link, unter dem Ihr Unternehmen die Datenschutzrichtlinie speichert.</td> 
     </tr>


   </tbody> 
   </table>

   <!-- removed this from the table, and added "Developer name" and following rows:
   [!UICONTROL App Description URL]</td> 
      <td>This can be a link to an "About us" page or a page with more information about the integration.> -->

1. Klicken Sie auf **[!UICONTROL Speichern]**.

## Konfigurieren und Verwenden der erstellten OAuth2-Anwendung

Für die weitere Konfiguration und Verwendung der erstellten OAuth2-Anwendung sind einige technische Kenntnisse erforderlich, einschließlich API-Aufrufen.

* Anweisungen zur Konfiguration und Verwendung der OAuth2-Anwendung mit Benutzeranmeldeinformationen (Autorisierungs-Code-Fluss) finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe eines Autorisierungs-Code-Flusses](../../wf-api/api/oauth-app-code-token-flow.md).
* Anweisungen zur Konfiguration und Verwendung der OAuth2-Anwendung mithilfe der Server-Authentifizierung (JWT-Fluss) finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe des JWT-Flusses](../../wf-api/api/oauth-app-jwt-flow.md).
* Anweisungen zur Konfiguration und Verwendung der OAuth2-Anwendung mithilfe von PKCE finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe von PKCE-Fluss](../../wf-api/api/oauth-app-pkce-flow.md).

## OAuth2-Prozesse für Autorisierungs-Code-Fluss

>[!NOTE]
>
>Ihre Benutzer greifen über die API auf [!UICONTROL OAuth2]-Anwendung zu. In diesem Abschnitt werden die Funktionen in allgemeinen Begriffen beschrieben. Er dient nur zu Informationszwecken.
>
>Spezifische Anweisungen zur Verwendung der OAuth2-Anwendung, einschließlich spezifischer API-Aufrufe, finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe des Autorisierungs-Code-Flusses](../../wf-api/api/oauth-app-code-token-flow.md).

### Autorisierung mit Autorisierungs-Code und Zugriffs-Token {#authorizing-with-an-authorization-code-and-access-token}

1. ClientApp benötigt einige Informationen von [!DNL Workfront], daher sendet es eine Anfrage an den [!DNL Workfront]-Endpunkt der `/authorize`-API. Die Anfrage enthält den RESPONSE_TYPE`code`, der angibt, dass die Anfrage einen Autorisierungs-Code zurückgeben soll.
1. Dieser Trigger [!DNL Workfront] eine Authentifizierungsaufforderung an den Benutzer senden. Der Benutzer kann seine Anmeldeinformationen in die Eingabeaufforderung eingeben, wodurch [!DNL Workfront] Berechtigung zur Kommunikation mit ClientApp erhält. Wenn der Benutzer bereits bei [!DNL Workfront] angemeldet ist, kann dieser Schritt übersprungen werden.
1. Die [!DNL Workfront]-API sendet einen Autorisierungs-Code an ClientApp.
1. ClientApp sendet in einer Anfrage die folgenden Informationen an die [!DNL Workfront]-API `/token`   Endpunkt:

   * Der Autorisierungs-Code, der in Schritt 3 an ClientApp gesendet wurde. Dadurch wird die spezifische Instanz der Benutzerberechtigung identifiziert.
   * Das Client-Geheimnis, das beim Einrichten der ClientApp OAuth2-App in [!DNL Workfront] generiert wurde. Auf diese Weise können [!DNL Workfront] feststellen, dass die Anfrage von ClientApp stammt.

1. Wenn der Autorisierungs-Code und das Client-Geheimnis korrekt sind, sendet [!DNL Workfront] ein Zugriffs-Token an ClientApp. Dieses Zugriffstoken wird direkt von [!DNL Workfront] an ClientApp gesendet und kann von keinem anderen Benutzer und keiner anderen Client-Anwendung angezeigt, kopiert oder verwendet werden.
1. ClientApp sendet das Zugriffstoken zusammen mit der spezifischen Informationsanfrage an [!DNL Workfront].
1. Da das Zugriffstoken korrekt ist, sendet [!DNL Workfront] die Informationen an ClientApp.

#### Aktualisieren von Zugriffstoken

Aus Sicherheitsgründen laufen Zugriffstoken nach kurzer Zeit ab. Um neue Zugriffstoken zu erhalten, ohne jedes Mal Anmeldeinformationen eingeben zu müssen, verwendet [!DNL OAuth2] Aktualisierungstoken. Aktualisierungs-Token werden vom Client gespeichert.

Der Prozess zum Erfassen eines Aktualisierungs-Tokens ist identisch mit dem Verfahren, das im Abschnitt [Autorisieren mit einem Autorisierungs-Code und Zugriffs-Token](#authorizing-with-an-authorization-code-and-access-token) beschrieben wird. Die Anfrage für den Autorisierungs-Code enthält den `offline_access`, der angibt, dass die Anfrage ein Anfrage-Token zusammen mit dem Autorisierungs-Code zurückgeben soll.
