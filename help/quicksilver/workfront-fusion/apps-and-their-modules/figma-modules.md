---
filename: figma-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Bildmodule
description: 'Mit dem [!DNL Adobe Workfront Fusion] Bildmodule: Sie können Listen mit Kommentaren, Dateien, Dateiversionen oder Projekten abrufen. Sie können auch einen Kommentar posten oder einen Aufruf an die Figma-API richten.'
author: Becky
exl-id: d88db592-32d4-4765-952f-9ffb58cf1720
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2261'
ht-degree: 1%

---

# [!DNL Figma] Module

Mit dem [!DNL Adobe Workfront Fusion] [!DNL Figma] -Module können Sie Listen mit Kommentaren, Dateien, Dateiversionen oder Projekten abrufen. Sie können auch einen Kommentar posten oder einen Aufruf an die [!DNL Figma] API.

Informationen zum Erstellen eines Szenarios finden Sie unter [Erstellen eines Szenarios](../../workfront-fusion/scenarios/create-a-scenario.md).

Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] Plan*</td>
      <td>
        <p>[!UICONTROL Pro] oder höher</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] license*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td>
      <td >
        <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Produkt</td>
      <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td>
    </tr>
  </tbody>
</table>


Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Verwendung [!DNL Figma] -Module, müssen Sie über eine [!DNL Figma] -Konto.

## [!DNL Figma] Module und ihre Felder

