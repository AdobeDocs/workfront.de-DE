---
filename: figma-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Figma-Module
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: d88db592-32d4-4765-952f-9ffb58cf1720
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '2375'
ht-degree: 0%

---

# [!DNL Figma] Module

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [FIGMA-Module](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/figma-modules.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Mit den [!DNL Adobe Workfront Fusion] [!DNL Figma] können Sie Listen von Kommentaren, Dateien, Dateiversionen oder Projekten abrufen. Sie können auch einen Kommentar posten oder einen Aufruf an die [!DNL Figma]-API durchführen.

Anweisungen zum Erstellen eines Szenarios finden Sie unter [Erstellen eines Szenarios](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

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
      <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td>
      <td>
        <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p>
      </td>
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

Um [!DNL Figma]-Module verwenden zu können, müssen Sie über ein [!DNL Figma]-Konto verfügen.

## Figma API-Informationen

Der Figma-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Basis-URL</td> 
   <td> https://api.figma.com/v1</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Version</td> 
   <td> v1 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v1.8.25</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Figma] Module und ihre Felder

Beim Konfigurieren [!DNL Figma] Module zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder dem Service weitere [!DNL Figma] angezeigt werden. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Kommentare](#comments)

* [Projekte und Dateien](#projects-and-files)

* [Komponenten und Stile](#components-and-styles)

* [Sonstige](#other)


### Kommentare

* [Kommentar löschen](#delete-a-comment)

* [Kommentare auflisten](#list-comments)

* [Kommentar posten](#post-a-comment)


#### [!UICONTROL Kommentar löschen]

Dieses Aktionsmodul löscht einen einzelnen Kommentar aus einer Datei.

<table style="table-layout:auto"> 
  <col/>
  <col />
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td> <p>Anweisungen zum Verbinden Ihres [!DNL Figma]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen.</a></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datei-ID]</td>
      <td>Geben Sie die Datei-ID der Datei ein, zu der Sie einen Kommentar hinzufügen möchten, oder mappen Sie sie. </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL-Kommentar]</td>
      <td>Geben Sie den Text des Kommentars ein, den Sie löschen möchten.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Kommentare auflisten]

Dieses Suchmodul listet alle Kommentare auf, die an eine einzelne Datei in [!DNL Figma] angehängt sind.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td> <p>Anweisungen zum Verbinden Ihres [!DNL Figma]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datei-ID]</td>
      <td>
        <p>Geben Sie die Datei-ID der Datei ein, für die Sie Kommentare abrufen möchten, oder mappen Sie sie. </p>
        <ul>
          <li>
            <p>Wenn Sie die ID nicht kennen, klicken Sie auf <b>[!UICONTROL Dateien suchen]</b> und geben Sie die ID des Projekts, mit dem die Datei verknüpft ist, ein oder mappen Sie sie. Wählen Sie dann die Datei aus.</p>
          </li>
          <li>
            <p>Wenn Sie die Projekt-ID nicht kennen, klicken Sie auf <b>[!UICONTROL Projekte suchen]</b> und geben Sie die ID des Teams ein, dem das Projekt gehört, dem die Datei zugeordnet ist, oder mappen Sie sie. Wählen Sie dann das Projekt aus und wählen Sie die Datei aus.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Geben Sie die maximale Anzahl von Kommentaren ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL Kommentar posten]

Dieses Aktionsmodul postet einen Kommentar in eine Figma-Datei.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td> <p>Anweisungen zum Verbinden Ihres [!DNL Figma]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen.</a></p>
    </tr>
    <tr>
      <td  role="rowheader">[!UICONTROL Datei-ID]</td>
      <td>
        <p>Geben Sie die Datei-ID der Datei ein, an die Sie einen Kommentar senden möchten, oder mappen Sie sie. </p>
        <ul>
          <li>
            <p>Wenn Sie die Datei-ID nicht kennen, klicken Sie auf <b>[!UICONTROL Dateien suchen]</b> und geben Sie die ID des Projekts, mit dem die Datei verknüpft ist, ein oder mappen Sie sie. Wählen Sie dann die Datei aus.</p>
          </li>
          <li>
            <p>Wenn Sie versuchen, die Datei-ID zu finden und die Projekt-ID nicht kennen, klicken Sie auf <b>[!UICONTROL Projekte suchen]</b> und geben Sie die ID des Teams ein, dem das Projekt gehört, dem die Datei zugeordnet ist, oder ordnen Sie sie zu. Wählen Sie das Projekt und dann die Datei aus.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL-Kommentar]</td>
      <td>Geben Sie den Text des Kommentars ein.</td>
    </tr>
  </tbody>
</table>


### Projekte und Dateien

* [Datei oder Bild abrufen](#get-a-file-or-image)

* [Dateiversionsverlauf auflisten](#list-file-version-history)

* [Projektdateien auflisten](#list-project-files)

* [Auflisten von Projekten](#list-projects)


#### [!UICONTROL Datei oder Bild abrufen]

Dieses Aktionsmodul ruft eine einzelne Datei oder ein einzelnes Bild aus einer Figmabibliothek ab

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td> <p>Anweisungen zum Verbinden Ihres [!DNL Figma]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Objekttyp]</td>
      <td>
        <p>Wählen Sie den Typ des Objekts aus, das Sie abrufen möchten.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL-Datei]</b>
            </p>
            <p>Das Modul gibt das Dokument zurück, auf das [!UICONTROL Key] als JSON-Objekt verweist. Der Dateischlüssel kann aus einer beliebigen Figmadatei-URL geparst werden.</p>
            <p>Felder finden Sie unter <a href="#Get2" class="MCXref xref" >[!UICONTROL Datei oder Bild abrufen: Datei]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL-Dateiknoten]</b>
            </p>
            <p>Gibt die Knoten zurück, auf die von IDs als JSON-Objekt verwiesen wird. Die Knoten werden aus der [!DNL Figma]-Datei abgerufen, auf die der [!UICONTROL-Schlüssel] verweist.</p>
            <p>Felder finden Sie unter <a href="#Get3" class="MCXref xref" >[!UICONTROL Datei oder Bild abrufen: Dateiknoten]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL image]</b>
            </p>
            <p>Das Modul rendert Bilder aus einer -Datei.</p>
            <p>Felder finden Sie unter <a href="#Get4" class="MCXref xref" >[!UICONTROL Datei oder Bild abrufen: Bild]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Bildfüllungen]</b>
            </p>
            <p>Das Modul gibt Download-Links für alle Bilder zurück, die in Bildausfüllungen in einem Dokument vorhanden sind. Bildfüllungen sind die Darstellungen [!DNL Figma] vom Benutzer bereitgestellten Bilder. Wenn Sie ein Bild in [!DNL Figma] ziehen, erstellt [!DNL Figma] ein Rechteck mit einer einzigen Füllung, die das Bild darstellt, und die Benutzenden können das Rechteck (und die Eigenschaften der Füllung) transformieren.</p>
            <p>Felder finden Sie unter <a href="#Get5" class="MCXref xref" >[!UICONTROL Datei oder Bild abrufen: Bilddateien]</a>.</p>
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
      <td role="rowheader">[!UICONTROL-Dateischlüssel]</td>
      <td>Wählen Sie die Datei aus, aus der Sie JSON zurückgeben möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Versions-ID]</td>
      <td>Geben Sie die Version der Datei ein, die das Modul zurückgeben soll, oder ordnen Sie sie zu. Lassen Sie dieses Feld für das aktuelle Modul leer.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Knoten-IDs]</td>
      <td>
        <p>Um nur eine Teilmenge des Dokuments zurückzugeben, geben Sie die Knoten ein, die das Modul zurückgeben soll. Das -Modul gibt die aufgelisteten Knoten, ihre untergeordneten Elemente und alles zurück, was sich zwischen dem Stammknoten und den aufgelisteten Knoten befindet.</p>
        <p>Klicken Sie für jeden Knoten, den Sie zurückgeben möchten, auf <b>[!UICONTROL Hinzufügen]</b> und geben Sie den Text des Knotens ein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL-Tiefe]</td>
      <td>
        <p>Geben Sie eine Ganzzahl ein, die darstellt, wie tief in der Dokumentstruktur Sie Ergebnisse zurückgeben möchten, oder ordnen Sie sie zu. </p>
        <div class="example"><span class="autonumber"><span><b>Beispiel: </b></span></span>
          <ul>
            <li>
              <p>Um nur Seiten zurückzugeben, geben Sie <code>1</code> ein.</p>
            </li>
            <li>
              <p>Um Seiten und Objekte der obersten Ebene zurückzugeben, geben Sie <code>2</code> ein.</p>
            </li>
          </ul>
        </div>
        <p>Um alle Knoten zurückzugeben, lassen Sie dieses Feld leer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Geometry]</td>
      <td>Um Vektordaten zurückzugeben, geben Sie <code>paths</code> ein.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Plugin-Daten]</td>
      <td>Eine kommagetrennte Liste von Plug-in-IDs und/oder die Zeichenfolge "[!UICONTROL shared]". Alle Daten, die im Dokument vorhanden sind, das von diesen Plug-ins geschrieben wurde, werden in das Ergebnis in den <code>pluginData</code>- und <code>sharedPluginData</code>-Eigenschaften aufgenommen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Verzweigungsdaten]</td>
      <td>Aktivieren Sie diese Option, um Metadaten der Verzweigung für die angeforderte Datei zurückzugeben. Wenn es sich bei der Datei um eine Verzweigung handelt, wird der Schlüssel der Hauptdatei in die zurückgegebene Antwort aufgenommen. Wenn die Datei Verzweigungen hat, werden deren Metadaten in die zurückgegebene Antwort aufgenommen. Standard: <code>false</code>.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Datei oder Bild abrufen: Dateiknoten]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Dateischlüssel]</td>
      <td>Wählen Sie die Datei aus, aus der Sie JSON zurückgeben möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Knoten-IDs]</td>
      <td>
        <p>Geben Sie die Knoten ein, die das Modul zurückgeben und konvertieren soll</p>
        <p>Klicken Sie für jeden Knoten, den Sie zurückgeben möchten, auf <b>[!UICONTROL Hinzufügen]</b> und geben Sie den Text des Knotens ein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Versions-ID]</td>
      <td>Geben Sie die Version der Datei ein, die das Modul zurückgeben soll, oder ordnen Sie sie zu. Lassen Sie dieses Feld für das aktuelle Modul leer.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL-Tiefe]</td>
      <td>
        <p>Geben Sie eine Ganzzahl ein, die darstellt, wie tief in der Dokumentstruktur Sie Ergebnisse zurückgeben möchten, oder ordnen Sie sie zu. </p>
        <div class="example"><span class="autonumber"><span><b>Beispiel: </b></span></span>
          <ul>
            <li>
              <p>Um nur Seiten zurückzugeben, geben Sie <code>1</code> ein.</p>
            </li>
            <li>
              <p>Um Seiten und Objekte der obersten Ebene zurückzugeben, geben Sie <code>2</code> ein.</p>
            </li>
          </ul>
        </div>
        <p>Um alle Knoten zurückzugeben, lassen Sie dieses Feld leer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Geometry]</td>
      <td>Um Vektordaten zurückzugeben, geben Sie <code>paths</code> ein.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Plugin-Daten]</td>
      <td>Eine kommagetrennte Liste von Plug-in-IDs und/oder die Zeichenfolge „shared“. Alle Daten, die im Dokument vorhanden sind, das von diesen Plug-ins geschrieben wurde, werden in das Ergebnis in den Eigenschaften pluginData und sharedPluginData aufgenommen.</td>
    </tr>
  </tbody>
