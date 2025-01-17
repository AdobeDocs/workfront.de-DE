---
title: Adobe PDF Services
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: e0a5736b-dbdb-43c6-83ff-e88a5625a5bf
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '3809'
ht-degree: 0%

---

# [!DNL Adobe PDF Services]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Adobe PDF Services](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/pdf-modules.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Mit dem [!DNL Adobe Workfront Fusion] [!DNL Adobe PDF Services] können Sie Daten aus einer PDF-Datei extrahieren oder eine neue PDF-Datei aus den von Ihnen bereitgestellten Daten generieren. Darüber hinaus können Sie eine Vielzahl von Dateitypen in PDF oder PDF in andere Dateitypen konvertieren. Mit PDF-Services können Sie außerdem Metadaten für eine PDF-Datei kombinieren, komprimieren oder lesen sowie den Passwortschutz für die Datei steuern.

Anweisungen zum Erstellen eines Szenarios finden Sie unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

Informationen über die API, die für PDF-Services verwendet wird, finden Sie unter [Adobe Document Generation API](https://www.adobe.io/apis/documentcloud/dcsdk/doc-generation.html).

## Sicherheitsüberlegungen bei der Verwendung von [!DNL Adobe PDF Services]

<!--

* [You do not need an [!DNL Adobe] account](#you-do-not-need-an-adobe-account) 
* [[!DNL Workfront Fusion] does not store your files](#workfront-fusion-does-not-store-your-files)

### You do not need an [!DNL Adobe] account 

Because [!DNL Workfront Fusion] is part of the [!DNL Adobe] product suite, you don't need a separate [!DNL Adobe] account to use these tools. Each tool accesses [!DNL Adobe] PDF functionality without using a connection.

Although [!DNL Workfront Fusion] does not require an [!DNL Adobe] account to use the PDF Services, the modules do require a connection. There are no credentials involved in this connection, and you provide only a name for the connection itself.

### [!DNL Workfront Fusion] does not store your files 

-->

Der [!DNL Adobe PDF Services] kann Ihre Dateien lesen, konvertieren oder ändern, Ihre Dateien oder Daten jedoch weder [!DNL Adobe] noch [!DNL Workfront Fusion] speichern. Dies bedeutet, dass:

* Sie behalten die Kontrolle über Ihre Dateien, einschließlich ihrer Sicherheit
* Sie benötigen kein [!UICONTROL Adobe]-Speicher- oder Cloud-Speicherkonto, um die PDF-Services zu verwenden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td>
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Lizenz **</td> 
   <td>
   <p>Aktuelle Lizenzanforderung: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!DNL Adobe Workfront] [!UICONTROL Select] oder [!UICONTROL Prime] verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu nutzen. [!DNL Workfront Fusion] ist im [!DNL Workfront] [!UICONTROL Ultimate] enthalten.</p>
   <p>Oder</p>
   <p>Legacy-Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Um einen OAuth-Server-zu-Server zu erstellen, müssen Sie die Adobe PDF Services-API in Ihrer Adobe Developers Console hinzufügen. Wählen Sie beim Hinzufügen der API die Option OAuth-Server-zu-Server aus.

Anweisungen finden Sie unter [Hinzufügen einer API zu einem Projekt mithilfe von OAuth](https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/) in der Entwicklerdokumentation für Adobe.

## Adobe PDF Services-API-Informationen

Der Adobe PDF Services-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Basis-URL</td> 
   <td>https://pdf-services-stage.adobe.io</td> 
  </tr>
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v2.1.4</td> 
  </tr>
 </tbody> 
 </table>

## Erstellen einer Verbindung zu [!DNL Adobe PDF Services]

So erstellen Sie eine Verbindung für Ihre [!DNL Adobe PDF Services]:

1. Klicken Sie in einem beliebigen [!DNL Adobe PDF Services] auf **[!UICONTROL Hinzufügen]** neben dem Feld Verbindung .

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
            <p>Wählen Sie aus, ob Sie eine Server-zu-Server-Verbindung oder eine JWT-Verbindung erstellen möchten.</p>
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
          <td>Geben Sie Ihre [!DNL Adobe] [!UICONTROL Client ID] ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des [!DNL Adobe Developer Console].<p>Anweisungen zum Suchen von Anmeldeinformationen finden Sie unter <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Anmeldeinformationen</a> in der Entwicklerdokumentation für Adobe.</p></td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client-Geheimnis]</td>
          <td>Geben Sie Ihren [!DNL Adobe] [!UICONTROL Client Secret] ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des [!DNL Adobe Developer Console].<p>Anweisungen zum Suchen von Anmeldeinformationen finden Sie unter <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Anmeldeinformationen</a> in der Entwicklerdokumentation für Adobe.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID des technischen Kontos] (nur JWT)</td>
          <td>Geben Sie Ihre [!DNL Adobe] [!UICONTROL ID des technischen Kontos] ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des [!DNL Adobe Developer Console].<p>Anweisungen zum Suchen von Anmeldeinformationen finden Sie unter <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Anmeldeinformationen</a> in der Entwicklerdokumentation für Adobe.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Organisations-ID] (nur JWT)</td>
          <td>Geben Sie Ihre [!DNL Adobe] [!UICONTROL Organisations-ID] ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des [!DNL Adobe Developer Console].<p>Anweisungen zum Suchen von Anmeldeinformationen finden Sie unter <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Anmeldeinformationen</a> in der Entwicklerdokumentation für Adobe.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Meta Scopes] (nur JWT)</td>
          <td>
            Geben Sie alle für die Verbindung erforderlichen Metabereiche ein.
          </td>
        </tr>
       </tbody>
    </table>