Bei der Konfiguration [!DNL Figma] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Figma] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Kommentare](#comments)

* [Projekte und Dateien](#projects-and-files)

* [Komponenten und Stile](#components-and-styles)

* [Sonstige](#other)


### Kommentare

* [Löschen von Kommentaren](#delete-a-comment)

* [Kommentare auflisten](#list-comments)

* [Posten eines Kommentars](#post-a-comment)


#### [!UICONTROL Löschen von Kommentaren]

Dieses Aktionsmodul löscht einen einzelnen Kommentar aus einer Datei.

<table style="table-layout:auto"> 
  <col/>
  <col />
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td> <p>Anweisungen zum Verbinden der [!DNL Figma] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen.</a></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datei-ID]</td>
      <td>Geben Sie die Datei-ID der Datei ein oder ordnen Sie sie zu, aus der Sie einen Kommentar löschen möchten. </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Kommentar]</td>
      <td>Geben Sie den Text des Kommentars ein, den Sie löschen möchten.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Kommentare auflisten]

Dieses Suchmodul listet alle Kommentare auf, die an eine einzelne Datei in [!DNL Figma].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td> <p>Anweisungen zum Verbinden der [!DNL Figma] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datei-ID]</td>
      <td>
        <p>Geben Sie die Datei-ID der Datei ein oder ordnen Sie sie zu, für die Sie Kommentare abrufen möchten. </p>
        <ul>
          <li>
            <p>Wenn Sie die ID nicht kennen, klicken Sie auf <b>[!UICONTROL Dateien suchen]</b> und geben Sie die Kennung des Projekts ein, mit dem die Datei verknüpft ist, oder ordnen Sie sie zu. Wählen Sie dann die Datei aus.</p>
          </li>
          <li>
            <p>Wenn Sie die Kennung des Projekts nicht kennen, klicken Sie auf <b>[!UICONTROL Projekte suchen]</b> und geben Sie die Kennung des Teams ein, dem die Datei gehört, oder ordnen Sie sie zu. Wählen Sie dann das Projekt aus und wählen Sie die Datei aus.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Geben Sie die maximale Anzahl von Kommentaren ein oder ordnen Sie sie zu, die das Modul während der Ausführung jedes Szenarios zurückgeben soll.</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL Posten eines Kommentars]

Dieses Aktionsmodul sendet einen Kommentar in eine Figma-Datei.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td> <p>Anweisungen zum Verbinden der [!DNL Figma] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen.</a></p>
    </tr>
    <tr>
      <td  role="rowheader">[!UICONTROL Datei-ID]</td>
      <td>
        <p>Geben Sie die Datei-ID der Datei ein oder ordnen Sie sie zu, an die Sie einen Kommentar posten möchten. </p>
        <ul>
          <li>
            <p>Wenn Sie die Kennung der Datei nicht kennen, klicken Sie auf <b>[!UICONTROL Dateien suchen]</b> und geben Sie die Kennung des Projekts ein, mit dem die Datei verknüpft ist, oder ordnen Sie sie zu. Wählen Sie dann die Datei aus.</p>
          </li>
          <li>
            <p>Wenn Sie versuchen, die Kennung der Datei zu finden und die Kennung des Projekts nicht kennen, klicken Sie auf <b>[!UICONTROL Projekte suchen]</b> und geben Sie die Kennung des Teams ein, dem das Projekt gehört, mit dem die Datei verknüpft ist, oder ordnen Sie sie zu. Wählen Sie das Projekt aus und wählen Sie dann die Datei aus.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Kommentar]</td>
      <td>Geben Sie den Text des Kommentars ein.</td>
    </tr>
  </tbody>
</table>


### Projekte und Dateien

* [Datei oder Bild abrufen](#get-a-file-or-image)

* [Verlauf der Dateiversionen auflisten](#list-file-version-history)

* [Projektdateien auflisten](#list-project-files)

* [Auflisten von Projekten](#list-projects)


#### [!UICONTROL Datei oder Bild abrufen]

Dieses Aktionsmodul ruft eine einzelne Datei oder ein Bild aus einer Figma-Bibliothek ab

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td> <p>Anweisungen zum Verbinden der [!DNL Figma] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Objekttyp]</td>
      <td>
        <p>Wählen Sie den Objekttyp aus, den Sie abrufen möchten.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Datei]</b>
            </p>
            <p>Das Modul gibt das Dokument zurück, auf das [!UICONTROL Key] verweist, als JSON-Objekt. Der Dateischlüssel kann von jeder beliebigen Figma-Datei-URL geparst werden.</p>
            <p>Informationen zu Feldern finden Sie unter <a href="#Get2" class="MCXref xref" >[!UICONTROL Datei oder Bild abrufen: Datei]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Dateiknoten]</b>
            </p>
            <p>Gibt die Knoten zurück, auf die durch IDs als JSON-Objekt verwiesen wird. Die Knoten werden aus dem [!DNL Figma] -Datei referenziert durch [!UICONTROL Key].</p>
            <p>Informationen zu Feldern finden Sie unter <a href="#Get3" class="MCXref xref" >[!UICONTROL Datei oder Bild abrufen: Dateiknoten]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Bild]</b>
            </p>
            <p>Das Modul rendert Bilder aus einer Datei.</p>
            <p>Informationen zu Feldern finden Sie unter <a href="#Get4" class="MCXref xref" >[!UICONTROL Datei oder Bild abrufen: Bild]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Bilddateien]</b>
            </p>
            <p>Das Modul gibt Downloadlinks für alle Bilder zurück, die in Bilddateien in einem Dokument vorhanden sind. Bildbearbeitung [!DNL Figma] stellt alle vom Benutzer bereitgestellten Bilder dar. Wenn Sie ein Bild in [!DNL Figma], [!DNL Figma] erstellt ein Rechteck mit einer einzelnen Füllung, die das Bild darstellt, und der Benutzer kann das Rechteck (und die Eigenschaften auf der Füllung) transformieren.</p>
            <p>Informationen zu Feldern finden Sie unter <a href="#Get5" class="MCXref xref" >[!UICONTROL Datei oder Bild abrufen: Bildfüllungen]</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL Datei oder Bild abrufen: Datei]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Dateischlüssel]</td>
      <td>Wählen Sie die Datei aus, von der Sie JSON zurückgeben möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Version-ID]</td>
      <td>Geben Sie die Version der Datei ein, die das Modul zurückgeben soll, oder ordnen Sie sie zu. Lassen Sie dieses Feld für das aktuelle Modul leer.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Knoten-IDs]</td>
      <td>
        <p>Um nur eine Teilmenge des Dokuments zurückzugeben, geben Sie die Knoten ein, die das Modul zurückgeben soll. Das Modul gibt die aufgelisteten Knoten, ihre untergeordneten Elemente und alles zwischen dem Stammknoten und den aufgelisteten Knoten zurück.</p>
        <p>Klicken Sie für jeden Knoten, den Sie zurückgeben möchten, auf <b>[!UICONTROL Hinzufügen]</b> und geben Sie den Text des Knotens ein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tiefe]</td>
      <td>
        <p>Geben Sie eine Ganzzahl ein oder ordnen Sie sie zu, die angibt, wie tief in die Dokumentstruktur Sie Ergebnisse zurückgeben möchten. </p>
        <div class="example"><span class="autonumber"><span><b>Beispiel: </b></span></span>
          <ul>
            <li>
              <p>Geben Sie nur zur Rückgabe von Seiten ein. <code>1</code>.</p>
            </li>
            <li>
              <p>Um Seiten und Objekte der obersten Ebene zurückzugeben, geben Sie <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>Um alle Knoten zurückzugeben, lassen Sie dieses Feld leer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Geometry]</td>
      <td>Um Vektordaten zurückzugeben, geben Sie <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Plugin data]</td>
      <td>Eine kommagetrennte Liste mit Plug-in-IDs und/oder der Zeichenfolge "[!UICONTROL shared]". Alle Daten, die im Dokument vorhanden sind, das von diesen Plug-ins geschrieben wurde, werden in das Ergebnis in <code>pluginData</code> und <code>sharedPluginData</code> Eigenschaften.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Verzweigungsdaten]</td>
      <td>Aktivieren Sie diese Option, um Verzweigungsmetadaten für die angeforderte Datei zurückzugeben. Wenn es sich bei der Datei um einen Zweig handelt, wird der Schlüssel der Hauptdatei in die zurückgegebene Antwort aufgenommen. Wenn die Datei Verzweigungen enthält, werden ihre Metadaten in die zurückgegebene Antwort aufgenommen. Standard: <code>false</code>.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Datei oder Bild abrufen: Dateiknoten]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Dateischlüssel]</td>
      <td>Wählen Sie die Datei aus, von der Sie JSON zurückgeben möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Knoten-IDs]</td>
      <td>
        <p>Geben Sie die Knoten ein, die das Modul zurückgeben und konvertieren soll</p>
        <p>Klicken Sie für jeden Knoten, den Sie zurückgeben möchten, auf <b>[!UICONTROL Hinzufügen]</b> und geben Sie den Text des Knotens ein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Version-ID]</td>
      <td>Geben Sie die Version der Datei ein, die das Modul zurückgeben soll, oder ordnen Sie sie zu. Lassen Sie dieses Feld für das aktuelle Modul leer.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tiefe]</td>
      <td>
        <p>Geben Sie eine Ganzzahl ein oder ordnen Sie sie zu, die angibt, wie tief in die Dokumentstruktur Sie Ergebnisse zurückgeben möchten. </p>
        <div class="example"><span class="autonumber"><span><b>Beispiel: </b></span></span>
          <ul>
            <li>
              <p>Geben Sie nur zur Rückgabe von Seiten ein. <code>1</code>.</p>
            </li>
            <li>
              <p>Um Seiten und Objekte der obersten Ebene zurückzugeben, geben Sie <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>Um alle Knoten zurückzugeben, lassen Sie dieses Feld leer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Geometry]</td>
      <td>Um Vektordaten zurückzugeben, geben Sie <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Plugin data]</td>
      <td>Eine kommagetrennte Liste mit Plug-in-IDs und/oder der Zeichenfolge "shared". Alle Daten, die im Dokument vorhanden sind, das von diesen Plug-ins geschrieben wurde, werden in das Ergebnis in den Eigenschaften pluginData und sharedPluginData aufgenommen.</td>
    </tr>
  </tbody>
