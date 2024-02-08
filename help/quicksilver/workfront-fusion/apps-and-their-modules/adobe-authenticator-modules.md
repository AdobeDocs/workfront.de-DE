---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Adobe Authenticator-Modul
description: Mit dem Adobe Authenticator-Modul können Sie über eine einzige Verbindung eine Verbindung zu einem beliebigen Adobe-Produkt mit einer API herstellen.
author: Becky
feature: Workfront Fusion
source-git-commit: 07443d85e160004c273fc977629dd9f588cc23b2
workflow-type: tm+mt
source-wordcount: '880'
ht-degree: 1%

---

# Adobe Authenticator-Module

Mit dem Adobe Authenticator-Modul können Sie über eine Verbindung eine Verbindung zu einer beliebigen Adobe-API herstellen. Dadurch können Sie leichter mit Adobe-Produkten verbunden werden, die noch keinen speziellen Fusion-Connector haben.

Der Vorteil gegenüber den HTTP-Modulen besteht darin, dass Sie eine Verbindung wie in einer dedizierten App erstellen können.

Eine Liste der verfügbaren Adobe-APIs finden Sie unter X. Sie können möglicherweise nur die APIs verwenden, denen Sie zugewiesen sind.

## Zugriffsanforderungen

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] Plan</td>
      <td>
        <p>Neu: Beliebig</p><p>Oder</p><p>Aktuell: [!UICONTROL Pro] oder höher</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td>
      <td>
        <p>Neu: Standard</p><p>Oder</p><p>Aktuell: [!UICONTROL Plan], [!UICONTROL Arbeit]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] Lizenz</td>
      <td>
   <p>Aktuelle Anforderungen an die Fusionszulassung: nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Legacy-Fusion-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Produkt</td>
      <td>
   <p>Neuer Workfront-Plan: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Aktueller Workfront-Plan: Ihr Unternehmen muss kaufen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td>
    </tr>
  </tbody>
</table>

## Voraussetzungen

