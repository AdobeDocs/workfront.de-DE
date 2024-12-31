---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Steckverbinder
navigation-topic: apps-and-their-modules
title: Adobe Lightroom-Module
description: Mit den Adobe Lightroom-Modulen können Sie ein Adobe Workfront Fusion-Szenario starten, das auf Ereignissen in Ihrem Adobe Lightroom-Konto basiert.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: e48bdf18-49f0-436e-9182-16c9da2b3169
source-git-commit: 6f4ba4cde26978305a58cedb9ed606c6032496f1
workflow-type: tm+mt
source-wordcount: '2370'
ht-degree: 0%

---

# [!DNL Adobe Lightroom]


In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die [!DNL Adobe Lightroom] verwenden, und sie mit mehreren Anwendungen und Services von Drittanbietern verbinden.

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
      <td >
        <p>[!UICONTROL Workfront Fusion for Work Automation and Integration]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Produkt</td>
      <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu nutzen.</td>
    </tr>
    </tr>
  </tbody>
</table>


&#42;Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

&#42;&#42;Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [!DNL [Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Voraussetzungen

Bevor Sie den [!DNL Adobe Lightroom]-Connector verwenden können, müssen Sie sicherstellen, dass die folgenden Voraussetzungen erfüllt sind:

* Sie müssen über ein aktives [!DNL Adobe Lightroom] verfügen.


## Adobe Lightroom-API-Informationen

Der Adobe Lightroom-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Basis-URL</td> 
   <td>https://lr.adobe.io</td> 
  </tr>
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v1.17.128</td> 
  </tr>
 </tbody> 
 </table>

## Erstellen einer Verbindung mit Adobe Lightroom

So erstellen Sie eine Verbindung für Ihre [!DNL Adobe Lightroom]:

1. Klicken Sie **[!UICONTROL Hinzufügen]** neben dem Feld Verbindung auf.

1. Füllen Sie die folgenden Felder aus:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[!UICONTROL Verbindungsname]</td>
        <td>
          <p>Geben Sie einen Namen für diese Verbindung ein.</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Umgebung]</td>
        <td>Wählen Sie aus, ob Sie eine Verbindung zu einer Produktions- oder Nicht-Produktionsumgebung herstellen.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Typ]</td>
        <td>Wählen Sie aus, ob Sie eine Verbindung zu einem Service-Konto oder einem persönlichen Konto herstellen möchten.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client-ID]</td>
        <td>Geben Sie Ihre [!UICONTROL Adobe] [!UICONTROL Client ID] ein. Diese finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client-Geheimnis]</td>
        <td>Geben Sie Ihren [!DNL Adobe] [!UICONTROL Client Secret] ein. Diese finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des [!DNL Adobe Developer Console]</td>
        </tr>
      </tbody>
    </table>

1. Klicken Sie **[!UICONTROL Fortfahren]**, um die Verbindung zu speichern und zum Modul zurückzukehren.



## Adobe Lightroom-Module und ihre Felder