</table>


##### Datei oder Bild abrufen: Bild

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Dateischlüssel]</td>
      <td>Wählen Sie die Datei aus, aus der Sie JSON zurückgeben möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Knoten-IDs]</td>
      <td>
        <p>Geben Sie die Knoten ein, die das Modul rendern soll.</p>
        <p>Klicken Sie für jeden Knoten, den Sie rendern möchten, auf <b>[!UICONTROL Hinzufügen]</b> und geben Sie den Text des Knotens ein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Scale]</td>
      <td>Um das Bild zu skalieren, geben Sie den Skalierungsfaktor ein oder mappen Sie ihn. Diese Zahl muss zwischen 0,01 und 4 liegen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL-Format]</td>
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
      <td role="rowheader">[!UICONTROL SVG - Include ID]</td>
      <td>Aktivieren Sie diese Option, um ID-Attribute für alle SVG-Elemente einzuschließen. Standard: [!UICONTROL false].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SVG - Strich vereinfachen]</td>
      <td>Aktivieren Sie diese Option, um innere/äußere Konturen zu vereinfachen und wenn möglich das Konturattribut anstelle von &lt;Maske&gt; zu verwenden. Standard: [!UICONTROL true].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Absolute Grenzen verwenden]</td>
      <td>Aktivieren Sie diese Option, um die vollständigen Abmessungen des Knotens zu verwenden, unabhängig davon, ob er abgeschnitten wird oder ob der Raum um ihn herum leer ist. Hiermit können Sie Textknoten ohne Zuschnitt exportieren. Standard: [!UICONTROL false].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Versions-ID]</td>
      <td>Geben Sie die Version der Datei ein, die das Modul zurückgeben soll, oder ordnen Sie sie zu. Lassen Sie dieses Feld für das aktuelle Modul leer.</td>
    </tr>
  </tbody>
