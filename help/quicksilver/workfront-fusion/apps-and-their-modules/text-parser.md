---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: Text-Parser
description: Sie können das Text-Parser-Tool verwenden, um Text zur Verwendung in anderen zu analysieren [!DNL Adobe Workfront Fusion] Szenario-Module. Der Text-Parser benötigt keine Verbindung.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d71cf64-4f86-42c5-81e7-8fc15333cbd7
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1010'
ht-degree: 0%

---

# [!UICONTROL Text-Parser]

Sie können die [!UICONTROL Textparser-Tool] , um Text zur Verwendung in anderen zu analysieren [!DNL Adobe Workfront Fusion] Szenario-Module. Die [!UICONTROL Text-Parser] erfordert keine Verbindung.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p> <p>[!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Text-Parser] Module und ihre Felder

Bei der Konfiguration [!UICONTROL Text-Parser] Module, [!DNL Adobe Workfront Fusion] zeigt die unten aufgeführten Felder an. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Transformatoren

* [[!UICONTROL Abrufen von Elementen von HTML]](#get-elements-from-html)
* [[!UICONTROL Elemente aus Text abrufen]](#get-elements-from-text)
* [[!UICONTROL HTML in Text]](#html-to-text)
* [[!UICONTROL Übereinstimmungsmuster]](#match-pattern)
* [[!UICONTROL Ersetzen]](#replace)

#### [!UICONTROL Abrufen von Elementen von HTML]

Ruft die gewünschten Elemente aus dem HTML-Code ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Fortfahren der Routenausführung, selbst wenn das Modul keine Treffer findet]</td> 
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
   <td> <p>Geben Sie den HTML-Code ein oder ordnen Sie ihn zu, aus dem Sie die angegebenen Elementtypen abrufen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elemente aus Text abrufen]

Analysiert Elemente aus Text basierend auf dem angegebenen Muster.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Eingabetext]</td> 
   <td> <p>Geben Sie den Text ein oder ordnen Sie ihn zu, den Sie analysieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Muster]</td> 
   <td> <p>Wählen Sie das Muster aus, das die Elemente widerspiegelt, die Sie aus dem Text analysieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Doppelte Vorfälle ignorieren]</td> 
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
   <td> <p>Wählen Sie den Typ des Zeilenumbruchs (Zeilenumbruch) aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Überschriften in Großbuchstaben]</p> </td> 
   <td> <p>Aktivieren Sie diese Option, um in Überschriften-Tags eingeschlossenen Text zu konvertieren (z. B. &lt;h2&gt; &lt;/h2&gt;) in Text in Großbuchstaben.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Übereinstimmungsmuster]

Die [!UICONTROL Übereinstimmungsmuster] -Modul ermöglicht es Ihnen, aus einem bestimmten Text Textelemente zu finden und zu extrahieren, die einem Suchmuster entsprechen. Dieses Modul verwendet reguläre Ausdrücke (auch als regex oder regexp bezeichnet).

Ein regulärer Ausdruck ist eine Folge von Zeichen, bei denen jedes Zeichen ein Metazeichen mit einer besonderen Bedeutung oder ein reguläres Zeichen mit einer literalen Bedeutung ist. Diese Zeichen und Metazeichen identifizieren ein Muster, das für die Suche nach Text verwendet werden kann. Wenn Sie beispielsweise nach Namen suchen möchten, können Sie einen regulären Ausdruck einrichten, um nach einem Muster zu suchen, das aus zwei aufeinander folgenden Wörtern besteht, die mit Großbuchstaben beginnen. Reguläre Ausdrücke sind ein leistungsstarkes Werkzeug zum Durchsuchen und Bearbeiten von Text.

Eine Diskussion über reguläre Ausdrücke geht über den Rahmen dieses Artikels hinaus. Wir empfehlen die folgenden Ressourcen:

