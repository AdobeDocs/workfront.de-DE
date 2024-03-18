---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Adobe Lightroom-Module
description: Mit den Adobe Lightroom-Modulen können Sie ein Adobe Workfront Fusion-Szenario starten, das auf Ereignissen in Ihrem Adobe Lightroom-Konto basiert.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
source-git-commit: e99bd69c712a7685512eecc7fccc8211013a259d
workflow-type: tm+mt
source-wordcount: '2244'
ht-degree: 0%

---

# [!DNL Adobe Lightroom] Module

<!--Add Connection info-->

In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL Adobe Lightroom], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.

Informationen zum Erstellen eines Szenarios finden Sie unter [Erstellen eines Szenarios](../../workfront-fusion/scenarios/create-a-scenario.md).

Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
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
        <p>[!UICONTROL Workfront Fusion für Arbeitsautomatisierung und -integration]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Produkt</td>
      <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td>
    </tr>
    </tr>
  </tbody>
</table>


&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

&#42;&#42;Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [!DNL [Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Voraussetzungen

Bevor Sie die [!DNL Adobe Lightroom] müssen Sie sicherstellen, dass die folgenden Voraussetzungen erfüllt sind:

* Sie müssen über eine aktive [!DNL Adobe Lightroom] -Konto.

## Herstellen einer Verbindung zu Adobe Lightroom



## Adobe Lightroom-Module und ihre Felder

Bei der Konfiguration [!DNL Adobe Lightroom] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Adobe Lightroom] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Sonstige](#other)
* [Assets](#assets)
* [Alben](#albums)

### Sonstige

* [Konsistenzprüfung](#health-check)
* [Abrufen von Benutzerkatalog-Metadaten](#retrieve-user-catalog-metadata)

#### Konsistenzprüfung

Dieses Aktionsmodul ruft eine Versionskennung des Lightroom-Servers ab und zeigt, ob der Lightroom-Dienst derzeit ausgeführt wird.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom], siehe <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Credentials]</td>
      <td>
        <p>Wenn Sie bestimmte Anmeldeinformationen angeben möchten, um sicherzustellen, dass ein bestimmter Server ausgeführt wird, klicken Sie auf Element hinzufügen und geben Sie die Anmeldeinformationen ein.</p><p>Autorisierungs-Header werden automatisch hinzugefügt.</p>
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
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom], siehe <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Credentials]</td>
      <td>
        <p>Wenn Sie bestimmte Anmeldeinformationen angeben möchten, um sicherzustellen, dass Sie auf das richtige Benutzerkonto zugreifen können, klicken Sie auf Element hinzufügen und geben Sie die Anmeldeinformationen ein.</p><p>Autorisierungs-Header werden automatisch hinzugefügt.</p>
      </td>
    </tr>
  </tbody>
</table>

### Assets

* [Erstellen einer Asset-Originaldatei](#create-an-asset-external-xmp-develop-setting-file)
* [Erstellen eines Assets](#create-an-asset)
* [Erstellen einer externen Asset-XMP-Entwicklungs-Einstellungsdatei](#create-an-asset-external-xmp-develop-setting-file)
* [Ausgabeformate für eine Originaldatei generieren](#generate-renditions-for-an-original-file)
* [Abrufen eines Katalog-Assets](#get-a-catalog-asset)
* [Laden Sie die neuesten externen XMP für die Entwicklung von Assets herunter.](#get-the-latest-asset-external-xmp-develop-setting-file)
* [Abrufen der neuesten Asset-Ausgabedarstellung](#get-the-latest-asset-rendition)
* [Abrufen von Assets](#retrieve-assets)

#### Erstellen einer Asset-Originaldatei

Dieses Aktionsmodul erstellt und lädt eine Originaldatei für ein Asset hoch.


<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom], siehe <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die Kennung des Katalogs ein, der das Asset enthält, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset-ID]</td>
      <td>
        <p>Geben Sie die ID des Assets ein oder ordnen Sie sie zu, für das Sie eine Datei erstellen und hochladen möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Länge des Inhalts in Byte]</td>
      <td>
        <p>Geben Sie die Länge des Inhalts in Byte ein oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Byte range]</td>
      <td>
        <p>Geben Sie den Byte-Bereich für die Anforderung ein oder ordnen Sie ihn zu, einschließlich erster und letzter Byte und der Entitätslänge gemäß RFC 2616. Sollte nur eingeschlossen werden, wenn die Daten zu groß sind, um in einen einzelnen Aufruf hochgeladen werden zu können.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inhaltstyp]</td>
      <td>
        <p>Wählen Sie den Inhaltstyp für die neue Datei aus.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Erstellen eines Assets

Dieses Aktionsmodul erstellt ein neues Asset mit anfänglichen Metadaten und Importinformationen.


<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom], siehe <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die ID des Katalogs ein oder ordnen Sie sie zu, in dem das Asset erstellt wird.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset-ID]</td>
      <td>
        <p>Geben Sie die ID des neuen Assets ein oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset-Typ]</td>
      <td>
        <p>Wählen Sie aus, ob es sich bei dem Asset um ein Bild oder ein Video handelt.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datetime user created]</td>
      <td>
        <p>Datum im Format eingeben oder zuordnen <code>YYYY-MM-DDT00:00:00-00:00</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datetime user updated]</td>
      <td>
        <p>Datum im Format eingeben oder zuordnen <code>YYYY-MM-DDT00:00:00-00:00</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datum erfasst]</td>
      <td>
        <p>Datum im Format eingeben oder zuordnen <code>YYYY-MM-DDT00:00:00-00:00</code>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Erstellen einer externen Asset-XMP-Entwicklungs-Einstellungsdatei

