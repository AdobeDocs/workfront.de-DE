---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: http-modules
title: HTTP &gt; Anforderungsmodul erstellen
description: Adobe Workfront Fusion HTTP &gt; Make a request module ist ein universelles Modul, mit dem Sie eine HTTP-Anforderung konfigurieren und an einen Server senden können. Die empfangene HTTP-Antwort ist dann im Ausgabebundle enthalten.
author: Becky
feature: Workfront Fusion
exl-id: 7857c395-ce84-480e-8fa2-065035ac5b95
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 0%

---

# [!UICONTROL HTTP] >[!UICONTROL Stellen eines Anfrage-Moduls]

>[!NOTE]
>
>Für Adobe Workfront Fusion ist zusätzlich zu einer [!DNL Adobe Workfront] -Lizenz eine [!DNL Adobe Workfront Fusion] -Lizenz erforderlich.

Das [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Anforderungsmodul erstellen] ist ein universelles Modul, mit dem Sie eine HTTP-Anforderung konfigurieren und an einen Server senden können. Die empfangene HTTP-Antwort ist dann im Ausgabebundle enthalten.

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

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [Adobe Workfront Fusion-Lizenzen](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!UICONTROL HTTP] >[!UICONTROL Stellen einer Anforderung ]-Modulkonfiguration

Wenn Sie das Modul [!UICONTROL HTTP] >[!UICONTROL Anforderung senden] konfigurieren, zeigt [!DNL Adobe Workfront Fusion] die unten aufgeführten Felder an. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Alle Status als Fehler auswerten (mit Ausnahme von 2xx und 3xx)] </td> 
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
   <td> <p>Fügen Sie die Header der Anforderung in Form eines standardmäßigen JSON-Objekts hinzu. Beispiel: <code>{"Content-type":"application/json"}</code></p> </td> 
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
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>Dieser Nachrichtentyp wird zu [!UICONTROL POST]-Daten mit <code>[!UICONTROL application/x-www-form-urlencoded]</code> verwendet.</p> <p>Bei <code>application/x-www-form-urlencoded</code> ist der Hauptteil der an den Server gesendeten HTTP-Nachricht im Wesentlichen eine Abfragezeichenfolge. Die Schlüssel und Werte werden in Schlüssel-Wert-Paaren kodiert, die durch <code>&amp;</code> getrennt sind, und in einem <code>=</code> zwischen Schlüssel und Wert. </p> <p>Verwenden Sie stattdessen für Binärdaten "<code>[!UICONTROL multipart/form-data]</code>".</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>Beispiel: </b></span></span> 
       <p>Beispiel für das resultierende HTTP-Anforderungsformat:</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL Multipart/form-data]</strong> </p> <p>Das Multipart/form-data[!UICONTROL] ist eine HTTP-Multipart-Anfrage zum Senden von Dateien und Daten. Sie wird häufig zum Hochladen von Dateien auf den Server verwendet.</p> <p>Fügen Sie Felder hinzu, die in der Anfrage gesendet werden sollen. Jedes Feld muss ein Schlüssel-Wert-Paar enthalten.</p> 
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
   <td role="rowheader"> <p>[!UICONTROL Benutzername]</p> </td> 
   <td> <p> Geben Sie den Benutzernamen ein, wenn Sie eine Anfrage mit einer einfachen Autorisierung senden möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kennwort] </td> 
   <td> <p>Geben Sie das Kennwort ein, wenn Sie eine Anfrage mit einer einfachen Autorisierung senden möchten.</p> </td> 
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
   <td> <p>Standardmäßig verarbeitet [!DNL Workfront Fusion] mehrere Werte für denselben URL-Abfragezeichenfolgen-Parameterschlüssel wie Arrays. Beispielsweise wird <code>www.test.com?foo=bar&amp;foo=baz</code> in <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code> umgewandelt. Aktivieren Sie diese Option, um diese Funktion zu deaktivieren. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Komprimierten Inhalt anfordern]</td> 
   <td> <p> Aktivieren Sie diese Option, um eine komprimierte Version der Website anzufordern.</p> <p>Fügt eine <code>[!UICONTROL Accept-Encoding]</code> -Kopfzeile hinzu, um komprimierten Inhalt anzufordern.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Gegenseitige TLS verwenden]</td> 
   <td> <p>Aktivieren Sie diese Option, um in der HTTP-Anforderung die Verwendung von TLS mit Gegenseitigkeit vorzunehmen.</p> <p>Weitere Informationen zu TLS auf Gegenseitige Basis finden Sie unter <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">Verwenden von TLS auf Gegenseitiger Basis in HTTP-Modulen in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Beispiel:** Dieses Beispiel zeigt, wie das Modul so eingerichtet wird, dass eine [!UICONTROL POST] -Anfrage mit JSON-Payload gesendet wird:
>
>![](assets/make-a-request-example-350x522.png)

>[!NOTE]
>
>Um sicherzustellen, dass Ihr [!UICONTROL JSON] gültig ist, können Sie einen der verfügbaren Online-Dienste wie [https://jsonlint.com/](https://jsonlint.com/) verwenden. Sie können auch [!UICONTROL JSON] >[!UICONTROL JSON-Modul erstellen] verwenden, um die JSON dynamisch zu erstellen und alle erforderlichen Maskierungen vorzunehmen.
>
>Das Mischen von JSON-Teilen mit Ausdrücken und Elementen direkt im Feld [!UICONTROL Inhalt anfordern] wird nicht empfohlen, da dies zu einer ungültigen JSON führen kann.
