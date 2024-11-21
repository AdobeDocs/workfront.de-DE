---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connector
navigation-topic: apps-and-their-modules
title: Google Drive Module
description: Mit den [!DNL Adobe Workfront Fusion Google Drive] Modulen können Sie Ihre Dateien, Ordner oder freigegebenen Laufwerke in Ihrem [!DNL Google Drive] überwachen, durchsuchen, erstellen, aktualisieren, löschen und verwalten.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d620c93-d1bf-4451-9f76-1d6fd850cec9
source-git-commit: 2e91e9a4c691430f3c98e3cbddb30706ea57f84a
workflow-type: tm+mt
source-wordcount: '2958'
ht-degree: 0%

---

# [!DNL Google Drive] Module

Mit den Modulen [!DNL Adobe Workfront Fusion] [!DNL Google Drive] können Sie Ihre Dateien, Ordner oder freigegebenen Laufwerke in Ihrem [!DNL Google Drive] überwachen, durchsuchen, erstellen, aktualisieren, löschen und verwalten.

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Ihr [!DNL Google Drive] -Konto mit mehreren Drittanbieteranwendungen und -diensten verbinden.

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

## Google Drive-API-Informationen

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

Wenn Sie Benutzer [!DNL @gmail.com] oder [!DNL @googlemail.com] sind, müssen Sie einen OAuth-Client für [den  [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) erstellen, um [!UICONTROL Client-ID] und den [!UICONTROL Client-Geheimnis] zu erhalten.

Eine schrittweise Anleitung zum Erstellen des OAuth-Clients (und Abrufen der [!UICONTROL Client-ID] und des [!UICONTROL Client-Geheimnisses]) finden Sie unter [Verbinden [!DNL Adobe Workfront Fusion] mit [!DNL Google Services] mithilfe eines benutzerdefinierten OAuth-Clients](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter [Erstellen einer Verbindung mit [!UICONTROL Adobe Workfront Fusion] - Grundlegende Anweisungen](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Google Drive] Module und ihre Felder

Wenn Sie [!DNL Google Drive] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Google Drive] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)



* [Trigger](#triggers)
* [Aktionen](#actions)

### Trigger

* [[!UICONTROL Dateien im Ordner überwachen]](#watch-files-in-folder)
* [[!UICONTROL Alle Dateien ansehen]](#watch-all-files)
* [[!UICONTROL Geteilte Dateien ansehen]](#watch-shared-files)
* [[!UICONTROL Kommentare ansehen]](#watch-comments)

#### [!UICONTROL Dateien im Ordner überwachen]

Ruft Dateidetails ab, wenn eine Datei im angegebenen Ordner hinzugefügt oder geändert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Ordner auswählen, der überwacht werden soll]</td>
    <td >Wählen Sie den Ordner auf Ihrem Laufwerk aus, in dem Sie die Dateien ansehen möchten.</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL Welche Dateien sind zu sehen?]</td>
   <td> <p>Wählen Sie den Dateityp aus, den Sie ansehen möchten.</p> 
    <ul> 
     <li>[!UICONTROL All]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL [!DNL Google Documents] Dateien in Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Documents] konvertieren möchten.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL [!DNL Google Spreadsheets] Dateien in Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Spreadsheets] konvertieren möchten.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL [!DNL Google Slides] Dateien in Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Slides] konvertieren möchten.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL [!DNL Google Drawings] Dateien in Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Drawings] konvertieren möchten.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Watch]</td>
    <td>Wählen Sie aus, ob Sie neue Dateien und alle Änderungen oder nur neue Dateien ansehen möchten.</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL Maximale Anzahl heruntergeladener Dateien]</td>
    <td>Legen Sie die maximale Anzahl von Ergebnissen fest, die [!DNL Workfront Fusion] während eines Zyklus herunterladen wird (die Anzahl der Wiederholungen pro Szenario-Ausführung).</td>
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
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Welche Dateien sind zu sehen?]</td> 
   <td> <p>Wählen Sie den Dateityp aus, den Sie ansehen möchten.</p> 
    <ul> 
     <li>[!UICONTROL All]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL [!DNL Google Documents] Dateien in Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Documents] konvertieren möchten.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL [!DNL Google Spreadsheets] Dateien in Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Spreadsheets] konvertieren möchten.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL [!DNL Google Slides] Dateien in Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Slides] konvertieren möchten.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL [!DNL Google Drawings] Dateien in Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Drawings] konvertieren möchten.</td>
  </tr>  
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>Wählen Sie aus, ob Sie neue Dateien und alle Änderungen oder nur neue Dateien ansehen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl heruntergeladener Dateien]</td> 
   <td>Legen Sie die maximale Anzahl von Ergebnissen fest, die [!DNL Workfront Fusion] während eines Zyklus herunterladen wird (die Anzahl der Wiederholungen pro Szenario-Ausführung).</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Geteilte Dateien ansehen]

