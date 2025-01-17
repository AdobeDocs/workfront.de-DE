---
title: Aufrufen der MS Graph REST-API über das  [!DNL Adobe Workfront Fusion] HTTP &gt; Erstellen eines OAuth 2.0-Anfragemoduls
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 1%

---

# Rufen Sie die [!UICONTROL MS Graph REST-]) über das [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0-Anfrage stellen]-Modul auf

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Rufen Sie die MS Graph REST-API auf](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/call-the-ms-graph-rest-api.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

<!-- Audited: 3/2024-->

Viele [!DNL Microsoft] Webservices werden über die [!DNL Microsoft Graph API] aufgerufen. Sie können eine Verbindung zum [!DNL Microsoft Graph API] herstellen, indem Sie das Modul [!DNL HTTP] [!DNL Workfront Fusion] > [!UICONTROL OAuth 2.0-Anfrage ].

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

## Registrieren von [!DNL Workfront Fusion] im [!DNL Microsoft Application Registration Portal]

Um eine Verbindung zum [!DNL Microsoft Graph REST API] herzustellen, müssen Sie zunächst [!DNL Adobe Workfront Fusion] registrieren.

1. Beginnen Sie mit der Registrierung einer neuen Anwendung, wie unter [Registrieren Sie Ihre Anwendung](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) in der [!DNL Microsoft]-Dokumentation beschrieben.

   Im Rahmen der Registrierung benötigt [!DNL Microsoft] die folgenden Informationen:

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Anwendungsname]</td>
        <td>Geben Sie einen Namen für das Programm ein, z. B. „Mein [!DNL Workfront Fusion] Programm“.</td>
      </tr>
      <tr>
        <td>[!UICONTROL Umleitungs-URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. Notieren Sie sich nach Abschluss der App-Registrierung die [!UICONTROL Anwendungs-ID].

   >[!IMPORTANT]
   >
   >Sie benötigen die Anwendungs-ID, um Ihre Verbindung in [!DNL Workfront Fusion] einzurichten.

1. Generieren Sie ein [!UICONTROL Anwendungsgeheimnis]. Notieren Sie sich dieses Geheimnis.

   Anweisungen finden Sie unter [Registrieren Ihrer App](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) in der [!DNL Microsoft].

   >[!IMPORTANT]
   >
   >Sie benötigen das [!UICONTROL Anwendungsgeheimnis], um Ihre Verbindung in [!DNL Workfront Fusion] einzurichten.

1. Konfigurieren Sie die Berechtigungen für Ihr Programm.

   Einzelheiten zum Auffinden und Konfigurieren dieser Felder finden Sie im Abschnitt „Konfigurieren von Berechtigungen für Microsoft-Diagramme“ in [Zugriff ohne Benutzer erhalten](https://docs.microsoft.com/en-us/graph/auth-v2-service) der Dokumentation zu [!UICONTROL Microsoft].

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Welche Berechtigungen benötigt Ihre Anwendung?]</td> 
      <td>Wählen Sie <code>[!UICONTROL Delegated permissions]</code> aus.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Berechtigungen auswählen]</td> 
      <td> <p>Wählen Sie die folgenden Berechtigungen aus:</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>Alle anderen für Ihre Integrationen erforderlichen Berechtigungen (Beispiel: <code>User.Read</code>)</p> </li> 
       </ul> <p><b>Wichtig</b>: Zum Einrichten Ihrer Verbindung in [!DNL Workfront Fusion] benötigen Sie die ausgewählten Berechtigungen.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fahren Sie mit [Konfigurieren  [!DNL MS Graph API]  Verbindung in [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion) fort.

## Konfigurieren der [!DNL MS Graph API] in [!DNL Workfront Fusion]

Nach der Registrierung von [!DNL Workfront Fusion] wie unter [Registrieren [!DNL Workfront Fusion]  im  [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal) beschrieben, können Sie Ihre Verbindung im Anforderungsmodul [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 ].

1. Fügen Sie ein [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0-Aufruf durchführen]-Modul zu Ihrem Szenario hinzu.
1. Klicken Sie **[!UICONTROL Hinzufügen]** neben dem Feld [!UICONTROL Verbindung].
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
      <td role="rowheader"> <p role="rowheader">[!UICONTROL-Flusstyp]</p> </td> 
      <td><code>[!UICONTROL Authorization Code]</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL URI autorisieren]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/authorize</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token-URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL-Umfang]</td> 
      <td> <p>Geben Sie die Berechtigungen ein, die Sie in Schritt 4 von <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrieren [!DNL Workfront Fusion] im [!DNL Microsoft Application Registration Portal]</a> ausgewählt haben.</p> <p>Klicken Sie für jeden Bereich auf <b>[!UICONTROL Hinzufügen]</b> und geben Sie die Berechtigung ein.</p> <p>Beispiel: <code>offline_access</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL-Bereichstrennzeichen]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client-ID]</td> 
      <td>Geben Sie die [!UICONTROL Anwendungs-ID] aus Schritt 2 unter <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">[!DNL Workfront Fusion] im [!DNL Microsoft Application Registration Portal]</a> registrieren] ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client-Geheimnis]</td> 
      <td>Geben Sie den [!UICONTROL Application Secret] ein, den Sie in Schritt 3 unter <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrieren [!DNL Workfront Fusion] im [!DNL Microsoft Application Registration Portal]</a> generiert haben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Parameter autorisieren]</td> 
      <td> <p>Fügen Sie die folgenden Autorisierungsparameter hinzu:</p> 
       <ul> 
        <li> <p>[!UICONTROL-Schlüssel]:<code> response_mode</code> [!UICONTROL-Wert]: <code>query</code></p> </li> 
        <li> <p>[!UICONTROL key]: <code>prompt </code>[!UICONTROL value]: <code>consent</code></p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Zugriffstokenparameter]</td> 
      <td>Sie müssen in dieses Feld nichts eingeben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token-Parameter aktualisieren]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Klicken Sie auf <b>[!UICONTROL Hinzufügen]</b>.</p> </li> 
        <li value="2"> <p>Geben Sie im Feld <b>[!UICONTROL Key]</b> den Wert <code>scope</code> ein.</p> </li> 
        <li value="3"> <p>Geben Sie im Feld <b>[!UICONTROL Value]</b> alle [!UICONTROL scope]s ein, die Sie in das Bereichsfeld eingegeben haben, getrennt durch Leerzeichen.</p> <p>Beispiel: <code>offline_access openid User.Read</code></p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Benutzerdefinierte Kopfzeilen]</td> 
      <td>Sie müssen in dieses Feld nichts eingeben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token-Platzierung]</td> 
      <td><code>[!UICONTROL In the header]</code> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie **[!UICONTROL Weiter]**.
1. Klicken Sie im eingeblendeten Fenster auf **[!UICONTROL Akzeptieren]**, um die Verbindung herzustellen und zum Modul zurückzukehren.
