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
exl-id: f20192ea-e363-4fba-8bd2-b1d50443918d
source-git-commit: 5b2de063836c2cf668e14edfbc5a12f9321d26ca
workflow-type: tm+mt
source-wordcount: '3966'
ht-degree: 0%

---

# [!DNL Adobe Photoshop] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL Adobe Photoshop] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.


Wenn Sie Anweisungen zum Erstellen eines Szenarios benötigen, finden Sie weitere Informationen unter [Erstellen eines Szenarios](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Zugriffsanforderungen

+++**Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.**

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
      <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</td>
    </tr>
    </tr>
  </tbody>
</table>


&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

&#42;&#42;Informationen zu [!DNL Adobe Workfront Fusion] Lizenzen finden Sie unter [!DNL [Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

+++

## Voraussetzungen

Bevor Sie den Connector [!DNL Adobe Photoshop] verwenden können, müssen Sie sicherstellen, dass die folgenden Voraussetzungen erfüllt sind:

* Sie müssen über ein aktives [!DNL Adobe Photoshop] -Konto verfügen.

## Erstellen einer Verbindung zu [!DNL Adobe Photoshop]

So erstellen Sie eine Verbindung für Ihre [!DNL Adobe Photoshop] -Module:

1. Klicken Sie neben dem Feld Verbindung auf **[!UICONTROL Hinzufügen]** .

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
        <td>Geben Sie Ihren [!DNL Adobe] [!UICONTROL Client Secret] ein. Dies finden Sie im [!UICONTROL Credentials]-Detailabschnitt des [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL ID des technischen Kontos]</td>
        <td>Geben Sie Ihre [!DNL Adobe] [!UICONTROL ID des technischen Kontos] ein. Dies finden Sie im [!UICONTROL Credentials]-Detailabschnitt des [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Organisations-ID]</td>
        <td>Geben Sie Ihre [!DNL Adobe] [!UICONTROL Organisations-ID] ein. Dies finden Sie im [!UICONTROL Credentials]-Detailabschnitt des [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Privater Schlüssel]</td>
        <td>
          <p>Geben Sie den privaten Schlüssel ein, der beim Erstellen Ihrer Anmeldedaten in der [!DNL Adobe Developer Console] generiert wurde. </p>
          <p>So extrahieren Sie Ihren privaten Schlüssel oder Ihr Zertifikat:</p>
          <ol>
            <li value="1">
              <p>Klicken Sie auf <b>[!UICONTROL Extract]</b>.</p>
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
              <p>Klicken Sie auf <b>Speichern</b> , um die Datei zu extrahieren und zum Setup der Verbindung zurückzukehren.</p>
            </li>
          </ol>
        </td>
        </tr>
      </tbody>
    </table>

1. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindung zu speichern und zum Modul zurückzukehren.

## [!DNL Adobe Photoshop] Module und ihre Felder

Wenn Sie [!DNL Adobe Photoshop] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Adobe Photoshop] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Anwenden von Photoshop-Bearbeitungen](#apply-psd-edits)
* [Automatische Farbkorrektur eines Bildes](#auto-color-correct-an-image)
* [Bildformat konvertieren](#convert-image-format)
* [Erstellen von Masken](#create-a-mask)
* [Neue PSD erstellen](#create-a-new-psd)
* [Bearbeiten von Textebenen](#edit-text-layers)
* [Execute Depth Blur](#execute-depth-blur)
* [Ausführen von Photoshop-Aktionen](#execute-photoshop-actions)
* [Ausführen von Photoshop-Aktionen (JSON)](#execute-photoshop-actions-json)
* [Ausführen des Produkt-Zuschnitts](#execute-product-crop)
* [Ebeneninformationen abrufen](#get-layer-info)
* [Benutzerdefinierte API-Aufrufe durchführen](#make-a-custom-api-call)
* [Hintergrund entfernen](#remove-background)
* [Ersetzen eines Smart-Objekts](#replace-a-smart-object)
* [Größe eines Bildes ändern](#resize-an-image)
* [Bild mit Wasserzeichen versehen](#watermark-an-image)

### Anwenden von PSD-Bearbeitungen

Dieses Aktionsmodul wendet eine Vielzahl von Bearbeitungen auf Dokument- und Ebenenebene an.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Photoshop] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Photoshop]</a> .</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Input) Speicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem die zu bearbeitende Datei gespeichert ist.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Speicherort der [!UICONTROL (Eingabe)-Datei]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad der Datei ein, die Sie bearbeiten möchten, oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Optionen &gt; Dokument &gt; Bildgröße) Höhe]</p>
      </td>
      <td> Geben Sie die Höhe des Bildes in Pixel ein oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Optionen &gt; Dokument &gt; Bildgröße) Breite]</p>
      </td>
      <td> Geben Sie die Breite des Bildes in Pixel ein oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Optionen &gt; Dokument &gt; Arbeitsflächengröße) Oben]</p>
      </td>
   <td> Geben Sie die Y-Koordinate der linken oberen Ecke des Dokuments ein oder ordnen Sie sie in Pixel zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Optionen &gt; Dokument &gt; Arbeitsflächengröße) Unten</p>
      </td>
   <td> Geben Sie die Y-Koordinate der rechten unteren Ecke des Dokuments ein oder ordnen Sie sie in Pixel zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Optionen &gt; Dokument &gt; Arbeitsflächengröße) Links]</p>
      </td>
   <td> Geben Sie die X-Koordinate der linken oberen Ecke des Dokuments ein oder ordnen Sie sie in Pixel zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Optionen &gt; Dokument &gt; Arbeitsflächengröße) Rechts</p>
      </td>
   <td> Geben Sie die X-Koordinate der rechten unteren Ecke des Dokuments ein oder ordnen Sie sie in Pixel zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Optionen &gt; Dokument) Zuschnitt]</p>
      </td>
   <td> Wählen Sie Transparente Pixel aus, um den Schnitt auf transparenten Pixeln im Bild zu basieren. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Optionen) Standardschrift]</p>
      </td>
   <td> Geben Sie den vollständigen Postscript-Namen der Schrift ein, die als globaler Standard für das Dokument verwendet werden soll. Diese Schrift wird für alle Textebenen verwendet, die eine fehlende Schrift aufweisen und für diese Ebene keine andere Schrift speziell bereitgestellt wurde. Wenn diese Schriftart fehlt, wird die unter "Verwalten fehlender Schriftarten"angegebene Option wirksam. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Optionen) Schriftarten]</p>
      </td>
   <td> Klicken Sie für jede Schriftart, die das Dokument benötigt, auf Element hinzufügen und geben Sie den Speicherort der Schriftart und den Speicherort der Datei ein. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Optionen) Verwalten fehlender Schriftarten]</p>
      </td>
   <td> Wählen Sie die Aktion aus, die ausgeführt werden soll, wenn mindestens eine Schriftart im Dokument fehlt. <ul><li><code>fail</code>: Der Auftrag wird nicht erfolgreich ausgeführt und der Status wird auf "Fehlgeschlagen"gesetzt, wobei die Details des Fehlers im Detailabschnitt im Status angegeben werden.</li><li><code>useDefault</code>: Der Auftrag wird jedoch erfolgreich sein, standardmäßig werden alle fehlenden Schriftarten durch ArialMT ersetzt.</li></ul></td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Options-)Ebenen]</p>
      </td>
   <td> Klicken Sie für jede Ebene, die Sie hinzufügen möchten, auf Element hinzufügen und füllen Sie die Ebenendetails aus. <p>Weitere Informationen zu Ebenenoptionen finden Sie unter <a href="https://developer.adobe.com/firefly-services/docs/photoshop/api/photoshop_applyPsdEdits/">Anwenden von PSD-Bearbeitungen</a> in der Adobe Photoshop-Dokumentation.  </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ausgaben]</td>
      <td>
        <p>Klicken Sie für jede zu erstellende konvertierte Datei auf Element hinzufügen und geben Sie den Speicherort, den Speicherort und den Typ wie in dieser Tabelle aufgeführt ein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Speicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem die neue Datei gespeichert werden soll.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) File location]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad ein, in dem die neue Datei gespeichert werden soll, oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) Type]</p>
      </td>
   <td>Wählen Sie den Dateityp aus, in den Sie die Datei konvertieren möchten. </td> 
    </tr>
    <tr>
      <td role="rowheader">Überschreiben von [!UICONTROL (Ausgabe)]</td>
      <td>
        <p>Wählen Sie aus, ob die neu bearbeitete Datei bereits existierende Ausgabedateien überschreibt. Dies gilt nur für Dateien im Adobe-Speicher.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximale Anzahl an zurückgegebenen Ergebnissen]</p>
      </td>
   <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td> 
    </tr>
    </tbody>
