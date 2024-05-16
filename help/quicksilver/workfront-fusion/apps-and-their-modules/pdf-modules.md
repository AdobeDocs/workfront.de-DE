---
title: Adobe PDF Services
description: Adobe PDF Services
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: e0a5736b-dbdb-43c6-83ff-e88a5625a5bf
source-git-commit: ba161761acfc57e271f8593f534a5f7510187559
workflow-type: tm+mt
source-wordcount: '3719'
ht-degree: 0%

---

# [!DNL Adobe PDF Services]

Mit dem [!DNL Adobe Workfront Fusion] [!DNL Adobe PDF Services], können Sie Daten aus einer PDF-Datei extrahieren oder eine neue PDF-Datei aus den von Ihnen bereitgestellten Daten generieren. Darüber hinaus können Sie verschiedene Dateitypen in PDF oder PDF in andere Dateitypen konvertieren. Mit PDF Services können Sie auch Metadaten für eine PDF-Datei kombinieren, komprimieren oder lesen sowie den Kennwortschutz für die Datei steuern.

Informationen zum Erstellen eines Szenarios finden Sie unter [Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

Informationen zur API für PDF-Services finden Sie unter [Adobe Document Generation API](https://www.adobe.io/apis/documentcloud/dcsdk/doc-generation.html).

## Sicherheitsaspekte bei Verwendung von [!DNL Adobe PDF Services]

<!--

* [You do not need an [!DNL Adobe] account](#you-do-not-need-an-adobe-account) 
* [[!DNL Workfront Fusion] does not store your files](#workfront-fusion-does-not-store-your-files)

### You do not need an [!DNL Adobe] account 

Because [!DNL Workfront Fusion] is part of the [!DNL Adobe] product suite, you don't need a separate [!DNL Adobe] account to use these tools. Each tool accesses [!DNL Adobe] PDF functionality without using a connection.

Although [!DNL Workfront Fusion] does not require an [!DNL Adobe] account to use the PDF Services, the modules do require a connection. There are no credentials involved in this connection, and you provide only a name for the connection itself.

### [!DNL Workfront Fusion] does not store your files 

-->

Die [!DNL Adobe PDF Services] Sie können Ihre Dateien lesen, konvertieren oder ändern, aber weder [!DNL Adobe] nor [!DNL Workfront Fusion] Speichern Sie Ihre Dateien oder Daten. Das bedeutet:

* Sie behalten die Kontrolle über Ihre Dateien, einschließlich ihrer Sicherheit
* Sie benötigen keine [!UICONTROL Adobe] Speicher- oder Cloud-Speicher-Konto zur Verwendung der PDF Services.

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
   <p>Aktuelle Lizenzanforderungen: nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Um eine OAuth-Server-zu-Server-API zu erstellen, müssen Sie die Adobe PDF Services-API in Ihrer Adobe Developers Console hinzufügen. Wählen Sie beim Hinzufügen der API die Option OAuth Server-to-Server aus.

Anweisungen finden Sie unter [Hinzufügen einer API zum Projekt mithilfe von OAuth](https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/) In der Adobe-Entwicklerdokumentation.

## Erstellen Sie eine Verbindung zu [!DNL Adobe PDF Services]

So erstellen Sie eine Verbindung für [!DNL Adobe PDF Services] -Module:

1. In jeder [!DNL Adobe PDF Services] Modul, klicken Sie auf **[!UICONTROL Hinzufügen]** neben dem Feld Verbindung .

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
          <td>Geben Sie Ihre [!DNL Adobe] [!UICONTROL Client ID]. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] im Abschnitt [!DNL Adobe Developer Console].<p>Anweisungen zum Auffinden von Anmeldeinformationen finden Sie unter <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Anmeldeinformationen</a> in der Adobe-Entwicklerdokumentation.</p></td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client Secret]</td>
          <td>Geben Sie Ihre [!DNL Adobe] [!UICONTROL Client Secret]. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] im Abschnitt [!DNL Adobe Developer Console].<p>Anweisungen zum Auffinden von Anmeldeinformationen finden Sie unter <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Anmeldeinformationen</a> in der Adobe-Entwicklerdokumentation.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Technische Konto-ID] (nur JWT)</td>
          <td>Geben Sie Ihre [!DNL Adobe] [!UICONTROL Technische Konto-ID]. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] im Abschnitt [!DNL Adobe Developer Console].<p>Anweisungen zum Auffinden von Anmeldeinformationen finden Sie unter <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Anmeldeinformationen</a> in der Adobe-Entwicklerdokumentation.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Organisations-ID] (nur JWT)</td>
          <td>Geben Sie Ihre [!DNL Adobe] [!UICONTROL Organisations-ID]. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] im Abschnitt [!DNL Adobe Developer Console].<p>Anweisungen zum Auffinden von Anmeldeinformationen finden Sie unter <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Anmeldeinformationen</a> in der Adobe-Entwicklerdokumentation.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Meta Scopes] (nur JWT)</td>
          <td>
            Geben Sie die für die Verbindung erforderlichen Metadatenbereiche ein.
          </td>
        </tr>
       </tbody>
    </table>