Dieses Aktionsmodul unterstützt zwei Workflows. Der erste Workflow besteht darin, die externe XMP-Entwicklungs-Einstellungsdatei für das Asset hochzuladen. Der zweite Workflow besteht darin, eine externe XMP zu erstellen, indem eine Einstellungsdatei aus der externen xmp-Entwicklungseinstellungsdatei eines anderen Assets kopiert wird.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom], siehe <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Länge des Inhalts in Byte]</td>
      <td>
        <p>Geben Sie die Länge des Inhalts in Byte ein oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Neue XMP/Entwicklungsdatei hochladen oder kopieren]</td>
      <td>
        <p>Wählen Sie aus, ob Sie eine neue Datei hochladen oder eine Datei aus einem vorhandenen Asset kopieren.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die Kennung des Katalogs ein, der das Asset enthält, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset-ID]</td>
      <td>
        <p>Geben Sie die ID des Assets ein oder ordnen Sie sie zu, in das Sie eine Datei hochladen oder kopieren möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Link zur XMP/Entwicklungsdatei]</td>
      <td>
        <p>Geben Sie einen Link ein oder ordnen Sie ihn der Datei zu, die Sie hochladen oder kopieren möchten.</p><p>Diese Datei muss JSON beim Kopieren einer Datei oder XML beim Hochladen einer Datei sein.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Ausgabeformate für eine Originaldatei generieren

Dieses Aktionsmodul generiert asynchron Ausgabedarstellungen für eine Originaldatei.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom], siehe <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ausgabetyp(en) (durch Semikolon getrennt)]</td>
      <td>
        <p>Geben Sie den Ausgabedarstellungstyp für die Ausgabedarstellung ein, die Sie erstellen möchten. Trennen Sie bei der Eingabe mehrerer Typen diese durch ein Semikolon (;). <p>Mögliche Typen:</p><ul><li><code>fullsize</code></li><li><code>2560</code></li></ul></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Länge des Inhalts in Byte]</td>
      <td>
        <p>Geben Sie die Länge des Inhalts in Byte ein oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die Kennung des Katalogs ein, der das Asset enthält, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset-ID]</td>
      <td>
        <p>Geben Sie die ID des Assets ein oder ordnen Sie sie zu, für das Sie eine Ausgabedarstellung einer Datei erstellen möchten.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Abrufen eines Katalog-Assets

Dieses Aktionsmodul ruft Informationen zu einem einzelnen Asset in einem Katalog ab. Der Katalog muss dem Benutzer gehören, dessen Anmeldeinformationen in der in diesem Modul verwendeten Verbindung dargestellt sind.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom], siehe <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die Kennung des Katalogs ein, der das Asset enthält, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset-ID]</td>
      <td>
        <p>Geben Sie die ID des Assets ein oder ordnen Sie sie zu, für das Sie Informationen abrufen möchten.</p>
      </td>
    </tr>
  </tbody>
</table>


#### Abrufen der neuesten externen Asset-XMP zur Entwicklung einer Einstellungsdatei