1. Klicken Sie **[!UICONTROL Fortfahren]**, um die Verbindung zu speichern und zum Modul zurückzukehren.


## [!DNL Adobe PDF Services] Module und ihre Felder

Beim Konfigurieren von [!DNL PDF Services] zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können je nach Faktoren wie Ihrer Zugriffsebene in der App oder im Service weitere Felder angezeigt werden. Ein fetter Titel in einem Modul kennzeichnet ein erforderliches Feld.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Kombinieren von PDF-Dateien]](#combine-pdf-files)
* [[!UICONTROL Komprimieren von PDF-Dateien]](#compress-pdf-files)
* [[!UICONTROL Dokument in PDF-Datei konvertieren]](#convert-document-to-pdf-file)
* [[!UICONTROL HTML in PDF-Datei konvertieren]](#convert-html-to-pdf-file)
* [[!UICONTROL Bild in PDF-Datei konvertieren]](#convert-image-to-pdf-file)
* [[!UICONTROL PDF in Dokument konvertieren]](#convert-pdf-to-document)
* [[!UICONTROL PDF in Bild konvertieren]](#convert-pdf-to-image)
* [[!UICONTROL Text/Tabelle extrahieren]](#extract-text--table)
* [[!UICONTROL Dokument generieren]](#generate-document)
* [[!UICONTROL Linearisieren einer PDF-Datei]](#linearize-a-pdf-file)
* [[!UICONTROL OCR für PDF-Datei]](#ocr-for-pdf-file)
* [[!UICONTROL Seitenbearbeitung]](#page-manipulation)
* [[!UICONTROL Automatisches Tagging der Barrierefreiheit von PDF]](#pdf-accessibility-auto-tag)
* [[!UICONTROL PDF-Dateieigenschaften]](#pdf-file-properties)
* [[!UICONTROL Protect PDF-Datei]](#protect-pdf-file)
* [[!UICONTROL Entfernen des Schutzes einer PDF-Datei]](#remove-protection-of-a-pdf-file)
* [Aufspalten einer PDF-Datei](#split-a-pdf-file)

### [!UICONTROL Kombinieren von PDF-Dateien]

Dieses Action-Modul nimmt mehrere PDF-Dateien und kombiniert sie zu einer einzigen PDF-Datei. Beispielsweise könnte dieses Modul alle Dokumente in einem [!UICONTROL Workfront]-Projekt nach Abschluss des Projekts zu einer einzigen PDF kombinieren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services] finden Sie unter <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Dokumente]</td> 
   <td> <p>Sie können ein Aggregator-Modul verwenden, um Dokumente zu sammeln und zu einer PDF zu kombinieren, oder Sie können die Dokumente manuell hinzufügen. </p> <p>Es wird empfohlen, ein [!UICONTROL Array Aggregator]-Modul zu verwenden, um die Ausgabe eines vorherigen Moduls zu aggregieren. Mithilfe eines Aggregators müssen Sie nicht wissen, welche Namen, Speicherorte oder Anzahl von Dateien kombiniert werden sollen. Die Verwendung eines Aggregators ist daher viel flexibler und skalierbarer als die manuelle Eingabe der zu kombinierenden Dokumente.</p> <p>Um das Dateimodul [!UICONTROL PDF kombinieren] mit einem Aggregator verwenden zu können, müssen Sie die Zuordnung für das Feld [!UICONTROL Documents] aktivieren. </p> <p>In diesem Beispiel identifiziert das Modul [!UICONTROL READ RELATED RECORDS] Dokumente, die mit einem Projekt verknüpft sind, und das Modul [!UICONTROL DOWNLOAD DOCUMENTS] lädt jedes davon herunter. Alle PDF werden in einem Array zusammengefasst, das an das Dateimodul [!UICONTROL Combine PDF] übergeben wird.</p> <p> <img src="assets/combine-example-350x104.png" style="width: 350;height: 104;"> </p> <p>Sie können Dokumente auch manuell eingeben.</p> <p>Für jedes Dokument, das in die kombinierte PDF aufgenommen werden soll:</p> 
    <ol> 
     <li value="1"> <p>Klicken Sie auf [!UICONTROL Dokument hinzufügen]</p> </li> 
     <li value="2"> <p>Wählen Sie im Feld [!UICONTROL Source-Datei] das Modul aus, das das einzuschließende Dokument ausgibt, oder ordnen Sie den Namen und die Daten der Quelldatei zu. </p> </li> 
     <li value="3"> <p>(Optional) Wenn Sie nur bestimmte Seiten aus der Quelldatei einbeziehen möchten, klicken Sie für jeden Seitenbereich, den Sie hinzufügen möchten, im Feld [!UICONTROL Pages] auf <strong>[!UICONTROL Element hinzufügen]</strong>, geben Sie dann die erste und letzte Seite des einzuschließenden Seitenbereichs ein und klicken Sie auf <strong>[!UICONTROL Hinzufügen]</strong>. Sie können mehrere Seitenbereiche aus einem einzelnen Dokument einbeziehen.</p> </li> 
     <li value="4"> <p>Klicken Sie auf <strong>[!UICONTROL Hinzufügen]</strong>. </p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Komprimieren von PDF-Dateien]

Dieses Aktionsmodul nimmt eine PDF-Datei und komprimiert sie. Dies kann nützlich sein, um Bandbreite oder Speicher zu sparen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services] finden Sie unter <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> <p>Die Quelldatei muss im PDF-Format vorliegen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Komprimierungsgrad]</td> 
   <td>Wählen Sie die Komprimierungsstufe aus, die Sie verwenden möchten.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Dokument in PDF-Datei konvertieren]

Dieses Tool konvertiert ein Dokument in eine PDF-Datei. Die Quelldatei muss eines der folgenden Dokumentenformate aufweisen:

* DOC
* XLS
* PPT
* TXT
* RTF

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services] finden Sie unter <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> <p>Die Quelldatei muss in einem der folgenden Formate vorliegen:</p> 
    <ul> 
     <li> <p>DOC</p> </li> 
     <li> <p>XLS</p> </li> 
     <li> <p>PPT</p> </li> 
     <li> <p>TXT</p> </li> 
     <li> <p>RTF</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Language]</td> 
   <td> <p>Wählen Sie die Standardsprache für das Quelldokument. Dadurch kann das Modul eine geeignete Schriftart auswählen, wenn diese nicht in der Quelldatei enthalten ist.</p> <p>Wählen Sie aus den folgenden Sprachen aus:</p> 
    <ul> 
     <li> <p>en-US (Standard): Englisch (USA)</p> </li> 
     <li> <p>ca-ES: Katalanisch (Spanien)</p> </li> 
     <li> <p>CS-CZ: Tschechisch (Tschechische Republik)</p> </li> 
     <li> <p>da-DK: Dänisch (Dänemark)</p> </li> 
     <li> <p>de-DE: Deutsch (Deutschland)</p> </li> 
     <li> <p>en-AE: Englisch (Vereinigte Arabische Emirate)</p> </li> 
     <li> <p>en-GB: Englisch (Vereinigtes Königreich)</p> </li> 
     <li> <p>en-IL: Englisch (Israel)</p> </li> 
     <li> <p>en-US: Englisch (Vereinigte Staaten von Amerika)</p> </li> 
     <li> <p>es-ES: Spanisch (Spanien)</p> </li> 
     <li> <p>es-MX: Spanisch (Mexiko)</p> </li> 
     <li> <p>eu-ES: Baskisch (Spanien)</p> </li> 
     <li> <p>FI-FI: Finnisch (Finnland)</p> </li> 
     <li> <p>fr-CA: Französisch (Kanada)</p> </li> 
     <li> <p>fr-FR: Französisch (Frankreich)</p> </li> 
     <li> <p>fr-MA: Französisch (Marokko)</p> </li> 
     <li> <p>hr-hr: Kroatisch (Kroatien)</p> </li> 
     <li> <p>hu-hu: Ungarisch (Ungarn)</p> </li> 
     <li> <p>it-IT: Italienisch (Italien)</p> </li> 
     <li> <p>JA-JP: Japanisch (Japan)</p> </li> 
     <li> <p>kr-KR: Koreanisch (Südkorea)</p> </li> 
     <li> <p>NB-NO: Norwegisch Bokmål (Norwegen)</p> </li> 
     <li> <p>NL-NL: Niederländisch (Niederlande)</p> </li> 
     <li> <p>PL-PL: Polnisch (Polen)</p> </li> 
     <li> <p>pt-BR: Portugiesisch (Brasilien)</p> </li> 
     <li> <p>PT-PT: Portugiesisch (Portugal)</p> </li> 
     <li> <p>ro-RO: Rumänisch (Rumänien)</p> </li> 
     <li> <p>RU-RU: Russisch (Russland)</p> </li> 
     <li> <p>SK-SK: Slowakisch (Slowakei)</p> </li> 
     <li> <p>sl-SI: Slowenisch (Slowenien)</p> </li> 
     <li> <p>SV-SE: Schwedisch (Schweden)</p> </li> 
     <li> <p>TR-TR: Türkisch (Türkei)</p> </li> 
     <li> <p>UK-UA: Ukrainisch (Ukraine)</p> </li> 
     <li> <p>zh-CN: Chinesisch (Festlandchina)</p> </li> 
     <li> <p>zh-TW: Chinesisch (Taiwan)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL HTML in PDF-Datei konvertieren]

Dieses Tool konvertiert eine HTML-Datei in eine PDF-Datei.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services] finden Sie unter <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> <p>Wichtig: Die Source-Datei muss im HTML- oder ZIP-Format vorliegen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON]</td> 
   <td> <p>Wenn Ihr HTML auf JavaScript-Variablen verweist, können Sie diese Variablen hier einbeziehen. </p> <p>Klicken Sie für jede Variable auf <strong>[!UICONTROL Element hinzufügen]</strong> und schließen Sie den Schlüssel und den Wert der Variablen ein.</p> <p>Hinweis:   
     <ul> 
      <li> <p>Beim Erstellen einer PDF aus einer ZIP-Datei muss das Quellmaterial ein Skriptelement enthalten, z. B.: <code> &lt;script src='./json.js' type='text/javascript'&gt;&lt;/script&gt;</code> </p> </li> 
      <li> <p>Beim Erstellen eines PDF aus einer URL wird der Inhalt dieses JSON-Objekts in die VM des Browsers eingefügt, bevor die Seite gerendert wird. </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kopf- und Fußzeile einschließen]</td> 
   <td> <p>Aktivieren Sie diese Option, um Kopf- und Fußzeilen für das PDF-Dokument zu erstellen.</p> 
    <ul> 
     <li> <p>Die Kopfzeile enthält ein Datum und den Titel des Dokuments.</p> </li> 
     <li> <p>Die Fußzeile enthält den Dateinamen und eine Seitennummer.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seitenbreite]</td> 
   <td>Geben Sie die Breite des Papiers in Zoll ein. Das Modul benutzt diese Information, um die Seiten in der erstellten PDF-Datei zu formatieren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seitenhöhe]</td> 
   <td>Geben Sie die Höhe des Papiers in Zoll ein. Das Modul benutzt diese Information, um die Seiten in der erstellten PDF-Datei zu formatieren.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Bild in PDF-Datei konvertieren]

Dieses Tool konvertiert ein Bild in eine PDF-Datei.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services] finden Sie unter <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Bilddatei der Quelldatei zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDF in Dokument konvertieren]