</table>



### Automatische Farbkorrektur eines Bildes

Diese automatische Farbe des Aktionsmoduls korrigiert das angegebene Bild.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Photoshop] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Photoshop]</a> .</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Input) Speicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem die Datei gespeichert ist, deren Farbe korrekt dargestellt werden soll.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Speicherort der [!UICONTROL (Eingabe)-Datei]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad der Datei ein, deren Farbe Sie korrigieren möchten, oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Speicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem die neue Datei gespeichert werden soll.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) File location]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad ein, in dem die neue Datei gespeichert werden soll, oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) Type]</p>
      </td>
   <td>Wählen Sie den Dateityp aus, in den Sie die Datei konvertieren möchten. </td> 
    </tr>
    <tr>
      <td role="rowheader">Überschreiben von [!UICONTROL (Ausgabe)]</td>
      <td>
        <p>Wählen Sie aus, ob die neu bearbeitete Datei bereits existierende Ausgabedateien überschreibt. Dies gilt nur für Dateien im Adobe-Speicher.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximale Anzahl an zurückgegebenen Ergebnissen]</p>
      </td>
   <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td> 
    </tr>
    </tbody>
</table>


### Bildformat konvertieren

Dieses Aktionsmodul konvertiert eine Datei in JPEG, PNG, PSD oder TIFF.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Photoshop] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Photoshop]</a> .</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Input) Speicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, aus dem die Datei gespeichert ist, aus der Sie den Hintergrund entfernen möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Speicherort der [!UICONTROL (Eingabe)-Datei]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad der Datei ein oder ordnen Sie sie zu, aus der Sie den Hintergrund entfernen möchten. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ausgaben]</td>
      <td>
        <p>Klicken Sie für jede zu erstellende konvertierte Datei auf Element hinzufügen und geben Sie den Speicherort, den Speicherort und den Typ wie in dieser Tabelle aufgeführt ein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Speicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem die neue Datei gespeichert werden soll.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) File location]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad ein, in dem die neue Datei gespeichert werden soll, oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) Type]</p>
      </td>
   <td>Wählen Sie den Dateityp aus, in den Sie die Datei konvertieren möchten. </td> 
    </tr>
    <tr>
      <td role="rowheader">Überschreiben von [!UICONTROL (Ausgabe)]</td>
      <td>
        <p>Wählen Sie aus, ob die neu bearbeitete Datei bereits existierende Ausgabedateien überschreibt. Dies gilt nur für Dateien im Adobe-Speicher.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximale Anzahl an zurückgegebenen Ergebnissen]</p>
      </td>
   <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td> 
    </tr>
    </tbody>