1. Klicks **[!UICONTROL Weiter]** , um die Verbindung zu speichern und zum Modul zurückzukehren.


## [!DNL Adobe PDF Services] Module und ihre Felder

Bei der Konfiguration [!DNL PDF Services], [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche Felder angezeigt werden. Ein fett gedruckter Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Dokument generieren]](#generate-document)
* [[!UICONTROL Text/Tabelle extrahieren]](#extract-text--table)
* [[!UICONTROL PDF-Dateien kombinieren]](#combine-pdf-files)
* [[!UICONTROL PDF-Dateien komprimieren]](#compress-pdf-files)
* [[!UICONTROL Dokument in PDF-Datei konvertieren]](#convert-document-to-pdf-file)
* [[!UICONTROL HTML in PDF-Datei konvertieren]](#convert-html-to-pdf-file)
* [[!UICONTROL Bild in PDF-Datei konvertieren]](#convert-image-to-pdf-file)
* [[!UICONTROL PDF in Dokument konvertieren]](#convert-pdf-to-document)
* [[!UICONTROL PDF in Bild konvertieren]](#convert-pdf-to-image)
* [[!UICONTROL PDF-Datei Linearisieren]](#linearize-a-pdf-file)
* [[!UICONTROL OCR für PDF-Datei]](#ocr-for-pdf-file)
* [[!UICONTROL Seitenbearbeitung]](#page-manipulation)
* [[!UICONTROL PDF Barrierefreiheit automatisch taggen]](#pdf-accessibility-auto-tag)
* [[!UICONTROL PDF-Dateieigenschaften]](#pdf-file-properties)
* [[!UICONTROL Protect PDF-Datei]](#protect-pdf-file)
* [[!UICONTROL Schutz einer PDF-Datei entfernen]](#remove-protection-of-a-pdf-file)
* [PDF-Datei teilen](#split-a-pdf-file)

### [!UICONTROL Dokument generieren]

Die [!UICONTROL Dokument generieren] -Modul ist eine leistungsstarke Möglichkeit, eine PDF zu erstellen, die die von Ihnen ausgewählten Daten enthält. Sie können sie formatieren, indem Sie [!DNL Microsoft Word] oder durch Bereitstellung von Daten im JSON-Format.

Weitere Informationen über [!UICONTROL [!DNL Adobe PDF Services] Dokument generieren] -Funktion, siehe [Übersicht über die Dokumenterstellung](https://www.adobe.io/apis/documentcloud/dcsdk/docs.html) im [!DNL Adobe Document Services] Dokumentation.

* [Verwenden Sie die [!UICONTROL Dokument generieren] -Modul mit [!DNL Microsoft Word] template](#use-the-generate-document-module-with-a-microsoft-word-template)
* [Verwenden Sie die [!UICONTROL Dokument generieren] -Modul mit JSON](#use-the-generate-document-module-with-json)

#### Verwenden Sie die [!UICONTROL Dokument generieren] -Modul mit [!DNL Microsoft Word] template

<!--
>[!NOTE]
>
>For a discussion of Microsoft Word templates, see [Microsoft Word Template modules](../../workfront-fusion/apps-and-their-modules/microsoft-word-templates-modules.md). 
>
>You do not need to use Microsoft Word template modules to use a Microsoft Word template with the PDF Services Generate document module.
-->

So verwenden Sie die [!UICONTROL Dokument generieren] -Modul mit [!UICONTROL Microsoft Word] -Vorlage verwenden, müssen Sie zunächst die Vorlage erstellen. Anweisungen finden Sie unter &quot;Erstellen einer Vorlage&quot;im [!DNL Microsoft Office] Dokumentation.

Füllen Sie die [!UICONTROL Dokument generieren] Modulfelder wie folgt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung aus, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services], siehe <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quelldatei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> <p>Diese Quelldatei ist [!DNL Microsoft Word ]-Vorlage, die das -Modul zum Generieren der neuen PDF verwendet.</p> <p>Wir empfehlen, ein Projekt in [!DNL Workfront] für die [!DNL Microsoft Word] Vorlagen, die Sie in [!DNL Workfront Fusion]. Anschließend können Sie die [!DNL Workfront] &gt; [!UICONTROL Dokument herunterladen] Modul, um die entsprechende Vorlage in Ihr Szenario zu ziehen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgabeformat]</td> 
   <td> <p>Wählen Sie das Format für das generierte Dokument aus.</p> 
    <ul> 
     <li> <p>PDF</p> </li> 
     <li> <p>DOCX</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Daten für die Zusammenführung]</td> 
   <td> <p>Geben Sie für jedes Wert-Tag in Ihrer Vorlage, das Sie durch Text ersetzen möchten, Folgendes ein:</p> 
    <ul> 
     <li> <p>[!UICONTROL Schlüssel]</p> <p>Geben Sie einen Schlüssel ein. In der Vorlage ist der Schlüssel der im Wert-Tag angezeigte Text. Wenn Sie beispielsweise Text im Wert-Tag platzieren möchten <code>&#123;&#123;name&#125;&#125;</code>, eingeben <code>name </code>im Schlüsselfeld.</p> </li> 
     <li> <p>Werttyp</p> <p>Wählen Sie aus, ob es sich bei den Daten im Wertefeld um einen Wert, ein Objekt oder ein Array von Objekten handelt.</p> </li> 
     <li> <p>[!UICONTROL Wert]</p> <p>Geben Sie den Text ein oder ordnen Sie ihn zu, der im generierten Dokument anstelle des Wert-Tags angezeigt werden soll.</p> </li> 
    </ul> <p> <img src="assets/generate-with-template-350x241.png" style="width: 350;height: 241;"> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Verwenden Sie die [!UICONTROL Dokument generieren] -Modul mit JSON

So verwenden Sie die [!UICONTROL Dokument generieren] -Modul mit JSON verwenden, füllen Sie die Felder wie folgt aus:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung aus, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services], siehe <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quelldatei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgabeformat]</td> 
   <td> <p>Wählen Sie das Format für das generierte Dokument aus.</p> 
    <ul> 
     <li> <p>PDF</p> </li> 
     <li> <p>DOCX</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Daten für die Zusammenführung]</td> 
   <td> <p>Um JSON in diesem Modul zu verwenden, müssen Sie die Zuordnung für dieses Feld aktivieren.</p> <p>Geben Sie die JSON-Datei ein oder ordnen Sie sie zu, aus der das Dokument generiert werden soll. </p> <p>Sie können JSON direkt in dieses Feld eingeben oder die JSON-Ausgabe über ein JSON-Modul zuordnen.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung aus, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services], siehe <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quelldatei]</td> 
   <td>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elemente, die als JSON extrahiert werden sollen]</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Text]</p> </li> 
     <li> <p>[!UICONTROL Tabellen]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Begrenzungsrahmen extrahieren?]</td> 
   <td>Aktivieren Sie diese Option, um Daten zum Begrenzungsrahmen des Textes zu extrahieren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formatierungsinformationen für die Ausgabe einschließen?]</td> 
   <td>Aktivieren Sie diese Option, um der JSON-Ausgabe Stilinformationen hinzuzufügen.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDF-Dateien kombinieren]

Dieses Aktionsmodul nimmt mehrere PDF-Dateien und fasst sie zu einer PDF-Datei zusammen. Beispielsweise könnte dieses Modul alle Dokumente in einer [!UICONTROL Workfront] nach Abschluss des Projektes in eine einzige PDF aufzunehmen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung aus, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services], siehe <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dokumente]</td> 
   <td> <p>Sie können ein Aggregatormodul verwenden, um Dokumente zu einer PDF zu kombinieren, oder Sie können die Dokumente manuell hinzufügen. </p> <p>Es wird empfohlen, ein [!UICONTROL Array Aggregator]-Modul zu verwenden, um die Ausgabe eines vorherigen Moduls zu aggregieren. Mithilfe eines Aggregators müssen Sie nicht die Namen, Speicherorte oder Anzahl der zu kombinierenden Dateien kennen. Die Verwendung eines Aggregators ist daher viel flexibler und skalierbarer als die manuelle Eingabe der zu kombinierenden Dokumente.</p> <p>Um das Dateimodul [!UICONTROL PDF] mit einem Aggregator kombinieren zu können, müssen Sie die Zuordnung im Feld [!UICONTROL Dokumente] aktivieren. </p> <p>In diesem Beispiel identifiziert das Modul [!UICONTROL Read Related Records] Dokumente, die mit einem Projekt verknüpft sind, und das Modul [!UICONTROL Download Documents] lädt jedes einzelne herunter. Alle PDF werden in einem Array aggregiert, das an das Dateimodul [!UICONTROL PDF] übergeben wird.</p> <p> <img src="assets/combine-example-350x104.png" style="width: 350;height: 104;"> </p> <p>Sie können Dokumente auch manuell eingeben.</p> <p>Für jedes Dokument, das in die kombinierte PDF aufgenommen werden soll:</p> 
    <ol> 
     <li value="1"> <p>Klicken Sie auf [!UICONTROL Dokument hinzufügen]</p> </li> 
     <li value="2"> <p>Wählen Sie im Feld [!UICONTROL Quelldatei] das Modul aus, das das einzuschließende Dokument ausgibt, oder ordnen Sie den Namen und die Daten der Quelldatei zu. </p> </li> 
     <li value="3"> <p>(Optional) Wenn Sie nur bestimmte Seiten aus der Quelldatei einbeziehen möchten, klicken Sie für jeden Seitenbereich, den Sie hinzufügen möchten, auf <strong>[!UICONTROL Element hinzufügen]</strong> Geben Sie im Feld [!UICONTROL Seiten] die erste und letzte Seite des einzuschließenden Seitenbereichs ein und klicken Sie auf <strong>[!UICONTROL Hinzufügen]</strong>. Sie können mehr als einen Seitenbereich in ein einzelnes Dokument einschließen.</p> </li> 
     <li value="4"> <p>Klicks <strong>[!UICONTROL Hinzufügen]</strong>. </p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDF-Dateien komprimieren]

Dieses Aktionsmodul nimmt eine PDF-Datei und komprimiert sie. Dies kann zur Einsparung von Bandbreite oder Speicher nützlich sein.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung aus, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services], siehe <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quelldatei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> <p>Die Quelldatei muss im PDF-Format vorliegen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Komprimierungsstufe]</td> 
   <td>Wählen Sie die gewünschte Komprimierungsstufe aus.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Dokument in PDF-Datei konvertieren]

Dieses Tool konvertiert ein Dokument in eine PDF-Datei. Die Quelldatei muss eines der folgenden Dokumentenformate sein:

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
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung aus, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services], siehe <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quelldatei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> <p>Die Quelldatei muss eines der folgenden Formate aufweisen:</p> 
    <ul> 
     <li> <p>DOC</p> </li> 
     <li> <p>XLS</p> </li> 
     <li> <p>PPT</p> </li> 
     <li> <p>TXT</p> </li> 
     <li> <p>RTF</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sprache]</td> 
   <td> <p>Wählen Sie die Standardsprache für das Quelldokument aus. Dadurch kann das Modul eine geeignete Schriftart auswählen, wenn die Schriftart nicht in der Quelldatei enthalten ist.</p> <p>Wählen Sie aus den folgenden Sprachen aus:</p> 
    <ul> 
     <li> <p>en-US (Standard): Englisch (USA)</p> </li> 
     <li> <p>ca-ES: Katalanisch (Spanien)</p> </li> 
     <li> <p>cs-CZ: Tschechisch (Tschechische Republik)</p> </li> 
     <li> <p>da-DK: Dänisch (Dänemark)</p> </li> 
     <li> <p>de-DE: Deutsch (Deutschland)</p> </li> 
     <li> <p>en-AE: Englisch (Vereinigte Arabische Emirate)</p> </li> 
     <li> <p>en-GB: Englisch (Vereinigtes Königreich)</p> </li> 
     <li> <p>en-IL: Englisch (Israel)</p> </li> 
     <li> <p>en-US: English (United States of America)</p> </li> 
     <li> <p>es-ES: Spanisch (Spanien)</p> </li> 
     <li> <p>es-MX: Spanisch (Mexiko)</p> </li> 
     <li> <p>eu-ES: Baskisch (Spanien)</p> </li> 
     <li> <p>fi-FI: Finnisch (Finnland)</p> </li> 
     <li> <p>fr-CA: Französisch (Kanada)</p> </li> 
     <li> <p>fr-FR: Französisch (Frankreich)</p> </li> 
     <li> <p>fr-MA: Französisch (Marokko)</p> </li> 
     <li> <p>hr-HR: Kroatisch (Kroatien)</p> </li> 
     <li> <p>hu-HU: Ungarisch (Ungarn)</p> </li> 
     <li> <p>IT: Italienisch (Italien)</p> </li> 
     <li> <p>ja-JP: Japanisch (Japan)</p> </li> 
     <li> <p>kr-KR: Korea (Südkorea)</p> </li> 
     <li> <p>nb-NO: Norwegisch Bokmål (Norwegen)</p> </li> 
     <li> <p>nl-NL: Niederländisch (Niederlande)</p> </li> 
     <li> <p>pl-PL: Polnisch (Polen)</p> </li> 
     <li> <p>pt-BR: Portugiesisch (Brasilien)</p> </li> 
     <li> <p>pt-PT: Portugiesisch (Portugal)</p> </li> 
     <li> <p>ro-RO: Rumänisch (Rumänien)</p> </li> 
     <li> <p>Ru-RU: Russisch (Russland)</p> </li> 
     <li> <p>sk-SK: Slowakisch (Slowakei)</p> </li> 
     <li> <p>sl-SI: Slowenisch (Slowenien)</p> </li> 
     <li> <p>sv-SE: Schwedisch (Schweden)</p> </li> 
     <li> <p>tr-TR: Türkisch (Türkei)</p> </li> 
     <li> <p>uk-UA: Ukrainisch (Ukraine)</p> </li> 
     <li> <p>zh-CN: Chinesisch (Festland China)</p> </li> 
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
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung aus, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services], siehe <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quelldatei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> <p>Wichtig: Die Quelldatei muss im HTML- oder ZIP-Format vorliegen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON]</td> 
   <td> <p>Wenn Ihre HTML auf JavaScript-Variablen verweist, können Sie diese Variablen hier einbeziehen. </p> <p>Klicken Sie für jede Variable auf <strong>[!UICONTROL Element hinzufügen]</strong> und den Schlüssel und Wert der Variablen einschließen.</p> <p>Hinweis:   
     <ul> 
      <li> <p>Beim Erstellen einer PDF aus einer ZIP-Datei muss das Quellmaterial ein Skriptelement enthalten, z. B.: <code> &lt;script src='./json.js' type='text/javascript'&gt;&lt;/script&gt;</code> </p> </li> 
      <li> <p>Beim Erstellen einer PDF aus einer URL wird der Inhalt dieses JSON-Objekts in die Browser-VM eingefügt, bevor die Seite gerendert wird. </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kopf- und Fußzeile einschließen]</td> 
   <td> <p>Aktivieren Sie diese Option, um Kopf- und Fußzeilen für das PDF-Dokument zu erstellen.</p> 
    <ul> 
     <li> <p>Die Kopfzeile enthält ein Datum und den Dokumenttitel.</p> </li> 
     <li> <p>Die Fußzeile enthält den Dateinamen und eine Seitenzahl.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seitenbreite]</td> 
   <td>Geben Sie die Breite des Papiers in Zoll ein. Das -Modul verwendet diese Informationen, um die Seiten in der erstellten PDF-Datei zu formatieren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seitenhöhe]</td> 
   <td>Geben Sie die Höhe des Papiers in Zoll ein. Das -Modul verwendet diese Informationen, um die Seiten in der erstellten PDF-Datei zu formatieren.</td> 
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
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung aus, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services], siehe <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quelldatei]</td> 
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
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung aus, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services], siehe <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quelldatei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> <p>Die Quelldatei muss im PDF-Format vorliegen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Files Format]</td> 
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