</table>

##### Datei oder Bild abrufen: Bilddateien

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Dateischlüssel]</td>
      <td>Wählen Sie die Datei aus, aus der Sie JSON zurückgeben möchten.</td>
    </tr>
  </tbody>
</table>

### [!UICONTROL Dateiversionsverlauf auflisten]

Dieses Suchmodul gibt den Versionsverlauf einer einzelnen Datei in „Figma.
<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td> <p>Anweisungen zum Verbinden Ihres [!DNL Figma]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen.</a></p>
    <tr>
      <td role="rowheader">[!UICONTROL Datei-ID]</td>
      <td>
        <p>Geben Sie die Datei-ID der Datei ein, für die Sie den Versionsverlauf abrufen möchten, oder ordnen Sie sie zu. </p>
        <ul>
          <li>
            <p>Wenn Sie die Datei-ID nicht kennen, klicken Sie auf <b>[!UICONTROL Dateien suchen]</b> und geben Sie die ID des Projekts, mit dem die Datei verknüpft ist, ein oder mappen Sie sie. Wählen Sie dann die Datei aus.</p>
          </li>
          <li>
            <p>Wenn Sie versuchen, die Datei-ID zu finden und die Projekt-ID nicht kennen, klicken Sie auf <b>[!UICONTROL Projekte suchen]</b> und geben Sie die ID des Teams ein, dem das Projekt gehört, dem die Datei zugeordnet ist, oder ordnen Sie sie zu. Wählen Sie das Projekt und dann die Datei aus.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Geben Sie die maximale Anzahl von Datensätzen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</td>
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
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td> <p>Anweisungen zum Verbinden Ihres [!DNL Figma]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datei-ID]</td>
      <td>
        <p>Geben Sie die Projekt-ID für das Projekt ein, für das Sie Dateien abrufen möchten, oder ordnen Sie sie zu. </p>
        <ul>
          <li>
            <p>Wenn Sie die Projekt-ID nicht kennen, klicken Sie auf <b>[!UICONTROL Projekte suchen]</b> und geben Sie die ID des Teams ein, dem das Projekt zugeordnet ist, oder mappen Sie sie, und wählen Sie dann das Projekt aus.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Geben Sie die maximale Anzahl von Datensätzen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Projekte auflisten]