</table>



### Erstellen von Masken

Dieses Aktionsmodul gibt eine PNG-Datei mit einem Mast zurück, der um den Betreff angewendet wird.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Photoshop] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Photoshop]</a> .</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Input) Speicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, aus dem die Datei gespeichert wird, aus der Sie eine Maske erstellen möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Speicherort der [!UICONTROL (Eingabe)-Datei]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad der Datei ein oder ordnen Sie sie zu, aus der Sie eine Maske erstellen möchten. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Speicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem die Maskendatei gespeichert werden soll.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) File location]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad ein, in dem die Maskendatei gespeichert werden soll, oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Wählen Sie aus, ob die neu bearbeitete Datei bereits existierende Ausgabedateien überschreibt. Dies gilt nur für Dateien im Adobe-Speicher.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Farbraum]</p>
      </td>
   <td>Wählen Sie aus, ob das Ausgabebild die Farbe RGB oder RGBA verwendet. </td> 
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Mask format]</p>
      </td>
   <td>Wählen Sie aus, ob die Maske weich (gefedert) oder binär sein soll. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Optimize]</p>
      </td>
   <td>Wählen Sie Leistung , um die Geschwindigkeit zu optimieren, oder Batch , um Wartezeiten zu ermöglichen. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Nachbearbeitungsprozess]</p>
      </td>
   <td></td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Version]</p>
      </td>
   <td>Der Standardwert ist 4.0.</td> 
    </tr> 
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximale Anzahl an zurückgegebenen Ergebnissen]</p>
      </td>
   <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td> 
    </tr>
    </tbody>
