---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connector
navigation-topic: apps-and-their-modules
title: Microsoft OneDrive-Module
description: In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die OneDrive verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 13a25c6c-bdf1-467d-bd90-ebd763c59235
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '4073'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL OneDrive] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

Wenn Sie Anweisungen zum Erstellen eines Szenarios benötigen, finden Sie weitere Informationen unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## Voraussetzungen

Um [!DNL OneDrive] -Module zu verwenden, müssen Sie über ein [!DNL Microsoft OneDrive] -Konto verfügen.




## Verbinden des [!DNL OneDrive]-Dienstes mit [!DNL Workfront Fusion]

Anweisungen zum Verbinden Ihres [!DNL OneDrive]-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter [Erstellen einer Verbindung mit [!UICONTROL Adobe Workfront Fusion] - Grundlegende Anweisungen](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Einige Microsoft-Apps verwenden dieselbe Verbindung, die an individuelle Benutzerberechtigungen gebunden ist. Daher werden beim Erstellen einer Verbindung im Bildschirm für die Genehmigung von Berechtigungen alle Berechtigungen angezeigt, die zuvor für die Verbindung dieses Benutzers gewährt wurden, zusätzlich zu den neuen Berechtigungen, die für die aktuelle Anwendung erforderlich sind.
>
>Wenn beispielsweise ein Benutzer über den Excel-Connector über die Berechtigung &quot;Tabelle lesen&quot;verfügt und dann im Outlook-Connector eine Verbindung zum Lesen von E-Mails erstellt, zeigt der Bildschirm für die Genehmigung der Berechtigungen sowohl die bereits erteilte Berechtigung &quot;Tabelle lesen&quot;als auch die neu erforderliche Berechtigung &quot;E-Mail schreiben&quot;an.

## [!DNL Microsoft OneDrive] Module und ihre Felder

Wenn Sie [!DNL OneDrive] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL OneDrive] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Datei/Ordner](#filefolder)
* [Sonstige](#other)

### Datei/Ordner

* [[!UICONTROL Dateien/Ordner überwachen]](#watch-filesfolders)
* [[!UICONTROL Dateien/Ordner durchsuchen]](#search-filesfolders)
* [[!UICONTROL Datei abrufen]](#get-a-file)
* [[!UICONTROL Datei herunterladen]](#download-a-file)
* [[!UICONTROL  Datei hochladen]](#upload-a-file)
* [[!UICONTROL Erstellen eines Ordners]](#create-a-folder)
* [[!UICONTROL Einen Freigabe-Link abrufen]](#get-a-share-link)
* [[!UICONTROL Verschieben einer Datei/eines Ordners]](#move-a-filefolder)
* [[!UICONTROL Eine Datei kopieren]](#copy-a-file)
* [[!UICONTROL Datei/Ordner löschen]](#delete-a-filefolder)

#### [!UICONTROL Dateien/Ordner überwachen]

Dieses Trigger-Modul startet ein Szenario, wenn eine Datei oder ein Ordner erstellt oder aktualisiert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL OneDrive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Überwachte Dateien/Ordner]</td> 
   <td> <p>Wählen Sie aus, wie Sie Dateien oder Ordner überwachen möchten:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Nach Erstellungszeit]</b> </p> <p>Suchen Sie nach neuen Dateien oder Ordnern.</p> </li> 
     <li> <p><b>[!UICONTROL Nach Aktualisierungszeit]</b> </p> <p>Suchen Sie nach aktualisierten vorhandenen Dateien oder Ordnern.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] Standort auswählen]</td> 
   <td> <p>Wählen Sie den Standort aus, den Sie überwachen möchten:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mein Laufwerk]</b> </p> <p>Wählen Sie aus, ob das Modul eine Laufwerk-ID eingeben soll.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Ja]</b> </p> <p>Geben Sie die ID des Laufwerks ein, das das Modul überwachen soll.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> <p>Navigieren Sie zu dem Ordner, den das Modul überwachen soll. Sie können auch eine Abfrage eingeben, um die zurückgegebenen Ergebnisse zu filtern.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Für mich freigegeben]</b> </p> <p>Das Modul überwacht Dateien, die für den Eigentümer des Laufwerks freigegeben wurden.</p> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Wählen Sie die SharePoint-Site aus, die das Modul überwachen soll. Verfügbare Sites sind Sites , gefolgt vom angemeldeten Benutzer.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Wählen Sie die Gruppe aus, deren Laufwerk das Modul überwachen soll.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elementtyp auswählen]</td> 
   <td> <p>Wählen Sie aus, ob Sie Dateien, Ordner oder beides ansehen möchten.</p> <p>Hinweis: Sie können nicht auf Ordner in einem [!UICONTROL Shared For Me]-Laufwerk achten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>



#### [!UICONTROL Dateien/Ordner durchsuchen]

Dieses Suchmodul gibt Dateien und Ordner basierend auf von Ihnen festgelegten Kriterien zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL OneDrive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] Standort auswählen]</td> 
   <td> <p>Wählen Sie den Standort aus, den Sie suchen möchten:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mein Laufwerk]</b> </p> <p>Wählen Sie aus, ob das Modul eine Laufwerk-ID eingeben soll.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Ja]</b> </p> <p>Geben Sie die Kennung des Laufwerks ein, nach dem das Modul suchen soll.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> <p>Navigieren Sie zu dem Ordner, nach dem das Modul suchen soll. Sie können auch eine Abfrage eingeben, um die zurückgegebenen Ergebnisse zu filtern.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Für mich freigegeben]</b> </p> <p>Das Modul sucht Dateien, die für den Eigentümer des Laufwerks freigegeben wurden.</p> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Wählen Sie die [!DNL SharePoint]-Site aus, die das Modul durchsuchen soll. Verfügbare Sites sind Sites , gefolgt vom angemeldeten Benutzer.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Wählen Sie die Gruppe aus, deren Laufwerk das Modul durchsuchen soll.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elementtyp auswählen]</td> 
   <td> <p>Wählen Sie aus, ob Sie nach Dateien, Ordnern oder beidem suchen möchten.</p> <p>Hinweis: Sie können nicht nach Ordnern in einem [!UICONTROL Shared For Me]-Laufwerk suchen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei abrufen]