Dieses Suchmodul gibt eine Liste aller Projekte innerhalb des angegebenen Teams zurück.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td> <p>Anweisungen zum Verbinden Ihres [!DNL Figma]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Team-ID]</td>
      <td>Geben Sie die Projekt-ID des Projekts ein, für das Sie Dateien abrufen möchten, oder ordnen Sie sie zu. Die Team-ID finden Sie in der URL der Team-Seite in Figma</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Geben Sie die maximale Anzahl von Datensätzen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</td>
    </tr>
  </tbody>
</table>


### Komponenten und Stile

#### [!UICONTROL Abrufen eines Stils oder einer Komponente]

Dieses Aktionsmodul ruft einen einzelnen Stil, eine einzelne Komponente oder einen Satz von Stilen oder Komponenten ab.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td> <p>Anweisungen zum Verbinden Ihres [!DNL Figma]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen.</a></p>
    </tr>
    <tr>
      <td role="rowheader">&lt;[!UICONTROL Object&gt;-Schlüssel]</td>
      <td>Geben Sie den Schlüssel (eindeutige Kennung) des Objekts ein, das Sie abrufen möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Team-ID]</td>
      <td>Geben Sie die ID des Teams ein, mit dem der Datensatz oder die Datensätze verknüpft sind, oder ordnen Sie sie zu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Seitengröße]</td>
      <td>Geben Sie die Anzahl der Ergebnisse ein, die pro Seite zurückgegeben werden sollen, oder mappen Sie sie. Standardwert: 30.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL nach]</td>
      <td>
        <p>Geben Sie die Nummer des Ergebnisses ein, nach der Ergebnisse abgerufen werden sollen, oder mappen Sie sie. Dies kann mit dem Feld [!UICONTROL Seitengröße] kombiniert werden, um die Ergebnisse zu paginieren.</p>
        <p>Dieser Wert entspricht nicht den Objekt-IDs.</p>
        <p>Dieses Feld kann nicht in Kombination mit dem Feld [!UICONTROL Before] verwendet werden.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL davor]</td>
      <td>
        <p>Geben Sie die Nummer des Ergebnisses ein, bevor Sie mit dem Abrufen der Ergebnisse beginnen möchten, oder mappen Sie sie. Dies kann mit dem Feld [!UICONTROL Seitengröße] kombiniert werden, um die Ergebnisse zu paginieren.</p>
        <p>Dieser Wert entspricht nicht den Objekt-IDs.</p>
        <p>Dieses Feld kann nicht in Kombination mit dem Feld [!UICONTROL After] verwendet werden.</p>
      </td>
    </tr>
  </tbody>
