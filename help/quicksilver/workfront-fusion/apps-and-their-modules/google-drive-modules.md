---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Steckverbinder
navigation-topic: apps-and-their-modules
title: Google-Laufwerkmodule
description: Mit  [!DNL Adobe Workfront Fusion Google Drive]  Modulen können Sie Ihre Dateien, Ordner oder freigegebenen Laufwerke in Ihrem überwachen, suchen, erstellen, aktualisieren, löschen und verwalten [!DNL Google Drive].
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d620c93-d1bf-4451-9f76-1d6fd850cec9
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '2958'
ht-degree: 0%

---

# [!DNL Google Drive]

Mit den [!DNL Adobe Workfront Fusion] [!DNL Google Drive]-Modulen können Sie Ihre Dateien, Ordner oder freigegebenen Laufwerke in Ihrer [!DNL Google Drive] überwachen, suchen, erstellen, aktualisieren, löschen und verwalten.

In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Ihr [!DNL Google Drive]-Konto mit mehreren Anwendungen und Services von Drittanbietern verbinden.

Anweisungen zum Erstellen eines Szenarios finden Sie unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## Informationen zur Google Drive-API

Der Google Drive-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Basis-URL</td> 
   <td> https://www.googleapis.com/drive/v3</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Version</td> 
   <td> v3 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v4.1.22</td> 
  </tr>
 </tbody> 
 </table>



## Verbinden von [!DNL Google Drive] mit [!DNL Workfront Fusion]

Wenn Sie [!DNL @gmail.com] oder [!DNL @googlemail.com] Benutzer sind, müssen Sie einen OAuth-Client auf [ erstellen [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) um [!UICONTROL Client-ID] und [!UICONTROL Client-Geheimnis] zu erhalten.

Eine schrittweise Anleitung zum Erstellen des OAuth-Clients (und zum Abrufen von [!UICONTROL Client-ID] und [!UICONTROL Client-Geheimnis]) finden Sie unter [Verbinden [!DNL Adobe Workfront Fusion] mit [!DNL Google Services] Verwenden eines benutzerdefinierten OAuth-Clients](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter [Erstellen einer Verbindung mit [!UICONTROL Adobe Workfront Fusion] - Grundlegende Anweisungen](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Google Drive] Module und ihre Felder

Beim Konfigurieren [!DNL Google Drive] Module zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder dem Service weitere [!DNL Google Drive] angezeigt werden. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)



* [Trigger](#triggers)
* [Aktionen](#actions)

### Trigger

* [[!UICONTROL Dateien im Ordner ansehen]](#watch-files-in-folder)
* [[!UICONTROL Alle Dateien ansehen]](#watch-all-files)
* [[!UICONTROL Freigegebene Dateien ansehen]](#watch-shared-files)
* [[!UICONTROL Kommentare ansehen]](#watch-comments)

#### [!UICONTROL Dateien im Ordner ansehen]

Ruft Dateidetails ab, wenn eine Datei im angegebenen Ordner hinzugefügt oder geändert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL-Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Wählen Sie den zu überwachenden Ordner aus]</td>
    <td >Wählen Sie den Ordner auf Ihrem Laufwerk aus, in dem die Dateien überwacht werden sollen.</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL Welche Dateien beobachtet werden]</td>
   <td> <p>Wählen Sie aus, welchen Dateityp Sie beobachten möchten.</p> 
    <ul> 
     <li>[!UICONTROL ALL]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL [!DNL Google Documents] Dateien ins Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Documents] konvertieren möchten.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL [!DNL Google Spreadsheets] Dateien ins Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Spreadsheets] konvertieren möchten.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL [!DNL Google Slides] Dateien ins Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Slides] konvertieren möchten.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL [!DNL Google Drawings] Dateien ins Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Drawings] konvertieren möchten.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Uhr]</td>
    <td>Wählen Sie aus, ob neue Dateien und alle Änderungen oder nur neue Dateien angesehen werden sollen.</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL Maximale Anzahl heruntergeladener Dateien]</td>
    <td>Legen Sie die maximale Anzahl von Ergebnissen fest, die [!DNL Workfront Fusion] während eines Zyklus herunterladen (die Anzahl der Wiederholungen pro Szenario-Ausführung).</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Alle Dateien ansehen]