Dieses Aktionsmodul ruft die Metadaten einer angegebenen Datei ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL OneDrive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eingabetaste (Datei-ID und Dateipfad)]</td> 
   <td>Wählen Sie aus, ob die Datei anhand der Datei-ID oder des Dateipfads identifiziert werden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datei-ID eingeben] / [!UICONTROL Dateipfad]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Datei-ID oder den Dateipfad eingeben möchten:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Manuell eingeben]</b> </p> <p>Wählen Sie diese Option aus, wenn Sie die ID oder den Pfad direkt eingeben oder sie einem vorherigen Modul zuordnen möchten.</p> </li> 
     <li> <p><b>[!UICONTROL Auswahl aus einer Liste]</b> </p> <p>Wählen Sie diese Option aus, wenn Sie aus einer Liste der verfügbaren Dateien oder Pfade auswählen möchten. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] Standort auswählen]</td> 
   <td> <p>Wählen Sie den Standort aus, den Sie suchen möchten:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mein Laufwerk]</b> </p> <p>Wählen Sie aus, ob das Modul eine Laufwerk-ID eingeben soll.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Ja]</b> </p> <p>Geben Sie die Kennung des Laufwerks ein, das die gewünschte Datei enthält.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Wählen Sie die SharePoint-Site aus, die die gewünschte Datei enthält. Verfügbare Sites sind Sites , gefolgt vom angemeldeten Benutzer.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Wählen Sie die Gruppe aus, deren Laufwerk die gewünschte Datei enthält.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Wählen Sie das Laufwerk aus oder ordnen Sie es zu, das die gewünschte Datei enthält. Dieses Feld ist nicht verfügbar, wenn Sie im Feld [!UICONTROL Enable to Enter a Drive ID] die Option [!UICONTROL No] ausgewählt haben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datei] / [!UICONTROL Datei-ID] / [!UICONTROL Dateipfad]</td> 
   <td> <p>Wenn Sie die Option [!UICONTROL Manuell eingeben] ausgewählt haben, geben Sie die Datei-ID oder den Pfad der Datei ein, die Sie abrufen möchten.</p> <p>Wenn Sie [!UICONTROL Auswahl aus der Liste] ausgewählt haben, wählen Sie die gewünschte Datei aus.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei herunterladen]