</table>

### Neue PSD erstellen

Dieses Aktionsmodul erstellt eine neue PSD mit optionalen Ebenen und generiert Ausgabedarstellungen oder speichert sie als PSD.

Informationen zu Feldern, die sich auf dieses Modul beziehen, finden Sie unter [Erstellen einer neuen PSD](https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/documentCreate) in der Adobe Photoshop-Dokumentation.

### Bearbeiten von Textebenen

Dieses Aktionsmodul bearbeitet Textebenen in einer Photoshop-Datei.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Photoshop] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Photoshop]</a> .</td>
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

### Execute Depth Blur

Dieses Aktionsmodul führt die Tiefenschärfe für die ausgewählte Datei aus.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Photoshop] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Photoshop]</a> .</td>
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
        <p>Weitere Informationen zu anderen Optionen für den Tiefenunschärfenschärfe finden Sie unter <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/depthBlur">Execute Depth Blur </a> in der Dokumentation zur Adobe Photoshop-API.</p>
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

### Ausführen von Photoshop-Aktionen

Dieses Aktionsmodul führt eine Photoshop-Aktion für das ausgewählte Bild aus.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Photoshop] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Photoshop]</a> .</td>
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

### Ausführen von Photoshop-Aktionen (JSON)

Dieses Aktionsmodul führt Photoshop-Aktionen mithilfe von JSON-Befehlen aus.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Photoshop] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Photoshop]</a> .</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Input) Speicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem die zu bearbeitende Datei gespeichert ist.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Speicherort der [!UICONTROL (Eingabe)-Datei]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad der Datei ein, die Sie bearbeiten möchten, oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Action JSON]</td>
      <td>
        <p>Geben Sie den JSON-Befehl für die Aktion ein, die Sie ausführen möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Schriftarten/Muster/Pinsel/Zusätzliche Bilder]</td>
      <td>
        <p>Klicken Sie für jede Schrift, jedes Muster, jede Bürste oder jedes zusätzliche Bild, das Sie in dieser Aktion verwenden möchten, auf Element hinzufügen und geben Sie den Speicherort und den Speicherort des Elements ein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Schriftart/Muster/Pinseldatei-URL]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad der Datei ein, die Sie verwenden möchten, oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dateispeicher ausgibt]</td>
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
    <tr>
      <td role="rowheader">[!UICONTROL Ausgaben]</td>
      <td>
        <p>Klicken Sie für jede zu erstellende konvertierte Datei auf Element hinzufügen und geben Sie den Speicherort, den Speicherort und den Typ wie in dieser Tabelle aufgeführt ein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Speicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem die neue Datei gespeichert werden soll.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) File location]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad ein, in dem die neue Datei gespeichert werden soll, oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) Type]</p>
      </td>
   <td>Wählen Sie den Dateityp aus, in den Sie die Datei konvertieren möchten. </td> 
    </tr>
    <tr>
      <td role="rowheader">Überschreiben von [!UICONTROL (Ausgabe)]</td>
      <td>
        <p>Wählen Sie aus, ob die neu bearbeitete Datei bereits existierende Ausgabedateien überschreibt. Dies gilt nur für Dateien im Adobe-Speicher.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximale Anzahl an zurückgegebenen Ergebnissen]</p>
      </td>
   <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td> 
    </tr>
      </tbody>
</table>

### Ausführen des Produkt-Zuschnitts

Dieses Aktionsmodul führt das Zuschneiden auf dem ausgewählten Bild aus.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Photoshop] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Photoshop]</a> .</td>
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

### Ebeneninformationen abrufen

Dieses Aktionsmodul ruft Ebeneninformationen aus der angegebenen PSD-Datei ab.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Photoshop] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Photoshop]</a> .</td>
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

### Benutzerdefinierte API-Aufrufe durchführen

Dieses Aktionsmodul führt einen benutzerdefinierten Aufruf an die Photoshop-API durch.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Photoshop] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Photoshop]</a> .</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Geben Sie einen Pfad relativ zu <code>https://image.adobe.io/pie/psdService</code> ein. Beispiel: <code>/photoshopActions</code></p>
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
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> in Ihrer JSON platzieren Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