Ruft Dateidetails ab, wenn eine Datei in Ihrem [!DNL Google Drive] hinzugefügt oder geändert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Welche Dateien beobachtet werden]</td> 
   <td> <p>Wählen Sie aus, welchen Dateityp Sie beobachten möchten.</p> 
    <ul> 
     <li>[!UICONTROL ALL]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL [!DNL Google Documents] Dateien ins Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Documents] konvertieren möchten.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL [!DNL Google Spreadsheets] Dateien ins Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Spreadsheets] konvertieren möchten.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL [!DNL Google Slides] Dateien ins Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Slides] konvertieren möchten.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL [!DNL Google Drawings] Dateien ins Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Drawings] konvertieren möchten.</td>
  </tr>  
  <tr> 
   <td>[!UICONTROL Uhr]</td> 
   <td>Wählen Sie aus, ob neue Dateien und alle Änderungen oder nur neue Dateien angesehen werden sollen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl heruntergeladener Dateien]</td> 
   <td>Legen Sie die maximale Anzahl von Ergebnissen fest, die [!DNL Workfront Fusion] während eines Zyklus herunterladen (die Anzahl der Wiederholungen pro Szenario-Ausführung).</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Freigegebene Dateien ansehen]

Trigger, wenn eine neue Datei für Sie freigegeben oder eine vorhandene freigegebene Datei aktualisiert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Wählen Sie den zu überwachenden Ordner aus]</td> 
   <td>Wählen Sie den freigegebenen Ordner aus, in dem die Dateien überwacht werden sollen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Welche Dateien beobachtet werden]</td> 
   <td> <p>Wählen Sie aus, welchen Dateityp Sie beobachten möchten.</p> 
    <ul> 
     <li>[!UICONTROL ALL]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL [!DNL Google Documents] Dateien ins Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Documents] konvertieren möchten.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL [!DNL Google Spreadsheets] Dateien ins Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Spreadsheets] konvertieren möchten.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL [!DNL Google Slides] Dateien ins Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Slides] konvertieren möchten.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL [!DNL Google Drawings] Dateien ins Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Drawings] konvertieren möchten.</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Uhr]</td> 
   <td>Wählen Sie aus, ob neue Dateien und alle Änderungen oder nur neue Dateien angesehen werden sollen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl heruntergeladener Dateien]</td> 
   <td>Legen Sie die maximale Anzahl von Ergebnissen fest, die [!DNL Workfront Fusion] während eines Zyklus herunterladen (die Anzahl der Wiederholungen pro Szenario-Ausführung).</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kommentare ansehen]