</table>


##### Datei oder Bild abrufen: Bild

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Dateischlüssel]</td>
      <td>Wählen Sie die Datei aus, von der Sie JSON zurückgeben möchten.</td>
    </tr>
    <tr>
      <td role="rowheader" [!UICONTROL>Knoten-IDs]</td>
      <td>
        <p>Geben Sie die Knoten ein, die das Modul rendern soll.</p>
        <p>Klicken Sie für jeden Knoten, den Sie rendern möchten, auf <b>[!UICONTROL Hinzufügen]</b> und geben Sie den Text des Knotens ein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Skala]</td>
      <td>Um das Bild zu skalieren, geben Sie den Skalierungsfaktor ein oder ordnen Sie ihn zu. Diese Zahl muss zwischen 0,01 und 4 liegen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Format]</td>
      <td>
        <p>Wählen Sie das Format für die Bildausgabe aus.</p>
        <ul>
          <li>
            <p>JPG</p>
          </li>
          <li>
            <p>PNG</p>
          </li>
          <li>
            <p>SVG</p>
          </li>
          <li>
            <p>PDF</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SVG - Einschluss-ID]</td>
      <td>Aktivieren Sie diese Option, um ID-Attribute für alle SVG-Elemente einzuschließen. Standard: [!UICONTROL false].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SVG - Simplify Stroke]</td>
      <td>Aktivieren Sie diese Option, um Innen-/Außenstriche zu vereinfachen, und verwenden Sie nach Möglichkeit anstelle von &lt;mask&gt;. Standard: [!UICONTROL true].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Absolute Grenzen verwenden]</td>
      <td>Aktivieren Sie diese Option, um die vollständigen Dimensionen des Knotens zu verwenden, unabhängig davon, ob der Knoten beschnitten oder der Leerraum um ihn herum leer ist. Verwenden Sie dies, um Textknoten ohne Zuschneiden zu exportieren. Standard: [!UICONTROL false].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Version-ID]</td>
      <td>Geben Sie die Version der Datei ein, die das Modul zurückgeben soll, oder ordnen Sie sie zu. Lassen Sie dieses Feld für das aktuelle Modul leer.</td>
    </tr>
  </tbody>