Beim Konfigurieren [!DNL Adobe Lightroom] Module zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder dem Service weitere [!DNL Adobe Lightroom] angezeigt werden. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Sonstige](#other)
* [Assets](#assets)
* [Alben](#albums)

### Sonstige

* [Konsistenzprüfung](#health-check)
* [Abrufen von Benutzerkatalog-Metadaten](#retrieve-user-catalog-metadata)

#### Konsistenzprüfung

Dieses Aktionsmodul ruft eine Lightroom-Server-Versions-ID ab und zeigt an, ob der Lightroom-Service derzeit ausgeführt wird.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom] finden Sie unter <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL]</td>
      <td>
        <p>Wenn Sie bestimmte Anmeldeinformationen angeben möchten, um sicherzustellen, dass ein bestimmter Server ausgeführt wird, klicken Sie auf Element hinzufügen und geben Sie die Anmeldeinformationen ein.</p><p>Autorisierungskopfzeilen werden automatisch hinzugefügt.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Abrufen von Benutzerkatalog-Metadaten

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom] finden Sie unter <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL]</td>
      <td>
        <p>Wenn Sie bestimmte Anmeldeinformationen angeben möchten, um sicherzustellen, dass Sie auf das richtige Benutzerkonto zugreifen können, klicken Sie auf Element hinzufügen und geben Sie die Anmeldeinformationen ein.</p><p>Autorisierungskopfzeilen werden automatisch hinzugefügt.</p>
      </td>
    </tr>
  </tbody>
</table>

### Assets

* [Erstellen einer Asset-Originaldatei](#create-an-asset-external-xmp-develop-setting-file)
* [Erstellen von Assets](#create-an-asset)
* [Erstellen einer Einstellungsdatei für die externe XMP-Entwicklung eines Assets](#create-an-asset-external-xmp-develop-setting-file)
* [Erzeugen von Ausgabedarstellungen für eine Originaldatei](#generate-renditions-for-an-original-file)
* [Abrufen eines Katalog-Assets](#get-a-catalog-asset)
* [Abrufen der neuesten Einstellung für die Entwicklung externer Asset-XMP](#get-the-latest-asset-external-xmp-develop-setting-file)
* [Abrufen der neuesten Asset-Ausgabedarstellung](#get-the-latest-asset-rendition)
* [Abrufen von Assets](#retrieve-assets)

#### Erstellen einer Asset-Originaldatei

Dieses Aktionsmodul erstellt eine Originaldatei für ein Asset und lädt sie hoch.


<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom] finden Sie unter <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die ID des Katalogs ein, der das Asset enthält, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset-ID]</td>
      <td>
        <p>Geben Sie die ID des Assets ein, für das Sie eine Datei erstellen und hochladen möchten, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Länge des Inhalts in Byte]</td>
      <td>
        <p>Geben Sie die Länge des Inhalts in Byte ein oder mappen Sie sie.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Bytebereich]</td>
      <td>
        <p>Geben Sie den Bytebereich für die Anfrage ein, einschließlich des ersten und letzten Bytes und der Entitätslänge, wie in RFC 2616 definiert. Sollte nur enthalten sein, wenn die Daten zu groß sind, um in einem einzigen Aufruf hochgeladen zu werden.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Content-Typ]</td>
      <td>
        <p>Content-Typ für die neue Datei auswählen.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Erstellen von Assets

Dieses Aktionsmodul erstellt ein neues Asset mit anfänglichen Metadaten und Importinformationen.


<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom] finden Sie unter <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die ID des Katalogs ein, in dem das Asset erstellt wird, oder mappen Sie sie.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset-ID]</td>
      <td>
        <p>Geben Sie die ID des neuen Assets ein oder mappen Sie sie.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset-Typ]</td>
      <td>
        <p>Wählen Sie aus, ob das Asset ein Bild oder ein Video ist.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datum/Uhrzeit der Erstellung]</td>
      <td>
        <p>Geben Sie ein Datum im Format <code>YYYY-MM-DDT00:00:00-00:00</code> ein oder mappen Sie es.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datetime-Benutzer aktualisiert]</td>
      <td>
        <p>Geben Sie ein Datum im Format <code>YYYY-MM-DDT00:00:00-00:00</code> ein oder mappen Sie es.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datum erfasst]</td>
      <td>
        <p>Geben Sie ein Datum im Format <code>YYYY-MM-DDT00:00:00-00:00</code> ein oder mappen Sie es.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Erstellen einer Einstellungsdatei für die externe XMP-Entwicklung eines Assets

Dieses Aktionsmodul unterstützt zwei Workflows. Der erste Workflow besteht darin, die externe XMP-Entwicklungseinstellungsdatei für das Asset hochzuladen. Der zweite Workflow besteht darin, eine externe XMP-Entwicklungseinstellungsdatei zu erstellen, indem Sie sie aus der externen XMP-Entwicklungseinstellungsdatei eines anderen Assets kopieren.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom] finden Sie unter <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Länge des Inhalts in Byte]</td>
      <td>
        <p>Geben Sie die Länge des Inhalts in Byte ein oder mappen Sie sie.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Neue XMP-/Entwicklungsdatei hochladen oder kopieren]</td>
      <td>
        <p>Wählen Sie aus, ob Sie eine neue Datei hochladen oder eine Datei aus einem vorhandenen Asset kopieren.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die ID des Katalogs ein, der das Asset enthält, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset-ID]</td>
      <td>
        <p>Geben Sie die ID des Assets ein, das Sie hochladen oder in das Sie eine Datei kopieren möchten, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Link to XMP/develop file]</td>
      <td>
        <p>Geben Sie einen Link zu der Datei ein, die Sie hochladen oder kopieren möchten, oder ordnen Sie ihn zu.</p><p>Diese Datei muss JSON sein, wenn eine Datei kopiert wird, oder XML, wenn eine Datei hochgeladen wird.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Erzeugen von Ausgabedarstellungen für eine Originaldatei

