---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connector
navigation-topic: apps-and-their-modules
title: Google-Folienmodule
description: Mit den Adobe Workfront Fusion Google Slides-Modulen können Sie Präsentationen erstellen, aktualisieren, auflisten und/oder löschen und Bilder in Präsentationen in Ihrem Google Slides-Konto hochladen.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 680a5328-1d50-4434-beda-7a4670a6e458
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1575'
ht-degree: 0%

---

# [!DNL Google Slides]-Module

Die [!DNL Adobe Workfront Fusion] [!DNL Google Slides] -Module ermöglichen es Ihnen, Präsentationen zu erstellen, zu aktualisieren, aufzulisten und/oder zu löschen und Bilder in Präsentationen in [!DNL Google Slides] -Konto.

Zur Verwendung [!DNL Google Slides] mit [!DNL Workfront Fusion], muss ein [!DNL Google] -Konto. Wenn Sie keine [!DNL Google] -Konto erstellen können, können Sie eines im [!DNL Google] Hilfeseite für Konten.

Sie benötigen [!DNL Google Slides] in [!DNL Google Drive].

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p> </td> 
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

Verwendung [!DNL Google Slides] -Module, müssen Sie über eine [!DNL Google] -Konto.

## [!DNL Google Slides] Module und ihre Felder

Bei der Konfiguration [!DNL Google Slides] -Modulen, zeigt Workfront Fusion die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Google Slides] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Präsentation](#presentation)
* [Sonstige](#other)

### Präsentation

* [[!UICONTROL Presentations ansehen]](#watch-presentations)
* [[!UICONTROL Presentations auflisten]](#list-presentations)
* [[!UICONTROL Präsentation abrufen]](#get-a-presentation)
* [[!UICONTROL Abrufen einer Seite/Miniatur]](#get-a-pagethumbnail)
* [[!UICONTROL Erstellen einer Präsentation anhand einer Vorlage]](#create-a-presentation-from-a-template)
* [[!UICONTROL Hochladen eines Bildes in eine Präsentation]](#upload-an-image-to-a-presentation)
* [[!UICONTROL Diagramm aktualisieren]](#refresh-a-chart)
* [[!UICONTROL Folie hinzufügen/löschen]](#adddelete-a-slide)

#### [!UICONTROL Presentations ansehen]

Trigger bei der Erstellung oder Aktualisierung einer neuen Präsentation.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google Slides] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch] </td> 
   <td> <p>Wählen Sie die Option zum Ansehen der Präsentationen aus:</p> 
    <ul> 
     <li> <p>[!UICONTROL Erstellungsdatum]</p> </li> 
     <li> <p>[!UICONTROL Änderungsdatum]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Die maximale Anzahl von Präsentationen, die Workfront Fusion während eines Szenario-Ausführungszyklus zurückgibt.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Presentations auflisten]

Ruft eine Liste aller Präsentationen ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google Slides] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Speicherort des Laufwerks auswählen]</td> 
   <td> <p>Wählen Sie die [!DNL Google Drive] wo sich die Präsentationen befinden, die Sie auflisten möchten:</p> 
    <ul> 
     <li>[!UICONTROL Mein Laufwerk]</li> 
     <li>[!UICONTROL Für mich freigegeben]</li> 
     <li>[!UICONTROL [!DNL Google] Freigegebenes Laufwerk]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner-ID]</td> 
   <td> <p>Wählen Sie den Ordnerspeicherort der Präsentationen aus, die Sie auflisten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Die maximale Anzahl an Präsentationen [!DNL Workfront Fusion] sollte während eines Szenario-Ausführungszyklus zurückgegeben werden.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Präsentation abrufen]

Ruft die neueste Version einer bestimmten Präsentation ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google Slides] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie die [!DNL Google Drive] wo sich die Präsentationen befinden, die Sie auflisten möchten:</p> 
    <ul> 
     <li>[!UICONTROL Mein Laufwerk]</li> 
     <li>[!UICONTROL Für mich freigegeben]</li> 
     <li>[!UICONTROL [!DNL Google] Freigegebenes Laufwerk]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Präsentations-ID]</td> 
   <td> <p> Wählen Sie die Präsentation aus, die Sie abrufen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Abrufen einer Seite/Miniatur]

Ruft die neueste Version der angegebenen Seite oder der Miniaturansicht einer Seite in der Präsentation ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google Slides] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Präsentations-ID]</td> 
   <td> <p> Wählen Sie die Präsentations-ID aus, die Sie abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seitenobjekt-ID]</td> 
   <td> <p> Wählen Sie die Folie aus, für die Sie die Details des Seitenobjekts anzeigen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seitenminiatur anzeigen]</td> 
   <td> <p> Aktivieren Sie das Kontrollkästchen, wenn Sie die Informationen zur Seitenminiatur anzeigen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Erstellen einer Präsentation anhand einer Vorlage]