Dieses Tool konvertiert eine PDF-Datei in ein Dokument. Sie können eines der folgenden Formate für die Ausgabedatei auswählen.

* DOC
* DOCX
* PPTX
* XLSX
* RTF

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services] finden Sie unter <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> <p>Die Quelldatei muss im PDF-Format vorliegen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgabedateiformat]</td> 
   <td> <p>Wählen Sie das Format aus, in dem die Dateien ausgegeben werden sollen:</p> 
    <ul> 
     <li> <p>DOC</p> </li> 
     <li> <p>DOCX</p> </li> 
     <li> <p>PPTX</p> </li> 
     <li> <p>XLSX</p> </li> 
     <li> <p>RTF</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDF in Bild konvertieren]

Dieses Tool konvertiert eine PDF in ein Bild im PNG- oder JPEG-Format, das dann als ZIP-Datei ausgegeben wird. Die PDF wird in ein Bild pro Seite konvertiert, und jedes Bild endet mit der Seitenzahl. Die Bilddateien werden dann zu einer ZIP-Datei zusammengefasst.

Beispielsweise würde eine Datei namens „TestFile“ mit acht Seiten acht Bilder erzeugen, „TestFile_1“ bis „TestFile_8“. Die Ausgabe des Moduls ist eine ZIP-Datei mit den 8 Bildern.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services] finden Sie unter <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> <p>Die Quelldatei muss im PDF-Format vorliegen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgabedateiformat]</td> 
   <td> <p>Wählen Sie das Format aus, in dem die Dateien ausgegeben werden sollen:</p> 
    <ul> 
     <li>PNG</li> 
     <li>JPEG</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Text/Tabelle extrahieren]

