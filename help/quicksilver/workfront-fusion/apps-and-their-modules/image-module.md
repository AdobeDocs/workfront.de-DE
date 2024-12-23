---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Bildmodule
description: Mit den Adobe Workfront Fusion Image-Modulen können Sie Informationen zu einem bestimmten Bild (Abmessungen, Typ usw.) abrufen, ein Bild in ein anderes Dateiformat konvertieren und die Bildgröße direkt ändern.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 89efa9d5-00c9-4bb5-97b3-2b2f9d73721d
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '912'
ht-degree: 0%

---

# Bildmodule

Mit den [!DNL Adobe Workfront Fusion] [!UICONTROL Bild] -Modulen können Sie Informationen zu einem bestimmten Bild (Dimensionen, Typ usw.) abrufen, ein Bild in ein anderes Dateiformat konvertieren und die Bildgröße direkt ändern.

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

## [!UICONTROL Bild] -Module und ihre Felder

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

* [[!UICONTROL Größe ändern]](#resize)
* [[!UICONTROL Konvertieren eines Formats]](#convert-a-format)
* [[!UICONTROL Metadaten extrahieren]](#extract-metadata)

### [!UICONTROL Größe ändern]

Dieses Transformatormodul ändert die Höhe und Breite eines Bildes gemäß den von Ihnen festgelegten Kriterien.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie die Quelle des Bildes aus, das Sie konvertieren möchten. Sie können die Ausgabe aus einem vorherigen Modul auswählen oder die Datendatei und den Dateinamen zuordnen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Daten]</td> 
   <td>Ordnen Sie die Datei zu, die Sie konvertieren möchten. Dieses Feld ist verfügbar, wenn Sie [!UICONTROL Map] im Feld [!UICONTROL Source-Datei] ausgewählt haben.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dateiname]</td> 
   <td>Geben Sie einen Namen für die konvertierte Datei ein. Dieses Feld ist verfügbar, wenn Sie [!UICONTROL Map] im Feld [!UICONTROL Source-Datei] ausgewählt haben.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ich möchte]</td> 
   <td>Wählen Sie aus, ob Sie das Verhältnis von Höhe und Breite beibehalten oder die Abmessungen in eine bestimmte Höhe und Breite ändern möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL laut</td> 
   <td> <p>Wählen Sie aus, wie das Modul die neue Bildgröße bestimmen soll. Dieses Feld wird angezeigt, wenn Sie im Feld "I will to"(Ich möchte die Breite der Höhe beibehalten) ausgewählt haben. Andere Felder werden je nach Auswahl in diesem Feld angezeigt.</p> 
    <ul> 
     <li> <p>[!UICONTROL Maximale Breite]</p> <p>Reduziert ein Bild auf eine von Ihnen festgelegte Breite. Die Höhe wird automatisch berechnet.</p> </li> 
     <li> <p>[!UICONTROL Maximale Höhe]</p> <p>Reduziert ein Bild auf eine von Ihnen angegebene Höhe. Die Breite wird automatisch berechnet.</p> </li> 
     <li> <p>[!UICONTROL Maximale Höhe oder Breite]</p> <p>Reduziert ein Bild so, dass seine Höhe und Breite die von Ihnen angegebenen Werte nicht überschreiten. Da bei dieser Option das Verhältnis von Höhe und Breite beibehalten wird, kann eine der Dimensionen kleiner als angegeben sein. Wenn beispielsweise Höhe und Breite jeweils als 40 angegeben sind, wird ein Bild der Größe 400 x 300 auf 40 x 30 reduziert.</p> </li> 
     <li> <p>[!UICONTROL Mindestbreite]</p> <p>Vergrößert ein Bild auf eine von Ihnen festgelegte Breite. Die Höhe wird automatisch berechnet.</p> </li> 
     <li> <p>[!UICONTROL Mindesthöhe]</p> <p>Vergrößert ein Bild auf eine von Ihnen angegebene Höhe. Die Breite wird automatisch berechnet.</p> </li> 
     <li> <p>[!UICONTROL Mindesthöhe oder -breite]</p> <p>Vergrößert ein Bild so, dass seine Höhe und Breite nicht kleiner sind als die von Ihnen angegebenen Werte. Da bei dieser Option das Verhältnis von Höhe und Breite beibehalten wird, kann eine der Dimensionen größer sein als angegeben. Wenn beispielsweise Höhe und Breite jeweils als 300 angegeben sind, wird ein Bild der Größe 40 x 30 auf 400 x 300 vergrößert.</p> </li> 
     <li> <p>[!UICONTROL Prozent]</p> <p>Ändert die Bildgröße um einen Prozentwert basierend auf dem angegebenen Wert. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Breite]</td> 
   <td>Geben Sie die gewünschte Breite des in der Größe angepassten Bildes in Pixel ein oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Höhe]</td> 
   <td>Geben Sie die gewünschte Höhe des in der Größe angepassten Bildes in Pixel ein oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Konvertieren eines Formats]

Dieses Transformatormodul ändert das Format einer Bilddatei. Dieses Modul ist mit den folgenden Formaten kompatibel:

* PNG
* JPG
* GIF
* BMP

Sowohl die Quelldatei als auch die Ausgabe müssen in einem dieser Formate vorliegen. Beispielsweise kann das Modul [!UICONTROL Bild] >[!UICONTROL Format konvertieren] eine PNG-Datei in eine BMP-Datei oder eine BMP in eine JPG umwandeln.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie die Quelle des Bildes aus, das Sie konvertieren möchten. Sie können die Ausgabe aus einem vorherigen Modul auswählen oder die Datendatei und den Dateinamen zuordnen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Daten]</td> 
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

### [!UICONTROL Metadaten extrahieren]

Dieses Transformatormodul gibt grundlegende Informationen zu einem Modul zurück.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie die Quelle des Bildes aus, das Sie konvertieren möchten. Sie können die Ausgabe aus einem vorherigen Modul auswählen oder die Datendatei und den Dateinamen zuordnen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Daten]</td> 
   <td>Ordnen Sie die Datei zu, die Sie konvertieren möchten. Dieses Feld ist verfügbar, wenn Sie im Feld [!UICONTROL Source-Datei] die Option Karte ausgewählt haben.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dateiname]</td> 
   <td>Geben Sie einen Namen für die konvertierte Datei ein. Dieses Feld ist verfügbar, wenn Sie im Feld [!UICONTROL Source-Datei] die Option Karte ausgewählt haben.</td> 
  </tr> 
 </tbody> 
</table>

## Mögliche Probleme

### Aktion mit Fehler beendet

Es gibt drei Fälle, in denen eine Aktion mit einem Fehler beendet werden kann:

* Die empfangenen Daten lagen nicht im Format JPG/GIF/PNG/BMP vor.
* Die maximale Breite/Höhe wurde beim Ändern der Bildabmessungen überschritten. Die Bildgröße darf 3840 Pixel Breite und 2160 Pixel Höhe nicht überschreiten
* Die maximal zulässige Größe eines Bildes wurde beim Ändern der Abmessungen oder des Formats des Bildes überschritten.