</table>

##### Datei oder Bild abrufen: Bildfüllungen

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Dateischlüssel]</td>
      <td>Wählen Sie die Datei aus, von der Sie JSON zurückgeben möchten.</td>
    </tr>
  </tbody>
</table>

### [!UICONTROL Verlauf der Dateiversionen auflisten]

Dieses Suchmodul gibt den Versionsverlauf einer einzelnen Datei in [!UICONTROL Figma].
<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td> <p>Anweisungen zum Verbinden der [!DNL Figma] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen.</a></p>
    <tr>
      <td role="rowheader">[!UICONTROL Datei-ID]</td>
      <td>
        <p>Geben Sie die Datei-ID der Datei ein oder ordnen Sie sie zu, für die Sie den Versionsverlauf abrufen möchten. </p>
        <ul>
          <li>
            <p>Wenn Sie die Kennung der Datei nicht kennen, klicken Sie auf <b>[!UICONTROL Dateien suchen]</b> und geben Sie die Kennung des Projekts ein, mit dem die Datei verknüpft ist, oder ordnen Sie sie zu. Wählen Sie dann die Datei aus.</p>
          </li>
          <li>
            <p>Wenn Sie versuchen, die Kennung der Datei zu finden und die Kennung des Projekts nicht kennen, klicken Sie auf <b>[!UICONTROL Projekte suchen]</b> und geben Sie die Kennung des Teams ein, dem das Projekt gehört, mit dem die Datei verknüpft ist, oder ordnen Sie sie zu. Wählen Sie das Projekt aus und wählen Sie dann die Datei aus.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Projektdateien auflisten]

Dieses Suchmodul gibt eine Liste aller Dateien im angegebenen Projekt zurück.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td> <p>Anweisungen zum Verbinden der [!DNL Figma] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datei-ID]</td>
      <td>
        <p>Geben Sie die Projekt-ID ein oder ordnen Sie sie dem Projekt zu, für das Sie Dateien abrufen möchten. </p>
        <ul>
          <li>
            <p>Wenn Sie die Kennung des Projekts nicht kennen, klicken Sie auf <b>[!UICONTROL Projekte suchen]</b> und geben Sie die Kennung des Teams ein, mit dem das Projekt verknüpft ist, oder ordnen Sie sie zu. Wählen Sie dann das Projekt aus.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Auflisten von Projekten]

Dieses Suchmodul gibt eine Liste aller Projekte innerhalb des angegebenen Teams zurück.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td> <p>Anweisungen zum Verbinden der [!DNL Figma] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Team ID]</td>
      <td>Geben Sie die Projekt-ID des Projekts ein oder ordnen Sie sie zu, für das Sie Dateien abrufen möchten. Die Team-ID finden Sie auf der URL der Team-Seite in Figma .</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td>
    </tr>
  </tbody>
</table>


### Komponenten und Stile

#### [!UICONTROL Abrufen eines Stils oder einer Komponente]