Trigger, wenn eine neue Datei für Sie freigegeben oder eine vorhandene freigegebene Datei aktualisiert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner auswählen, der überwacht werden soll]</td> 
   <td>Wählen Sie den freigegebenen Ordner aus, in dem Sie die Dateien anzeigen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Welche Dateien sind zu sehen?]</td> 
   <td> <p>Wählen Sie den Dateityp aus, den Sie ansehen möchten.</p> 
    <ul> 
     <li>[!UICONTROL All]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL [!DNL Google Documents] Dateien in Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Documents] konvertieren möchten.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL [!DNL Google Spreadsheets] Dateien in Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Spreadsheets] konvertieren möchten.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL [!DNL Google Slides] Dateien in Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Slides] konvertieren möchten.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL [!DNL Google Drawings] Dateien in Format konvertieren]</td>
    <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Drawings] konvertieren möchten.</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>Wählen Sie aus, ob Sie neue Dateien und alle Änderungen oder nur neue Dateien ansehen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl heruntergeladener Dateien]</td> 
   <td>Legen Sie die maximale Anzahl von Ergebnissen fest, die [!DNL Workfront Fusion] während eines Zyklus herunterladen wird (die Anzahl der Wiederholungen pro Szenario-Ausführung).</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kommentare ansehen]

Trigger, wenn ein Kommentar zur ausgewählten Datei hinzugefügt oder geändert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei]</td> 
   <td>Wählen Sie die Datei aus, die Sie für Kommentare überwachen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>Wählen Sie aus, ob Sie alle Änderungen oder nur neue Kommentare überwachen möchten</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl zurückgegebener Kommentare]</td> 
   <td>Legen Sie die maximale Anzahl von Kommentaren fest, die [!DNL Workfront Fusion] während eines Zyklus zurückgibt (die Anzahl der Wiederholungen pro Szenario-Ausführung).</td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL  Datei hochladen]](#upload-a-file)
* [[!UICONTROL Datei aktualisieren]](#update-a-file)
* [[!UICONTROL Eine Datei kopieren]](#copy-a-file)
* [[!UICONTROL Datei löschen]](#delete-a-file)
* [[!UICONTROL Verschieben einer Datei/eines Ordners in den Papierkorb]](#move-a-filefolder-to-trash)
* [[!UICONTROL Datei abrufen]](#get-a-file)
* [[!UICONTROL Suchen nach Dateien/Ordnern]](#search-for-filesfolders)
* [[!UICONTROL Erstellen eines Ordners]](#create-a-folder)
* [[!UICONTROL Einen Freigabe-Link abrufen]](#get-a-share-link)

#### [!UICONTROL  Datei hochladen]

Lädt eine Datei in Ihren [!DNL Google Drive] hoch.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Destination]</td> 
   <td> <p>Wählen Sie das Ziel aus, in das Sie eine Datei hochladen möchten.</p> 
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
   <td>Wählen Sie aus, ob Sie eine von einem vorherigen Modul übergebene Datei verwenden möchten oder ob Sie die Datei manuell zuordnen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dateiname]</td> 
   <td>Wählen Sie den Dateinamen aus. Diese Option ist verfügbar, wenn Sie "[!UICONTROL Map]"im Feld [!UICONTROL Quelldatei] auswählen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Daten]</td> 
   <td>Wählen Sie die Datendatei aus, die Sie hochladen möchten. Diese Option ist verfügbar, wenn Sie "[!UICONTROL Map]"im Feld [!UICONTROL Quelldatei] auswählen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Titel]</td> 
   <td>Geben Sie einen Titel für die neue Datei ein.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei konvertieren]</td> 
   <td>Durch Aktivierung dieser Option kann das Modul Dateien in das entsprechende [!DNL Google] -Format konvertieren.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei aktualisieren]

Aktualisiert die Metadaten oder Inhalte einer Datei.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ziel]</td> 
   <td> <p>Wählen Sie das Ziel aus, in das Sie eine Datei hochladen möchten.</p> 
    <ul> 
     <li>[!UICONTROL Mein Laufwerk]</li> 
     <li>[!UICONTROL Für mich freigegeben]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL In einen Ordner verschieben]</td> 
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
   <td>Wählen Sie aus, ob Sie eine von einem vorherigen Modul übergebene Datei verwenden möchten oder ob Sie die Datei manuell zuordnen möchten. Dieses Feld ist verfügbar, wenn Sie die Option zum Ändern des Dateiinhalts im vorherigen Feld ausgewählt haben.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dateiname]</td> 
   <td>Wählen Sie den Dateinamen aus. Diese Option ist verfügbar, wenn Sie "[!UICONTROL Map]"im Feld [!UICONTROL Quelldatei] auswählen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Daten]</td> 
   <td>Wählen Sie die Datendatei aus, die Sie hochladen möchten. Diese Option ist verfügbar, wenn Sie "[!UICONTROL Map]"im Feld [!UICONTROL Quelldatei] auswählen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eine Datei kopieren]