Trigger beim Hinzufügen oder Ändern eines Kommentars zur ausgewählten Datei.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Datei]</td> 
   <td>Wählen Sie die Datei aus, die auf Kommentare überwacht werden soll.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Uhr]</td> 
   <td>Wählen Sie aus, ob Sie alle Änderungen oder nur neue Kommentare überwachen möchten</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl der zurückgegebenen Kommentare]</td> 
   <td>Legen Sie die maximale Anzahl von Kommentaren fest, die [!DNL Workfront Fusion] während eines Zyklus zurückgeben (die Anzahl der Wiederholungen pro Szenario-Durchgang).</td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL Datei hochladen]](#upload-a-file)
* [[!UICONTROL Aktualisieren einer Datei]](#update-a-file)
* [[!UICONTROL Kopieren einer Datei]](#copy-a-file)
* [[!UICONTROL Datei löschen]](#delete-a-file)
* [[!UICONTROL Verschieben einer Datei/eines Ordners in den Papierkorb]](#move-a-filefolder-to-trash)
* [[!UICONTROL Datei abrufen]](#get-a-file)
* [[!UICONTROL Suchen nach Dateien/Ordnern]](#search-for-filesfolders)
* [[!UICONTROL Ordner erstellen]](#create-a-folder)
* [[!UICONTROL Link freigeben]](#get-a-share-link)

#### [!UICONTROL Datei hochladen]

Lädt eine Datei in Ihr [!DNL Google Drive] hoch.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Destination]</td> 
   <td> <p>Wählen Sie das Ziel aus, an das Sie eine Datei hochladen möchten.</p> 
    <ul> 
     <li>[!DNL My Drive]</li> 
     <li>[!DNL Shared with Me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zielordner]</td> 
   <td>Wählen Sie den Ordner aus, in den Sie eine Datei hochladen möchten. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source-Datei]</td> 
   <td>Wählen Sie aus, ob Sie eine Datei verwenden möchten, die von einem früheren Modul übergeben wurde, oder ob Sie die Datei manuell zuordnen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dateiname]</td> 
   <td>Wählen Sie den Dateinamen. Diese Option ist verfügbar, wenn Sie im Feld [!UICONTROL-Quelldatei] die Option "[!UICONTROL Map]" auswählen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Daten]</td> 
   <td>Wählen Sie die Datendatei aus, die Sie hochladen möchten. Diese Option ist verfügbar, wenn Sie im Feld [!UICONTROL-Quelldatei] die Option "[!UICONTROL Map]" auswählen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Titel]</td> 
   <td>Geben Sie einen Titel für die neue Datei ein.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei konvertieren]</td> 
   <td>Wenn diese Option aktiviert ist, kann das Modul Dateien in das entsprechende [!DNL Google] konvertieren.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aktualisieren einer Datei]

Aktualisiert die Metadaten oder Inhalte einer Datei.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Ziel]</td> 
   <td> <p>Wählen Sie das Ziel aus, an das Sie eine Datei hochladen möchten.</p> 
    <ul> 
     <li>[!UICONTROL Mein Laufwerk]</li> 
     <li>[!UICONTROL für mich freigegeben]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL In Ordner verschieben]</td> 
   <td>Wenn Sie die Datei in einen anderen Ordner verschieben möchten, wählen Sie den Ordner aus, in den Sie die Datei verschieben möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei-ID]</td> 
   <td>Ordnen Sie die ID der Datei zu, die Sie aktualisieren möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Titel]</td> 
   <td>Geben Sie einen Titel für die aktualisierte Datei ein.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dateiinhalt ändern]</td> 
   <td>Wählen Sie aus, ob Sie den Inhalt der Datei ersetzen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source-Datei]</td> 
   <td>Wählen Sie aus, ob Sie eine Datei verwenden möchten, die von einem früheren Modul übergeben wurde, oder ob Sie die Datei manuell zuordnen möchten. Dieses Feld ist verfügbar, wenn Sie im vorherigen Feld ausgewählt haben, den Dateiinhalt zu ändern.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dateiname]</td> 
   <td>Wählen Sie den Dateinamen. Diese Option ist verfügbar, wenn Sie im Feld [!UICONTROL-Quelldatei] die Option "[!UICONTROL Map]" auswählen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Daten]</td> 
   <td>Wählen Sie die Datendatei aus, die Sie hochladen möchten. Diese Option ist verfügbar, wenn Sie im Feld [!UICONTROL-Quelldatei] die Option "[!UICONTROL Map]" auswählen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kopieren einer Datei]

Kopiert eine Datei an den neuen Speicherort.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Ziel]</td> 
   <td> <p>Wählen Sie das Ziel aus, an das Sie eine Datei hochladen möchten.</p> 
    <ul> 
     <li>[!UICONTROL Mein Laufwerk]</li> 
     <li>[!UICONTROL für mich freigegeben]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zielordner]</td> 
   <td>Wählen Sie den Ordner aus, in den sich die zu kopierende Datei befindet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei-ID]</td> 
   <td>Ordnen Sie die ID der Datei zu, die Sie aktualisieren möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Der Name der Kopie]</td> 
   <td>Geben Sie einen Titel für die neue Datei ein. Lassen Sie dieses Feld leer, wenn Sie den ursprünglichen Dateinamen nicht ändern möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei löschen]

Löscht dauerhaft eine Datei oder einen Ordner.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei-ID]</td> 
   <td>Ordnen Sie die ID der Datei zu, die Sie löschen möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Verschieben einer Datei/eines Ordners in den Papierkorb]

Verschiebt eine Datei oder einen Ordner in den Papierkorb.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei-ID]</td> 
   <td>Ordnen Sie die ID der Datei zu, die Sie in den Papierkorb verschieben möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei abrufen]