Dieses Aktionsmodul lädt die angegebene Datei herunter.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL OneDrive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eingabetaste (Datei-ID und Dateipfad)]</td> 
   <td>Wählen Sie aus, ob die Datei anhand der Datei-ID oder des Dateipfads identifiziert werden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Datei-ID/Dateipfad eingeben</td> 
   <td> <p>Wählen Sie aus, wie Sie die Datei-ID oder den Dateipfad eingeben möchten:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Manuell eingeben]</b> </p> <p>Wählen Sie diese Option aus, wenn Sie die ID oder den Pfad direkt eingeben oder sie einem vorherigen Modul zuordnen möchten.</p> </li> 
     <li> <p><b>[!UICONTROL Auswahl aus einer Liste]</b> </p> <p>Wählen Sie diese Option aus, wenn Sie aus einer Liste der verfügbaren Dateien oder Pfade auswählen möchten. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] Standort auswählen]</td> 
   <td> <p>Wählen Sie den Speicherort aus, der die herunterzuladende Datei enthält:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mein Laufwerk]</b> </p> <p>Wählen Sie aus, ob das Modul eine Laufwerk-ID eingeben soll.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Ja]</b> </p> <p>Geben Sie die ID des Laufwerks ein, das die herunterzuladende Datei enthält.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Wählen Sie die SharePoint-Site aus, die die herunterzuladende Datei enthält. Verfügbare Sites sind Sites , gefolgt vom angemeldeten Benutzer.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Wählen Sie die Gruppe aus, deren Laufwerk die Datei enthält, die Sie herunterladen möchten.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Wählen Sie das Laufwerk aus oder ordnen Sie es zu, das die herunterzuladende Datei enthält. Dieses Feld ist nicht verfügbar, wenn Sie im Feld [!UICONTROL Enable to Enter a Drive ID] die Option [!UICONTROL No] ausgewählt haben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datei] / [!UICONTROL Datei-ID] / [!UICONTROL Dateipfad]</td>
   <td> <p>Wenn Sie die Option [!UICONTROL Manuell eingeben] ausgewählt haben, geben Sie die Datei-ID oder den Pfad der Datei ein, die Sie herunterladen möchten.</p> <p>Wenn Sie [!UICONTROL Auswahl aus der Liste] ausgewählt haben, wählen Sie die Datei aus, die Sie herunterladen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL In PDF konvertieren]</td> 
   <td> <p>Aktivieren Sie diese Option, um die Datei in eine PDF-Datei zu konvertieren. Sie können aus den folgenden Dateitypen konvertieren:</p> 
    <table style="table-layout:auto"> 
     <col> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td> 
        <ul> 
         <li> <p> <p>CSV</p> </p> </li> 
         <li> <p> <p>DOC</p> </p> </li> 
         <li> <p> <p>DOCX</p> </p> </li> 
         <li> <p> <p>ODP</p> </p> </li> 
         <li> <p> <p>ODS</p> </p> </li> 
         <li> <p> <p>ODT</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p> <p>POT</p> </p> </li> 
         <li> <p> <p>POTM</p> </p> </li> 
         <li> <p> <p>POTX</p> </p> </li> 
         <li> <p> <p>PPS</p> </p> </li> 
         <li> <p> <p>PPSX</p> </p> </li> 
         <li> <p> <p>PPSXM</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p>PPT</p> </li> 
         <li> <p>PPTM</p> </li> 
         <li> <p>PPTX</p> </li> 
         <li> <p>RTF</p> </li> 
         <li> <p>XLS</p> </li> 
         <li> <p>XLSX</p> </li> 
        </ul> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL  Datei hochladen]