### Hintergrund entfernen

Dieses Aktionsmodul identifiziert den Hauptbetreff des Bildes und entfernt den Hintergrund.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Photoshop] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Photoshop]</a> .</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Input) Speicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, aus dem die Datei gespeichert ist, aus der Sie den Hintergrund entfernen möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Speicherort der [!UICONTROL (Eingabe)-Datei]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad der Datei ein oder ordnen Sie sie zu, aus der Sie den Hintergrund entfernen möchten. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Speicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem die neue Datei gespeichert werden soll.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) File location]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad ein, in dem die neue Datei gespeichert werden soll, oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Wählen Sie aus, ob die neu bearbeitete Datei bereits existierende Ausgabedateien überschreibt. Dies gilt nur für Dateien im Adobe-Speicher.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Farbraum]</p>
      </td>
   <td>Wählen Sie aus, ob das Ausgabebild die Farbe RGB oder RGBA verwendet. </td> 
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Mask format]</p>
      </td>
   <td>Wählen Sie aus, ob die Kanten des Bildes weich (gefedert) oder binär sein sollen. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Optimize]</p>
      </td>
   <td>Wählen Sie Leistung , um die Geschwindigkeit zu optimieren, oder Batch , um Wartezeiten zu ermöglichen. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Nachbearbeitungsprozess]</p>
      </td>
   <td></td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Version]</p>
      </td>
   <td>Der Standardwert ist 4.0.</td> 
    </tr> 
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximale Anzahl an zurückgegebenen Ergebnissen]</p>
      </td>
   <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td> 
    </tr>
    </tbody>
</table>



### Ersetzen eines Smart-Objekts

Dieses Aktionsmodul ersetzt ein Smart-Objekt innerhalb einer PSD-Ebene und generiert neue Ausgabedarstellungen.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Photoshop] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Photoshop]</a> .</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Input) Speicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem das Smart-Objekt gespeichert ist.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Speicherort der [!UICONTROL (Eingabe)-Datei]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad des Smart-Objekts ein oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Layers]</p>
      </td>
   <td>Klicken Sie für jede Ebene, die Sie dem Smart-Objekt hinzufügen möchten, auf Element hinzufügen und geben Sie den Namen oder die ID des Objekts, den Dateidienst, in dem das Smart-Objekt gespeichert ist, sowie die URL oder den Pfad der Ebene ein.<p>Beschreibungen der erweiterten Einstellungen in diesem Bereich finden Sie unter <a href="https://developer.adobe.com/firefly-services/docs/photoshop/api/photoshop_replaceSmartObject/">Ersetzen eines Smart-Objekts</a> in der Dokumentation zur Photoshop-API </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ausgaben]</td>
      <td>
        <p>Klicken Sie für jede neue Ausgabedarstellung, die das Modul erstellen soll, auf Element hinzufügen und füllen Sie die folgenden Felder aus. Sie können maximal 25 Ausgabedateien haben.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Speicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem die neue Datei gespeichert werden soll.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) File location]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad ein, in dem die neue Datei gespeichert werden soll, oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) Breite]</p>
      </td>
   <td> Die Breite der Ausgabedatei in Pixel. Das Modul behält das ursprüngliche Seitenverhältnis bei. </td> 
    </tr>
    <tr>
      <td role="rowheader">Überschreiben von [!UICONTROL (Ausgabe)]</td>
      <td>
        <p>Wählen Sie aus, ob die neu bearbeitete Datei bereits existierende Ausgabedateien überschreibt. Dies gilt nur für Dateien im Adobe-Speicher.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximale Anzahl an zurückgegebenen Ergebnissen]</p>
      </td>
   <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td> 
    </tr>
    </tbody>
</table>



### Größe eines Bildes ändern