Dieses Aktionsmodul ruft einen einzelnen Stil oder eine einzelne Komponente oder einen Satz von Stilen oder Komponenten ab.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td> <p>Anweisungen zum Verbinden der [!DNL Figma] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen.</a></p>
    </tr>
    <tr>
      <td role="rowheader">&lt;[!UICONTROL Objekt&gt; Schlüssel]</td>
      <td>Geben Sie den Schlüssel (die eindeutige Kennung) des Objekts ein, das Sie abrufen möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Team ID]</td>
      <td>Geben Sie die Kennung des Teams ein oder ordnen Sie sie zu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Seitengröße]</td>
      <td>Geben Sie die Zahl oder die Ergebnisse ein, die pro Seite zurückgegeben werden sollen, oder ordnen Sie sie zu. Standard: 30.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nach]</td>
      <td>
        <p>Geben Sie die Anzahl der Ergebnisse ein oder ordnen Sie sie zu, nach denen die Ergebnisse abgerufen werden sollen. Dies kann mit dem Feld [!UICONTROL Seitengröße] kombiniert werden, um Ergebnisse zu paginieren.</p>
        <p>Dieser Wert entspricht nicht Objekt-IDs.</p>
        <p>Dieses Feld kann nicht zusammen mit dem Feld [!UICONTROL Before] verwendet werden.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Before]</td>
      <td>
        <p>Geben Sie die Anzahl der Ergebnisse ein oder ordnen Sie sie zu, bevor Sie mit dem Abrufen der Ergebnisse beginnen. Dies kann mit dem Feld [!UICONTROL Seitengröße] kombiniert werden, um Ergebnisse zu paginieren.</p>
        <p>Dieser Wert entspricht nicht Objekt-IDs.</p>
        <p>Dieses Feld kann nicht in Kombination mit dem Feld [!UICONTROL Nach] verwendet werden.</p>
      </td>
    </tr>
  </tbody>
</table>


### Sonstige

* [API-Aufruf](#make-an-api-call)

* [Ereignisse beobachten](#watch-events)


#### [!UICONTROL API-Aufruf]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die Figma-API ausführen, ohne die Authentifizierung durchführen zu müssen. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von anderen Figma-Modulen nicht erreicht werden kann.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td> <p>Anweisungen zum Verbinden der [!DNL Figma] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Geben Sie einen Pfad relativ zu ein <code>https://api.figma.com/v1/</code>.</p>
        <p>Beispiel: <code>[!DNL files/7179110/comments]</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Methode]</td>
      <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Header]</td>
      <td>
        <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p>
        <p>Beispiel: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] fügt die Autorisierungskopfzeilen für Sie hinzu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td>
      <td>
        <p>Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p>
        <p>Beispiel: <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Notiz:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> Fügen Sie die Anführungszeichen in Ihre JSON-Datei außerhalb der bedingten Anweisung ein.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Ereignisse beobachten]

Dieses Trigger-Modul startet ein Szenario, wenn eines der folgenden Ereignisse für ein bestimmtes Team in Ihrer [!DNL Figma] Teamraum

* Dateiaktualisierung

* Aktualisierung der Dateiversion

* Datei löschen

* Bibliotheksveröffentlichung

* Dateikommentar

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>
        <p>Wählen Sie den Webhook aus, den das Modul überwacht.</p>
        <p>So fügen Sie einen neuen Webhook hinzu:</p>
        <ol>
          <li value="1">
            <p>Klicken <b>[!UICONTROL Hinzufügen]</b> neben dem Feld [!UICONTROL Webhook] .</p>
          </li>
          <li value="2">
            <p>Wählen Sie die Verbindung aus, die Sie für diesen Webhook verwenden möchten. Anweisungen zum Verbinden der [!DNL Figma] Konto für [!UICONTROL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!UICONTROL Adobe Workfront Fusion] - Grundlegende Anweisungen.</a></p>
          </li>
          <li value="3">
            <p>Wählen Sie den Ereignistyp aus, den das Modul überwachen soll.</p>
          </li>
          <li value="4">
            <p>Geben Sie die Kennung des Teams ein, dessen Ereignisse der Webhook überwachen soll.</p>
          </li>
          <li value="5">
            <p>Geben Sie den [!UICONTROL Status] oder die [!UICONTROL Beschreibung] der Ereignisse ein, die der Webhook sehen soll.</p>
          </li>
          <li value="6">
            <p>Klicken <b>[!UICONTROL Save]</b> , um den Webhook zu speichern und zum Modul zurückzukehren.</p>
          </li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>