Dieses Aktionsmodul lädt eine Datei in den angegebenen Ordner hoch.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL OneDrive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Eingabetaste (Ordnerspeicherort-ID und -pfad)</td> 
   <td>Wählen Sie aus, ob Sie den Zielordner anhand der Kennung oder anhand eines Pfads identifizieren möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] Standort auswählen]</td> 
   <td> <p>Wählen Sie den Speicherort aus, an den Sie eine Datei hochladen möchten:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mein Laufwerk]</b> </p> <p>Wählen Sie aus, ob das Modul eine Laufwerk-ID eingeben soll.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Ja]</b> </p> <p>Wählen Sie das Laufwerk aus, das die gewünschte Datei enthält.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Wählen Sie die [!DNL SharePoint]-Site aus, die den Ordner enthält, in den Sie eine Datei hochladen möchten. Verfügbare Sites sind Sites , gefolgt vom angemeldeten Benutzer.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Wählen Sie die Gruppe aus, deren Laufwerk den Ordner enthält, in den Sie eine Datei hochladen möchten.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Wählen Sie das Laufwerk aus, das den Ordner enthält, in den Sie eine Datei hochladen möchten. Dieses Feld ist nicht verfügbar, wenn Sie im Feld [!UICONTROL Enable to Enter a Drive ID] die Option [!UICONTROL No] ausgewählt haben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Wenn die Datei mit demselben Namen vorhanden ist,</td> 
   <td>Wählen Sie aus, wie verfahren werden soll, wenn bereits eine Datei mit demselben Namen existiert.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Beschreibung]</td> 
   <td>Fügen Sie der hochgeladenen Datei eine Beschreibung hinzu.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Erstellen eines Ordners]

Dieses Aktionsmodul erstellt einen neuen Ordner im angegebenen Laufwerk.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL OneDrive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] Standort auswählen]</td> 
   <td> <p>Wählen Sie den Speicherort aus, an dem Sie einen Ordner erstellen möchten:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mein Laufwerk]</b> </p> <p>Wählen Sie aus, ob das Modul eine Laufwerk-ID eingeben soll.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Ja]</b> </p> <p>Wählen Sie das Laufwerk aus, auf dem Sie einen Ordner erstellen möchten.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Wählen Sie die [!DNL SharePoint]-Site aus, auf der Sie einen Ordner erstellen möchten. Verfügbare Sites sind Sites , gefolgt vom angemeldeten Benutzer.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Wählen Sie die Gruppe aus, der der Ordner gehört, in dem Sie einen Ordner erstellen möchten.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Wählen Sie das Laufwerk aus, auf dem Sie einen Ordner erstellen möchten. Dieses Feld ist nicht verfügbar, wenn Sie im Feld [!UICONTROL Enable to Enter a Drive ID] die Option [!UICONTROL No] ausgewählt haben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner]</td> 
   <td>Wenn der neue Ordner ein Unterordner sein soll, navigieren Sie zu dem Ordner, in dem sich der Ordner befinden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Neuer Ordnername]</td> 
   <td> <p>Geben Sie einen Namen für den neuen Ordner ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Wenn der Ordner mit demselben Namen vorhanden ist</td> 
   <td>Wählen Sie aus, wie verfahren werden soll, wenn bereits eine Datei mit demselben Namen existiert.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Einen Freigabe-Link abrufen]