Erstellt eine neue Präsentation, indem alle Tags wie `{{Name}}`, `{{Email}}` in einer Vorlage mit den bereitgestellten Daten.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google Slides] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Titel] </td> 
   <td> <p>Geben Sie einen Namen für die neue Präsentation ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eine Präsentation kopieren]</td> 
   <td> <p> Wählen Sie die Option aus, wenn Sie eine vorhandene Präsentation kopieren:</p> 
    <ul> 
     <li>[!UICONTROL Nach Zuordnung]</li> 
     <li>[!UICONTROL Nach Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kopie der vorhandenen Präsentations-ID]</td> 
   <td> <p> Geben Sie den Pfad oder die Präsentations-ID einer vorhandenen Präsentation ein, die Sie kopieren möchten. Dieses Feld wird angezeigt, wenn Sie die Präsentation [!UICONTROL By Mapping] erstellen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie die [!DNL Google Drive] wo sich die Präsentationen befinden, die Sie auflisten möchten:</p> 
    <ul> 
     <li>[!UICONTROL Mein Laufwerk]</li> 
     <li>[!UICONTROL Für mich freigegeben]</li> 
     <li>[!UICONTROL [!DNL Google] Freigegebenes Laufwerk]</li> 
    </ul> <p>Dieses Feld wird angezeigt, wenn Sie die Präsentation erstellen [!UICONTROL Nach Dropdown].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Präsentations-ID]</td> 
   <td> <p> Wählen Sie die Präsentations-ID der Präsentation aus, die Sie als Vorlage verwenden möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Werte] </td> 
   <td> <p>Fügen Sie die Werte hinzu:</p> 
    <ul> 
     <li><strong>[!UICONTROL Tag]</strong>: Geben Sie das Tag ein, das Sie in der Präsentation ersetzen möchten. Beispiel: <code>&#123;&#123;Name&#125;&#125;</code></li> 
     <li><strong>[!UICONTROL Ersetzter Wert]</strong>: Geben Sie den Wert ein, durch den das vorhandene Tag ersetzt werden soll. Wenn beispielsweise eine Zeichenfolge <code>&#123;&#123;Name}}</code><code>Sample</code></li></ul></td></tr><tr><td role="rowheader"></td><td><p></p><ul><li></li><li></li><li></li></ul></td></tr><tr><td role="rowheader"><p></p></td><td><p></p></td></tr><tr><td role="rowheader"></td><td><p></p></td></tr><tr><td role="rowheader"></td><td><p></p></td></tr></tbody></table>

#### [!UICONTROL Hochladen eines Bildes in eine Präsentation]

Lädt ein Bild mit den bereitgestellten Daten hoch.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google Slides] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Präsentation auswählen]</td> 
   <td> <p>Wählen Sie aus, wie die Präsentation ausgewählt werden soll, in die Sie ein Bild hochladen.</p> 
    <ul> 
     <li>[!UICONTROL Nach Zuordnung]</li> 
     <li>[!DNL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie die [!DNL Google Drive] wo sich die Präsentationen befinden, die Sie auflisten möchten:</p> 
    <ul> 
     <li>[!UICONTROL Mein Laufwerk]</li> 
     <li>[!UICONTROL Für mich freigegeben]</li> 
     <li>[!UICONTROL [!DNL Google] Freigegebenes Laufwerk]</li> 
    </ul> <p>Dieses Feld wird angezeigt, wenn Sie die Präsentation erstellen [!UICONTROL Nach Dropdown].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Präsentations-ID]</td> 
   <td> <p> Wählen Sie die Präsentations-ID der Präsentation aus, in die Sie ein Bild hochladen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Werte]</td> 
   <td> <p>Werte Fügen Sie die Werte hinzu:</p> 
    <ul> 
     <li><strong>[!UICONTROL Tag]</strong>: Geben Sie das Tag ein, dem Sie die URL hinzufügen möchten.</li> 
     <li><strong>[!UICONTROL Bild-URL]</strong>: Geben Sie den Pfad oder die URL zum Bild ein, das Sie hochladen möchten.</li> 
    </ul> <p>Hinweis: Die Bilder müssen kleiner als 50 MB sein, 25 Megapixel nicht überschreiten und im PNG-, JPEG- oder GIF-Format vorliegen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Diagramm aktualisieren]

Aktualisiert die Diagrammdaten, die in einer durch die Kennung angegebenen Präsentation gespeichert sind.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google Slides] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie die [!DNL Google Drive] wo sich die Präsentationen befinden, die Sie auflisten möchten:</p> 
    <ul> 
     <li>[!UICONTROL Mein Laufwerk]</li> 
     <li>[!UICONTROL Für mich freigegeben]</li> 
     <li>[!UICONTROL [!DNL Google] Freigegebenes Laufwerk]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Präsentations-ID]</td> 
   <td> <p>Wählen Sie die Präsentations-ID der Präsentation aus, die das zu aktualisierende Diagramm enthält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Diagrammobjekt-ID]</td> 
   <td> <p> Wählen Sie das Diagramm aus, das Sie aktualisieren möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Folie hinzufügen/löschen]