Dieses Tool konvertiert eine PDF in ein Bild im PNG- oder JPEG-Format, das dann als ZIP ausgegeben wird. Die PDF wird in ein Bild pro Seite konvertiert, und jedes Bild endet mit der Seitenzahl. Die Bilddateien werden dann in einer ZIP-Datei zusammengefasst.

Beispielsweise würde eine Datei mit dem Namen &quot;TestFile&quot;mit 8 Seiten 8 Bilder mit dem Namen &quot;TestFile_1&quot;bis &quot;TestFile_8&quot;erzeugen. Die Ausgabe des Moduls ist eine ZIP-Datei, die die 8 Bilder enthält.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung aus, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services], siehe <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quelldatei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> <p>Die Quelldatei muss im PDF-Format vorliegen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Files Format]</td> 
   <td> <p>Wählen Sie das Format aus, in dem die Dateien ausgegeben werden sollen:</p> 
    <ul> 
     <li>PNG</li> 
     <li>JPEG</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDF-Datei Linearisieren]

Dieses Tool linearisiert ein PDF-Dokument, um ein Web-optimiertes PDF-Dokument zu erstellen. Ein linearisiertes PDF-Dokument kann seitenweise angezeigt werden, ohne dass das gesamte Dokument heruntergeladen werden muss.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung aus, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services], siehe <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quelldatei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL OCR für PDF-Datei]

