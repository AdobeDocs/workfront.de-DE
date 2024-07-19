---
filename: microsoft-word-templates-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Microsoft Word-Vorlagenmodule
description: In einem Adobe Workfront Fusion-Szenario können Sie Workflows automatisieren, die Microsoft Word-Vorlagen verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 889b417c-04a9-4dbf-9a34-0dab65f11f03
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '1401'
ht-degree: 0%

---

# [!DNL Microsoft Word Template] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL Microsoft Word Templates] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

Wenn Sie Anweisungen zum Erstellen eines Szenarios benötigen, finden Sie weitere Informationen unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> 
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
     --> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     --> </td> 
   </tr>
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Um [!DNL Miscrosoft Word Templates] mit [!DNL Adobe Workfront Fusion] zu verwenden, ist ein [!DNL Office 365] -Konto erforderlich. Sie können eine unter www.office.com erstellen.



## Verbinden des [!DNL Office]-Dienstes mit [!DNL Workfront Fusion]

Anweisungen zum Verbinden Ihres [!DNL Office]-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter [Erstellen einer Verbindung mit [!UICONTROL Adobe Workfront Fusion] - Grundlegende Anweisungen](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Einige Microsoft-Apps verwenden dieselbe Verbindung, die an individuelle Benutzerberechtigungen gebunden ist. Daher werden beim Erstellen einer Verbindung im Bildschirm für die Genehmigung von Berechtigungen alle Berechtigungen angezeigt, die zuvor für die Verbindung dieses Benutzers gewährt wurden, zusätzlich zu den neuen Berechtigungen, die für die aktuelle Anwendung erforderlich sind.
>
>Wenn beispielsweise ein Benutzer über den Excel-Connector über die Berechtigung &quot;Tabelle lesen&quot;verfügt und dann im Outlook-Connector eine Verbindung zum Lesen von E-Mails erstellt, zeigt der Bildschirm für die Genehmigung der Berechtigungen sowohl die bereits erteilte Berechtigung &quot;Tabelle lesen&quot;als auch die neu erforderliche Berechtigung &quot;E-Mail schreiben&quot;an.

## Verwenden von [!DNL Microsoft Word Templates] -Modulen

Sie können ein [!DNL Microsoft Word Template] -Modul verwenden, um Daten aus mehreren Webdiensten in ein [!DNL Microsoft Word] -Dokument zusammenzuführen.

Sie können beispielsweise diese [!DNL Microsoft Word] -Vorlage verwenden:

![](assets/word-template-before-filled-350x62.png)

So erstellen Sie dieses Dokument:

![](assets/word-template-exampled-filled-350x85.png)

## Über Wert-Tags

Eine [!DNL Microsoft Word] -Vorlage ist ein normales [!DNL Microsoft Word] -Dokument (.docx-Datei) mit speziellen Tags im Text, die bestimmen, wo und wie Daten zusammengeführt oder ausgefüllt werden. Es gibt drei Arten von Tags:

* [Einfaches Wert-Tag](#simple-value-tag)
* [Bedingungs-Tag](#condition-tag)
* [Schleifentag](#loop-tag)

### Einfaches Wert-Tag {#simple-value-tag}

Ein einfaches Wert-Tag wird einfach durch einen entsprechenden Wert ersetzt. Der Name des Tags entspricht dem Wert des Felds [!UICONTROL Schlüssel] , der in zwei geschweifte Klammern gesetzt wird, beispielsweise


<pre>&lbrace;&lbrace;name&rbrace;&rbrace;</pre>


.

**Beispiel:** Um ein Dokument zu erstellen, in dem &quot;Hi, Petr!&quot;steht, können Sie ein [!DNL Microsoft Word Template] -Modul verwenden, um die folgende Vorlage zu erstellen:

<pre>&gt; Hi &lbrace;&lbrace;name&rbrace;&rbrace;!</pre>

Dazu richten Sie das -Modul wie folgt ein:

![](assets/word-template-simple-value-350x286.png)

### Bedingungs-Tag {#condition-tag}

Sie können ein Bedingungs-Tag verwenden, um Text einzuschließen, der nur gerendert werden soll, wenn bestimmte Bedingungen erfüllt sind. Um den Text einzuschließen, platzieren Sie ihn zwischen öffnenden und schließenden Bedingungs-Tags wie &quot;hasPhone&quot;, wenn die Bedingung lautet, ob die Daten eine Telefonnummer enthalten oder nicht. Dem Namen eines öffnenden Tags wird ein Hash-Zeichen # vorangestellt, dem Namen eines schließenden Tags ein Schrägstrich vorangestellt, wie im folgenden Beispiel gezeigt.

**Beispiel:** Um ein Dokument zu erstellen, das die Telefonnummer eines Kunden enthält, wenn die Eingabedaten eine Telefonnummer, aber keine E-Mail-Adresse enthalten, können Sie ein [!DNL Microsoft Word Template] -Modul verwenden und die folgende Vorlage erstellen:
<pre>&gt; &lbrace;&lbrace;#hasPhone&rbrace;&rbrace;Telefon: &lbrace;&lbrace;phone&rbrace;&rbrace; &lbrace;&lbrace;/hasPhone&rbrace;&rbrace;</pre><pre>&gt; &lbrace;&lbrace;#hasEmail&rbrace;&rbrace;Email: &lbrace;&lbrace;email&rbrace;&rbrace; &lbrace;&lbrace;/hasEmail&rbrace;&rbrace;</pre>Dazu richten Sie das -Modul wie folgt ein:

![](assets/word-template-conditional-350x501.png)

Im Dokument würde die Telefonnummer wie folgt aussehen:
<pre>&gt; Telefon: 4445551234</pre>

### Schleifentag {#loop-tag}

Sie können ein Loop-Tag, auch als Abschnitt-Tag bezeichnet, verwenden, um einen Textabschnitt zu wiederholen. Schließen Sie den Text ein, indem Sie ihn zwischen den öffnenden und schließenden Schleifen-Tags platzieren. Dem Namen eines öffnenden Tags wird ein Hash-Zeichen # vorangestellt; dem Namen eines schließenden Tags wird ein Schrägstrich / vorangestellt.

* [Schleifen-Tag mit Ausfüllen eines Dokumentmoduls](#loop-tag-with-fill-out-a-document-module)
  <!-- [Loop tag with Fill a document with a batch of data module](#loop-tag-with-fill-a-document-with-a-batch-of-data-module)-->

#### Schleifen-Tag mit Dokumentmodul ausfüllen {#loop-tag-with-fill-out-a-document-module}

**Beispiel:** Um ein Dokument zu erstellen, in dem der Name und die Telefonnummer jedes Kontakts in einer Kundenliste aufgeführt sind, können Sie ein [!DNL Microsoft Word Template] -Modul verwenden und die folgende Vorlage erstellen:

<pre>&gt; {#contact}</pre><pre>&gt;     &lbrace;&lbrace;name&rbrace;&rbrace;, &lbrace;&lbrace;phone&rbrace;&rbrace;</pre><pre>&gt; &lbrace;&lbrace;/contact&rbrace;&rbrace;</pre>

Dazu richten Sie das -Modul wie folgt ein:


![](assets/word-template-fill-out-a-document-350x732.png)

Das -Modul erstellt das folgende Dokument:

```
> Jan Toman, 4445551234
> Eduard Salo, 4445552345
```

<!--

#### Loop tag with Fill a document with a batch of data module {#loop-tag-with-fill-a-document-with-a-batch-of-data-module}

**Example:** You can export Google contacts into a table that you create using loop tags.

The first module loads the template. The next module retrieves all contacts from the group you specify in [!DNL Google Contacts]. The aggregator module aggregates all values retrieved from Google Contacts and merges them into the template. And the last module saves the filled template to the desired location.

![](assets/word-template-batch-scenario-350x124.png)

You could use this scenario with the following template:

![](assets/word-template-batch-template-350x26.png)

To do this, you would set up the module as follows:

![](assets/word-template-batch-module-setup-350x323.png)

The module would create the following document:

![](assets/word-template-batch-document-350x46.png)
-->

## [!DNL Microsoft Word Template] Module

Diese Module erfordern keine Verbindung.

* [Ausfüllen eines Dokuments](#fill-out-a-document)
* [Füllen eines Dokuments mit einem Datenstapel](#fill-a-document-with-a-batch-of-data)

### [!UICONTROL Ausfüllen eines Dokuments] {#fill-out-a-document}

Mit diesem Transformatormodul können Sie ein Dokument mit den von Ihnen angegebenen Daten ausfüllen. Sie kann mit einfachen Werte-Tags, Bedingungs-Tags oder Schleifentags verwendet werden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start-Trennzeichen des zu ersetzenden Texts]</td> 
   <td> <p>Geben Sie die Zeichen ein, die am Anfang des zu ersetzenden Texts markiert werden sollen. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Geben Sie <code>[[</code> ein, wenn Sie einen Text ähnlich dem folgenden ersetzen möchten: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Endtrennzeichen des zu ersetzenden Texts]</p> </td> 
   <td> <p>Geben Sie die Zeichen ein, die am Ende des zu ersetzenden Texts markiert werden sollen. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Geben Sie <code>]]</code> ein, wenn Sie einen Text ähnlich dem folgenden ersetzen möchten: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p> Ordnen Sie die Datei zu, die Sie vom vorherigen Modul hochladen möchten (z. B. HTTP &gt; Datei abrufen oder Dropbox &gt; Dateimodul abrufen). Oder geben Sie die Datendatei manuell ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name der ausgefüllten Datei]</td> 
   <td>Geben Sie einen Dateinamen (einschließlich Erweiterung) für die Zielausgabedatei ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datenquelle]</td> 
   <td> <p>Wählen Sie eine Option, um anzugeben, ob die von Ihnen verwendeten Daten aus einem Formular oder aus einer Rohdatenkollektion stammen (nicht verarbeitete Computerdaten).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Werte]</td> 
   <td> <p>Hierbei muss es sich um ein Array von Kollektionen handeln, wobei Folgendes gilt:</p> 
    <ul> 
     <li>Jede Kollektion entspricht einem Dateneintrag und enthält ein Element <code>entry</code></li> 
     <li>Element <code>entry </code>enthält eine Sammlung von <code>key </code>und <code>value</code></li> 
     <li>Element <code>key </code>enthält den Namen des Tags</li> 
     <li>item <code>value </code>enthält den Wert des Tags</li> 
    </ul> 
    <p>So fügen Sie einen Eintrag hinzu:</p>
    <ol> 
     <li> Klicken Sie auf <b>[!UICONTROL Element hinzufügen]</b>. </li> 
     <li>Wählen Sie den Werttyp des Eintrags aus.</li> 
     <li>Fügen Sie den Namen und den Wert hinzu. Weitere Informationen finden Sie im Beispiel für den ausgewählten Werttyp in diesem Artikel. 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">Einfaches Wert-Tag</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">Bedingungs-Tag</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">Schleifentag</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Füllen eines Dokuments mit einem Datenstapel] {#fill-a-document-with-a-batch-of-data}

Dieses Aggregatormodul ist nützlich, wenn Ihre Dateneinträge als separate Bundles vorliegen. Mit diesem Modul können Sie einfach die für das Feld Wert erforderliche Struktur einrichten und Elemente jedem Wert zuordnen. Im Gegensatz zum Dokumentmodul ausfüllen erlaubt das Feld Werte unter Dokument mit einem Stapel Datenmodul ausfüllen nur einen einzigen Eintrag, der Variablen enthält.

Sie können dieses Modul auch dann verwenden, wenn Ihre Dateneinträge als Array vorliegen, indem Sie mit dem Modul *Iterator* den Inhalt des Arrays in eine Reihe von Bundles umwandeln.

Die tatsächlichen Werte werden für jedes eingehende Bundle erstellt und ausgefüllt. Die Vorlage wird erzeugt, nachdem alle Eingabebundles verarbeitet wurden.

Dieses Aggregatormodul ist besonders für die Erstellung von Listen oder Berichten nützlich.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td>Wählen Sie das Modul aus, das die Quelle Ihres Textes darstellt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start-Trennzeichen des zu ersetzenden Texts]</td> 
   <td> <p>Geben Sie die Zeichen ein, die am Anfang des zu ersetzenden Texts markiert werden sollen. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Geben Sie <code>[[</code> ein, wenn Sie einen Text ähnlich dem folgenden ersetzen möchten: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Endtrennzeichen des zu ersetzenden Texts]</p> </td> 
   <td> <p>Geben Sie die Zeichen ein, die am Ende des zu ersetzenden Texts markiert werden sollen. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Geben Sie <code>]]</code> ein, wenn Sie einen Text ähnlich dem folgenden ersetzen möchten: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Gruppe nach]</td> 
   <td> Definieren Sie einen Ausdruck, der ein oder mehrere zugeordnete Elemente enthält. Die aggregierten Daten werden unter Gruppen mit demselben Ausdruckswert getrennt. Jede Gruppe gibt als separates Bundle aus, das einen Schlüssel mit dem ausgewerteten Ausdruck und dem aggregierten Text enthält. Auf diese Weise können Sie den Schlüssel als Filter in nachfolgenden Modulen verwenden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verarbeitung nach einer leeren Aggregation stoppen]</td> 
   <td>Aktivieren Sie diese Option, um die Verarbeitung zu stoppen, wenn eine Aggregation keine Bundles enthält.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p> Ordnen Sie die Datei zu, die Sie vom vorherigen Modul hochladen möchten (z. B. HTTP &gt; Datei abrufen oder Dropbox &gt; Dateimodul abrufen). Oder geben Sie die Datendatei manuell ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name der ausgefüllten Datei]</td> 
   <td>Geben Sie einen Dateinamen (einschließlich Erweiterung) für die Zielausgabedatei ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datenquelle]</td> 
   <td> <p>Wählen Sie eine Option, um anzugeben, ob die von Ihnen verwendeten Daten aus einem Formular oder aus einer Rohdatenkollektion stammen (nicht verarbeitete Computerdaten).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Werte]</td> 
   <td> <p>Hierbei muss es sich um ein Array von Kollektionen handeln, wobei Folgendes gilt:</p> 
    <ul> 
     <li>Jede Kollektion entspricht einem Dateneintrag und enthält ein Element <code>entry</code></li> 
     <li>Element <code>entry </code>enthält eine Sammlung von <code>key </code>und <code>value</code></li> 
     <li>Element <code>key </code>enthält den Namen des Tags</li> 
     <li>item <code>value </code>enthält den Wert des Tags</li> 
    </ul> 
    <p>So fügen Sie einen Eintrag hinzu:</p>
    <ol> 
     <li> Klicken Sie auf <b>[!UICONTROL Element hinzufügen]</b>. </li> 
     <li>Wählen Sie den Werttyp des Eintrags aus.</li> 
     <li>Fügen Sie den Namen und den Wert hinzu. Weitere Informationen finden Sie im Beispiel für den ausgewählten Werttyp in diesem Artikel. 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">Einfaches Wert-Tag</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">Bedingungs-Tag</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">Schleifentag</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>
