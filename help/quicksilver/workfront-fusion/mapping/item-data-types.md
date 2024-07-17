---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Elementdatentypen in  [!DNL Adobe Workfront Fusion]
description: Ihre [!DNL Adobe Workfront Fusion] Szenarien können die Typen von Elementen enthalten, die unten in einem Bundle aufgeführt sind.
author: Becky
feature: Workfront Fusion
exl-id: 36c25a86-0d05-4871-a6a6-4fd54cfcc4b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---

# Elementdatentypen in [!DNL Adobe Workfront Fusion]

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz*</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Elementdatentypen

Sie können die unten aufgeführten Elementtypen in einem Bundle enthalten.

Informationen darüber, welche Elementtypen [!DNL Workfront Fusion] die Konvertierung zwischen einander ermöglichen, finden Sie unter [Typerzwingung in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Text</p> </td> 
   <td> <p>Der gängigste Elementtyp. Bei einigen Textelementen überprüft [!DNL Adobe Workfront Fusion], ob die maximal zulässige Länge oder die minimale zulässige Länge eingehalten wird oder ob das Element eine Formatüberprüfung durchführt (E-Mail, URL oder Dateiname).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Zahl</p> </td> 
   <td> <p>Bei einigen numerischen Elementen kann [!DNL Workfront Fusion] die Eingabe für einen bestimmten Bereich (den erlaubten Mindest- oder Maximalwert) validieren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Boolesch (Ja/Nein)</p> </td> 
   <td> <p>Dieser Typ wird für Elemente mit nur zwei möglichen Werten verwendet: true oder false. </p> <p>Beim Festlegen von Modulen kann der boolesche Typ in zwei verschiedenen Formularen angezeigt werden:</p> 
    <ul> 
     <li> <p>Das Kontrollkästchen Pflichtfeld wird angezeigt, wenn das Feld Pflichtfeld ist und ausgefüllt werden muss.</p> <p> <img src="assets/boolean-checkbox-350x158.jpg" style="width: 350;height: 158;"> </p> </li> 
     <li> <p>Optionale Felder, die leer gelassen werden können, werden als Auswahlfeld angezeigt, sodass unter drei Werten ausgewählt werden kann: <code>Yes</code>, <code>No</code> und <code>Not defined</code> (Standard).</p> <p> <img src="assets/boolean-convert-file-350x129.jpg" style="width: 350;height: 129;"> </p> </li> 
    </ul> <p>Sie können auf <strong>[!UICONTROL Map]</strong> klicken, wenn Sie den Wert einem Element aus einem anderen Modul zuordnen müssen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Datum</p> </td> 
   <td> <p>Datumsangaben werden im Datumsformat nach ISO 8601 eingegeben, z. B. <code>2015-09-18T11:58Z</code>. Sie können die Zeitzone in Ihren Profileinstellungen ändern, wie unter <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">Profileinstellungen in [!DNL Adobe Workfront Fusion]</a> ändern. </p> <p>Wenn Sie auf ein Feld klicken, für das ein Datum erforderlich ist, wird in den Moduleinstellungen ein Popup-Kalender angezeigt. Die Zeit ist für einige Elemente nicht erforderlich.</p> <p>Die Werte der Datumselemente werden mithilfe der in Ihrem Profil ausgewählten lokalen und Web-Zeitzone formatiert. Sie können die ISO 8601-Version des Werts eines Datumselements anzeigen, indem Sie den Mauszeiger über das Element bewegen.</p> <p>Hinweis: Wenn der ISO-Wert nicht angezeigt wird, ist das Element wahrscheinlich Text, kein Datum.</p> <p>Die Uhrzeit wird im Format <code>hours:minutes:seconds</code> eingegeben, z. B. <code>14:03:52</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Puffer (binäre Daten)</p> </td> 
   <td> <p>Dateiinhalt wird normalerweise als Inhalt vom Typ "Puffer"(Bildinhalt, Videodatei usw.) gesendet. In einigen Fällen sind Textdaten in diesem Typ enthalten (z. B. eine Textdatei). [!DNL Workfront Fusion] kann Textdaten im Binärcode automatisch in Text und Text in Textdaten im Binärcode konvertieren. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/mapping/about-mapping-files.md" class="MCXref xref">Über die Zuordnung von Dateien in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Sammlung</p> </td> 
   <td> <p>Eine Sammlung ist ein Element, das aus mehreren Unterelementen besteht. Das Element Absender in einer E-Mail-Nachricht ist ein Beispiel für eine Kollektion: Es enthält den Absendernamen (Texttyp) und die Absender-E-Mail-Adresse (Texttyp).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Auswählen (Menü)</p> </td> 
   <td> <p>Wenn Sie die Moduleinstellungen wie in <a href="../../workfront-fusion/modules/configure-a-modules-settings.md" class="MCXref xref">Einstellungen eines Moduls in [!DNL Adobe Workfront Fusion]</a> konfigurieren, können Sie aus mehreren Elementen desselben Typs auswählen. Ein Beispiel ist das Menü zur Ordnerauswahl in den Einstellungen für die [!DNL Dropbox] -Module. </p> <p>Beim Festlegen von Modulen kann das Auswahlmenü in zwei Formularen angezeigt werden:</p> <p> <p>Wenn eine Mehrfachauswahl möglich ist, werden mehrere Elemente mit Kontrollkästchen angezeigt.</p> <p> <img src="assets/image-kb-type-list-multi-350x232.jpg" style="width: 350;height: 232;"> </p> </p> <p>Wenn nur eine Option möglich ist, wird ein Dropdown-Menü angezeigt.</p> <p> <img src="assets/select-menu-dropdown-350x130.jpg" style="width: 350;height: 130;"> </p> <p>Wenn Sie ein Element aus einem anderen Modul zuordnen müssen, verwenden Sie die Schaltfläche <strong>Zuordnung</strong> . Diese Schaltfläche öffnet ein Textfeld anstelle des Auswahlmenüs. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref">Zuordnen von Informationen von einem Modul zu einem anderen in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Array</p> </td> 
   <td> <p>Sie können den Array-Typ verwenden, um mit mehreren Werten desselben Typs zu arbeiten, einschließlich Sammlungen. Ein Beispiel sind die [!UICONTROL E-Mail]-Module: Sie geben ein Array von Anlagen zurück und jede Anlage enthält Namen, Inhalt, Größe usw. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/mapping/map-an-array.md" class="MCXref xref">Zuordnen eines Arrays in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Validierung</p> </td> 
   <td> <p>[!DNL Workfront Fusion] kann eine Überprüfung für jeden Elementtyp durchführen. Wenn ein Element die Validierung nicht besteht, stoppt das Modul die Verarbeitung aufgrund eines Datenfehlers. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/errors/error-processing.md" class="MCXref xref">Fehlerverarbeitung in [!DNL Adobe Workfront Fusion]</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