Dieses Tool führt eine optische Zeichenerkennung (OCR) für eine Datei durch und erzeugt eine PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung aus, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services], siehe <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quelldatei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL OCR type]</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Modifiziertes Originalbild] stellt sicher, dass der Text durchsuchbar und auswählbar ist, ändert aber das Originalbild während des Bereinigungsprozesses (z. B. beim Verkleinern), bevor eine unsichtbare Textebene darüber platziert wird. Dieser Typ entfernt unerwünschte Artefakte und kann in einigen Szenarien zu einem lesbareren Dokument führen. </p> </li> 
     <li> <p>[!UICONTROL Ungeändertes Originalbild] überlagert auch eine durchsuchbare Textebene über dem Originalbild, in diesem Fall ist das Originalbild jedoch unverändert. Dieser Typ erzeugt maximale Wiedergabetreue zum Originalbild.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sprache]</td> 
   <td>Wählen Sie die Sprache dieses Dokuments aus.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Seitenbearbeitung]

Dieses Modul ermöglicht es Ihnen, Seiten in einem PDF-Dokument selektiv zu drehen oder zu löschen. Sie können beispielsweise die Hochformatansicht in die Querformatansicht ändern oder bestimmte PDF-Seiten aus dem Dokument entfernen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung aus, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services], siehe <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quelldatei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aktion]</td> 
   <td> <p>Wählen Sie die Aktion aus, die Sie für die Datei ausführen möchten.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Löschen]</b> </p> <p>Wählen Sie diese Option aus, um Seiten aus dem Dokument zu löschen.</p> </li> 
     <li> <p><b>[!UICONTROL Drehen]</b> </p> <p>Wählen Sie diese Option aus, um Seiten zu drehen, und geben Sie dann den Winkel in Grad im Uhrzeigersinn ein, um den Sie die Dokumentseiten in Bezug auf ihre Startausrichtung drehen möchten.</p> <p>Um zwischen Hochformat und Querformat zu wechseln oder umgekehrt, drehen Sie die Seite um 90 oder 270 Grad.</p> <p>Wenn eine Seite verkehrt herum ist, drehen Sie sie um 180 Grad.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seiten]</td> 
   <td> <p>Klicken Sie für jeden zu löschenden Seitenbereich auf <strong>[!UICONTROL Hinzufügen]</strong> und geben Sie dann die erste und letzte Seite des Seitenbereichs ein. </p> <p>Hinweis:   
     <ul> 
      <li> <p>Sie können negative Zahlen verwenden, um vom Ende des Dokuments zurückzuzählen. Die letzte Seite eines Dokuments ist -1, die zweite Seite der letzten Seite -2 usw.</p> </li> 
      <li> <p>Um eine einzelne Seite zu löschen, legen Sie dieselbe Seitenzahl fest wie Anfang und Ende des Bereichs.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, mit denen das Modul während der verschiedenen Ausführungszyklen eines Szenarios arbeiten soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDF Barrierefreiheit automatisch taggen]