Dieses Aktionsmodul ruft die letzte externe Asset-XMP-Einstellungsdatei ab.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom], siehe <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die Kennung des Katalogs ein, der das Asset enthält, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset-ID]</td>
      <td>
        <p>Geben Sie die ID des Assets ein oder ordnen Sie sie zu, das mit der XMP Entwicklungseinstellungsdatei verknüpft ist.</p>
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
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom], siehe <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die Kennung des Katalogs ein, der das Asset enthält, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset-ID]</td>
      <td>
        <p>Geben Sie die ID des Assets ein oder ordnen Sie sie zu, das mit der XMP Entwicklungseinstellungsdatei verknüpft ist.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ausgabetyp]</td>
      <td>
        <p>Wählen Sie den Ausgabetyp aus, den Sie abrufen möchten.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Abrufen von Assets

Dieses Aktionsmodul ruft Assets ab, die dem Benutzer gehören, dessen Anmeldeinformationen in der in diesem Modul verwendeten Verbindung dargestellt sind.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom], siehe <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die Kennung des Katalogs ein, der das Asset enthält, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Startzeitstempel]</td>
      <td>
        <p>Geben Sie einen Zeitstempel ein oder ordnen Sie ihn zu. Das Modul gibt Einträge zurück, die nach diesem Zeitstempel aktualisiert wurden.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Rückgabe von bereits erfassten Assets]</td>
      <td>
        <p>Datum im Format eingeben <code>YYYY-MM-DDT00:00:00</code>. Das Modul gibt Ergebnisse zurück, die vor diesem Datum erfasst wurden.</p><p> Dieses Feld kann nicht mit dem Feld verwendet werden <code>Return assets captured after</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Maximale Anzahl zurückgegebener Assets]</td>
      <td>
        <p>Legen Sie die maximale Anzahl von Assets fest, die [!DNL Workfront Fusion] wird während eines Ausführungszyklus zurückgegeben. Diese Zahl muss kleiner oder gleich 100 sein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SHA256 Hash-Wert der Originaldatei]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ausblenden von Assets in Stapeln?"]</td>
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
        <p>Geben Sie bis zu 100 Asset-IDs, durch Kommas getrennt, ein oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Typen der auszuschließenden Assets]</td>
      <td>
        <p>Wählen Sie aus, ob vollständige oder unvollständige Assets ausgeschlossen werden sollen. Lassen Sie dieses Feld leer, um alle Assets einzuschließen.</p>
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
* [Album erstellen](#create-an-album)
* [Album löschen](#delete-an-album)
* [Album abrufen](#get-an-album)
* [Auflisten von Assets eines Albums](#list-assets-of-an-album)
* [Abrufen von Alben](#retrieve-albums)
* [Aktualisieren eines Albums](#update-album)

#### Hinzufügen von Assets zu einem Album

Dieses Aktionsmodul fügt dem angegebenen Album mindestens ein Asset hinzu. Sie können bis zu 50 Assets in einem Ausführungszyklus hinzufügen.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom], siehe <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die ID des Katalogs ein oder ordnen Sie sie zu, der das Album enthält, dem Sie Assets hinzufügen möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Album-ID]</td>
      <td>
        <p>Geben Sie die Kennung des Albums ein oder ordnen Sie es zu, dem Sie Assets hinzufügen möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Assets]</td>
      <td>
        <p>Klicken Sie für jedes Asset, das Sie zum Album hinzufügen möchten, auf <b>Element hinzufügen</b> und geben Sie die folgenden Felder ein.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Asset-ID]</td>
      <td>
        <p>Geben Sie die ID des Assets ein oder ordnen Sie sie dem Album zu</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Ist dieses Asset ein Album-Titelbild?]</td>
      <td>
        <p>Wählen Sie aus, ob dieses Asset als Bild angezeigt werden soll, das das Album darstellt.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Order]</td>
      <td>
        <p></p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Metadaten]</td>
      <td>
        <p>Geben Sie alle Metadaten ein oder ordnen Sie sie dem Asset zu. Hierbei muss es sich um eine einzelne Textzeichenfolge mit einer maximalen Länge von 1-24 Zeichen handeln.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Remote ID]</td>
      <td>
        <p>Geben Sie eine Kennung für das Asset ein.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Album erstellen

