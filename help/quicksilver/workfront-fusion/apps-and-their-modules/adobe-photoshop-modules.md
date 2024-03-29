---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Adobe Photoshop-Module
description: Mit den Adobe Photoshop-Modulen können Sie ein Adobe Workfront Fusion-Szenario starten, das auf Ereignissen in Ihrem Adobe Photoshop-Konto basiert, Vereinbarungen und andere Datensätze erstellen, lesen oder aktualisieren, nach Datensätzen anhand von von Ihnen festgelegten Kriterien suchen und Dokumente hochladen.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
source-git-commit: 8d6f8217a58459539c9e4f4faa43e01d17d6ecee
workflow-type: tm+mt
source-wordcount: '1549'
ht-degree: 0%

---

# [!DNL Adobe Photoshop] Module

In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL Adobe Photoshop], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.


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

Bevor Sie die [!DNL Adobe Photoshop] müssen Sie sicherstellen, dass die folgenden Voraussetzungen erfüllt sind:

* Sie müssen über eine aktive [!DNL Adobe Photoshop] -Konto.

## Erstellen Sie eine Verbindung zu [!DNL Adobe Photoshop]

So erstellen Sie eine Verbindung für [!DNL Adobe Photoshop] -Module:

1. Klicks **[!UICONTROL Hinzufügen]** neben dem Feld Verbindung .

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
        <td role="rowheader">[!UICONTROL Client-ID]</td>
        <td>Geben Sie Ihre [!UICONTROL Adobe] [!UICONTROL Client ID] ein. Dies finden Sie im [!UICONTROL Credentials]-Detailabschnitt des [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Geben Sie Ihre [!DNL Adobe] [!UICONTROL Client Secret]. Dies finden Sie im [!UICONTROL Credentials]-Detailabschnitt des [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL ID des technischen Kontos]</td>
        <td>Geben Sie Ihre [!DNL Adobe] [!UICONTROL Technische Konto-ID]. Dies finden Sie im [!UICONTROL Credentials]-Detailabschnitt des [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Organisations-ID]</td>
        <td>Geben Sie Ihre [!DNL Adobe] [!UICONTROL Organisations-ID]. Dies finden Sie im [!UICONTROL Credentials]-Detailabschnitt des [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Privater Schlüssel]</td>
        <td>
          <p>Geben Sie den privaten Schlüssel ein, der beim Erstellen Ihrer Anmeldedaten im [!DNL Adobe Developer Console]. </p>
          <p>So extrahieren Sie Ihren privaten Schlüssel oder Ihr Zertifikat:</p>
          <ol>
            <li value="1">
              <p>Klicks <b>[!UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>Wählen Sie den Dateityp aus, den Sie extrahieren.</p>
            </li>
            <li value="3">
              <p>Wählen Sie die Datei aus, die den privaten Schlüssel oder das Zertifikat enthält.</p>
            </li>
            <li value="4">
              <p>Geben Sie das Kennwort für die Datei ein.</p>
            </li>
            <li value="5">
              <p>Klicks <b>Speichern</b> , um die Datei zu extrahieren und zur Einrichtung der [!UICONTROL ]e-Verbindung zurückzukehren.</p>
            </li>
          </ol>
        </td>
        </tr>
      </tbody>
    </table>

1. Klicks **[!UICONTROL Weiter]** , um die Verbindung zu speichern und zum Modul zurückzukehren.

## [!DNL Adobe Photoshop] Module und ihre Felder

Bei der Konfiguration [!DNL Adobe Photoshop] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Adobe Photoshop] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


### Aktionen

* [Neue PSD erstellen](#create-a-new-psd)
* [Bearbeiten von Textebenen](#edit-text-layers)
* [Execute Depth Blur](#execute-depth-blur)
* [Ausführen von Photoshop-Aktionen](#execute-photoshop-actions)
* [Ausführen des Produkt-Zuschnitts](#execute-product-crop)
* [Ebeneninformationen abrufen](#get-layer-info)
* [Benutzerdefinierte API-Aufrufe durchführen](#make-a-custom-api-call)

#### Neue PSD erstellen

Dieses Aktionsmodul erstellt eine neue PSD mit optionalen Ebenen und generiert Ausgabedarstellungen oder speichert sie als PSD.

Informationen zu Feldern, die sich auf dieses Modul beziehen, finden Sie unter [Neue PSD erstellen](https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/documentCreate) in der Adobe Photoshop-Dokumentation.

#### Bearbeiten von Textebenen

Dieses Aktionsmodul bearbeitet Textebenen in einer Photoshop-Datei.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Photoshop], siehe <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Photoshop]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dateispeicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem die zu bearbeitende Datei gespeichert ist.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad der Datei ein, die Sie bearbeiten möchten, oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Verwalten fehlender Schriftarten]</td>
      <td>
        <p>Wählen Sie die Aktion aus, die ausgeführt werden soll, wenn mindestens eine Schriftart im Dokument fehlt. Wenn die Schriftart nicht angegeben ist, verwendet das Modul die Standardschriftart.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Standardschrift]  </td>
      <td>
        <p>Geben Sie den vollständigen Postscript-Namen der Schrift ein, die als globaler Standard für das Dokument verwendet werden soll. Diese Schrift wird für alle Textebenen verwendet, die eine fehlende Schrift aufweisen und für diese Ebene keine andere Schrift speziell bereitgestellt wurde. Wenn diese Schriftart fehlt, wird die unter "Verwalten fehlender Schriftarten"angegebene Option wirksam.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Layers]</td>
   <td> <p>Weitere Informationen zu Ebenenoptionen finden Sie unter <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/text">Bearbeiten der Textebene</a> in der Adobe Photoshop-Dokumentation.</p>  </td>     </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Output file storage]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem die bearbeitete Datei gespeichert werden soll.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL der Ausgabedatei]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad ein, in dem die bearbeitete Datei gespeichert werden soll, oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file type]</p>
      </td>
   <td> Wählen Sie den Dateityp für die bearbeitete Datei aus. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Wählen Sie aus, ob die neu bearbeitete Datei bereits existierende Ausgabedateien überschreibt.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Komprimierung]</p>
      </td>
   <td> Wählen Sie die Komprimierungsstufe für die Ausgabedatei aus. </td> 
    </tr>
  </tbody>
</table>

#### Execute Depth Blur

Dieses Aktionsmodul führt die Tiefenschärfe für die ausgewählte Datei aus.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Photoshop], siehe <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Photoshop]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dateispeicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem die zu bearbeitende Datei gespeichert ist.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad der Datei ein, die Sie bearbeiten möchten, oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Output file storage]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem die bearbeitete Datei gespeichert werden soll.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL der Ausgabedatei]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad ein, in dem die bearbeitete Datei gespeichert werden soll, oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file type]</p>
      </td>
   <td> Wählen Sie den Dateityp für die bearbeitete Datei aus. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Andere Felder]</td>
      <td>
        <p>Weitere Informationen zu anderen Optionen für den Tiefenunschärfen finden Sie unter <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/depthBlur">Execute Depth Blur </a>in der Dokumentation zur Adobe Photoshop-API.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Wählen Sie aus, ob die neu bearbeitete Datei bereits existierende Ausgabedateien überschreibt.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Komprimierung]</p>
      </td>
   <td> Wählen Sie die Komprimierungsstufe für die Ausgabedatei aus. </td> 
    </tr>
  </tbody>