Mit diesem Aktionsmodul können Sie Daten aus einer PDF-Datei extrahieren. Das Modul gibt einzelne Textelemente aus, z. B. einen Absatz oder den Text in einer einzelnen Zelle einer Tabelle.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services] finden Sie unter <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Elemente, die als JSON extrahiert werden sollen]</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL-Text]</p> </li> 
     <li> <p>[!UICONTROL-Tabellen]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Begrenzungsrahmen extrahieren?]</td> 
   <td>Aktivieren Sie diese Option, um Daten über den Begrenzungsrahmen des Textes zu extrahieren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stilinformationen für die Ausgabe einschließen?]</td> 
   <td>Aktivieren Sie diese Option, um der JSON-Ausgabe Stilinformationen hinzuzufügen.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Dokument generieren]

Das [!UICONTROL Generate Document]-Modul ist eine leistungsstarke Methode, um eine PDF zu erstellen, die ausgewählte Daten enthält. Sie können sie mit einer [!DNL Microsoft Word]-Vorlage formatieren oder Daten im JSON-Format bereitstellen.

Weitere Informationen zur Funktion [!UICONTROL [!DNL Adobe PDF Services] Dokument generieren ] Sie unter [Überblick über die Dokumenterstellung](https://www.adobe.io/apis/documentcloud/dcsdk/docs.html) in der [!DNL Adobe Document Services].

* [Verwenden des Moduls [!UICONTROL Dokument generieren] mit einer  [!DNL Microsoft Word] -Vorlage](#use-the-generate-document-module-with-a-microsoft-word-template)
* [Verwenden des Moduls [!UICONTROL Dokument generieren] mit JSON](#use-the-generate-document-module-with-json)

#### Verwenden des [!UICONTROL Generate Document]-Moduls mit einer [!DNL Microsoft Word] Vorlage

<!--
>[!NOTE]
>
>For a discussion of Microsoft Word templates, see [Microsoft Word Template modules](../../workfront-fusion/apps-and-their-modules/microsoft-word-templates-modules.md). 
>
>You do not need to use Microsoft Word template modules to use a Microsoft Word template with the PDF Services Generate document module.
-->

Um das Modul [!UICONTROL Dokument generieren] mit einer [!UICONTROL Microsoft Word]-Vorlage zu verwenden, müssen Sie zunächst die Vorlage erstellen. Anweisungen hierzu finden Sie in der [!DNL Microsoft Office]-Dokumentation unter „Erstellen einer Vorlage“.

Füllen Sie die Modulfelder [!UICONTROL Dokument generieren] wie folgt aus:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services] finden Sie unter <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> <p>Diese Quelldatei ist die -[!DNL Microsoft Word ], die das -Modul zum Generieren der neuen PDF verwendet.</p> <p>Es wird empfohlen, ein Projekt in [!DNL Workfront] für die [!DNL Microsoft Word] Vorlagen zu erstellen, die Sie in [!DNL Workfront Fusion] verwenden. Anschließend können Sie das Modul [!DNL Workfront] &gt; [!UICONTROL Dokument herunterladen] verwenden, um die entsprechende Vorlage in Ihr Szenario zu ziehen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgabeformat]</td> 
   <td> <p>Format des erstellten Dokuments auswählen.</p> 
    <ul> 
     <li> <p>PDF</p> </li> 
     <li> <p>DOCX</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Daten für Zusammenführung]</td> 
   <td> <p>Füllen Sie für jedes Wert-Tag in Ihrer Vorlage, das Sie durch Text ersetzen möchten, Folgendes aus:</p> 
    <ul> 
     <li> <p>[!UICONTROL-Schlüssel]</p> <p>Einen Schlüssel eingeben. In der Vorlage entspricht der Schlüssel dem Text, der im Wert -Tag angezeigt wird. Wenn Sie beispielsweise Text im Wert-Tag-<code>&#123;&#123;name&#125;&#125;</code> platzieren möchten, geben Sie <code>name </code>im Schlüsselfeld ein.</p> </li> 
     <li> <p>Werttyp</p> <p>Wählen Sie aus, ob die Daten im Wertfeld ein Wert, ein Objekt oder ein Array von Objekten sind.</p> </li> 
     <li> <p>[!UICONTROL-Wert]</p> <p>Geben Sie den Text ein, der im generierten Dokument anstelle des Wert-Tags angezeigt werden soll, oder ordnen Sie ihn zu.</p> </li> 
    </ul> <p> <img src="assets/generate-with-template-350x241.png" style="width: 350;height: 241;"> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Verwenden des Moduls [!UICONTROL Dokument generieren] mit JSON