Ruft die Datei mit der angegebenen ID ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Documents] Dateien ins Format konvertieren]</td> 
   <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Documents] konvertieren möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Spreadsheets] Dateien ins Format konvertieren]</td> 
   <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Spreadsheets] konvertieren möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Slides] Dateien ins Format konvertieren]</td> 
   <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Slides] konvertieren möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Drawings] Dateien ins Format konvertieren]</td> 
   <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Drawings] konvertieren möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei-ID]</td> 
   <td>Ordnen Sie die ID der Datei zu, die Sie abrufen möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suchen nach Dateien/Ordnern]

Sucht basierend auf Suchkriterien nach Dateien oder Ordnern.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Ziel]</td> 
   <td> <p>Wählen Sie das Ziel aus, das Sie suchen möchten.</p> 
    <ul> 
     <li>[!UICONTROL Mein Laufwerk]</li> 
     <li>[!UICONTROL für mich freigegeben]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner auflisten]</td> 
   <td>Navigieren Sie zu dem Ordner, in dem Sie nach den Dateien oder Ordnern suchen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL abrufen]</td> 
   <td> <p> Wählen Sie aus, ob Sie nach Dateien, Ordnern oder beidem suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Suche]</p> </td> 
   <td> <p>Wählen Sie den Typ der Suche aus, die Sie durchführen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Suche innerhalb von Datei-/Ordnernamen]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL-Abfrage]</strong> </p> <p>Geben Sie einen Teil des Dateinamens oder des vollständigen Dateinamens (einschließlich des Suffix) ein, nach dem gesucht werden soll.</p> </li> 
       <li> <p><strong>[!UICONTROL Suchoptionen]</strong> </p> <p>Wählen Sie aus, ob Sie nach dem genauen Begriff suchen möchten oder ob Sie nach Namen suchen möchten, die den Suchbegriff enthalten.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Volltext]-Suche</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL-Abfrage]</strong> </p> <p>Geben Sie einen beliebigen Suchbegriff ein, den Sie in Ihrem [!DNL Google Drive] suchen möchten.</p> </li> 
      </ul> </li> 
     <li> <p><strong>Benutzerdefinierte Suchanfrage eingeben</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL-Abfrage]</strong> </p> <p>Geben Sie die benutzerdefinierte Suchabfrage ein. Weitere Informationen finden Sie im Abschnitt [!UICONTROL Nach Dateien suchen] dieses Artikels.</p> </li> 
       <li> <p><strong>Fügen Sie den oben ausgewählten Ordner zur Abfrage hinzu</strong> </p> <p>Sucht in der übergeordneten Sammlung nach dem Ordner. Dadurch werden alle Dateien und Ordner gefunden, die sich direkt in dem oben ausgewählten Ordner befinden.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl der zurückgegebenen Ergebnisse]</td> 
   <td>Legen Sie die maximale Anzahl von Dateien oder Ordnern fest, die [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgeben.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Die Routenausführung auch dann fortsetzen, wenn das Modul keine Ergebnisse zurückgibt]</td> 
   <td>Aktivieren Sie diese Option, um sicherzustellen, dass das Szenario nicht angehalten wird, wenn das Modul keine Ergebnisse zurückgibt.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ordner erstellen]

Erstellt einen Ordner am angegebenen Speicherort.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Ziel]</td> 
   <td> <p>Wählen Sie das Ziel aus, an das Sie eine Datei hochladen möchten.</p> 
    <ul> 
     <li>[!UICONTROL Mein Laufwerk]</li> 
     <li>[!UICONTROL für mich freigegeben]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Speicherort des neuen Ordners]</td> 
   <td>Navigieren Sie zu der Position, an der Sie einen neuen Ordner erstellen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Der Name des neuen Ordners]</td> 
   <td>Geben Sie einen Namen für den Ordner ein, den Sie erstellen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Freigabeordner]</td> 
   <td>Wählen Sie diese Option aus, wenn Sie den Ordner für alle mit dem Link [!UICONTROL Share] freigeben möchten. Andernfalls ist der Freigabe-Link nur für den Eigentümer.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Link freigeben]

Ruft den Freigabe-Link für eine Datei in Google Drive ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei-ID]</td> 
   <td>Ordnen Sie die ID der Datei zu, für die Sie den Freigabe-Link abrufen möchten.</td> 
  </tr> 
 </tbody> 
</table>

## Fehlerbehebung

### Datei kann nicht hochgeladen oder aktualisiert werden

Es gibt mehrere Situationen, in denen das Hochladen oder Aktualisieren einer Datei fehlschlägt:

* Die hochgeladene Datei ist zu groß und überschreitet die maximale Dateigröße, die für Ihren [!DNL Google Drive] zulässig ist, oder Sie haben Ihr [!DNL Google Drive] Speicherlimit überschritten. Sie können entweder Ihren Speicherplan aktualisieren oder vorhandene Dateien aus dem [!DNL Google Drive]-Service löschen.
* Der ausgewählte Ordner, in den die Datei hochgeladen werden soll, existiert nicht mehr. Das Szenario stoppt und es ist dann erforderlich, erneut einen Zielordner auszuwählen.

## Nach Dateien suchen

Im Modul Listen-Dateien in einem Ordner können Sie Ihre eigene Abfrage verwenden, die aus folgenden Teilen besteht:

* **[!UICONTROL Feld]** - Attribut der zu durchsuchenden Datei, z. B. `name` der Datei.

* **[!UICONTROL Operator]** - Test, der an den Daten durchgeführt wird, um eine Übereinstimmung bereitzustellen, z. B. `contains`.

* **[!UICONTROL Value]** - Der Inhalt des zu testenden Attributs, z. B. der Name der `My cool document`.

Kombinieren Sie Klauseln mit den `and` oder `or` und negieren Sie die Abfrage mit `not`.

* [Felder](#fields)
* [Werttypen](#value-types)
* [Operatoren](#operators)
* [Beispiele](#examples)

### Felder

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Feld </th> 
   <th>Werttyp </th> 
   <th>Operatoren</th> 
   <th> <p> Beschreibung</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>[!UICONTROL title]</code></td> 
   <td>Zeichenfolge</td> 
   <td><code>contains</code><sup>1</sup>, <code>=</code>, <code>!=</code></td> 
   <td> <p> Name der Datei.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL fullText]</code> </td> 
   <td>Zeichenfolge </td> 
   <td><code>contains</code><sup>2, 3</sup> </td> 
   <td> <p> Vollständiger Text der Datei mit Name, Beschreibung, Inhalt und indizierbarem Text.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL mimeType]</code> </td> 
   <td> Zeichenfolge</td> 
   <td><code>contains</code>, <code>=</code>, <code>!=</code></td> 
   <td> <p> MIME-Typ der Datei.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL modifiedDate]</code> </td> 
   <td> date<sup>4</sup></td> 
   <td><code> &lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> Datum der letzten Änderung der Datei.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL lastViewedByMeDate]</code> </td> 
   <td> date<sup>4</sup></td> 
   <td><code>&lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> Datum, an dem der Benutzer eine Datei zuletzt angezeigt hat.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL trashed]</code></td> 
   <td>Boolescher Wert </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p> Ob die Datei im Papierkorb ist oder nicht.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL starred]</code></td> 
   <td>Boolescher Wert </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p>Ob die Datei gestartet ist oder nicht.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL parents]</code></td> 
   <td>Ansammlung </td> 
   <td><code>in </code> </td> 
   <td> <p>Ob die [!UICONTROL parent]-Auflistung die angegebene ID enthält.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL owners]</code></td> 
   <td>Ansammlung </td> 
   <td><code>in </code> </td> 
   <td> <p>Benutzer, denen die Datei gehört.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL writers]</code></td> 
   <td>Ansammlung </td> 
   <td><code>in </code> </td> 
   <td> <p>Benutzer mit der Berechtigung zum Ändern der Datei.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL readers] </code> </td> 
   <td>Ansammlung </td> 
   <td><code>in </code> </td> 
   <td> <p>Benutzer, die zum Lesen der Datei berechtigt sind.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL sharedWithMe]</code> </td> 
   <td>Boolescher Wert </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p> Dateien, die sich in der Sammlung „Für mich freigegeben“ des Benutzers befinden.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL properties] </code> </td> 
   <td>Ansammlung</td> 
   <td><code>has </code> </td> 
   <td> <p> Öffentliche benutzerdefinierte Dateieigenschaften.</p> </td> 
  </tr> 
 </tbody> 
</table>

Beachten Sie Folgendes über Operatoren in diesen Feldern:

* Der `contains` Operator führt nur einen Präfixabgleich für eine `title` durch.

  Beispielsweise entspricht der Titel „HelloWorld“ für `title contains 'Hello'`, aber nicht für `title contains 'World'`.

