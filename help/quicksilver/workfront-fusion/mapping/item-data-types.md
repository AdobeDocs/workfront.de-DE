---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Elementdatentypen in [!DNL Adobe Workfront Fusion]
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 36c25a86-0d05-4871-a6a6-4fd54cfcc4b1
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 1%

---

# Elementdatentypen in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Elementdatentypen](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/mapping-panel/data-types/item-data-types.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] Lizenz**</td> 
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

## Elementdatentypen

Sie können die unten aufgeführten Elementtypen in einem Bundle enthalten.

Informationen dazu, welche Elementtypen [!DNL Workfront Fusion] Konvertierungen untereinander ermöglichen, finden Sie unter [Typzwang in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Text</p> </td> 
   <td> <p>Der häufigste Elementtyp. Bei einigen Textelementen prüft [!DNL Adobe Workfront Fusion], ob die maximal oder minimal zulässige Länge erreicht wird oder ob das Element eine Formatvalidierung (E-Mail, URL oder Dateiname) durchführt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Zahl</p> </td> 
   <td> <p>Bei einigen numerischen Elementen können [!DNL Workfront Fusion] die Eingabe für einen bestimmten Bereich (den minimal oder maximal zulässigen Wert) überprüfen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Boolesch (ja/nein)</p> </td> 
   <td> <p>Dieser Typ wird für Elemente mit nur zwei möglichen Werten verwendet: true oder false. </p> <p>Beim Festlegen von Modulen kann der boolesche Typ in zwei verschiedenen Formen angezeigt werden:</p> 
    <ul> 
     <li> <p>Das Kontrollkästchen Pflichtfeld wird angezeigt, wenn das Feld Pflichtfeld ist und ausgefüllt werden muss.</p> <p> <img src="assets/boolean-checkbox-350x158.jpg" style="width: 350;height: 158;"> </p> </li> 
     <li> <p>Optionale Felder, die leer gelassen werden können, werden als Auswahlfeld angezeigt, sodass aus drei Werten ausgewählt werden kann: <code>Yes</code>, <code>No</code> und <code>Not defined</code> (Standard).</p> <p> <img src="assets/boolean-convert-file-350x129.jpg" style="width: 350;height: 129;"> </p> </li> 
    </ul> <p>Sie können auf <strong>[!UICONTROL Map]</strong> klicken, wenn Sie den Wert einem Element aus einem anderen Modul zuordnen müssen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Datum</p> </td> 
   <td> <p>Datumsangaben werden im ISO 8601-Datumsformat eingegeben, z. B. <code>2015-09-18T11:58Z</code>. Sie können die Zeitzone in Ihren Profileinstellungen ändern, wie unter <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">Ändern von Profileinstellungen in [!DNL Adobe Workfront Fusion]</a> beschrieben. </p> <p>Wenn Sie auf ein Feld klicken, für das ein Datum erforderlich ist, wird in den Moduleinstellungen ein Popup-Kalender angezeigt. Bei einigen Elementen ist keine Zeit erforderlich.</p> <p>Die Werte von Datumselementen werden mithilfe der in Ihrem Profil ausgewählten lokalen Zeitzone und Web-Zeitzone formatiert. Sie können die ISO 8601-Version des Werts eines Datumselements anzeigen, indem Sie den Mauszeiger über das Element bewegen.</p> <p>Hinweis: Wenn der ISO-Wert nicht angezeigt wird, ist das Element wahrscheinlich Text, kein Datum.</p> <p>Die Uhrzeit wird im <code>hours:minutes:seconds</code> Format eingegeben, z. B. <code>14:03:52</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Puffer (Binärdaten)</p> </td> 
   <td> <p>Dateiinhalte werden normalerweise als Inhalte vom Typ „Puffer“ gesendet (Bildinhalte, Videodateien und andere). In einigen Fällen sind in diesem Typ Textdaten enthalten (z. B. eine Textdatei). [!DNL Workfront Fusion] ist in der Lage, Textdaten im Binärcode automatisch in Text und Text in Textdaten im Binärcode zu konvertieren. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/mapping/about-mapping-files.md" class="MCXref xref">Über Zuordnungsdateien in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Sammlung</p> </td> 
   <td> <p>Eine Sammlung ist ein Element, das aus mehreren Unterelementen besteht. Das Absenderelement in einer E-Mail-Nachricht ist ein Beispiel für eine Sammlung: Es enthält den Absendernamen (Texttyp) und die Absender-E-Mail-Adresse (Texttyp).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Auswählen (Menü)</p> </td> 
   <td> <p>Wenn Sie die Moduleinstellungen konfigurieren, wie in <a href="../../workfront-fusion/modules/configure-a-modules-settings.md" class="MCXref xref">Konfigurieren der Moduleinstellungen in [!DNL Adobe Workfront Fusion]</a> beschrieben, können Sie aus mehreren Elementen desselben Typs auswählen. Ein Beispiel hierfür ist das Menü Ordnerauswahl in den Einstellungen für die [!DNL Dropbox]. </p> <p>Beim Festlegen von Modulen kann das Auswahlmenü in zwei Formen angezeigt werden:</p> <p> <p>Wenn die Mehrfachauswahl möglich ist, werden mehrere Elemente mit Kontrollkästchen angezeigt.</p> <p> <img src="assets/image-kb-type-list-multi-350x232.jpg" style="width: 350;height: 232;"> </p> </p> <p>Wenn nur eine Option möglich ist, wird ein Dropdown-Menü angezeigt.</p> <p> <img src="assets/select-menu-dropdown-350x130.jpg" style="width: 350;height: 130;"> </p> <p>Wenn Sie ein Element aus einem anderen Modul zuordnen müssen, verwenden Sie die Schaltfläche <strong>Map</strong>. Mit dieser Schaltfläche wird ein Textfeld anstelle des Auswahlmenüs geöffnet. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref">Zuordnen von Informationen von einem Modul zu einem anderen in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Array</p> </td> 
   <td> <p>Sie können den Array-Typ verwenden, um mit mehreren Werten desselben Typs zu arbeiten, einschließlich Sammlungen. Ein Beispiel sind die [!UICONTROL E-Mail]-Module: Sie geben ein Array von Anlagen zurück und jede Anlage enthält Namen, Inhalt, Größe usw. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/mapping/map-an-array.md" class="MCXref xref">Zuordnen eines Arrays in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Validierung</p> </td> 
   <td> <p>[!DNL Workfront Fusion] kann für jeden Elementtyp eine Validierung durchführen. Wenn ein Element die Validierung nicht besteht, stoppt das Modul die Verarbeitung aufgrund eines Datenfehlers. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/errors/error-processing.md" class="MCXref xref">Fehlerverarbeitung in [!DNL Adobe Workfront Fusion]</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
