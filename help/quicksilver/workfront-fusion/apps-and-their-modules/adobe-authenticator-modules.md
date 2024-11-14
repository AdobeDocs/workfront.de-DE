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
exl-id: 74c943fb-37ad-4d91-8af7-9808ba69992e
source-git-commit: 4914e6e30d6c4a16de5bd2c91bc6f8e4f208c078
workflow-type: tm+mt
source-wordcount: '1209'
ht-degree: 1%

---

# Adobe Authenticator-Module

Mit dem Adobe Authenticator-Modul können Sie über eine Verbindung eine Verbindung zu einer beliebigen Adobe-API herstellen. Dadurch können Sie leichter mit Adobe-Produkten verbunden werden, die noch keinen speziellen Fusion-Connector haben.

Der Vorteil gegenüber den HTTP-Modulen besteht darin, dass Sie eine Verbindung wie in einer dedizierten App erstellen können.

Eine Liste der verfügbaren Adobe-APIs finden Sie unter [Adobe-APIs](https://developer.adobe.com/apis). Sie können möglicherweise nur die APIs verwenden, denen Sie zugewiesen sind.

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
   <p>Aktuelle Fusion-Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Legacy-Fusion-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Produkt</td>
      <td>
   <p>Neuer Workfront-Plan: Wenn Sie über den [!UICONTROL Select] oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Aktueller Workfront-Plan: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td>
    </tr>
  </tbody>
</table>

## Voraussetzungen

* Sie müssen Zugriff auf das Adobe-Produkt haben, mit dem das Modul eine Verbindung herstellen soll.
* Sie müssen Zugriff auf die Adobe Developer Console haben.
* Sie müssen über ein Projekt in der Adobe Developer Console verfügen, das die API enthält, mit der das Modul eine Verbindung herstellen soll. Sie können:

   * Erstellen Sie ein neues Projekt mit der API.

     Oder
   * Fügen Sie die API einem vorhandenen Projekt hinzu.

  Informationen zum Erstellen oder Hinzufügen einer API zu einem Projekt in Adobe Developer Console finden Sie unter [Erstellen eines Projekts](https://developer.adobe.com/dep/guides/dev-console/create-project/) in der Adobe-Dokumentation.

## Verbindung erstellen

Eine Adobe Authenticator-Verbindung stellt eine Verbindung zu einem einzelnen Projekt in der Adobe Developer Console her. Um dieselbe Verbindung für mehr als eine Adobe-API zu verwenden, fügen Sie die APIs zum selben Projekt hinzu und erstellen Sie eine Verbindung zu diesem Projekt.

Sie können separate Verbindungen zu separaten Projekten erstellen, Sie können jedoch keine Verbindung verwenden, um auf eine API zuzugreifen, die sich nicht auf das in dieser Verbindung angegebene Projekt bezieht.

>[!IMPORTANT]
>
>Mit dem Adobe Authenticator-Connector haben Sie die Wahl zwischen einer OAuth-Server-zu-Server-Verbindung oder einer JWT-Verbindung (Service Account). Adobe hat veraltete JWT-Anmeldeinformationen, die nach dem 1. Januar 2025 nicht mehr funktionieren werden. **Daher empfehlen wir dringend, OAuth-Verbindungen zu erstellen.**
>
>Weitere Informationen zu diesen Verbindungstypen finden Sie unter [Serverauthentifizierung für Server](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/) in der Adobe-Dokumentation

So erstellen Sie eine Verbindung:

1. Klicken Sie in einem beliebigen Adobe Authenticator-Modul neben dem Feld Verbindung auf **Hinzufügen** .
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
        <td>Geben Sie Ihre [!DNL Adobe] Client-ID ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des Abschnitts [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Geben Sie Ihr [!DNL Adobe] Client-Geheimnis ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des Abschnitts [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Bereiche]</td>
        <td>Wenn Sie eine OAuth-Verbindung ausgewählt haben, geben Sie die für diese Verbindung benötigten Bereiche ein.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID des technischen Kontos]</td>
        <td>Geben Sie Ihre [!DNL Adobe] ID des technischen Kontos ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des Abschnitts [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Organisations-ID]</td>
        <td>Wenn Sie eine JWT-Verbindung ausgewählt haben, geben Sie Ihre [!DNL Adobe] Organisations-ID ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des Abschnitts [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Meta Scopes]</td>
        <td>Wenn Sie eine JWT-Verbindung ausgewählt haben, geben Sie die für diese Verbindung benötigten Meta-Bereiche ein. </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Privater Schlüssel]</td>
        <td>
          <p>Wenn Sie eine JWT-Verbindung ausgewählt haben, geben Sie den privaten Schlüssel ein, der beim Erstellen Ihrer Anmeldedaten in [!DNL Adobe Developer Console] generiert wurde. </p>
          <p>So extrahieren Sie Ihren privaten Schlüssel oder Ihr Zertifikat:</p>
          <ol>
            <li value="1">
              <p>Klicken Sie auf <b>[!UICONTROL Extract]</b>.</p>
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
              <p>Klicken Sie auf <b>[!UICONTROL Save]</b> , um die Datei zu extrahieren und zur Verbindungseinrichtung zurückzukehren.</p>
            </li>
          </ol>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Basis-URLs]</td>
        <td>Sie müssen die Basis-URLs hinzufügen, die dieser Authentifizierer zulassen soll. Wenn Sie das Modul zum Erstellen eines benutzerdefinierten API-Aufrufs später im Szenario verwenden, fügen Sie einen relativen Pfad zur ausgewählten URL hinzu. Durch Eingabe von URLs hier können Sie steuern, worauf das Modul Benutzerdefinierte API-Aufrufe erstellen eine Verbindung herstellen kann, was die Sicherheit erhöht.<p>Klicken Sie für jede Basis-URL, die Sie dem Authentifizierer hinzufügen möchten, auf <b>Element hinzufügen</b> und geben Sie die Basis-URL ein.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Authentifizierungs-URL]</td>
        <td>Lassen Sie dieses Feld leer, um die standardmäßige Adobe IMS-Authentifizierungs-URL von <code>https://ims-na1.adobelogin.com</code> zu verwenden. Wenn Sie Adobe IMS nicht zur Authentifizierung verwenden, geben Sie die URL ein, die für die Authentifizierung verwendet werden soll.</td>
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

1. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindung zu speichern und zum Modul zurückzukehren.

## Module

* [Benutzerdefinierte API-Aufrufe durchführen](#make-a-custom-api-call)
* [Benutzerdefinierte API-Aufrufe durchführen (veraltet)](#make-a-custom-api-call-legacy)

### Benutzerdefinierte API-Aufrufe durchführen

Mit diesem Aktionsmodul können Sie eine beliebige Adobe-API aufrufen. Es unterstützt große Dateien anstelle von Nur-Text-Texten.

Dieses Modul wurde am 14. November 2024 bereitgestellt. Jeder Adobe Authenticator > Vor diesem Datum konfigurierte benutzerdefinierte API-Aufruf behandelt keine großen Dateien und wird jetzt als Modul Benutzerdefinierten API-Aufruf (Legacy) betrachtet.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Verbindung]</td>
     <td>Anweisungen zum Erstellen einer Verbindung mit dem Adobe Authenticator-Modul finden Sie in diesem Artikel unter <a href="#create-a-connection" class="MCXref xref" >Erstellen einer Verbindung</a> .</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Basis-URL]</p>
      </td>
      <td>
        <p>Geben Sie die Basis-URL des API-Punkts ein, mit dem Sie eine Verbindung herstellen möchten.</p>
      </td>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL]</p>
      </td>
      <td>
        <p>Geben Sie den Pfad relativ zur Basis-URL ein.</p>
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
      <td role="rowheader">[!UICONTROL Textkörper]</td>
   <td> Wählen Sie den Nachrichtentyp für diese API-Anfrage aus:
   <ul>
   <li>application/x-www-form-urlencoded</li>
   <li>Raw</li>
   <li>multipart/form-data</li>
   </ul>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Felder]  </td>
      <td>
        <p>Klicken Sie für jede Datei, die Sie der APU-Anforderung hinzufügen möchten, auf "<b>Element hinzufügen</b>"und geben Sie den Text der Datei ein (für Rohdaten) oder geben Sie den Schlüssel "<code>uploadedFile</code>"ein und ordnen Sie die Daten der Datei zu.</p>
      </td>
    </tr>
    </tr>
  </tbody>
</table>

### Benutzerdefinierte API-Aufrufe durchführen (veraltet)

Mit diesem Aktionsmodul können Sie eine beliebige Adobe-API aufrufen.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Verbindung]</td>
     <td>Anweisungen zum Erstellen einer Verbindung mit dem Adobe Authenticator-Modul finden Sie in diesem Artikel unter <a href="#create-a-connection" class="MCXref xref" >Erstellen einer Verbindung</a> .</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Basis-URL]</p>
      </td>
      <td>
        <p>Geben Sie die Basis-URL des API-Punkts ein, mit dem Sie eine Verbindung herstellen möchten.</p>
      </td>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL]</p>
      </td>
      <td>
        <p>Geben Sie den Pfad relativ zur Basis-URL ein.</p>
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
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> in Ihrer JSON platzieren Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
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