Um das Modul [!UICONTROL Dokument generieren] mit JSON zu verwenden, füllen Sie die Felder wie folgt aus:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services] finden Sie unter <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgabeformat]</td> 
   <td> <p>Format des erstellten Dokuments auswählen.</p> 
    <ul> 
     <li> <p>PDF</p> </li> 
     <li> <p>DOCX</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Daten für Zusammenführung]</td> 
   <td> <p>Um JSON in diesem Modul verwenden zu können, müssen Sie die Zuordnung für dieses Feld aktivieren.</p> <p>Geben Sie die JSON-Datei ein, aus der das Dokument generiert werden soll, oder ordnen Sie sie zu. </p> <p>Sie können JSON direkt in dieses Feld eingeben oder die JSON-Ausgabe aus einem JSON-Modul zuordnen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Linearisieren einer PDF-Datei]

Dieses Tool linearisiert ein PDF-Dokument, um ein Web-optimiertes PDF-Dokument zu erstellen. Ein linearisiertes PDF-Dokument kann seitenweise angezeigt werden, ohne dass das gesamte Dokument heruntergeladen werden muss.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services] finden Sie unter <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL OCR für PDF-Datei]

Dieses Tool führt die optische Zeichenerkennung (OCR) für eine Datei durch und erzeugt eine PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services] finden Sie unter <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL OCR-Typ]</td> 
   <td> 
    <ul> 
     <li> <p>Der Typ [!UICONTROL Geändertes Originalbild] stellt sicher, dass Text durchsuchbar und auswählbar ist, ändert aber das Originalbild während des Bereinigungsprozesses (z. B. entzerrt), bevor er eine unsichtbare Textebene darüber platziert. Dieser Typ entfernt unerwünschte Artefakte und kann in einigen Szenarien zu einem besser lesbaren Dokument führen. </p> </li> 
     <li> <p>Der Typ [!UICONTROL Unchanged original image] überlagert ebenfalls eine durchsuchbare Textebene über dem Originalbild, aber in diesem Fall ist das Originalbild unverändert. Dieser Typ erzeugt maximale Wiedergabetreue gegenüber dem Originalbild.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Language]</td> 
   <td>Wählen Sie die Sprache dieses Dokuments aus.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Seitenbearbeitung]

