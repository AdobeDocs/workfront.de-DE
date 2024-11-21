---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: Text-Parser
description: Sie können das Text-Parser-Tool verwenden, um Text zur Verwendung in anderen [!DNL Adobe Workfront Fusion] Szenariomodulen zu analysieren. Der Text-Parser benötigt keine Verbindung.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d71cf64-4f86-42c5-81e7-8fc15333cbd7
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 0%

---

# [!UICONTROL Text parser]

Sie können das [!UICONTROL Text-Parser-Tool] verwenden, um Text zur Verwendung in anderen [!DNL Adobe Workfront Fusion] -Szenariomodulen zu analysieren. Der [!UICONTROL Text-Parser] benötigt keine Verbindung.

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
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
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

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Informationen zur Text Parser-API

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

## [!UICONTROL Text parser] -Module und ihre Felder

Wenn Sie die Module [!UICONTROL Text parser] konfigurieren, zeigt [!DNL Adobe Workfront Fusion] die unten aufgeführten Felder an. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Transformatoren

* [[!UICONTROL Abrufen von Elementen von HTML]](#get-elements-from-html)
* [[!UICONTROL Abrufen von Elementen aus Text]](#get-elements-from-text)
* [[!UICONTROL HTML zu Text]](#html-to-text)
* [[!UICONTROL Übereinstimmungsmuster]](#match-pattern)
* [[!UICONTROL Replace]](#replace)

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

#### [!UICONTROL Abrufen von Elementen aus Text]

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

#### [!UICONTROL HTML zu Text]

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
   <td> <p>Wählen Sie den Typ des Zeilenumbruchs aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Überschriften in Großbuchstaben]</p> </td> 
   <td> <p>Aktivieren Sie diese Option, um in Überschriften-Tags eingeschlossenen Text (z. B. &lt;h2&gt; &lt;/h2&gt;) in Großbuchstaben zu konvertieren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Übereinstimmungsmuster]

Mit dem Modul [!UICONTROL Match pattern] können Sie Zeichenfolgenelemente finden und extrahieren, die mit einem Suchmuster aus einem bestimmten Text übereinstimmen. Dieses Modul verwendet reguläre Ausdrücke (auch als regex oder regexp bezeichnet).

Ein regulärer Ausdruck ist eine Folge von Zeichen, bei denen jedes Zeichen ein Metazeichen mit einer besonderen Bedeutung oder ein reguläres Zeichen mit einer literalen Bedeutung ist. Diese Zeichen und Metazeichen identifizieren ein Muster, das für die Suche nach Text verwendet werden kann. Wenn Sie beispielsweise nach Namen suchen möchten, können Sie einen regulären Ausdruck einrichten, um nach einem Muster zu suchen, das aus zwei aufeinander folgenden Wörtern besteht, die mit Großbuchstaben beginnen. Reguläre Ausdrücke sind ein leistungsstarkes Werkzeug zum Durchsuchen und Bearbeiten von Text.

Eine Diskussion über reguläre Ausdrücke geht über den Rahmen dieses Artikels hinaus. Wir empfehlen die folgenden Ressourcen:

* Die vollständige Liste der Metazeichen finden Sie unter [Reguläre Ausdrücke](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions) in den MDN-Webdocs.
* Für ein Tutorial zum Erstellen regulärer Ausdrücke empfehlen wir [RegexOne](https://regexone.com/).
* Für das Experimentieren mit regulären Ausdrücken empfehlen wir die Website [Reguläre Ausdrücke 101](https://regex101.com/) . Wählen Sie im linken Bereich den ECMAScript (JavaScript)-FLAVOR aus.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Muster] </td> 
   <td> <p>Geben Sie das Muster des regulären Ausdrucks ein. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span> <code>[+-]?(\d+(\.\d+)?|\.\d+)([eE][+-]?\d+)?</code> extrahiert alle Zahlen in den bereitgestellten Text.</p> <p>Hinweis:  <p>Das Muster sollte mindestens eine Erfassungsgruppe in Klammern <code>()</code> enthalten. Wenn das Muster keine Erfassungsgruppen enthält, ist das Ausgabebundle leer.</p> </p> </td> 
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
   <td> <p>Aktivieren Sie diese Option, um sicherzustellen, dass Start- und Endmetazeichen (<code>^</code> und <code>$</code>) mit dem Anfang oder Ende jeder Zeile übereinstimmen, und nicht nur mit dem Anfang oder Ende der gesamten Eingabezeichenfolge.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>Aktivieren Sie diese Option, um sicherzustellen, dass der Punkt (.) mit Zeilenumbruchzeichen (<code>\n</code>) übereinstimmt.</td> 
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

#### [!UICONTROL Replace]

Sucht den eingegebenen Text nach einem bestimmten Wert oder regulären Ausdruck und ersetzt das Ergebnis durch den neuen Wert.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Muster] </td> 
   <td> <p>Geben Sie den Suchbegriff ein. Sie können auch einen regulären Ausdruck verwenden. Weitere Informationen zum regulären Ausdruck finden Sie im Modul <a href="#match-pattern" class="MCXref xref">[!UICONTROL Übereinstimmungsmuster]</a> .</p> </td> 
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
   <td> <p>Aktivieren Sie diese Option, um sicherzustellen, dass Start- und Endmetazeichen (<code>^</code> und <code>$</code>) mit dem Anfang oder Ende jeder Zeile übereinstimmen, und nicht nur mit dem Anfang oder Ende der gesamten Eingabezeichenfolge.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>Aktivieren Sie diese Option, um sicherzustellen, dass der Punkt (.) mit Zeilenumbruchzeichen (<code>\n</code>) übereinstimmt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>Geben Sie den zu suchenden Text ein.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Datenauswertung

Beim Datenscraping, manchmal auch als Web-Scraping, Datenextraktion oder Webernte bezeichnet, werden Daten von Websites erfasst und in Ihrer lokalen Datenbank oder in Tabellen gespeichert. Wenn Sie Daten von einer Website löschen möchten und Sie nicht mit regulären Ausdrücken vertraut sind, können Sie ein Tool zum Scraping von Daten verwenden.

Wenn das Daten-Scraping-Tool eine REST-API bereitstellt, können Sie über unsere universellen [[!UICONTROL HTTP]-Module](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md) und [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md) eine Verbindung mit ihr herstellen.