Kopiert eine Datei an den neuen Speicherort.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ziel]</td> 
   <td> <p>Wählen Sie das Ziel aus, in das Sie eine Datei hochladen möchten.</p> 
    <ul> 
     <li>[!UICONTROL Mein Laufwerk]</li> 
     <li>[!UICONTROL Für mich freigegeben]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zielordner]</td> 
   <td>Wählen Sie den Ordner aus, in dem sich die zu kopierende Datei befindet/</td> 
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

Löscht eine Datei oder einen Ordner dauerhaft.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a> .</p> </td> 
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
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei-ID]</td> 
   <td>Ordnen Sie die Kennung der Datei zu, die Sie in den Papierkorb verschieben möchten.</td> 
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
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Documents] Dateien in Format konvertieren]</td> 
   <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Documents] konvertieren möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Spreadsheets] Dateien in Format konvertieren]</td> 
   <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Spreadsheets] konvertieren möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Slides] Dateien in Format konvertieren]</td> 
   <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Slides] konvertieren möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Drawings] Dateien in Format konvertieren]</td> 
   <td>Wählen Sie das Dateiformat aus, in das Sie [!DNL Google Drawings] konvertieren möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei-ID]</td> 
   <td>Ordnen Sie die ID der Datei zu, die Sie abrufen möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suchen nach Dateien/Ordnern]

Sucht nach Dateien oder Ordnern basierend auf Suchkriterien.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ziel]</td> 
   <td> <p>Wählen Sie das Ziel aus, das Sie suchen möchten.</p> 
    <ul> 
     <li>[!UICONTROL Mein Laufwerk]</li> 
     <li>[!UICONTROL Für mich freigegeben]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Ordner auflisten</td> 
   <td>Navigieren Sie zu dem Ordner, nach dem Sie nach den Dateien oder Ordnern suchen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Retrieve]</td> 
   <td> <p> Wählen Sie aus, ob Sie nach Dateien, Ordnern oder beidem suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Suche]</p> </td> 
   <td> <p>Wählen Sie den Typ der Suche aus, die Sie durchführen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Suche in Datei-/Ordnernamen]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Abfrage]</strong> </p> <p>Geben Sie einen Teil des Dateinamens oder des vollständigen Dateinamens (einschließlich des Suffix) ein, nach dem Sie suchen möchten.</p> </li> 
       <li> <p><strong>[!UICONTROL Suchoptionen]</strong> </p> <p>Wählen Sie aus, ob Sie nach dem genauen Begriff suchen möchten oder ob Sie nach Namen suchen möchten, die den Suchbegriff enthalten.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Fulltext] search</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Abfrage]</strong> </p> <p>Geben Sie einen beliebigen Suchbegriff, den Sie suchen möchten, in Ihren [!DNL Google Drive] ein.</p> </li> 
      </ul> </li> 
     <li> <p><strong>Benutzerdefinierte Suchabfrage eingeben</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Abfrage]</strong> </p> <p>Geben Sie die benutzerdefinierte Suchabfrage ein. Weitere Informationen finden Sie im Abschnitt [!UICONTROL Suche nach Dateien] dieses Artikels.</p> </li> 
       <li> <p><strong>Fügen Sie den oben ausgewählten Ordner zur Abfrage hinzu</strong> </p> <p>Sucht den Ordner in der übergeordneten Sammlung. Dadurch werden alle Dateien und Ordner direkt im oben ausgewählten Ordner gefunden.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl an zurückgegebenen Ergebnissen]</td> 
   <td>Legen Sie die maximale Anzahl von Dateien oder Ordnern fest, die [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgibt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fortfahren der Routenausführung, selbst wenn das Modul keine Ergebnisse zurückgibt]</td> 
   <td>Aktivieren Sie diese Option, um sicherzustellen, dass das Szenario nicht angehalten wird, wenn das Modul keine Ergebnisse zurückgibt.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Erstellen eines Ordners]