* Der `contains` Operator führt für `fullText` nur eine Übereinstimmung für ganze Zeichenfolgen-Token durch.

  Wenn beispielsweise der Volltext eines Dokuments die Zeichenfolge „HelloWorld“ enthält, gibt nur der Abfrage-`fullText contains 'HelloWorld'` ein Ergebnis zurück. Abfragen wie `fullText contains 'Hello'` geben in diesem Szenario keine Ergebnisse zurück.

* Der Operator `contains` entspricht einem exakten alphanumerischen Satz, wenn er von doppelten Anführungszeichen umgeben ist.

  Wenn beispielsweise die `fullText` eines Dokuments die Zeichenfolge „Hello there world“ enthält, gibt die Abfrage-`fullText contains '"Hello there"'` ein Ergebnis zurück, die Abfrage-`fullText contains '"Hello world"'` jedoch nicht.

  Da die Suche alphanumerisch ist, gibt die Abfrage-`fullText contains '"Hello world"'` außerdem ein Ergebnis zurück, wenn die `fullText` eines Dokuments die Zeichenfolge „Hello_world“ enthält.

* Datumsfelder `type` derzeit nicht miteinander vergleichbar, sondern nur mit konstanten Datumsangaben.

### Werttypen

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Werttyp</th> 
   <th> <p> Notizen</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Zeichenfolge </td> 
   <td> <p>Mit einfachen Anführungszeichen umgeben ". Escape-Zeichen für einfache Anführungszeichen in Abfragen mit <code>\'</code>, z. B. <code> 'Valentine\'s Day'</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Boolesch </td> 
   <td> <p><code>true </code>oder <code>false</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Datum </td> 
   <td> <p>RFC-3339-Format, Standardzeitzone ist UTC, z. B. <code>2012-06-04T12:00:00-08:00</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Operatoren

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Benutzerin oder Benutzer </th> 
   <th> <p>Notizen</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>contains</code></td> 
   <td> <p>Der Inhalt einer Zeichenfolge ist in der anderen vorhanden.</p> </td> 
  </tr> 
  <tr> 
   <td><code>=</code> </td> 
   <td> <p> Der Inhalt einer Zeichenfolge oder eines booleschen Werts entspricht dem des anderen.</p> </td> 
  </tr> 
  <tr> 
   <td><code>!=</code> </td> 
   <td> <p> Der Inhalt einer Zeichenfolge oder eines booleschen Werts ist nicht identisch mit dem anderen.</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;</code> </td> 
   <td> <p> Ein Datum liegt vor einem anderen.</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;=</code> </td> 
   <td> <p> Ein Datum liegt vor oder ist gleich einem anderen Datum.</p> </td> 
  </tr> 
  <tr> 
   <td><code>></code> </td> 
   <td> <p> Ein Datum ist später als ein anderes.</p> </td> 
  </tr> 
  <tr> 
   <td><code>>=</code> </td> 
   <td> <p> Ein Datum ist später oder gleich einem anderen.</p> </td> 
  </tr> 
  <tr> 
   <td><code>in </code> </td> 
   <td> <p>Ein Element ist in einer Sammlung enthalten.</p> </td> 
  </tr> 
  <tr> 
   <td><code>and </code> </td> 
   <td> <p>Gibt Dateien zurück, die beiden Klauseln entsprechen.</p> </td> 
  </tr> 
  <tr> 
   <td><code>or </code> </td> 
   <td> <p>Gibt Dateien zurück, die einer der beiden Klauseln entsprechen.</p> </td> 
  </tr> 
  <tr> 
   <td><code>not </code> </td> 
   <td> <p>Negiert eine Suchklausel.</p> </td> 
  </tr> 
  <tr> 
   <td><code>has </code> </td> 
   <td> <p>Eine Sammlung enthält ein -Element, das den Parametern entspricht.</p> </td> 
  </tr> 
 </tbody> 
</table>

Bei zusammengesetzten Klauseln können Sie Klammern verwenden, um Klauseln zu gruppieren. Beispiel:
`modifiedDate > '2012-06-04T12:00:00' and (mimeType contains 'image/' or mimeType contains 'video/')` Diese Suche gibt alle Dateien mit dem Bild- oder Video-MIME-Typ zurück, deren letzte Änderung nach dem 4. Juni 2012 erfolgte. Da `and`- und `or`-Operatoren von links nach rechts ohne Klammern ausgewertet werden, gibt das obige Beispiel nur Bilder zurück, die nach dem 4. Juni 2012 geändert wurden, jedoch alle Videos, selbst die vor dem 4. Juni 2012.

