---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: http-modules
title: HTTP &gt; API-Schlüsselautorisierungsanfrage stellen
description: Diese [!DNL Adobe Workfront Fusion] Aktionsmodul sendet eine HTTPS-Anforderung an eine angegebene URL, die eine Autorisierung des API-Schlüssels erfordert, und verarbeitet die Antwort.
author: Becky
feature: Workfront Fusion
exl-id: 70bf87c7-6d51-4ef4-9dce-80ad004e613f
source-git-commit: 58db2129dd764d24b0a681735c2405be402d8b43
workflow-type: tm+mt
source-wordcount: '932'
ht-degree: 0%

---

# HTTP >[!UICONTROL API-Schlüsselautorisierungsanfrage stellen]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] erfordert [!DNL Adobe Workfront Fusion] zusätzlich zu einer Adobe Workfront-Lizenz.

Diese [!DNL Adobe Workfront Fusion] Aktionsmodul sendet eine HTTPS-Anforderung an eine angegebene URL, die eine Autorisierung des API-Schlüssels erfordert, und verarbeitet die Antwort.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!UICONTROL Adobe Workfront Fusion] Lizenzen, siehe [Adobe Workfront Fusion-Lizenzen](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!UICONTROL HTTP] >[!UICONTROL API-Schlüsselautorisierungsanfrage stellen] Modulkonfiguration

Wenn Sie die [!UICONTROL HTTP] >[!UICONTROL API-Schlüsselautorisierungsanfrage stellen] Modul, [!DNL Adobe Workfront Fusion] zeigt die unten aufgeführten Felder an. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Credentials]</td> 
   <td> <p>Wählen Sie den Schlüssel aus, der Ihre Anmeldedaten für die API-Schlüsselauthentifizierung enthält. Um einen neuen Schlüssel hinzuzufügen, klicken Sie auf <strong>[!UICONTROL Hinzufügen]</strong> und konfigurieren Sie die folgenden Informationen:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Schlüsselname]</strong></p> <p>Geben Sie einen Namen für diesen Satz von API-Anmeldeinformationen ein.</p> </li> 
     <li> <p><strong>[!UICONTROL Schlüssel]</strong> </p> <p>Geben Sie den API-Schlüssel ein.</p> </li> 
     <li> <p><strong>[!UICONTROL API Key placement]</strong> </p> <p>Wählen Sie aus, ob der API-Schlüssel in der Kopfzeile oder in der Abfrage des API-Aufrufs platziert werden soll.</p> </li> 
     <li> <p><strong>[!UICONTROL API-Schlüsselparametername]</strong> </p> <p>Geben Sie den Namen ein, mit dem der API-Aufruf den API-Schlüssel identifiziert, z. B. "apiKey"oder "X-API-Schlüssel". Diese Informationen finden Sie in der Dokumentation des Webdienstes, mit dem das Modul eine Verbindung herstellt.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Alle Status als Fehler auswerten (mit Ausnahme von 2xx und 3xx)] </td> 
   <td> <p>Verwenden Sie diese Option, um die Fehlerbehandlung einzurichten.</p> <p>Weitere Informationen finden Sie unter <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">Umgang mit Fehlern in Adobe Workfront Fusion</a>.</p> </td> 
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
   <td> <p>Der HTTP-Hauptteil sind die Datenbytes, die in einer HTTP-Transaktionsnachricht unmittelbar nach den Headern übertragen werden, wenn welche verwendet werden sollen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>Der Rohkörpertyp eignet sich im Allgemeinen für die meisten HTTP-Textkörperanforderungen, selbst wenn in der Entwicklerdokumentation keine zu sendenden Daten angegeben sind.</p> <p>Geben Sie im Feld [!UICONTROL Inhaltstyp] eine Form zum Analysieren der Daten an.</p> <p>Ungeachtet des ausgewählten Inhaltstyps gibt das Modul Daten in jedem Format ein, das in der Entwicklerdokumentation festgelegt oder benötigt wird.</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>Dieser Nachrichtentyp besteht aus [!UICONTROL POST]-Daten mithilfe von <code>application/x-www-form-urlencoded</code>.</p> <p>Für <code>[!UICONTROL application/x-www-form-urlencoded]</code>, ist der Hauptteil der an den Server gesendeten HTTP-Nachricht im Wesentlichen eine Abfragezeichenfolge. Die Schlüssel und Werte sind in Schlüssel/Wert-Paaren kodiert, getrennt durch <code>&amp;</code> und mit <code>=</code> zwischen dem Schlüssel und dem Wert. </p> <p>Verwenden Sie für Binärdaten <code>[!UICONTROL multipart/form-data]</code> anstatt.</p> 
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
   <td> <p>Geben Sie die Zeitüberschreitung der Anfrage in Sekunden (1-300) an. Der Standardwert beträgt 40 Sekunden.</p> </td> 
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
   <td> <p>Standardmäßig [!DNL Workfront Fusion] verarbeitet mehrere Werte für denselben URL-Abfragezeichenfolgenparameterschlüssel wie Arrays. Beispiel: <code>www.test.com?foo=bar&amp;foo=baz</code> wird in <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. Aktivieren Sie diese Option, um diese Funktion zu deaktivieren. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Komprimierten Inhalt anfordern]</td> 
   <td> <p> Aktivieren Sie diese Option, um eine komprimierte Version der Website anzufordern.</p> <p>Fügt eine <code>[!UICONTROL Accept-Encoding]</code> -Kopfzeile, um komprimierten Inhalt anzufordern.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Gegenseitige TLS verwenden]</td> 
   <td> <p>Aktivieren Sie diese Option, um in der HTTP-Anforderung die Verwendung von TLS mit Gegenseitigkeit vorzunehmen.</p> <p>Weitere Informationen zu TLS auf Gegenseitigkeit finden Sie unter <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">Verwenden von TLS auf Gegenseitigkeit in HTTP-Modulen in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
