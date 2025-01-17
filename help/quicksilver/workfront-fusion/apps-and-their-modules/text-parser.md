---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: Text-Parser
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d71cf64-4f86-42c5-81e7-8fc15333cbd7
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1097'
ht-degree: 0%

---

# [!UICONTROL Text-Parser]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Text-Parser](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/text-parser.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Sie können das [!UICONTROL Text-Parser-Tool] verwenden, um Text zur Verwendung in anderen [!DNL Adobe Workfront Fusion]-Szenario-Modulen zu analysieren. Der [!UICONTROL Text-Parser] erfordert keine Verbindung.

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
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## Text-Parser-API-Informationen

Der Text-Parser-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v2</td> 
  </tr>
 </tbody> 
 </table>

## [!UICONTROL Text-Parser] Module und ihre Felder

Beim Konfigurieren von [!UICONTROL Text-Parser]-Modulen zeigt [!DNL Adobe Workfront Fusion] die unten aufgeführten Felder an. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Transformatoren

* [[!UICONTROL Elemente vom HTML abrufen]](#get-elements-from-html)
* [[!UICONTROL Elemente aus Text abrufen]](#get-elements-from-text)
* [[!UICONTROL HTML in Text]](#html-to-text)
* [[!UICONTROL Übereinstimmungsmuster]](#match-pattern)
* [[!UICONTROL Ersetzen]](#replace)

#### [!UICONTROL Elemente vom HTML abrufen]

Ruft die gewünschten Elemente aus dem HTML-Code ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Die Routenausführung auch dann fortsetzen, wenn das Modul keine Übereinstimmungen findet]</td> 
   <td> <p>Aktivieren Sie diese Option, um sicherzustellen, dass das Modul das Szenario nicht stoppt, wenn es keine Ergebnisse zurückgibt.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Elementtyp]</td> 
   <td> <p> Wählen Sie den Elementtyp aus, den Sie aus dem HTML-Code abrufen möchten. </p> 
    <ul> 
     <li>[!UICONTROL Bild]</li> 
     <li>[!UICONTROL Link]</li> 
     <li>[!UICONTROL iFrame-Element(e)]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>Geben Sie den HTML-Code ein, von dem Sie die angegebenen Elementtypen abrufen möchten, oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elemente aus Text abrufen]

Analysiert Elemente aus Text anhand des angegebenen Musters.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Eingabetext]</td> 
   <td> <p>Geben Sie den Text ein, den Sie analysieren möchten, oder mappen Sie ihn.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Muster]</td> 
   <td> <p>Wählen Sie aus dem Text das Muster aus, das die zu analysierenden Elemente enthält.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Doppelte Vorkommen ignorieren]</td> 
   <td> <p>Aktivieren Sie dieses Kontrollkästchen, um doppelte Vorkommen eines Textelements zu ignorieren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL HTML in Text]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>Geben Sie den HTML-Code ein, den Sie in Nur-Text konvertieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zeilenumbruch] </td> 
   <td> <p>Wählen Sie den Zeilenumbruchtyp aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Großbuchstaben]</p> </td> 
   <td> <p>Aktivieren Sie diese Option, um in Überschriften-Tags eingeschlossenen Text (z. B. &lt;h2&gt; &lt;/h2&gt;) in Großbuchstaben zu konvertieren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Übereinstimmungsmuster]

Das [!UICONTROL Match pattern]-Modul ermöglicht es, Zeichenfolgenelemente zu finden und zu extrahieren, die einem Suchmuster aus einem bestimmten Text entsprechen. Dieses Modul verwendet reguläre Ausdrücke (auch als Regex oder Regex bezeichnet).

Ein regulärer Ausdruck ist eine Sequenz von Zeichen, in der jedes Zeichen entweder ein Metazeichen mit einer speziellen Bedeutung oder ein reguläres Zeichen mit einer wörtlichen Bedeutung ist. Diese Zeichen und Metazeichen identifizieren ein Muster, das für die Suche nach Text verwendet werden kann. Wenn Sie beispielsweise nach Namen suchen möchten, können Sie einen regulären Ausdruck einrichten, um nach einem Muster zu suchen, das aus zwei aufeinander folgenden Wörtern besteht, die mit Großbuchstaben beginnen. Reguläre Ausdrücke sind ein leistungsstarkes Tool zum Suchen und Bearbeiten von Text.

Eine Diskussion über reguläre Ausdrücke würde den Rahmen dieses Artikels sprengen. Wir empfehlen die folgenden Ressourcen:

* Eine vollständige Liste der Metazeichen finden Sie unter [Reguläre Ausdrücke](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions) in MDN-Webdokumenten.
* Für ein Tutorial zum Erstellen regulärer Ausdrücke empfehlen wir [RegexOne](https://regexone.com/).
* Zum Experimentieren mit regulären Ausdrücken empfehlen wir die Website [Reguläre Ausdrücke 101](https://regex101.com/). Wählen Sie im linken Bedienfeld das ECMAScript (JavaScript)-FLAVOR aus.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Muster] </td> 
   <td> <p>Geben Sie das Muster für reguläre Ausdrücke ein. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span> <code>[+-]?(\d+(\.\d+)?|\.\d+)([eE][+-]?\d+)?</code> extrahiert alle Ziffern im angegebenen Text.</p> <p>Hinweis:  <p>Das Muster muss mindestens eine Erfassungsgruppe in Klammern <code>()</code>. Wenn das Muster keine Erfassungsgruppen enthält, ist das Ausgabepaket leer.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Globale Übereinstimmung]</td> 
   <td> <p>Aktivieren Sie diese Option, um alle Übereinstimmungen im Text abzurufen. Jede Übereinstimmung wird in einem separaten Bundle ausgegeben. Wenn diese Option deaktiviert ist, ruft das Modul nur den ersten Eintrag ab.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Groß-/Kleinschreibung beachten]</td> 
   <td> <p> Aktivieren Sie diese Einstellung, damit bei Text zwischen Groß- und Kleinschreibung unterschieden wird.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL multiline] </td> 
   <td> <p>Aktivieren Sie diese Option, um sicherzustellen, dass die Anfangs- und Endmetazeichen (<code>^</code> und <code>$</code>) mit dem Beginn oder Ende jeder Zeile übereinstimmen, nicht nur mit dem Anfang oder Ende der gesamten Eingabezeichenfolge.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL SingleLine]</td> 
   <td>Aktivieren Sie diese Option, um sicherzustellen, dass der Punkt (.) mit Zeilenumbruchzeichen (<code>\n</code>) übereinstimmt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Die Routenausführung auch dann fortsetzen, wenn das Modul keine Ergebnisse zurückgibt]</td> 
   <td> <p>Aktivieren Sie diese Option, um sicherzustellen, dass das Modul das Szenario nicht stoppt, wenn es keine Ergebnisse zurückgibt.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Text] </td> 
   <td> <p>Geben Sie den Text ein, der dem Muster entsprechen soll, oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ersetzen]

Durchsucht den eingegebenen Text nach einem angegebenen Wert oder regulären Ausdruck und ersetzt das Ergebnis durch den neuen Wert.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Muster] </td> 
   <td> <p>Geben Sie den Suchbegriff ein. Sie können auch einen regulären Ausdruck verwenden. Weitere Informationen zum regulären Ausdruck finden Sie im <a href="#match-pattern" class="MCXref xref">[!UICONTROL Match Pattern]</a>-Modul.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Neuer Wert]</td> 
   <td> <p> Geben Sie einen Wert ein, der den Suchbegriff ersetzt.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Globale Übereinstimmung]</td> 
   <td> <p>Aktivieren Sie diese Option, um alle Übereinstimmungen im Text abzurufen. Jede Übereinstimmung wird in einem separaten Bundle ausgegeben. Wenn diese Option deaktiviert ist, ruft das Modul nur den ersten Eintrag ab.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Groß-/Kleinschreibung beachten]</td> 
   <td> <p> Aktivieren Sie diese Einstellung, damit bei Text zwischen Groß- und Kleinschreibung unterschieden wird.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL multiline] </td> 
   <td> <p>Aktivieren Sie diese Option, um sicherzustellen, dass die Anfangs- und Endmetazeichen (<code>^</code> und <code>$</code>) mit dem Beginn oder Ende jeder Zeile übereinstimmen, nicht nur mit dem Anfang oder Ende der gesamten Eingabezeichenfolge.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL SingleLine]</td> 
   <td>Aktivieren Sie diese Option, um sicherzustellen, dass der Punkt (.) mit Zeilenumbruchzeichen (<code>\n</code>) übereinstimmt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Text] </td> 
   <td> <p>Geben Sie den zu suchenden Text ein.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Daten-Scraping

Beim Daten-Scraping (manchmal auch als Web-Scraping, Datenextraktion oder Web-Sammeln bezeichnet) werden Daten von Websites erfasst und in Ihrer lokalen Datenbank oder in Tabellen gespeichert. Wenn Sie Daten von einer Website kratzen möchten und mit regulären Ausdrücken nicht vertraut sind, können Sie ein Tool zum Kratzen von Daten verwenden.

Wenn das Tool zum Daten-Scraping eine REST-API bereitstellt, können Sie über unsere universellen [[!UICONTROL HTTP]-Module](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md) und [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md)-Module eine Verbindung herstellen.