Erstellt eine leere Folie oder löscht eine vorhandene Folie auf der angegebenen Präsentation.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google Slides] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methode auswählen]</td> 
   <td> <p>Wählen Sie aus, ob Sie eine neue Folie hinzufügen oder eine Folie löschen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Presentation ID]</td> 
   <td> <p>Wählen Sie die Präsentations-ID der Präsentation aus, für die Sie eine Folie hinzufügen oder löschen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vordefinierter Layouttyp]</td> 
   <td> <p> Wählen Sie das vordefinierte Dialayout aus, das Sie für die hinzugefügte Folie verwenden möchten. Geben Sie Werte für zusätzliche Felder an (z. B. [!UICONTROL Title]).</p> 
    <ul> 
     <li>[!UICONTROL Leeres Layout, ohne Platzhalter]</li> 
     <li>[!UICONTROL Layout mit einer Beschriftung am unteren Rand]</li> 
     <li>[!UICONTROL Layout mit einem Titel und Untertitel]</li> 
     <li>[!UICONTROL Layout mit Titel und Hauptteil]</li> 
     <li>[!UICONTROL Layout mit einem Titel und zwei Spalten]</li> 
     <li>[!UICONTROL Layout mit nur einem Titel]</li> 
     <li>[!UICONTROL Layout mit einem Abschnittstitel]</li> 
     <li>[!UICONTROL Layout mit einem Titel und Untertitel auf der einen Seite und einer Beschreibung auf der anderen Seite]</li> 
     <li>[!UICONTROL Layout mit einem Titel und einem Text, angeordnet in einer Spalte]</li> 
     <li>[!UICONTROL Layout mit einem Hauptpunkt]</li> 
     <li>[!DNL Layout with a big number heading]</li> 
    </ul> <p>Dieses Feld ist verfügbar, wenn Sie zum Hinzufügen einer Folie ausgewählt haben.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Sonstige

* [[!UICONTROL API-Aufruf durchführen]](#make-an-api-call)
* [[!UICONTROL Links in eine Präsentation einfügen]](#insert-links-in-a-presentation)

#### [!UICONTROL API-Aufruf durchführen]

Führt einen beliebigen autorisierten API-Aufruf durch.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google Slides] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Geben Sie einen Pfad relativ zu https://developers.google.com/slides/ ein. z. B. Präsentation.</p> <p>Die Liste der verfügbaren Endpunkte finden Sie im Abschnitt <a href="https://developers.google.com/slides/reference/rest">[!DNL Google Slides] API-Dokumentation</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methode]</td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Geben Sie die gewünschten Anforderungsheader ein. Sie müssen keine Autorisierungskopfzeilen hinzufügen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p> Geben Sie die Abfragezeichenfolge der Anfrage ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Notiz:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> Fügen Sie die Anführungszeichen in Ihre JSON-Datei außerhalb der bedingten Anweisung ein.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Beispiel:** Mithilfe eines API-Aufrufs können Sie die Präsentationsdetails für die von Ihnen eingegebene Präsentations-ID abrufen. Sie können die Präsentations-ID in der URL finden, wenn Sie die Präsentation in [!DNL Google Slides].
>
>![](assets/api-call-350x13.png)
>
>Der folgende API-Aufruf gibt die Präsentationsdetails zurück:
>
>![](assets/presentation-details.png)
>
>Treffer der Suche finden Sie in der Ausgabe des Moduls unter [!UICONTROL Bundle] > [!UICONTROL body] > [!UICONTROL presentationId].
>
>In unserem Beispiel wurden die angeforderten Präsentationsdetails zurückgegeben:
>
>![](assets/presentation-details-2.png)

#### [!UICONTROL Links in eine Präsentation einfügen]

Dieses Modul macht alle Links in einer Präsentation klickbar oder fügt einen Link in alle übereinstimmenden Eingabetexte ein.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google Slides] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Präsentation auswählen]</td> 
   <td> <p>Wählen Sie aus, wie die Präsentation ausgewählt werden soll, in die Sie ein Bild hochladen.</p> 
    <ul> 
     <li>[!UICONTROL Nach Zuordnung]</li> 
     <li>[!UICONTROL Nach Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie die [!DNL Google Drive] wo sich die Präsentationen befinden, die Sie auflisten möchten:</p> 
    <ul> 
     <li>[!UICONTROL Mein Laufwerk]</li> 
     <li>[!UICONTROL Für mich freigegeben]</li> 
     <li>[!UICONTROL [!DNL Google] Freigegebenes Laufwerk]</li> 
    </ul> <p>Dieses Feld wird angezeigt, wenn Sie die Präsentation erstellen [!UICONTROL Nach Dropdown].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Präsentations-ID]</td> 
   <td> <p>Wählen Sie den Ordnerspeicherort der Präsentationen aus, die Sie auflisten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select]</td> 
   <td> <p>Wählen Sie aus, ob Sie alle Links in einer Präsentation anklickbar machen möchten oder ob Sie einen Link in alle entsprechenden Eingabetexte einfügen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Texteingaben]</td> 
   <td>Fügen Sie für jedes Textelement, für das Sie einen Link hinzufügen möchten, das Element sowie den zugehörigen Link zur Liste hinzu. Jedes Mal, wenn das Element in der Präsentation erscheint, wird es automatisch mit der angegebenen Seite verknüpft.</td> 
  </tr> 
 </tbody> 
</table>