Dieses Aktionsmodul gibt einen Freigabe-Link für die angegebene Datei zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL OneDrive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eingabetaste (Datei-ID und Dateipfad)]</td> 
   <td>Wählen Sie aus, ob die Datei anhand der Datei-ID oder des Dateipfads identifiziert werden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datei-ID eingeben] / [!UICONTROL Dateipfad]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Datei-ID oder den Dateipfad eingeben möchten:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Manuell eingeben]</b> </p> <p>Wählen Sie diese Option aus, wenn Sie die ID oder den Pfad direkt eingeben oder sie einem vorherigen Modul zuordnen möchten.</p> </li> 
     <li> <p><b>[!UICONTROL Auswahl aus einer Liste]</b> </p> <p>Wählen Sie diese Option aus, wenn Sie aus einer Liste der verfügbaren Dateien oder Pfade auswählen möchten. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] Standort auswählen]</td> 
   <td> <p>Wählen Sie den Speicherort aus, für den Sie einen Freigabe-Link abrufen möchten:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mein Laufwerk]</b> </p> <p>Wählen Sie aus, ob das Modul eine Laufwerk-ID eingeben soll.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Ja]</b> </p> <p>Geben Sie die ID des Laufwerks ein, das die Datei enthält, für die Sie einen Freigabe-Link abrufen möchten.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Wählen Sie die SharePoint-Site aus, die die Datei enthält, für die Sie einen Freigabe-Link abrufen möchten. Verfügbare Sites sind Sites , gefolgt vom angemeldeten Benutzer.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Wählen Sie die Gruppe aus, deren Laufwerk die Datei enthält, für die Sie einen Freigabe-Link abrufen möchten.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Wählen Sie das Laufwerk aus oder ordnen Sie es zu, das die Datei enthält, für die Sie einen Freigabe-Link abrufen möchten. Dieses Feld ist nicht verfügbar, wenn Sie im Feld [!UICONTROL Enable to Enter a Drive ID] die Option [!UICONTROL No] ausgewählt haben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datei] / [!UICONTROL Datei-ID] / [!UICONTROL Dateipfad]</td> 
   <td> <p>Wenn Sie die Option [!UICONTROL Manuell eingeben] ausgewählt haben, geben Sie die Datei-ID oder den Pfad der Datei ein, für die Sie einen Freigabe-Link abrufen möchten.</p> <p>Wenn Sie [!UICONTROL Select] aus der Liste ausgewählt haben, wählen Sie die Datei aus, für die Sie einen Freigabe-Link abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Berechtigungstyp]</td> 
   <td> <p>Wählen Sie aus, ob Personen mit dem Link Lese- und Schreibzugriff auf die Datei haben sollen oder ob sie nur lesen können.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Umfang]</td> 
   <td>Wählen Sie aus, ob die Datei für alle Benutzer mit dem Link oder nur für Mitglieder Ihrer Organisation verfügbar sein soll, die über den Link verfügen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Verschieben einer Datei/eines Ordners]