* Sie müssen Zugriff auf das Adobe-Produkt haben, mit dem das Modul eine Verbindung herstellen soll.
* Sie müssen Zugriff auf die Adobe Developer-Konsole haben.
* Sie müssen über ein Projekt in der Adobe Developer Console verfügen, das die API enthält, mit der das Modul eine Verbindung herstellen soll. Sie können:

   * Erstellen Sie ein neues Projekt mit der API.

     Oder
   * Fügen Sie die API einem vorhandenen Projekt hinzu.

  Informationen zum Erstellen oder Hinzufügen einer API zu einem Projekt in der Adobe Developer Console finden Sie unter [Projekt erstellen](https://developer.adobe.com/dep/guides/dev-console/create-project/) in der Adobe-Dokumentation.

## Verbindung erstellen

Eine Adobe Authenticator-Verbindung stellt eine Verbindung zu einem einzelnen Projekt in der Adobe Developer Console her. Um dieselbe Verbindung für mehr als eine Adobe-API zu verwenden, fügen Sie die APIs zum selben Projekt hinzu und erstellen Sie eine Verbindung zu diesem Projekt.

Sie können separate Verbindungen zu separaten Projekten erstellen, Sie können jedoch keine Verbindung verwenden, um auf eine API zuzugreifen, die sich nicht auf das in dieser Verbindung angegebene Projekt bezieht.

>[!IMPORTANT]
>
>Mit dem Adobe Authenticator-Connector haben Sie die Wahl zwischen einer OAuth-Server-zu-Server-Verbindung oder einer JWT-Verbindung (Service Account). Adobe hat veraltete JWT-Anmeldeinformationen, die nach dem 1. Januar 2025 nicht mehr funktionieren werden. **Daher empfehlen wir dringend, OAuth-Verbindungen zu erstellen.**
>
>Weitere Informationen zu diesen Verbindungstypen finden Sie unter [Server-zu-Server-Authentifizierung](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/) in der Adobe-Dokumentation

So erstellen Sie eine Verbindung:

1. Klicken Sie in einem beliebigen Adobe Authenticator-Modul auf **Hinzufügen** neben dem Feld Verbindung .
1. Füllen Sie die folgenden Felder aus:

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Verbindungstyp]</td>
        <td>
          <p>Wählen Sie aus, ob Sie eine OAuth-Server-zu-Server-Verbindung oder eine JWT-Verbindung (Service-Konto) erstellen möchten.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Verbindungsname]</td>
        <td>
          <p>Geben Sie einen Namen für diese Verbindung ein.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client-ID]</td>
        <td>Geben Sie Ihre [!DNL Adobe] Client-ID. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] im Abschnitt [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Geben Sie Ihre [!DNL Adobe] Client Secret. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] im Abschnitt [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Bereiche]</td>
        <td>Wenn Sie eine OAuth-Verbindung ausgewählt haben, geben Sie die für diese Verbindung benötigten Bereiche ein.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID des technischen Kontos]</td>
        <td>Geben Sie Ihre [!DNL Adobe] Kennung des technischen Kontos. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] im Abschnitt [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Organisations-ID]</td>
        <td>Wenn Sie eine JWT-Verbindung ausgewählt haben, geben Sie Ihre [!DNL Adobe] Organisations-ID. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] im Abschnitt [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Meta Scopes]</td>
        <td>Wenn Sie eine JWT-Verbindung ausgewählt haben, geben Sie die für diese Verbindung benötigten Meta-Bereiche ein. </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Privater Schlüssel]</td>
        <td>
          <p>Wenn Sie eine JWT-Verbindung ausgewählt haben, geben Sie den privaten Schlüssel ein, der generiert wurde, als Ihre Anmeldeinformationen in der [!DNL Adobe Developer Console]. </p>
          <p>So extrahieren Sie Ihren privaten Schlüssel oder Ihr Zertifikat:</p>
          <ol>
            <li value="1">
              <p>Klicks <b>[!UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>Wählen Sie den Dateityp aus, den Sie extrahieren.</p>
            </li>
            <li value="3">
              <p>Wählen Sie die Datei aus, die den privaten Schlüssel oder das Zertifikat enthält.</p>
            </li>
            <li value="4">
              <p>Geben Sie das Kennwort für die Datei ein.</p>
            </li>
            <li value="5">
              <p>Klicks <b>[!UICONTROL Save]</b> , um die Datei zu extrahieren und zur Verbindungseinrichtung zurückzukehren.</p>
            </li>
          </ol>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Umgebung]</td>
        <td>Wählen Sie aus, ob Sie eine Verbindung zu einer Produktions- oder Nicht-Produktionsumgebung herstellen möchten.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Typ]</td>
        <td>Wählen Sie aus, ob Sie eine Verbindung zu einem Dienstkonto oder einem persönlichen Konto herstellen möchten.</td>
      </tr>
    </tbody>
    </table>

1. Klicks **[!UICONTROL Weiter]** , um die Verbindung zu speichern und zum Modul zurückzukehren.

## Modul

### Benutzerdefinierte API-Aufrufe durchführen

Mit diesem Aktionsmodul können Sie eine beliebige Adobe-API aufrufen.

>[!TIP]
>
>Sie müssen die gesamte URL für die API eingeben, mit der Sie eine Verbindung herstellen möchten. Dieses Modul akzeptiert keine relativen URLs.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Verbindung]</td>
     <td>Anweisungen zum Erstellen einer Verbindung zum Adobe Authenticator-Modul finden Sie unter <a href="#create-a-connection" class="MCXref xref" >Verbindung erstellen</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL]</p>
      </td>
      <td>
        <p>Geben Sie die gesamte URL des API-Punkts ein, mit dem Sie eine Verbindung herstellen möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Methode]</p>
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Header]</td>
      <td>
        <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p>
        <p>Beispiel: <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion fügt Autorisierungskopfzeilen automatisch hinzu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Abfragezeichenfolge]  </td>
      <td>
        <p>Geben Sie die Abfragezeichenfolge der Anfrage ein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> Fügen Sie die Anführungszeichen in Ihre JSON-Datei außerhalb der bedingten Anweisung ein.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Geben Sie die maximale Anzahl von Ergebnissen an, die das Modul in einem Ausführungszyklus zurückgeben soll.</p>
      </td>
    </tr>
  </tbody>
</table>