</table>

#### Ausführen von Photoshop-Aktionen

Dieses Aktionsmodul führt eine Photoshop-Aktion für das ausgewählte Bild aus.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Photoshop], siehe <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Photoshop]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dateispeicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem die zu bearbeitende Datei gespeichert ist.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad der Datei ein, die Sie bearbeiten möchten, oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Aktionen file storage]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem die Aktionsdatei gespeichert wird.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Aktionsdatei-URL]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad der Aktionsdatei ein oder ordnen Sie sie zu. </td> 
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Aktionsname]</p>
      </td>
   <td> Wenn Sie nur eine bestimmte Aktion ausführen möchten, können Sie im ActionSet angeben, welche Aktion wiedergegeben werden soll. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Font/Pattern/Pinselspeicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem die Datei gespeichert ist, die Sie verwenden möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Schriftart/Muster/Pinseldatei-URL]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad der Datei ein, die Sie verwenden möchten, oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Output file storage]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem die bearbeitete Datei gespeichert werden soll.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL der Ausgabedatei]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad ein, in dem die bearbeitete Datei gespeichert werden soll, oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file type]</p>
      </td>
   <td> Wählen Sie den Dateityp für die bearbeitete Datei aus. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Wählen Sie aus, ob die neu bearbeitete Datei bereits existierende Ausgabedateien überschreibt.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Komprimierung]</p>
      </td>
   <td> Wählen Sie die Komprimierungsstufe für die Ausgabedatei aus. </td> 
    </tr>
  </tbody>