Dieses Aktionsmodul verschiebt eine Datei oder einen Ordner an einen neuen Ordnerspeicherort

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL OneDrive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eingabetaste (Datei-ID und Dateipfad)]</td> 
   <td>Wählen Sie aus, ob die Datei anhand der Datei-ID oder des Dateipfads identifiziert werden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datei-ID/Dateipfad eingeben]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Datei-ID oder den Dateipfad eingeben möchten:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Manuell eingeben]</b> </p> <p>Wählen Sie diese Option aus, wenn Sie die ID oder den Pfad direkt eingeben oder sie einem vorherigen Modul zuordnen möchten.</p> </li> 
     <li> <p><b>[!UICONTROL Auswahl aus einer Liste]</b> </p> <p>Wählen Sie diese Option aus, wenn Sie aus einer Liste der verfügbaren Dateien oder Pfade auswählen möchten. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] Standort auswählen]</td> 
   <td> <p>Wählen Sie den Speicherort aus, der die zu verschiebende Datei oder den Ordner enthält:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mein Laufwerk]</b> </p> <p>Wählen Sie aus, ob das Modul eine Laufwerk-ID eingeben soll.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Ja]</b> </p> <p>Geben Sie die ID des Laufwerks ein, das die zu verschiebende Datei oder den Ordner enthält.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Wählen Sie die [!DNL SharePoint]-Site aus, die die zu verschiebende Datei oder den Ordner enthält. Verfügbare Sites sind Sites , gefolgt vom angemeldeten Benutzer.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Wählen Sie die Gruppe aus, deren Laufwerk die zu verschiebende Datei oder den Ordner enthält.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Wählen Sie das Laufwerk aus oder ordnen Sie es zu, das die zu verschiebende Datei oder den Ordner enthält. Dieses Feld ist nicht verfügbar, wenn Sie im Feld [!UICONTROL Enable to Enter a Drive ID] die Option [!UICONTROL No] ausgewählt haben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Datei/Ordner von [!UICONTROL auswählen]</td> 
   <td>Wählen Sie aus, ob Sie eine Datei oder einen Ordner verschieben möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL Datei] / [!UICONTROL Datei-ID] / [!UICONTROL Dateipfad]</p> <p role="rowheader">[!UICONTROL Ordner] / [!UICONTROL Ordner-ID] / [!UICONTROL Ordnerpfad]</p> </td> 
   <td> <p>Wenn Sie die Option [!UICONTROL Manuell eingeben] ausgewählt haben, geben Sie die ID oder den Pfad der Datei oder des Ordners ein, die/den Sie verschieben möchten.</p> <p>Wenn Sie [!UICONTROL Select] aus der Liste ausgewählt haben, wählen Sie die zu verschiebende Datei oder den Ordner aus.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Neuen Ordnerspeicherort eingeben]</td> 
   <td> <p>Wählen Sie aus, wie Sie den Speicherort eingeben möchten, an den Sie die Datei oder den Ordner verschieben möchten:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Manuell eingeben]</b> </p> <p>Wählen Sie diese Option aus, wenn Sie die ID oder den Pfad direkt eingeben oder sie einem vorherigen Modul zuordnen möchten.</p> </li> 
     <li> <p><b>[!UICONTROL Auswahl aus einer Liste]</b> </p> <p>Wählen Sie diese Option aus, wenn Sie aus einer Liste der verfügbaren Dateien oder Pfade auswählen möchten. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] Standort auswählen]</td> 
   <td> <p>Wählen Sie den Speicherort aus, an den Sie die Datei oder den Ordner verschieben möchten:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mein Laufwerk]</b> </p> <p>Wählen Sie aus, ob das Modul eine Laufwerk-ID eingeben soll.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Ja]</b> </p> <p>Geben Sie die ID des Laufwerks ein, auf dem Sie die Datei oder den Ordner verschieben möchten.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Wählen Sie die [!DNL SharePoint]-Site aus, in die Sie die Datei oder den Ordner verschieben möchten. Verfügbare Sites sind Sites , gefolgt vom angemeldeten Benutzer.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Wählen Sie die Gruppe aus, auf deren Laufwerk Sie die Datei oder den Ordner verschieben möchten.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Wählen Sie das Laufwerk aus oder ordnen Sie es zu, das den Ordner enthält, in den Sie die Datei oder den Ordner verschieben möchten. Dieses Feld ist nicht verfügbar, wenn Sie im Feld [!UICONTROL Enable to Enter a Drive ID] die Option [!UICONTROL No] ausgewählt haben.</p> <p>Wenn Sie dieses Feld leer lassen, kann die Datei oder der Ordner nur innerhalb desselben [!DNL OneDrive] verschoben werden.</p> <p>Sie können Dateien und Ordner von [!UICONTROL My Drive] auf ein [!UICONTROL Site's Drive] oder ein [!UICONTROL Group's Drive] verschieben. </p> <p>Sie können Dateien von einem [!UICONTROL Site's Drive] nur auf dasselbe Laufwerk in derselben Site verschieben.</p> <p>Sie können Dateien von einem [!UICONTROL Group's Drive] nur auf dasselbe Laufwerk in derselben Gruppe verschieben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner]</td> 
   <td>Geben Sie den Ordner ein oder ordnen Sie ihn zu, in den Sie die Datei oder den Ordner verschieben möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eine Datei kopieren]