Dieses Aktionsmodul erstellt eine PDF, die für Anwendungsfälle der Barrierefreiheit mit Tags versehen ist. Außerdem wird ein optionaler Microsoft Excel-Bericht erstellt, der Probleme auflistet und Korrekturen vorschlägt.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung aus, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services], siehe <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quelldatei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Umschalt-Überschriften]</td> 
   <td> <p>Aktivieren Sie diese Option, um Überschriften im Dokument zu verschieben.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Bericht erstellen]</b> </p> <p>Aktivieren Sie diese Option, um einen Bericht zu generieren, in dem Probleme mit der Barrierefreiheit auf der PDF zusammen mit ihrem Standort aufgelistet und Vorschläge zur Behebung dieser Probleme unterbreitet werden.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDF-Dateieigenschaften]

Dieses Tool extrahiert grundlegende Informationen zum Dokument, z. B.:

* Seitenzahl
* PDF-Version
* Ob die Datei verschlüsselt ist
* Ob die Datei linerarisiert ist
* Ob die Datei eingebettete Dateien enthält

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung aus, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services], siehe <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quelldatei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Protect PDF-Datei]

Dieses Tool sichert ein PDF-Dokument mit einem Benutzer- oder Eigentümerkennwort. Außerdem werden Einschränkungen für bestimmte Funktionen wie Drucken, Bearbeiten und Kopieren im PDF-Dokument festgelegt. Wählen Sie den Typ des zu verschlüsselnden Inhalts und den Verschlüsselungsalgorithmus aus.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung aus, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services], siehe <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quelldatei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> <p>Die Quelldatei muss im PDF-Format vorliegen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kennwortschutz]</td> 
   <td> <p>Aktivieren Sie diese Option, um Kennwörter zum Verschlüsseln des PDF-Eingabedokuments zu verwenden. Wenn Sie diese Option aktivieren, müssen Sie einen Wert für einen oder beide der folgenden Werte angeben und eingeben: </p> 
    <ul> 
     <li> <p>[!UICONTROL userPassword]</p> </li> 
     <li> <p>[!UICONTROL ownerPassword] </p> </li> 
    </ul> <p>Jedes Kennwort kann bis zu 128 Zeichen lang sein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verschlüsselungsalgorithmus]</td> 
   <td> <p>Wählen Sie den Verschlüsselungsalgorithmus aus. </p> 
    <ul> 
     <li> <p>[!UICONTROL AES-128 encryption]</p> <p>Das Kennwort unterstützt nur LATIN-I-Zeichen. </p> </li> 
     <li> <p>[!UICONTROL AES-256 encryption]</p> <p>Das Kennwort unterstützt den Unicode-Zeichensatz</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inhalt zur Verschlüsselung]</td> 
   <td> <p>Wählen Sie den Typ des zu verschlüsselnden Inhalts aus.</p> 
    <ul> 
     <li> <p>[!UICONTROL Gesamter Inhalt]</p> </li> 
     <li> <p>[!UICONTROL Alle Inhalte außer Metadaten]</p> </li> 
     <li> <p>[!UICONTROL Only embedded data] </p> </li> 
    </ul> <p>Durch die Auswahl von "[!UICONTROL Only embedded data]"werden alle bereitgestellten Zugriffsberechtigungen als ineffektiv gerendert.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Berechtigungen]</td> 
   <td> <p>Wählen Sie alle Berechtigungen aus, die Sie einbeziehen möchten, um das Drucken, Bearbeiten oder Kopieren von Inhalten zu ermöglichen.</p> <p>Berechtigungseinstellungen werden nur verwendet, wenn [!UICONTROL ownerPassword] im Feld [!UICONTROL Password Protection Type] festgelegt ist.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Schutz einer PDF-Datei entfernen]