Dieses Aktionsmodul erstellt ein neues Album in Lightroom.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom], siehe <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die Kennung des Katalogs ein, in dem Sie ein Album erstellen möchten, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Album-ID]</td>
      <td>
        <p>Geben Sie eine ID für das neue Album ein oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Subtype]</td>
      <td>
        <p>Wählen Sie den Untertyp für das Album aus.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL API-Schlüssel]</td>
      <td>
        <p>Geben Sie den API-Schlüssel des Dienstes ein, der das Album erstellt.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Datetime user created]</td>
      <td>
        <p>Datum im Format eingeben oder zuordnen <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datetime user updated]</td>
      <td>
        <p>Datum im Format eingeben oder zuordnen <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Albumname]</td>
      <td>
        <p>Geben Sie einen Namen für das neue Album ein oder ordnen Sie ihn zu.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Cover ID]</td>
      <td>
        <p>Geben Sie die ID eines Assets ein oder ordnen Sie sie zu, das als Titelblatt dieses Albums verwendet werden soll.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Remote ID]</td>
      <td>
        <p>Geben Sie eine Kennung für das Asset ein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Erstellungsdatum]</td>
      <td>
        <p>Datum im Format eingeben oder zuordnen <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Aktualisiertes Datum]</td>
      <td>
        <p>Datum im Format eingeben oder zuordnen <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Wird das Album gelöscht?]</td>
      <td>
        <p>Aktivieren Sie diese Option, wenn der extern verknüpfte Inhalt gelöscht wurde.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL des Standorts zum Bearbeiten von zugehörigen Inhalten]</td>
      <td>
        <p>Wenn es eine URL gibt, über die Benutzer Inhalte dieses Albums bearbeiten können, geben Sie hier die URL ein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL des Standorts zum Anzeigen von zugehörigen Inhalten]</td>
      <td>
        <p>Wenn es eine URL gibt, über die Benutzer den Inhalt dieses Albums anzeigen können, geben Sie hier die URL ein.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Album löschen

Dieses Aktionsmodul löscht ein Album.

Das gelöschte Album muss von derselben Client-App erstellt worden sein, die es jetzt löscht, und es muss vom Untertyp sein `project` oder `project_set`.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom], siehe <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die Kennung des Katalogs ein, der das zu löschende Album enthält, oder ordnen Sie es zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Album-ID]</td>
      <td>
        <p>Geben Sie die Kennung des Albums ein, das Sie löschen möchten, oder ordnen Sie es zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Untergeordnete Alben löschen?]</td>
      <td>
        <p>Wählen Sie aus, ob Sie untergeordnete Alben des gelöschten Albums löschen möchten.</p>
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
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom], siehe <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die Kennung des Katalogs ein, der das Album enthält, das Sie abrufen möchten, oder ordnen Sie es zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Album-ID]</td>
      <td>
        <p>Geben Sie die Kennung des Albums ein oder ordnen Sie sie zu.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Auflisten von Assets eines Albums

Dieses Aktionsmodul ruft eine Liste von Assets im angegebenen Album ab.



#### Abrufen von Alben

Dieses Aktionsmodul ruft eine Liste von Alben im angegebenen Katalog ab.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom], siehe <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die Kennung des Katalogs ein, der Alben enthält, die Sie abrufen möchten, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Untertypen]</td>
      <td>
        <p>Geben Sie die Kennung des Albums ein oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name des Albums, das den aktuellen Ergebnissen vorausgeht]</td>
      <td>
        <p>Wenn Sie Ihre Ergebnisse paginieren, geben Sie den Namen des letzten Albums auf der vorherigen Seite ein oder ordnen Sie ihn zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Maximale Anzahl zurückgegebener Alben]</td>
      <td>
        <p>Legen Sie die maximale Anzahl von Assets fest, die [!DNL Workfront Fusion] wird während eines Ausführungszyklus zurückgegeben. Der Standardwert für dieses Feld ist 100. Dieses Modul kann mehr Alben als diese Grenze zurückgeben, wenn mehrere Alben an der Grenze dieselbe Anzahl aufweisen <code>name_after</code> -Wert.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Album aktualisieren

Dieses Aktionsmodul aktualisiert das angegebene Album.

Das aktualisierte Album muss von derselben Client-App erstellt worden sein, die es jetzt aktualisiert, und es muss vom Untertyp sein `project` oder `project_set`.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Lightroom], siehe <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Lightroom]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Katalog-ID]</td>
      <td>
        <p>Geben Sie die Kennung des Katalogs ein, der das zu aktualisierende Album enthält, oder ordnen Sie es zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Album-ID]</td>
      <td>
        <p>Geben Sie die Kennung des Albums ein, das Sie aktualisieren möchten, oder ordnen Sie es zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Andere Felder</td>
      <td>
      <td>Beschreibungen anderer Felder in diesem Modul finden Sie unter <a href="#create-an-album" class="MCXref xref" >Album erstellen</a> in diesem Artikel.</td>
      </td>
    </tr>
  </tbody>
</table>