Dieses Modul ermöglicht das selektive Drehen und Löschen von Seiten in einem PDF-Dokument. Sie können beispielsweise die Hochformat- in die Querformat-Ansicht ändern oder bestimmte Seiten aus dem PDF-Dokument entfernen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services] finden Sie unter <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Aktion]</td> 
   <td> <p>Wählen Sie die Aktion aus, die Sie mit der Datei durchführen möchten.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL DELETE]</b> </p> <p>Wählen Sie diese Option, um Seiten aus dem Dokument zu löschen.</p> </li> 
     <li> <p><b>[!UICONTROL Rotate]</b> </p> <p>Wählen Sie diese Option, um Seiten zu drehen, und geben Sie dann den Winkel (in Grad im Uhrzeigersinn) ein, um den die Dokumentseiten relativ zu ihrer Anfangsausrichtung gedreht werden sollen.</p> <p>Um von Hochformat zu Querformat oder umgekehrt zu drehen, drehen Sie die Seite um 90 oder 270 Grad.</p> <p>Wenn eine Seite umgedreht ist, drehen Sie sie um 180 Grad.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pages]</td> 
   <td> <p>Klicken Sie für jeden Seitenbereich, den Sie löschen möchten, auf <strong>[!UICONTROL Hinzufügen]</strong> und geben Sie dann die erste und letzte Seite des Seitenbereichs ein. </p> <p>Hinweis:   
     <ul> 
      <li> <p>Sie können negative Zahlen verwenden, um vom Ende des Dokuments zurückzuzählen. Die letzte Seite eines Dokuments ist -1, die vorletzte Seite -2 usw.</p> </li> 
      <li> <p>Um eine einzelne Seite zu löschen, legen Sie dieselbe Seitennummer als Beginn und Ende des Bereichs fest.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein, mit denen das Modul während jedes Szenario-Ausführungszyklus arbeiten soll, oder mappen Sie sie.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Automatisches Tagging der Barrierefreiheit von PDF]