Dieses Tool entfernt die Sicherheit (Kennwortschutz) aus einem PDF-Dokument.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung aus, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services], siehe <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quelldatei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> <p>Die Quelldatei muss im PDF-Format vorliegen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kennwort]</td> 
   <td>Geben Sie das Kennwort ein, das die Datei derzeit schützt.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDF-Datei teilen]

Dieses Aktionsmodul teilt ein PDF-Dokument in mehrere kleinere Dokumente auf. Sie legen fest, ob die Aufteilung nach Anzahl der Dateien, Seiten pro Datei oder Seitenbereichen erfolgen soll.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung aus, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services], siehe <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quelldatei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> <p>Die Quelldatei muss im PDF-Format vorliegen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aufspaltungsoption]</td> 
   <td>Wählen Sie aus, wie die Datei geteilt werden soll. 
   <ul>
   <li><p><b>Seitenbereiche</b></p><p>Klicken Sie für jeden Seitenbereich, der in ein separates Dokument aufgeteilt werden soll, auf <b>Hinzufügen</b> und geben Sie die Seite ein, auf der Sie beginnen möchten, sowie die Seite, auf der Sie enden möchten.</p></li>
   <li><p><b>Seitenzahl</b></p><p>Geben Sie die Anzahl der Seiten an, die Sie in die neuen Dokumente aufnehmen möchten.</p></li>
   <li><p><b>Anzahl Dateien</b></p><p>Geben Sie die Anzahl der Dateien mit gleicher Größe ein, in die Sie das Dokument aufteilen möchten.</p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>

## Benutzerdefinierte API-Aufrufe durchführen

Dieses Aktionsmodul enthält eine benutzerdefinierte HTTP-Anforderung an die PDF Services-API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Wählen Sie die Verbindung aus, die für dieses Modul verwendet werden soll.</p> Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe PDF Services], siehe <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe PDF Services]</a> in diesem Artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> Geben Sie einen relativen Pfad oder eine URL ein. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methode]</td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion fügt die Autorisierungskopfzeilen automatisch hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p>Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Felder]</td> 
   <td> <p>Klicken Sie für jedes Feld, das Sie zum API-Aufruf hinzufügen möchten, auf <b>Element hinzufügen</b> und geben Sie den Schlüssel und den optionalen Wert des Felds ein.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> Fügen Sie die Anführungszeichen in Ihre JSON-Datei außerhalb der bedingten Anweisung ein.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