* Eine vollständige Liste der Metazeichen finden Sie unter [Reguläre Ausdrücke](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions) in MDN-Webdocs.
* Für ein Tutorial zum Erstellen regulärer Ausdrücke empfehlen wir, [RegexOne](https://regexone.com/).
* Für das Experimentieren mit regulären Ausdrücken empfehlen wir die [Reguläre Ausdrücke 101](https://regex101.com/) Website. Wählen Sie im linken Bereich den ECMAScript (JavaScript)-FLAVOR aus.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Muster] </td> 
   <td> <p>Geben Sie das Muster des regulären Ausdrucks ein. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span> <code>[+-]?(\d+(\.\d+)?|\.\d+)([eE][+-]?\d+)?</code> extrahiert alle Zahlen im angegebenen Text.</p> <p>Notiz:  <p>Das Muster sollte mindestens eine Erfassungsgruppe in Klammern enthalten <code>()</code>. Wenn das Muster keine Erfassungsgruppen enthält, ist das Ausgabebundle leer.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Globale Übereinstimmung]</td> 
   <td> <p>Aktivieren Sie diese Option, um alle Übereinstimmungen im Text abzurufen. Jede Übereinstimmung wird in einem separaten Bundle ausgegeben. Wenn diese Option deaktiviert ist, ruft das Modul nur den ersten Eintrag ab.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Groß- und Kleinschreibung beachten]</td> 
   <td> <p> Aktivieren Sie diese Option, damit dieses Modul Text als Groß-/Kleinschreibung behandelt.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>Aktivieren Sie diese Option, um sicherzustellen, dass Anfangs- und Endmetazeichen (<code>^</code> und <code>$</code>) entspricht dem Anfang oder Ende jeder Zeile, nicht nur dem Anfang oder Ende der gesamten Eingabe-Zeichenfolge.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>Aktivieren Sie diese Option, um sicherzustellen, dass der Punkt (.) entspricht Zeilenumbruchzeichen (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fortfahren der Routenausführung, selbst wenn das Modul keine Ergebnisse zurückgibt]</td> 
   <td> <p>Aktivieren Sie diese Option, um sicherzustellen, dass das Modul das Szenario nicht stoppt, wenn es keine Ergebnisse zurückgibt.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>Geben Sie den Text ein oder ordnen Sie ihn dem Muster zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ersetzen]

Sucht den eingegebenen Text nach einem bestimmten Wert oder regulären Ausdruck und ersetzt das Ergebnis durch den neuen Wert.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Muster] </td> 
   <td> <p>Geben Sie den Suchbegriff ein. Sie können auch einen regulären Ausdruck verwenden. Weitere Informationen zum regulären Ausdruck finden Sie im Abschnitt <a href="#match-pattern" class="MCXref xref">[!UICONTROL Übereinstimmungsmuster]</a> -Modul.</p> </td> 
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
   <td>[!UICONTROL Groß- und Kleinschreibung beachten]</td> 
   <td> <p> Aktivieren Sie diese Option, damit dieses Modul Text als Groß-/Kleinschreibung behandelt.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>Aktivieren Sie diese Option, um sicherzustellen, dass Anfangs- und Endmetazeichen (<code>^</code> und <code>$</code>) entspricht dem Anfang oder Ende jeder Zeile, nicht nur dem Anfang oder Ende der gesamten Eingabe-Zeichenfolge.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>Aktivieren Sie diese Option, um sicherzustellen, dass der Punkt (.) entspricht Zeilenumbruchzeichen (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>Geben Sie den zu suchenden Text ein.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Datenauswertung

Beim Datenscraping, manchmal auch als Web-Scraping, Datenextraktion oder Webernte bezeichnet, werden Daten von Websites erfasst und in Ihrer lokalen Datenbank oder in Tabellen gespeichert. Wenn Sie Daten von einer Website löschen möchten und Sie nicht mit regulären Ausdrücken vertraut sind, können Sie ein Tool zum Datenscraping verwenden:

* [Apify](https://apify.com/)
* [Best Data Scraping Tools für 2019](https://www.octoparse.com/blog/best-data-scraping-tools-for-2019-top-10-reviews)

Wenn das Daten-Scraping-Tool eine REST-API bereitstellt, können Sie über unsere universelle [[!UICONTROL HTTP] Module](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md) und [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md) Module.