</table>


### Sonstige

* [Durchführen eines API-Aufrufs](#make-an-api-call)

* [Ereignisse ansehen](#watch-events)


#### [!UICONTROL Erstellen eines API-Aufrufs]

Mit diesem Aktionsmodul können Sie die Figma-API benutzerdefiniert authentifiziert aufrufen, ohne die Authentifizierung durchdenken zu müssen. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von den anderen Figma-Modulen nicht durchgeführt werden kann.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td> <p>Anweisungen zum Verbinden Ihres [!DNL Figma]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Geben Sie einen Pfad relativ zu <code>https://api.figma.com/v1/</code> ein.</p>
        <p>Beispiel: <code>[!DNL files/7179110/comments]</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL-Methode]</td>
      <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anfragemethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL-Kopfzeilen]</td>
      <td>
        <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p>
        <p>Beispiel: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] Fügt die Autorisierungskopfzeilen für Sie hinzu.</p>
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
      <td role="rowheader">[!UICONTROL body]</td>
   <td> <p>Fügen Sie den Hauptteil des Inhalts für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Wenn Sie bedingte Anweisungen wie <code>if</code> in Ihrer JSON-Datei verwenden, setzen Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Ereignisse ansehen]

Dieses Teammodul startet ein Szenario, wenn eines der folgenden Trigger für ein bestimmtes Team in Ihrem [!DNL Figma] Teambereich eintritt

* Dateiaktualisierung

* Dateiversionsaktualisierung

* Datei löschen

* Bibliothek veröffentlichen

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
            <p>Klicken Sie auf <b>[!UICONTROL Hinzufügen]</b> neben dem Feld [!UICONTROL Webhook].</p>
          </li>
          <li value="2">
            <p>Wählen Sie die Verbindung aus, die Sie für diesen Webhook verwenden möchten. Anweisungen zum Verbinden Ihres [!DNL Figma]-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!UICONTROL Adobe Workfront Fusion] - Grundanweisungen.</a></p>
          </li>
          <li value="3">
            <p>Wählen Sie den Ereignistyp aus, den das Modul überwachen soll.</p>
          </li>
          <li value="4">
            <p>Geben Sie die ID des Teams ein, dessen Ereignisse der Webhook überwachen soll.</p>
          </li>
          <li value="5">
            <p>Geben Sie den [!UICONTROL Status] oder [!UICONTROL Description] der Ereignisse ein, die der Webhook überwachen soll.</p>
          </li>
          <li value="6">
            <p>Klicken Sie auf <b>[!UICONTROL Speichern]</b>, um den Webhook zu speichern und zum Modul zurückzukehren.</p>
          </li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>