</table>

#### Ausführen des Produkt-Zuschnitts

Dieses Aktionsmodul führt das Zuschneiden auf dem ausgewählten Bild aus.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Photoshop], siehe <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Photoshop]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dateispeicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem die zu schneidende Datei gespeichert ist.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad der Datei ein, die Sie zuschneiden möchten, oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Unit]</p>
      </td>
   <td> Wählen Sie aus, ob Sie die Höhenanpassung in Pixel oder in Prozent beschreiben möchten. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Breite]</p>
      </td>
   <td> Geben Sie den Breitenabstand ein oder ordnen Sie ihn zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Höhe]</p>
      </td>
   <td> Geben Sie den Umfang des hinzuzufügenden Höhenabstands ein oder ordnen Sie ihn zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Output file storage]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem die bearbeitete Datei gespeichert werden soll.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL der Ausgabedatei]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad ein, in dem die bearbeitete Datei gespeichert werden soll, oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file type]</p>
      </td>
   <td> Wählen Sie den Dateityp für die bearbeitete Datei aus. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Wählen Sie aus, ob die neu bearbeitete Datei bereits existierende Ausgabedateien überschreibt.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Komprimierung]</p>
      </td>
   <td> Wählen Sie die Komprimierungsstufe für die Ausgabedatei aus. </td> 
    </tr>
  </tbody>
</table>

#### Ebeneninformationen abrufen

Dieses Aktionsmodul ruft Ebeneninformationen aus der angegebenen PSD-Datei ab.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Photoshop], siehe <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Photoshop]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dateispeicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, aus dem die Datei gespeichert ist, aus der Sie Ebeneninformationen abrufen möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad der Datei ein oder ordnen Sie sie zu, aus der Sie Ebeneninformationen abrufen möchten. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Miniaturansichten]</p>
      </td>
   <td> </td> 
    </tr>
  </tbody>
</table>

#### Benutzerdefinierte API-Aufrufe durchführen

Dieses Aktionsmodul führt einen benutzerdefinierten Aufruf an die Photoshop-API durch.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Photoshop], siehe <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Photoshop]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Geben Sie einen Pfad relativ zu ein <code>https://image.adobe.io/pie/psdService</code>. Beispiel: <code>/photoshopActions</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Methode]</p>
      </td>
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Header]</td>
      <td>
        <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p>
        <p>Beispiel: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] fügt automatisch Autorisierungskopfzeilen hinzu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Abfragezeichenfolge]  </td>
      <td>
        <p>Geben Sie die Abfragezeichenfolge der Anfrage ein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> Fügen Sie die Anführungszeichen in Ihre JSON-Datei außerhalb der bedingten Anweisung ein.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