Dieses Aktionsmodul erstellt eine PDF, die für Anwendungsfälle mit Barrierefreiheit getaggt ist. Außerdem wird ein optionaler Microsoft Excel-Bericht erstellt, der Probleme auflistet und Fehlerbehebungen vorschlägt.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services] finden Sie unter <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Shift-Überschriften]</td> 
   <td> <p>Aktivieren Sie diese Option, um Überschriften im Dokument zu verschieben.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Bericht generieren]</b> </p> <p>Aktivieren Sie diese Option, um einen Bericht zu generieren, der Zugänglichkeitsprobleme auf der PDF zusammen mit ihrer Position auflistet und Vorschläge zur Behebung dieser Probleme gibt.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDF-Dateieigenschaften]

Dieses Tool extrahiert grundlegende Informationen über das Dokument, z. B.:

* Seitenzahl
* PDF Version
* Ob die Datei verschlüsselt ist
* Ob die Datei linearisiert ist
* ob die Datei eingebettete Dateien enthält

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services] finden Sie unter <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Protect PDF-Datei]

Dieses Tool sichert ein PDF-Dokument mit einem Benutzer- oder Besitzerkennwort. Außerdem werden Einschränkungen für bestimmte Funktionen wie Drucken, Bearbeiten und Kopieren im PDF-Dokument festgelegt. Sie wählen den Typ des zu verschlüsselnden Inhalts und den Verschlüsselungsalgorithmus aus.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services] finden Sie unter <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> <p>Die Quelldatei muss im PDF-Format vorliegen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kennwortschutztyp]</td> 
   <td> <p>Aktivieren Sie diese Option, um Kennwörter zum Verschlüsseln des Eingabe-PDF-Dokuments zu verwenden. Wenn Sie diese Option aktivieren, müssen Sie einen Wert für eine oder beide der folgenden Optionen angeben und eingeben: </p> 
    <ul> 
     <li> <p>[!UICONTROL userPassword]</p> </li> 
     <li> <p>[!UICONTROL ownerPassword] </p> </li> 
    </ul> <p>Jedes Kennwort kann bis zu 128 Zeichen lang sein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verschlüsselungsalgorithmus]</td> 
   <td> <p>Wählen Sie den Verschlüsselungsalgorithmus. </p> 
    <ul> 
     <li> <p>[!UICONTROL AES-128-Verschlüsselung]</p> <p>Das Passwort unterstützt nur LATEIN-I-Zeichen. </p> </li> 
     <li> <p>[!UICONTROL AES-256-Verschlüsselung]</p> <p>Das Kennwort unterstützt den Unicode-Zeichensatz</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zu verschlüsselnder Inhalt]</td> 
   <td> <p>Wählen Sie den Typ des zu verschlüsselnden Inhalts aus.</p> 
    <ul> 
     <li> <p>[!UICONTROL Alle Inhalte]</p> </li> 
     <li> <p>[!UICONTROL Alle Inhalte außer Metadaten]</p> </li> 
     <li> <p>[!Nur UICONTROL eingebettete Daten] </p> </li> 
    </ul> <p>Durch die Auswahl von "[!UICONTROL Only embedded data]" werden alle bereitgestellten Zugriffsberechtigungen als unwirksam gerendert.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Berechtigungen]</td> 
   <td> <p>Wählen Sie alle Berechtigungen aus, die Sie einbeziehen möchten, um das Drucken, Bearbeiten oder Kopieren von Inhalten zuzulassen.</p> <p>Berechtigungseinstellungen werden nur verwendet, wenn im Feld [!UICONTROL Kennwortschutztyp] das Feld [!UICONTROL Kennwort] festgelegt ist.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Entfernen des Schutzes einer PDF-Datei]