Dieses Aktionsmodul generiert asynchron Ausgabedarstellungen für eine Originaldatei.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom] finden Sie unter <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ausgabedarstellungstyp(en) (durch Semikolon getrennt)]</td>
      <td>
        <p>Geben Sie den Ausgabedarstellungstyp für die Ausgabedarstellung ein, die Sie erstellen möchten. Wenn Sie mehr als einen Typ eingeben, trennen Sie sie durch ein Semikolon (;). <p>Mögliche Typen:</p><ul><li><code>fullsize</code></li><li><code>2560</code></li></ul></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Länge des Inhalts in Byte]</td>
      <td>
        <p>Geben Sie die Länge des Inhalts in Byte ein oder mappen Sie sie.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die ID des Katalogs ein, der das Asset enthält, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset-ID]</td>
      <td>
        <p>Geben Sie die ID des Assets ein, für das Sie eine Ausgabedarstellung einer Datei erstellen möchten, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Abrufen eines Katalog-Assets

Dieses Aktionsmodul ruft Informationen zu einem einzelnen Asset in einem Katalog ab. Der Katalog muss im Besitz des Benutzers sein, dessen Anmeldeinformationen in der in diesem Modul verwendeten Verbindung dargestellt werden.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom] finden Sie unter <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die ID des Katalogs ein, der das Asset enthält, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset-ID]</td>
      <td>
        <p>Geben Sie die ID des Assets ein, für das Sie Informationen abrufen möchten, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
  </tbody>
</table>


#### Abrufen der neuesten Einstellungsdatei für die externe Asset-XMP-Entwicklung

Dieses Aktionsmodul ruft die neueste externe XMP-Einstellungsdatei für Assets ab.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom] finden Sie unter <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die ID des Katalogs ein, der das Asset enthält, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset-ID]</td>
      <td>
        <p>Geben Sie die ID des Assets ein, das mit der XMP-Entwicklungseinstellungsdatei verknüpft ist, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Abrufen der neuesten Asset-Ausgabedarstellung

Dieses Aktionsmodul ruft die neueste Asset-Ausgabedarstellung des angegebenen Typs ab.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom] finden Sie unter <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die ID des Katalogs ein, der das Asset enthält, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset-ID]</td>
      <td>
        <p>Geben Sie die ID des Assets ein, das mit der XMP-Entwicklungseinstellungsdatei verknüpft ist, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ausgabedarstellungstyp]</td>
      <td>
        <p>Wählen Sie den Typ der Ausgabedarstellung aus, die Sie abrufen möchten.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Abrufen von Assets

Dieses Aktionsmodul ruft Assets ab, die dem Benutzer gehören, dessen Anmeldeinformationen in der in diesem Modul verwendeten Verbindung dargestellt werden.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom] finden Sie unter <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die ID des Katalogs ein, der das Asset enthält, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Startzeitstempel]</td>
      <td>
        <p>Zeitstempel eingeben oder zuordnen. Das Modul gibt Datensätze zurück, die nach diesem Zeitstempel aktualisiert wurden.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gibt zuvor erfasste Assets zurück]</td>
      <td>
        <p>Geben Sie ein Datum im Format <code>YYYY-MM-DDT00:00:00</code> ein. Das Modul gibt Ergebnisse zurück, die vor diesem Datum erfasst wurden.</p><p> Dieses Feld kann nicht mit dem <code>Return assets captured after</code> verwendet werden.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Maximale Anzahl der zurückgegebenen Assets]</td>
      <td>
        <p>Legen Sie die maximale Anzahl von Assets fest, die [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgeben. Diese Zahl muss kleiner oder gleich 100 sein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SHA256 Hash-Wert der Originaldatei]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Assets ausblenden, die sich innerhalb von Stacks befinden?“]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset-Untertypwerte]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset-IDs]</td>
      <td>
        <p>Geben Sie bis zu 100 Asset-IDs ein (durch Kommas getrennt) oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Typen der auszuschließenden Assets]</td>
      <td>
        <p>Wählen Sie aus, ob Sie vollständige oder unvollständige Assets ausschließen möchten. Um alle Assets einzubeziehen, lassen Sie dieses Feld leer.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Gruppenwerte]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Namenswerte]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Favoritenstatus]</td>
      <td>
        <p></p>
      </td>
    </tr>
    </tr>
  </tbody>
