---
title: Rufen Sie die MS Graph REST API über die [!DNL Adobe Workfront Fusion] HTTP &gt; Erstellen eines OAuth 2.0-Anforderungsmoduls
description: Rufen Sie die MS Graph REST API über die [!DNL Adobe Workfront Fusion] HTTP &gt; Erstellen eines OAuth 2.0-Anforderungsmoduls
author: Becky
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 1%

---

# Rufen Sie die[!UICONTROL  MS Graph REST API] über die [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0-Anfrage stellen] Modul

<!-- Audited: 3/2024-->

Viele [!DNL Microsoft] auf Webdienste über [!DNL Microsoft Graph API]. Sie können eine Verbindung zum [!DNL Microsoft Graph API], indem Sie die [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL OAuth 2.0-Anfrage stellen] -Modul.

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
   <p>Aktuell: Nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Veraltet: Beliebig </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Neu:</p> <ul><li>[!UICONTROL Select] oder [!UICONTROL Prime] [!DNL Workfront] Plan: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] ist enthalten.</li></ul>
   <p>Oder</p>
   <p>Aktuell: Ihr Unternehmen muss Einkäufe tätigen [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## registrieren [!DNL Workfront Fusion] im [!DNL Microsoft Application Registration Portal]

So erstellen Sie eine Verbindung zum [!DNL Microsoft Graph REST API]müssen Sie sich zuerst registrieren [!DNL Adobe Workfront Fusion].

1. Registrieren Sie eine neue Anwendung wie unter [App registrieren](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) im [!DNL Microsoft] Dokumentation.

   Im Rahmen der Registrierung [!DNL Microsoft] erfordert die folgenden Informationen:

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Anwendungsname]</td>
        <td>Geben Sie einen Namen für die Anwendung ein, z. B. [!DNL Workfront Fusion] Anwendung."</td>
      </tr>
      <tr>
        <td>[!UICONTROL Umleitungs-URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. Wenn Sie die App-Registrierung abgeschlossen haben, notieren Sie sich die [!UICONTROL Bewerbungs-ID].

   >[!IMPORTANT]
   >
   >Sie benötigen die Anwendungs-ID, um Ihre Verbindung in [!DNL Workfront Fusion].

1. Generieren Sie eine [!UICONTROL Anwendungsgeheimnis]. Notieren Sie sich dieses Geheimnis!

   Anweisungen finden Sie unter [App registrieren](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) im [!DNL Microsoft] Dokumentation.

   >[!IMPORTANT]
   >
   >Sie benötigen die [!UICONTROL Anwendungsgeheimnis] zur Einrichtung Ihrer Verbindung in [!DNL Workfront Fusion].

1. Konfigurieren Sie die Berechtigungen für Ihre Anwendung.

   Weitere Informationen zum Suchen und Konfigurieren dieser Felder finden Sie im Abschnitt &quot;Berechtigungen für Microsoft-Diagramm konfigurieren&quot;unter [Zugriff ohne Benutzer erhalten](https://docs.microsoft.com/en-us/graph/auth-v2-service) im [!UICONTROL Microsoft] Dokumentation.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Welchen Berechtigungstyp benötigt Ihre Anwendung?]</td> 
      <td>Auswählen <code>[!UICONTROL Delegated permissions]</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Berechtigungen auswählen]</td> 
      <td> <p>Wählen Sie die folgenden Berechtigungen aus:</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>Alle anderen für Ihre Integrationen erforderlichen Berechtigungen (Beispiel: <code>User.Read</code>)</p> </li> 
       </ul> <p><b>Wichtig</b>: Sie benötigen die ausgewählten Berechtigungen, um Ihre Verbindung in einzurichten. [!DNL Workfront Fusion].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fahren Sie mit [Konfigurieren Sie Ihre [!DNL MS Graph API] Verbindung in [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## Konfigurieren Sie Ihre [!DNL MS Graph API] Verbindung in [!DNL Workfront Fusion]

Nach der Registrierung [!DNL Workfront Fusion] wie in [registrieren [!DNL Workfront Fusion] im [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal), können Sie Ihre Verbindung im [!UICONTROL HTTP] > [!UICONTROL Erstellen einer OAuth 2.0] -Anfragemodul.

1. Hinzufügen einer [!UICONTROL HTTP] > [!UICONTROL Ausführen eines OAuth 2.0-Aufrufs] zu Ihrem Szenario.
1. Klicks **[!UICONTROL Hinzufügen]** neben dem [!UICONTROL connection] -Feld.
1. Konfigurieren Sie die Verbindungsfelder wie folgt:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Verbindungsname]</td> 
      <td>Geben Sie einen Namen für die Verbindung ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Flusstyp]</p> </td> 
      <td><code>[!UICONTROL Authorization Code]</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Autorisierungs-URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/authorize</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Umfang]</td> 
      <td> <p>Geben Sie die Berechtigungen ein, die Sie in Schritt 4 von <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">registrieren [!DNL Workfront Fusion] im [!DNL Microsoft Application Registration Portal]</a>.</p> <p>Klicken Sie für jeden Bereich auf <b>[!UICONTROL Hinzufügen]</b> und geben Sie die Berechtigung ein.</p> <p>Beispiel: <code>offline_access</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope separator]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client-ID]</td> 
      <td>Geben Sie die [!UICONTROL Anwendungs-ID] aus Schritt 2 in <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">registrieren [!DNL Workfront Fusion] im [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>Geben Sie den [!UICONTROL Application Secret] ein, den Sie in Schritt 3 unter <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">registrieren [!DNL Workfront Fusion] im [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Autorisierungsparameter]</td> 
      <td> <p>Fügen Sie die folgenden Autorisierungsparameter hinzu:</p> 
       <ul> 
        <li> <p>[!UICONTROL Schlüssel]:<code> response_mode</code> [!UICONTROL Wert]: <code>query</code></p> </li> 
        <li> <p>[!UICONTROL Schlüssel]: <code>prompt </code>[!UICONTROL Wert]: <code>consent</code></p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Zugriffstoken-Parameter]</td> 
      <td>Sie müssen in dieses Feld nichts eingeben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Parameter des Aktualisierungstokens]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Klicks <b>[!UICONTROL Hinzufügen]</b>.</p> </li> 
        <li value="2"> <p>Im <b>[!UICONTROL Schlüssel]</b> Feld, eingeben <code>scope</code>.</p> </li> 
        <li value="3"> <p>Im <b>[!UICONTROL Wert]</b> Geben Sie alle [!UICONTROL Perimeter]s ein, die Sie in das Perimeter-Feld eingegeben haben, getrennt durch Leerzeichen.</p> <p>Beispiel: <code>offline_access openid User.Read</code></p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Benutzerdefinierte Kopfzeilen]</td> 
      <td>Sie müssen in dieses Feld nichts eingeben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Placement]</td> 
      <td><code>[!UICONTROL In the header]</code> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicks **[!UICONTROL Weiter]**.
1. Klicken Sie im angezeigten Fenster auf **[!UICONTROL Accept]** , um die Verbindung abzuschließen und zum Modul zurückzukehren.