Erstellt einen Ordner am angegebenen Speicherort.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ziel]</td> 
   <td> <p>Wählen Sie das Ziel aus, in das Sie eine Datei hochladen möchten.</p> 
    <ul> 
     <li>[!UICONTROL Mein Laufwerk]</li> 
     <li>[!UICONTROL Für mich freigegeben]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Neuer Ordnerspeicherort]</td> 
   <td>Navigieren Sie zu dem Speicherort, an dem Sie einen neuen Ordner erstellen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Der Name des neuen Ordners]</td> 
   <td>Geben Sie einen Namen für den Ordner ein, den Sie erstellen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner freigeben]</td> 
   <td>Wählen Sie diese Option aus, wenn Sie den Ordner für alle Benutzer mit dem Link [!UICONTROL Freigabe] freigeben möchten. Andernfalls ist der Freigabe-Link nur für den Eigentümer bestimmt.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Einen Freigabe-Link abrufen]

Ruft den Freigabe-Link für eine Datei in Google Drive ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Google Drive] mit [!UICONTROL Workfront Fusion]</a> .</p> </td> 
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

* Die hochgeladene Datei ist zu groß und überschreitet die maximale Dateigrößenbeschränkung, die für Ihren [!DNL Google Drive] -Plan zulässig ist, oder Sie haben Ihr [!DNL Google Drive] -Speicherlimit überschritten. Sie können entweder Ihren Speicherplan aktualisieren oder vorhandene Dateien aus dem [!DNL Google Drive] -Dienst löschen.
* Der ausgewählte Ordner, in den die Datei hochgeladen werden soll, existiert nicht mehr. Das Szenario wird gestoppt und es ist dann erforderlich, einen Zielordner erneut auszuwählen.

## Suchen nach Dateien

In den Modullisten-Dateien in einem Ordner können Sie Ihre eigene Abfrage verwenden, die aus folgenden Teilen besteht:

* **[!UICONTROL Feld]** - Attribut der Datei, die gesucht wird, z. B. das Attribut `name` der Datei.

* **[!UICONTROL Operator]** - Test, der für die Daten durchgeführt wird, um eine Übereinstimmung bereitzustellen, z. B. `contains`.

* **[!UICONTROL Wert]** - Der Inhalt des Attributs, das getestet wird, z. B. der Name der Datei `My cool document`.

Kombinieren Sie die Klauseln mit den Konjunktionen `and` oder `or` und negieren Sie die Abfrage mit `not`.

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
   <td> <p> Vollständiger Text der Datei, einschließlich Name, Beschreibung, Inhalt und indexierbarem Text.</p> </td> 
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
   <td> <p> Gibt an, ob die Datei im Papierkorb ist.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL starred]</code></td> 
   <td>Boolescher Wert </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p>Gibt an, ob die Datei gestartet wird oder nicht.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL parents]</code></td> 
   <td>collection </td> 
   <td><code>in </code> </td> 
   <td> <p>Gibt an, ob die [!UICONTROL übergeordnete] Sammlung die angegebene ID enthält.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL owners]</code></td> 
   <td>collection </td> 
   <td><code>in </code> </td> 
   <td> <p>Benutzer, denen die Datei gehört.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL writers]</code></td> 
   <td>collection </td> 
   <td><code>in </code> </td> 
   <td> <p>Benutzer, die berechtigt sind, die Datei zu ändern.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL readers] </code> </td> 
   <td>collection </td> 
   <td><code>in </code> </td> 
   <td> <p>Benutzer mit Berechtigung zum Lesen der Datei.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL sharedWithMe]</code> </td> 
   <td>Boolescher Wert </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p> Dateien, die sich in der Sammlung "Für mich freigegeben"des Benutzers befinden.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL properties] </code> </td> 
   <td>collection</td> 
   <td><code>has </code> </td> 
   <td> <p> Öffentliche benutzerdefinierte Dateieigenschaften.</p> </td> 
  </tr> 
 </tbody> 