</table>

### Alben

* [Hinzufügen von Assets zu einem Album](#add-assets-to-an-album)
* [Erstellen eines Albums](#create-an-album)
* [Ein Album löschen](#delete-an-album)
* [Album abrufen](#get-an-album)
* [Auflisten der Assets eines Albums](#list-assets-of-an-album)
* [Abrufen von Alben](#retrieve-albums)
* [Aktualisieren eines Albums](#update-album)

#### Hinzufügen von Assets zu einem Album

Dieses Aktionsmodul fügt dem angegebenen Album mindestens ein Asset hinzu. Sie können bis zu 50 Assets in einem Ausführungszyklus hinzufügen.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom] finden Sie unter <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die ID des Katalogs ein, der das Album enthält, dem Sie Assets hinzufügen möchten, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Album-ID]</td>
      <td>
        <p>Geben Sie die ID des Albums ein, dem Sie Assets hinzufügen möchten, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Assets]</td>
      <td>
        <p>Klicken Sie für jedes Asset, das Sie dem Album hinzufügen möchten, auf <b>Element hinzufügen</b> und geben Sie die folgenden Felder ein.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Asset-ID]</td>
      <td>
        <p>Geben Sie die ID des Assets ein, das Sie dem Album hinzufügen möchten, oder ordnen Sie sie zu</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Ist dieses Asset ein Albumcover?]</td>
      <td>
        <p>Wählen Sie aus, ob dieses Asset als Bild für das Album angezeigt werden soll.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL-Reihenfolge]</td>
      <td>
        <p></p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Metadaten]</td>
      <td>
        <p>Geben Sie alle Metadaten ein, die Sie in das Asset aufnehmen möchten, oder ordnen Sie sie zu. Dies muss eine einzelne Textzeichenfolge mit einer maximalen Länge von 1-24 Zeichen sein.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Remote-ID]</td>
      <td>
        <p>Geben Sie eine Kennung für das Asset ein.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Erstellen eines Albums

Dieses Aktionsmodul erstellt ein neues Album in Lightroom.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom] finden Sie unter <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die ID des Katalogs ein, in dem Sie ein Album erstellen möchten, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Album-ID]</td>
      <td>
        <p>Geben Sie eine ID für das neue Album ein oder mappen Sie sie.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Untertyp]</td>
      <td>
        <p>Wählen Sie den Untertyp für das Album aus.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL API-Schlüssel]</td>
      <td>
        <p>Geben Sie den API-Schlüssel des Services ein, der das Album erstellt.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Datum/Uhrzeit der Erstellung]</td>
      <td>
        <p>Geben Sie ein Datum im Format <code>YYYY-MM-DDT00:00:00-00:00Z</code> ein oder mappen Sie es.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datetime-Benutzer aktualisiert]</td>
      <td>
        <p>Geben Sie ein Datum im Format <code>YYYY-MM-DDT00:00:00-00:00Z</code> ein oder mappen Sie es.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Albumname]</td>
      <td>
        <p>Geben Sie einen Namen für das neue Album ein oder mappen Sie ihn.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Cover ID]</td>
      <td>
        <p>Geben Sie die ID eines Assets ein, das als Cover für dieses Album verwendet werden soll, oder mappen Sie sie.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Remote-ID]</td>
      <td>
        <p>Geben Sie eine Kennung für das Asset ein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Erstellungsdatum]</td>
      <td>
        <p>Geben Sie ein Datum im Format <code>YYYY-MM-DDT00:00:00-00:00Z</code> ein oder mappen Sie es.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Aktualisiert am]</td>
      <td>
        <p>Geben Sie ein Datum im Format <code>YYYY-MM-DDT00:00:00-00:00Z</code> ein oder mappen Sie es.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Wird das Album gelöscht?]</td>
      <td>
        <p>Aktivieren Sie diese Option, wenn die extern verknüpften Inhalte gelöscht wurden.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL des Speicherorts zum Bearbeiten verknüpfter Inhalte]</td>
      <td>
        <p>Wenn es eine URL gibt, unter der Benutzer den Inhalt dieses Albums bearbeiten können, geben Sie die URL hier ein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL des Speicherorts zum Anzeigen verknüpfter Inhalte]</td>
      <td>
        <p>Wenn es eine URL gibt, unter der Benutzer den Inhalt dieses Albums anzeigen können, geben Sie die URL hier ein.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Ein Album löschen