Durch diese Aktion wird die Größe eines Bildes unter Verwendung des gleichen Seitenverhältnisses geändert.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Photoshop] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Photoshop]</a> .</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Speicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem die Datei gespeichert wird, deren Größe Sie ändern möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Dateispeicherort]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad der Datei ein, deren Größe Sie ändern möchten, oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ausgaben]</td>
      <td>
        <p>Klicken Sie für jede zu erstellende konvertierte Datei auf Element hinzufügen und geben Sie den Speicher, den Speicherort und andere Optionen ein, die in dieser Tabelle aufgeführt sind.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Typ]</p>
      </td>
   <td>Wählen Sie den Dateityp aus, in den Sie die Datei konvertieren möchten. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Breite]</p>
      </td>
   <td>Geben Sie eine Zahl ein, die die Breite des in der Größe angepassten Bildes in Pixel darstellt. Das Seitenverhältnis wird beibehalten.</td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Max. Breite]</p>
      </td>
   <td>Wenn die Breite 0 beträgt, kann Max. mit angegeben werden, um die Größe zu erhalten. Die maximale Breite hat Vorrang, da sie kleiner als die Dokumentbreite ist.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Wählen Sie aus, ob die neu bearbeitete Datei bereits existierende Ausgabedateien überschreibt. Dies gilt nur für Dateien im Adobe-Speicher.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Zuschneiden auf Arbeitsfläche]</p>
      </td>
   <td>Wählen Sie Ja , um die Ausgabedarstellungen auf die Leinwandgröße zu kürzen, oder Nein , um die Ebenengröße der Ausgabedarstellungen festzulegen.</td> 
    </tr>
    </tbody>
</table>

### Bild mit Wasserzeichen versehen

Dieses Aktionsmodul fügt dem ausgewählten Bild ein Wasserzeichen hinzu.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Photoshop] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Photoshop]</a> .</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Basis-/Eingabe-Speicher)</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem die Datei gespeichert ist, der Sie ein Wasserzeichen hinzufügen möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Speicherort der [!UICONTROL (Basis-/Eingabedatei)</p>
      </td>
   <td> Geben Sie die URL oder den Pfad der Datei ein oder ordnen Sie sie zu, der Sie ein Wasserzeichen hinzufügen möchten. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Wasserzeichen/Eingabe) Speicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem das Wasserzeichen, das Sie hinzufügen möchten, gespeichert wird.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Wasserzeichen/Eingabe) Speicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem das Wasserzeichen, das Sie hinzufügen möchten, gespeichert wird.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Wasserzeichen/Grenzen) Höhe]</p>
      </td>
   <td>Geben Sie die gewünschte Höhe des Wasserzeichens in Pixel ein oder ordnen Sie sie zu.</td> 
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Wasserzeichen/Grenzen) Breite]</p>
      </td>
   <td> Geben Sie die gewünschte Breite des Wasserzeichens in Pixel ein oder ordnen Sie sie zu. </td> 
    </tr>  
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Wasserzeichen/Grenzen) Links]</p>
      </td>
   <td> Geben Sie den Abstand (in Pixel) von der linken Seite des Bildes ein, den das Wasserzeichen aufweisen soll.</td> 
    </tr>  
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Wasserzeichen/Grenzen oben)</p>
      </td>
   <td> Geben Sie den Abstand (in Pixel) vom oberen Rand des Bildes ein, den das Wasserzeichen aufweisen soll.</td> 
    </tr>  
    </tr>  
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Speicher]</td>
      <td>
        <p>Wählen Sie den Dateidienst aus, in dem die mit Wasserzeichen versehene Datei gespeichert werden soll.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) File location]</p>
      </td>
   <td> Geben Sie die URL oder den Pfad ein, in dem die mit Wasserzeichen versehene Datei gespeichert werden soll, oder ordnen Sie sie zu. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) Type]</p>
      </td>
   <td>Wählen Sie den Dateityp aus, in den Sie die Datei konvertieren möchten. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) Breite]</p>
      </td>
   <td> Die Breite der Ausgabedatei in Pixel. Das Modul behält das ursprüngliche Seitenverhältnis bei. </td> 
    </tr>
    <tr>
      <td role="rowheader">Überschreiben von [!UICONTROL (Ausgabe)]</td>
      <td>
        <p>Wählen Sie aus, ob die neu bearbeitete Datei bereits existierende Ausgabedateien überschreibt. Dies gilt nur für Dateien im Adobe-Speicher.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximale Anzahl an zurückgegebenen Ergebnissen]</p>
      </td>
   <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td> 
    </tr>
    </tbody>
</table>