</table>

Beachten Sie Folgendes zu Operatoren in diesen Feldern:

* Der Operator `contains` führt nur Präfixabgleich für eine `title` durch.

  Beispielsweise entspricht der Titel &quot;HelloWorld&quot;für `title contains 'Hello'`, nicht aber für `title contains 'World'`.

* Der Operator `contains` führt nur die Übereinstimmung mit gesamten String-Token für `fullText` durch.

  Wenn beispielsweise der Volltext eines Dokuments die Zeichenfolge &quot;HelloWorld&quot;enthält, gibt nur die Abfrage `fullText contains 'HelloWorld'` ein Ergebnis zurück. Abfragen wie `fullText contains 'Hello'` würden in diesem Szenario keine Ergebnisse zurückgeben.

* Der Operator `contains` entspricht einem exakten alphanumerischen Ausdruck, wenn er von doppelten Anführungszeichen umgeben ist.

  Wenn beispielsweise die Zeichenfolge &quot;`fullText`&quot;eines Dokuments die Zeichenfolge &quot;Hello There world&quot;enthält, gibt die Abfrage &quot;`fullText contains '"Hello there"'`&quot;ein Ergebnis zurück, die Abfrage &quot;`fullText contains '"Hello world"'`&quot;jedoch nicht.

  Da die Suche alphanumerisch ist, gibt die Abfrage `fullText contains '"Hello world"'` außerdem ein Ergebnis zurück, wenn die `fullText` eines Dokuments die Zeichenfolge &quot;Hello_world&quot;enthält.

* Die Felder mit dem Datum `type` sind derzeit nicht miteinander vergleichbar, sondern nur mit konstanten Daten.

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
   <td> <p>Surround mit einfachen Anführungszeichen '. Maskieren Sie einfache Anführungszeichen in Abfragen mit <code>\'</code>, z. B. <code> 'Valentine\'s Day'</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Boolesch </td> 
   <td> <p><code>true </code>oder <code>false</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Datum </td> 
   <td> <p>Format RFC 3339, Standardzeitzone ist UTC, z. B. <code>2012-06-04T12:00:00-08:00</code>.</p> </td> 
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
   <td> <p> Der Inhalt einer Zeichenfolge oder eines booleschen Werts entspricht dem anderen.</p> </td> 
  </tr> 
  <tr> 
   <td><code>!=</code> </td> 
   <td> <p> Der Inhalt einer Zeichenfolge oder eines booleschen Werts ist nicht gleich dem anderen.</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;</code> </td> 
   <td> <p> Ein Datum ist früher als ein anderes.</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;=</code> </td> 
   <td> <p> Ein Datum ist früher oder gleich einem anderen.</p> </td> 
  </tr> 
  <tr> 
   <td><code>></code> </td> 
   <td> <p> Ein Datum ist nach dem anderen.</p> </td> 
  </tr> 
  <tr> 
   <td><code>>=</code> </td> 
   <td> <p> Ein Datum ist nach oder gleich einem anderen.</p> </td> 
  </tr> 
  <tr> 
   <td><code>in </code> </td> 
   <td> <p>Ein Element ist in einer Sammlung enthalten.</p> </td> 
  </tr> 
  <tr> 
   <td><code>and </code> </td> 
   <td> <p>Gibt Dateien zurück, die beide Klauseln erfüllen.</p> </td> 
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
   <td> <p>Eine Kollektion enthält ein Element, das den Parametern entspricht.</p> </td> 
  </tr> 
 </tbody> 
</table>

Bei zusammengesetzten Klauseln können Sie Klammern verwenden, um Klauseln zu gruppieren. Beispiel:
`modifiedDate > '2012-06-04T12:00:00' and (mimeType contains 'image/' or mimeType contains 'video/')` Diese Suche gibt alle Dateien mit einem Bild- oder Video-MIME-Typ zurück, deren letzte Änderung nach dem 4. Juni 2012 erfolgte. Da die Operatoren `and` und `or` von links nach rechts ohne Klammern ausgewertet werden, gibt das obige Beispiel nur Bilder zurück, die nach dem 4. Juni 2012 geändert wurden, gibt jedoch alle Videos zurück, selbst die vor dem 4. Juni 2012.