Dieses Aktionsmodul kopiert eine Datei in einen neuen Ordnerspeicherort

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL OneDrive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eingabetaste (Datei-ID und Dateipfad)]</td> 
   <td>Wählen Sie aus, ob die Datei anhand der Datei-ID oder des Dateipfads identifiziert werden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datei-ID eingeben] / [!UICONTROL Dateipfad]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Datei-ID oder den Dateipfad eingeben möchten:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Manuell eingeben]</b> </p> <p>Wählen Sie diese Option aus, wenn Sie die ID oder den Pfad direkt eingeben oder sie einem vorherigen Modul zuordnen möchten.</p> </li> 
     <li> <p><b>[!UICONTROL Auswahl aus einer Liste]</b> </p> <p>Wählen Sie diese Option aus, wenn Sie aus einer Liste der verfügbaren Dateien oder Pfade auswählen möchten. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] Standort auswählen]</td> 
   <td> <p>Wählen Sie den Speicherort aus, der die zu kopierende Datei enthält:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mein Laufwerk]</b> </p> <p>Wählen Sie aus, ob das Modul eine Laufwerk-ID eingeben soll.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Ja]</b> </p> <p>Geben Sie die ID des Laufwerks ein, das die zu kopierende Datei oder den Ordner enthält.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Wählen Sie die SharePoint-Site aus, die die zu verschiebende Datei enthält. Verfügbare Sites sind Sites , gefolgt vom angemeldeten Benutzer.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Wählen Sie die Gruppe aus, deren Laufwerk die zu kopierende Datei enthält.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Wählen Sie das Laufwerk aus oder ordnen Sie es zu, das die zu kopierende Datei enthält. Dieses Feld ist nicht verfügbar, wenn Sie im Feld [!UICONTROL Enable to Enter a Drive ID] die Option [!UICONTROL No] ausgewählt haben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL Datei] / [!UICONTROL Datei-ID] / [!UICONTROL Dateipfad]</p> </td> 
   <td> <p>Wenn Sie die Option [!UICONTROL Manuell eingeben] ausgewählt haben, geben Sie die ID oder den Pfad der Datei ein, die Sie kopieren möchten, oder ordnen Sie sie zu.</p> <p>Wenn Sie [!UICONTROL Select] aus der Liste ausgewählt haben, wählen Sie die zu kopierende Datei aus.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Neuen Ordnerspeicherort eingeben]</td> 
   <td> <p>Wählen Sie aus, wie Sie den Speicherort eingeben möchten, an den Sie die Datei kopieren möchten, oder:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Manuell eingeben]</b> </p> <p>Wählen Sie diese Option aus, wenn Sie die ID oder den Pfad direkt eingeben oder sie einem vorherigen Modul zuordnen möchten.</p> </li> 
     <li> <p><b>[!UICONTROL Auswahl aus einer Liste]</b> </p> <p>Wählen Sie diese Option aus, wenn Sie aus einer Liste verfügbarer Ordner auswählen möchten. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New OneDrive location]</td> 
   <td> <p>Wählen Sie den Speicherort aus, an den Sie den Filter kopieren möchten. Diese Option ist verfügbar, wenn Sie den neuen Ordnerspeicherort aus einer Liste auswählen.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mein Laufwerk]</b> </p> <p>Wählen Sie aus, ob das Modul eine Laufwerk-ID eingeben soll.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Ja]</b> </p> <p>Geben Sie die ID des Laufwerks ein, auf dem Sie die Datei kopieren möchten.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Wählen Sie die [!DNL SharePoint]-Site aus, in die Sie die Datei kopieren möchten. Verfügbare Sites sind Sites , gefolgt vom angemeldeten Benutzer.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Wählen Sie die Gruppe aus, auf deren Laufwerk Sie die Datei kopieren möchten.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Wählen Sie das Laufwerk aus oder ordnen Sie es zu, das den Ordner enthält, in den Sie die Datei kopieren möchten. Dieses Feld ist nicht verfügbar, wenn Sie im Feld [!UICONTROL Enable to Enter a Drive ID] die Option [!UICONTROL No] ausgewählt haben.</p> <p>Wenn Sie dieses Feld leer lassen, kann die Datei oder der Ordner nur innerhalb desselben [!UICONTROL OneDrive] kopiert werden.</p> <p>Sie können Dateien und Ordner von [!UICONTROL My Drive] in das Laufwerk einer [!UICONTROL Site] oder das Laufwerk einer [!UICONTROL Gruppe] kopieren. </p> <p>Sie können Dateien von einem [!UICONTROL Site's Drive] nur auf dasselbe Laufwerk auf derselben Site kopieren.</p> <p>Sie können Dateien aus dem Laufwerk einer [!UICONTROL Gruppe] nur auf dasselbe Laufwerk in derselben Gruppe kopieren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner]</td> 
   <td>Geben Sie den Ordner ein oder ordnen Sie ihn zu, in den Sie die Kopie oder den Ordner verschieben möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Neuer kopierter Dateiname]</td> 
   <td> <p>Geben Sie einen Namen für die neue Kopie der Datei ein oder ordnen Sie einen Namen zu. Wenn Sie den ursprünglichen Dateinamen nicht ändern möchten, können Sie dies leer lassen.</p> <p>Der Name muss die Dateierweiterung enthalten. Beispiel:<code> file.txt</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei/Ordner löschen]