Dieses Tool entfernt die Sicherheit (Passwortschutz) von einem PDF-Dokument.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services] finden Sie unter <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> <p>Die Quelldatei muss im PDF-Format vorliegen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kennwort]</td> 
   <td>Geben Sie das Passwort ein, mit dem die Datei derzeit geschützt ist.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Teilen Sie eine PDF-Datei auf]

Dieses Aktionsmodul teilt ein PDF-Dokument in mehrere kleinere Dokumente auf. Geben Sie an, ob die Seite nach Anzahl der Dateien, Seiten pro Datei oder Seitenbereichen aufgeteilt werden soll.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services] finden Sie unter <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> <p>Die Quelldatei muss im PDF-Format vorliegen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split-Option]</td> 
   <td>Wählen Sie aus, wie die Datei aufgeteilt werden soll. 
   <ul>
   <li><p><b>Seitenbereiche</b></p><p>Klicken Sie für jeden Seitenbereich, den Sie in ein separates Dokument aufteilen möchten, auf <b>Hinzufügen</b> und geben Sie die Seite, auf der Sie beginnen möchten, und die Seite, auf der Sie enden möchten, ein.</p></li>
   <li><p><b>Seitenzahl</b></p><p>Geben Sie die Anzahl der Seiten ein, die in die neuen Dokumente aufgenommen werden sollen.</p></li>
   <li><p><b>Anzahl Dateien</b></p><p>Geben Sie die Anzahl der Dateien mit gleichmäßiger Größe ein, in die Sie das Dokument aufteilen möchten.</p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>

## Erstellen eines benutzerdefinierten API-Aufrufs

Dieses Aktionsmodul erstellt eine benutzerdefinierte HTTP-Anfrage an die PDF-Services-API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services] finden Sie unter <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> Geben Sie einen relativen Pfad oder eine URL ein. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Methode]</td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anfragemethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Kopfzeilen]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion fügt die Autorisierungskopfzeilen automatisch hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p>Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Felder]</td> 
   <td> <p>Klicken Sie für jedes Feld, das Sie dem API-Aufruf hinzufügen möchten, <b> „Element hinzufügen</b> und geben Sie den Schlüssel und den optionalen Wert des Felds ein.</p> <p>Hinweis:  <p>Wenn Sie bedingte Anweisungen wie <code>if</code> in Ihrer JSON-Datei verwenden, setzen Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