### Beispiele

Alle Beispiele auf dieser Seite zeigen den nicht kodierten `<q>q</q>`, wobei `title = 'hello'` als `title+%3d+%27hello%27` kodiert ist. Client-Bibliotheken verarbeiten diese Kodierung automatisch.

* Suchen Sie nach Dateien mit dem Namen „hello“
  <pre>title = 'Hallo'</pre>
* Suchen nach Ordnern mit dem ordnerspezifischen MIME-Typ
  <pre>mimeType = 'application/vnd.google-apps.folder'</pre>
* Suchen nach Dateien, die keine Ordner sind
  <pre>mimeType != 'application/vnd.google-apps.folder'</pre>
* Suchen Sie nach Dateien mit einem Namen, der die Wörter „Hallo“ und „Auf Wiedersehen“ enthält
  <pre>Titel enthält „Hallo“ und [!UICONTROL name] enthält „Tschüss“</pre>
* Suchen Sie nach Dateien, deren Name nicht das Wort „Hallo“ enthält
  <pre>Titel enthält nicht „Hallo“</pre>
* Suchen Sie nach Dateien, die das Wort „Hallo“ im Inhalt enthalten
  <pre>fullText enthält „Hallo“</pre>
* Suchen Sie nach Dateien, die das Wort „Hallo“ nicht im Inhalt enthalten
  <pre>nicht fullText enthält „hello“</pre>
* Suchen Sie nach Dateien, die die exakte Phrase „hello world“ im Inhalt enthalten
  <pre>fullText Enthält "„Hello world“„fullText enthält "„hello_world“"</pre>
* Suchen Sie nach Dateien mit einer Abfrage, die das Zeichen &quot;\&quot; enthält (z. B. &quot;\authors„)
  <pre>fullText enthält '\\authors'</pre>
* Nach Dateien suchen, die von der `test@example.org` beschreibbar sind
  <pre>'test@example.org' in [!DNL writers]</pre>
* Suchen Sie nach dem ID-`1234567` in der `parents`. Dadurch werden alle Dateien und Ordner gefunden, die sich direkt in dem Ordner befinden, dessen ID `1234567` ist.
  <pre>„1234567“ in [!UICONTROL parent]</pre>
* Suchen Sie nach der Alias-ID `appDataFolder` in der `parents`. Dadurch werden alle Dateien und Ordner gefunden, die sich direkt unter dem [Anwendungsdatenordner](https://developers.google.com/drive/api/v2/appdata) befinden.
  <pre>'appDataFolder' in übergeordneten Elementen</pre>
* Nach Dateien suchen, die von den Benutzern `test@example.org` und `test2@example.org` geschrieben werden können
  <pre>"test@example.org" in Writern und "test2@example.org" in Writern</pre>
* Suchen Sie nach Dateien, die den Text „wichtigem“ enthalten und sich im Papierkorb befinden
  <pre>fullText Enthält „wichtigem“ Inhalt und Papierkorb = true</pre>
* Suche nach Dateien, die nach dem 4. Juni 2012 geändert wurden
  <pre>modifiedDate &gt; '2012-06-04T12:00:00' // Standard-Zeitzone ist UTC</pre><pre>modifiedDate &gt; '2012-06-04T12:00:00-08:00'</pre>
* Suchen Sie nach Dateien, die für den autorisierten Benutzer mit „Hallo“ im Namen freigegeben sind
  <pre>sharedWithMe und Titel enthalten 'hello'</pre>
* Suchen Sie nach Dateien mit einer [benutzerdefinierten Dateieigenschaft](https://developers.google.com/drive/api/v2/properties) namens `additionalID` mit dem Wert `8e8aceg2af2ge72e78`.
  <pre>properties hat { key='additionalID' and value='8e8aceg2af2ge72e78' and visible='PRIVATE' }</pre>

Source dieses Handbuchs ist [[!DNL Google Drive] Dokumentation](https://developers.google.com/drive/api/v2/search-shareddrives).