Dieses Aktionsmodul löscht die ausgewählte Datei.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL OneDrive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eingabe (Datei-/Ordner-ID und Pfad)]</td> 
   <td>Wählen Sie aus, ob die Datei anhand der Datei-ID oder des Dateipfads identifiziert werden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datei-/Ordner-ID eingeben/Datei-/Ordnerpfad eingeben</td> 
   <td> <p>Wählen Sie aus, wie Sie die Datei-ID oder den Dateipfad eingeben möchten:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Manuell eingeben]</b> </p> <p>Wählen Sie diese Option aus, wenn Sie die ID oder den Pfad direkt eingeben oder sie einem vorherigen Modul zuordnen möchten.</p> </li> 
     <li> <p><b>[!UICONTROL Auswahl aus einer Liste]</b> </p> <p>Wählen Sie diese Option aus, wenn Sie aus einer Liste der verfügbaren Dateien oder Pfade auswählen möchten. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] Standort auswählen]</td> 
   <td> <p>Wählen Sie den Standort aus, den Sie suchen möchten:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mein Laufwerk]</b> </p> <p>Wählen Sie aus, ob das Modul eine Laufwerk-ID eingeben soll.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Ja]</b> </p> <p>Geben Sie die ID des Laufwerks ein, das die zu löschende Datei oder den Ordner enthält.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Wählen Sie die [!DNL SharePoint]-Site aus, die die Datei oder den Ordner enthält, die/den Sie löschen möchten. Verfügbare Sites sind Sites , gefolgt vom angemeldeten Benutzer.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Wählen Sie die Gruppe aus, deren Laufwerk die Datei oder den Ordner enthält, die/den Sie löschen möchten.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Wählen Sie das Laufwerk aus oder ordnen Sie es zu, das die zu löschende Datei oder den zu löschenden Ordner enthält. Dieses Feld ist nicht verfügbar, wenn Sie im Feld [!UICONTROL Enable to Enter a Drive ID] die Option [!UICONTROL No] ausgewählt haben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Datei/Ordner von [!UICONTROL auswählen]</td> 
   <td>Wählen Sie aus, ob Sie eine Datei oder einen Ordner löschen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datei] / [!UICONTROL Datei-ID] / [!UICONTROL Dateipfad]</td>
   <td> <p>Wenn Sie die Option [!UICONTROL Manuell eingeben] ausgewählt haben, geben Sie die Datei-ID oder den Pfad der Datei ein, die Sie löschen möchten.</p> <p>Wenn Sie [!UICONTROL Select] aus der Liste ausgewählt haben, wählen Sie die Datei aus, die Sie löschen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Sonstige

#### [!UICONTROL API-Aufruf durchführen]

Dieses Modul führt einen benutzerdefinierten API-Aufruf durch.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL OneDrive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Geben Sie einen Pfad relativ zu <code>https://graph.microsoft.com</code> ein. Beispiel:<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methode]</td> 
   td&gt; <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion fügt die Autorisierungskopfzeilen für Sie hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p>Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> in Ihrer JSON platzieren Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>



## Wenn Sie eine Datei nicht hochladen oder aktualisieren können

Beim Hochladen oder Aktualisieren einer Datei treten mehrere mögliche Probleme auf:

* Die hochgeladene Datei ist zu groß und überschreitet die maximale Dateigrößenbeschränkung für Ihren [!DNL OneDrive]-Plan oder Sie haben das Speicherkontingent Ihres [!DNL OneDrive]-Kontos verwendet. Um mehr Speicherplatz zu erhalten, löschen Sie vorhandene Dateien aus [!DNL OneDrive] oder aktualisieren Sie Ihr [!DNL OneDrive] -Konto.
* OneDrive erlaubt nicht, zwei Dateien mit demselben Namen in einen einzigen Ordner hochzuladen. Wenn der Zielordner eine Datei mit demselben Namen wie die hochgeladene Datei enthält, wird die Ausführung des Szenarios mit einem Fehler beendet. Die Lösung besteht darin, die hochgeladene Datei einfach umzubenennen. Wenn Sie eine Datei aktualisieren möchten, verwenden Sie die Aktion [!UICONTROL Datei aktualisieren] .
* Der zuvor ausgewählte Ordner, in den die Datei hochgeladen wird, existiert nicht mehr. Das Szenario wird gestoppt und Sie müssen den Zielordner erneut auswählen.
