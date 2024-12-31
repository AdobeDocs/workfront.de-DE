---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Bildmodule
description: Mit Adobe Workfront Fusion-Bildmodulen können Sie Informationen zu einem bestimmten Bild abrufen (Abmessungen, Typ usw.), ein Bild in ein anderes Dateiformat konvertieren und die Bildgröße direkt ändern.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 89efa9d5-00c9-4bb5-97b3-2b2f9d73721d
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '912'
ht-degree: 0%

---

# Bildmodule

[!DNL Adobe Workfront Fusion] [!UICONTROL Image]-Module können Sie Informationen zu einem bestimmten Bild abrufen (Abmessungen, Typ usw.), ein Bild in ein anderes Dateiformat konvertieren und die Größe des Bildes direkt ändern.

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

## [!UICONTROL Image]-Module und ihre Felder

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

* [[!UICONTROL Größe ändern]](#resize)
* [[!UICONTROL Format konvertieren]](#convert-a-format)
* [[!UICONTROL Extrahieren von Metadaten]](#extract-metadata)

### [!UICONTROL Größe ändern]

Dieses Transformatormodul ändert die Höhe und Breite eines Bildes entsprechend den von Ihnen angegebenen Kriterien.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie die Quelle des Bildes aus, das Sie konvertieren möchten. Sie können die Ausgabe aus einem vorherigen Modul auswählen oder die Datendatei und den Dateinamen zuordnen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Daten]</td> 
   <td>Ordnen Sie die Datei zu, die Sie konvertieren möchten. Dieses Feld ist verfügbar, wenn Sie [!UICONTROL Map] im Feld [!UICONTROL Source-Datei] ausgewählt haben.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dateiname]</td> 
   <td>Geben Sie einen Namen für die konvertierte Datei ein. Dieses Feld ist verfügbar, wenn Sie [!UICONTROL Map] im Feld [!UICONTROL Source-Datei] ausgewählt haben.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ich möchte]</td> 
   <td>Wählen Sie aus, ob Sie das Verhältnis Höhe/Breite beibehalten oder die Bemaßungen auf eine bestimmte Höhe und Breite ändern möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL nach]</td> 
   <td> <p>Wählen Sie aus, wie das Modul die neue Bildgröße bestimmen soll. Dieses Feld wird angezeigt, wenn Sie ausgewählt haben, dass das Verhältnis von Höhe zu Breite im Feld Ich möchte beibehalten werden soll. Andere Felder werden je nach Auswahl in diesem Feld angezeigt.</p> 
    <ul> 
     <li> <p>[!UICONTROL Maximale Breite]</p> <p>Reduziert ein Bild auf eine angegebene Breite. Die Höhe wird automatisch berechnet.</p> </li> 
     <li> <p>[!UICONTROL Maximale Höhe]</p> <p>Reduziert ein Bild auf eine angegebene Höhe. Die Breite wird automatisch berechnet.</p> </li> 
     <li> <p>[!UICONTROL Maximale Höhe oder Breite]</p> <p>Verringert ein Bild so, dass seine Höhe und Breite die angegebenen Werte nicht überschreiten. Da diese Option das Verhältnis von Höhe zu Breite beibehält, kann eine der Bemaßungen kleiner als angegeben sein. Wenn beispielsweise Höhe und Breite als 40 angegeben sind, wird ein Bild mit einer Größe von 400 x 300 auf 40 x 30 reduziert.</p> </li> 
     <li> <p>[!UICONTROL Mindestbreite]</p> <p>Vergrößert ein Bild auf die angegebene Breite. Die Höhe wird automatisch berechnet.</p> </li> 
     <li> <p>[!UICONTROL Mindesthöhe]</p> <p>Vergrößert ein Bild auf eine angegebene Höhe. Die Breite wird automatisch berechnet.</p> </li> 
     <li> <p>[!UICONTROL Mindesthöhe oder -breite]</p> <p>Vergrößert ein Bild so, dass seine Höhe und Breite nicht kleiner sind als die angegebenen Werte. Da diese Option das Verhältnis von Höhe zu Breite beibehält, kann eine der Bemaßungen größer als angegeben sein. Wenn beispielsweise Höhe und Breite als 300 angegeben sind, wird ein Bild im Format 40x30 auf 400x300 vergrößert.</p> </li> 
     <li> <p>[!UICONTROL Prozent]</p> <p>Ändert die Bildgröße um einen Prozentsatz basierend auf dem von Ihnen angegebenen Wert. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Breite]</td> 
   <td>Geben Sie die gewünschte Breite des skalierten Bildes in Pixel ein oder mappen Sie sie.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Höhe]</td> 
   <td>Geben Sie die gewünschte Höhe des skalierten Bildes in Pixel ein oder mappen Sie sie.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Format konvertieren]

Dieses Transformatormodul ändert das Format einer Bilddatei. Dieses Modul ist mit den folgenden Formaten kompatibel:

* PNG
* JPG
* GIF
* BMP

Sowohl die Quelldatei als auch die Ausgabe müssen in einem der folgenden Formate vorliegen. Beispielsweise kann das Modul [!UICONTROL Image] > [!UICONTROL Format konvertieren] eine PNG-Datei in eine BMP-Datei oder eine BMP in eine JPG-Datei umwandeln.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie die Quelle des Bildes aus, das Sie konvertieren möchten. Sie können die Ausgabe aus einem vorherigen Modul auswählen oder die Datendatei und den Dateinamen zuordnen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Daten]</td> 
   <td>Ordnen Sie die Datei zu, die Sie konvertieren möchten. Dieses Feld ist verfügbar, wenn Sie [!UICONTROL Map] im Feld [!UICONTROL Source-Datei] ausgewählt haben.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dateiname]</td> 
   <td>Geben Sie einen Namen für die konvertierte Datei ein. Dieses Feld ist verfügbar, wenn Sie [!UICONTROL Map] im Feld [!UICONTROL Source-Datei] ausgewählt haben.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgabeformat]</td> 
   <td>Wählen Sie das Format aus, in das das Modul die Quelldatei konvertieren soll. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Extrahieren von Metadaten]

Dieses Transformatormodul gibt grundlegende Informationen über ein Modul zurück.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie die Quelle des Bildes aus, das Sie konvertieren möchten. Sie können die Ausgabe aus einem vorherigen Modul auswählen oder die Datendatei und den Dateinamen zuordnen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Daten]</td> 
   <td>Ordnen Sie die Datei zu, die Sie konvertieren möchten. Dieses Feld ist verfügbar, wenn Sie im Feld [!UICONTROL Source-Datei] die Option Zuordnung ausgewählt haben.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dateiname]</td> 
   <td>Geben Sie einen Namen für die konvertierte Datei ein. Dieses Feld ist verfügbar, wenn Sie im Feld [!UICONTROL Source-Datei] die Option Zuordnung ausgewählt haben.</td> 
  </tr> 
 </tbody> 
</table>

## Mögliche Probleme

### Aktion mit Fehler beendet

In drei Fällen kann eine Aktion mit einem Fehler beendet werden:

* Die empfangenen Daten liegen nicht im JPG/GIF/PNG/BMP-Format vor
* Die maximale Breite/Höhe wurde beim Ändern der Bildabmessungen überschritten. Die Bildgröße darf 3840 Pixel Breite und 2160 Pixel Höhe nicht überschreiten
* Die maximal zulässige Größe eines Bildes wurde beim Ändern der Abmessungen oder des Formats des Bildes überschritten.