Dieses Aktionsmodul löscht ein Album.

Das gelöschte Album muss von derselben Client-App erstellt worden sein, die es jetzt löscht, und es muss vom Untertyp `project` oder `project_set` sein.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom] finden Sie unter <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die ID des Katalogs ein, der das Album enthält, das Sie löschen möchten, oder mappen Sie sie.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Album-ID]</td>
      <td>
        <p>Geben Sie die ID des Albums ein, das Sie löschen möchten, oder mappen Sie sie.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Untergeordnete Alben löschen?]</td>
      <td>
        <p>Wählen Sie aus, ob Sie die untergeordneten Alben des gelöschten Albums löschen möchten.</p>
      </td>
    </tr>
  </tbody>
</table>

### Album abrufen

Dieses Aktionsmodul ruft das angegebene Album ab

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom] finden Sie unter <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die ID des Katalogs ein, der das abzurufende Album enthält, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Album-ID]</td>
      <td>
        <p>Geben Sie die ID des Albums ein, das Sie abrufen möchten, oder mappen Sie sie.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Auflisten der Assets eines Albums

Dieses Aktionsmodul ruft eine Liste der Assets im angegebenen Album ab.



#### Abrufen von Alben

Dieses Aktionsmodul ruft eine Liste der Alben im angegebenen Katalog ab.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom] finden Sie unter <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die ID des Katalogs ein, der Alben enthält, die Sie abrufen möchten, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Untertypen]</td>
      <td>
        <p>Geben Sie die ID des Albums ein, das Sie abrufen möchten, oder mappen Sie sie.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name des Albums, das den aktuellen Ergebnissen vorangestellt wird]</td>
      <td>
        <p>Wenn Sie Ihre Ergebnisse paginieren, geben Sie den Namen des letzten Albums auf der vorherigen Seite ein oder mappen Sie ihn.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Maximale Anzahl der zurückgegebenen Alben]</td>
      <td>
        <p>Legen Sie die maximale Anzahl von Assets fest, die [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgeben. Der Standardwert für dieses Feld ist 100. Dieses Modul kann mehr Alben als dieses Limit zurückgeben, wenn mehrere Alben an der Grenzlinie denselben <code>name_after</code> haben.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Album aktualisieren

Dieses Aktionsmodul aktualisiert das angegebene Album.

Das aktualisierte Album muss von derselben Client-Anwendung erstellt worden sein, die es jetzt aktualisiert, und es muss vom Untertyp `project` oder `project_set` sein.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom] finden Sie unter <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die ID des Katalogs ein, der das Album enthält, das Sie aktualisieren möchten, oder mappen Sie sie.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Album-ID]</td>
      <td>
        <p>Geben Sie die ID des Albums ein, das Sie aktualisieren möchten, oder mappen Sie sie.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Andere Felder</td>
      <td>
      <td>Beschreibungen anderer Felder in diesem Modul finden Sie unter <a href="#create-an-album" class="MCXref xref" >Erstellen eines </a>) in diesem Artikel.</td>
      </td>
    </tr>
  </tbody>
</table>