### Beispiele

Alle Beispiele auf dieser Seite zeigen den nicht kodierten Parameter `<q>q</q>`, wobei `title = 'hello'` als `title+%3d+%27hello%27` kodiert ist. Client-Bibliotheken verarbeiten diese Kodierung automatisch.

* Suchen Sie nach Dateien mit dem Namen &quot;hello&quot;
  <pre>title = 'hello'</pre>
* Suchen Sie mithilfe des ordnerspezifischen MIME-Typs nach Ordnern
  <pre>mimeType = 'application/vnd.google-apps.folder'</pre>
* Suchen Sie nach Dateien, die keine Ordner sind
  <pre>mimeType != 'application/vnd.google-apps.folder'</pre>
* Suchen Sie nach Dateien mit einem Namen, der die Wörter &quot;hello&quot;und &quot;bye&quot;enthält.
  <pre>title enthält "hello"und [!UICONTROL name] enthält "bye".</pre>
* Suchen Sie nach Dateien mit einem Namen, der das Wort &quot;hello&quot;nicht enthält.
  <pre>kein Titel enthält 'hello'</pre>
* Suchen Sie nach Dateien, die das Wort &quot;hello&quot;im Inhalt enthalten
  <pre>fullText enthält 'hello'</pre>
* Suchen Sie nach Dateien, die das Wort &quot;hello&quot;im Inhalt nicht enthalten
  <pre>not fullText contains 'hello'</pre>
* Suchen Sie nach Dateien, die den genauen Wortlaut &quot;hello world&quot;im Inhalt enthalten.
  <pre>fullText enthält '"hello world"'fullText enthält '"hello_world"'</pre>
* Suchen Sie nach Dateien mit einer Abfrage, die das Zeichen &quot;\&quot;enthält (z. B. &quot;\authors&quot;).
  <pre>fullText enthält '\\authors'</pre>
* Suchen Sie nach Dateien, die vom Benutzer `test@example.org` geschrieben werden können.
  <pre>"test@example.org"in [!DNL writers]</pre>
* Suchen Sie in der `parents` -Sammlung nach der ID `1234567` . Dadurch werden alle Dateien und Ordner gefunden, die sich direkt im Ordner befinden, dessen Kennung `1234567` lautet.
  <pre>"1234567"in [!UICONTROL Eltern]</pre>
* Suchen Sie in der `parents` -Sammlung nach der Alias-ID `appDataFolder` . Dadurch werden alle Dateien und Ordner gefunden, die sich direkt im Ordner [Anwendungsdaten](https://developers.google.com/drive/api/v2/appdata) befinden.
  <pre>"appDataFolder"in übergeordneten Elementen</pre>
* Suchen Sie nach Dateien, die von den Benutzern `test@example.org` und `test2@example.org` geschrieben werden können.
  <pre>"test@example.org"in Schriftstellern und "test2@example.org"in Schriftstellern</pre>
* Suchen Sie nach Dateien mit dem Text &quot;wichtig&quot;, die sich im Papierkorb befinden.
  <pre>fullText enthält "wichtig"und ist durchgestrichen = true</pre>
* Suchen Sie nach Dateien, die nach dem 4. Juni 2012 geändert wurden.
  <pre>modifiedDate &gt; '2012-06-04T12:00:00' // Standard-Zeitzone ist UTC</pre><pre>modifiedDate &gt; '2012-06-04T12:00:00-08:00'</pre>
* Suchen Sie nach Dateien, die für den autorisierten Benutzer mit &quot;hello&quot;im Namen freigegeben wurden.
  <pre>sharedWithMe und title enthält 'hello'</pre>
* Suchen Sie nach Dateien mit der benutzerdefinierten Dateieigenschaft ](https://developers.google.com/drive/api/v2/properties) mit dem Namen `additionalID` mit dem Wert `8e8aceg2af2ge72e78`.[
  <pre>properties hat { key='additionalID' und value='8e8aceg2af2ge72e78' und visibility='PRIVATE' }</pre>

Source dieses Handbuchs ist [[!DNL Google Drive] documentation](https://developers.google.com/drive/api/v2/search-shareddrives).
