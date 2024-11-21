---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;agile-and-teams;user-management
keywords: Connector
navigation-topic: apps-and-their-modules
title: Google Team Drive-Module
description: Mit den [!DNL Adobe Workfront Fusion Google Team Drive] Modulen können Sie Dateien überwachen, hochladen, aktualisieren, kopieren, löschen oder abrufen und Ordner in Ihrem [!DNL Google Shared] Laufwerk erstellen.
author: Becky
feature: Workfront Fusion
exl-id: 8b4c057f-bb98-44d1-9b71-cbeaa402a1c3
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1297'
ht-degree: 0%

---

# [!DNL Google Team Drive] Module

Mit den Modulen [!DNL Adobe Workfront Fusion] [!DNL Google Team Drive] können Sie Dateien überwachen, hochladen, aktualisieren, kopieren, löschen oder abrufen und Ordner in Ihrem [!DNL Google Shared Drive] erstellen.

Um [!DNL Google Team Drive] mit [!DNL Adobe Workfront Fusion] zu verwenden, ist ein [!DNL Google Workspace] -Konto erforderlich. Wenn Sie keines haben, können Sie ein [!DNL Google Workspace] -Konto auf der [[!DNL Google Workspace] Anmelde-Site](https://workspace.google.com/business/signup/welcome) erstellen.

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL Google Team Drive] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

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
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebene Funktionalität nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Um [!DNL Google Team Drive] -Module zu verwenden, müssen Sie über einen [!DNL Google Team Drive] verfügen.

## [!DNL Google Team Drive] Module und ihre Felder

Wenn Sie [!DNL Google Team Drive] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Google Team Drive] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Die Moduldialogfelder, die in **fett** angezeigt werden (im Szenario [!DNL Workfront Fusion] sind in diesem Dokumentationsartikel **nicht**), sind obligatorisch.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Trigger

#### [!UICONTROL Dateien ansehen]

Gibt Dateidetails zurück, wenn eine neue Datei im angegebenen Ordner hinzugefügt und/oder geändert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Team Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Wählen Sie das freigegebene Laufwerk aus, das Sie sehen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie den Ordner auf dem freigegebenen Laufwerk aus.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Welche Dateien sind zu sehen?]</td> 
   <td> <p> Wählen Sie den Dateityp aus, den Sie sehen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Documents] Dateien in Format konvertieren] </td> 
   <td> <p>Wählen Sie das Format aus, in das die überwachten [!DNL Google Documents]-Dateien konvertiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Sheets] Dateien in Format konvertieren] </td> 
   <td> <p>Wählen Sie das Format aus, in das die überwachten [!DNL Google Sheets]-Dateien konvertiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Slides] Dateien in Format konvertieren] </td> 
   <td> <p>Wählen Sie das Format aus, in das die überwachten [!DNL Google Slides]-Dateien konvertiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Drawings] Dateien in Format konvertieren] </td> 
   <td> <p>Wählen Sie das Format aus, in das die überwachten [!DNL Google Drawings]-Dateien konvertiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p> Wählen Sie aus, ob Sie den Ordner auf neue und geänderte Dateien oder nur auf neue Dateien überwachen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl heruntergeladener Dateien]</td> 
   <td> <p> Legen Sie die maximale Anzahl von Dateien fest, die [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgibt.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL  Datei hochladen]](#upload-a-file)
* [[!UICONTROL Datei aktualisieren]](#update-a-file)
* [[!UICONTROL Eine Datei kopieren]](#copy-a-file)
* [[!UICONTROL Datei löschen]](#delete-a-file)
* [[!UICONTROL Verschieben einer Datei in den Papierkorb]](#move-a-file-to-trash)
* [[!UICONTROL Datei abrufen]](#get-a-file)
* [[!UICONTROL Abrufen einer Dateiliste]](#get-a-file-list)
* [[!UICONTROL Erstellen eines Ordners]](#create-a-folder)

#### [!UICONTROL  Datei hochladen]

Lädt eine Datei auf das angegebene freigegebene Laufwerk hoch.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Team Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive] </td> 
   <td> <p>Wählen Sie das freigegebene Laufwerk aus, auf das Sie eine Datei hochladen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie den Ordner auf dem freigegebenen Laufwerk aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Source-Datei]</p> </td> 
   <td> <p>Geben Sie die Datei an, die Sie auf das freigegebene Laufwerk hochladen möchten.</p> <p>Ordnen Sie die Datei zu, die Sie vom vorherigen Modul hochladen möchten (z. B. [!UICONTROL HTTP] &gt;[!UICONTROL Datei abrufen] oder [!UICONTROL Dropbox] &gt;[!UICONTROL Datei abrufen)] oder geben Sie den Dateinamen und die Dateidaten manuell ein.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Titel]</td> 
   <td> <p> Geben Sie den Titel der Datei ein, die im freigegebenen Ordner angezeigt werden soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei konvertieren]</td> 
   <td> <p> Aktivieren Sie diese Option, um die Datei in das entsprechende Google-Format in Ihrem freigegebenen Ordner zu konvertieren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei aktualisieren]

Ändert den Dateinamen und/oder den Dateiinhalt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Team Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Wählen Sie das freigegebene Laufwerk aus, das die zu aktualisierende Datei enthält.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie den Ordner auf dem freigegebenen Laufwerk aus.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei-ID]</td> 
   <td> <p> Geben Sie die Kennung der Datei ein, die Sie aktualisieren möchten (zuordnen).</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Source-Datei]</p> </td> 
   <td>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Titel] </td> 
   <td> <p>Geben Sie den neuen Titel für die aktualisierte Datei ein.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei konvertieren]</td> 
   <td> <p> Aktivieren Sie diese Option, um die Datei in das entsprechende [!DNL Google] -Format in Ihrem freigegebenen Ordner zu konvertieren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eine Datei kopieren]

Kopiert eine angegebene Datei in den ausgewählten Ordner.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Team Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Wählen Sie das freigegebene Laufwerk aus, das die zu kopierende Datei enthält.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie den Zielordner aus, in den Sie die Datei kopieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei-ID]</td> 
   <td> <p> Geben Sie die Kennung der Datei ein, die Sie kopieren möchten (mappen Sie sie).</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Der Name der Kopierdatei]</p> </td> 
   <td> <p>Geben Sie den neuen Dateinamen ein, wenn Sie ihn am Zielspeicherort ändern möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei löschen]

Löscht eine angegebene Datei.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Team Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei-ID]</td> 
   <td> <p> Geben Sie die Kennung der Datei ein, die Sie löschen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Verschieben einer Datei in den Papierkorb]

Verschiebt eine angegebene Datei in den Papierkorb.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Team Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei-ID]</td> 
   <td> <p> Geben Sie die Kennung der Datei ein, die Sie in den Papierkorb verschieben möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei abrufen]

Ruft Details zur angegebenen Datei ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Team Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Documents] Dateien in Format konvertieren] </td> 
   <td> <p>Wählen Sie das Format aus, in das die [!DNL Google Documents]-Dateien konvertiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Sheets] Dateien in Format konvertieren] </td> 
   <td> <p>Wählen Sie das Format aus, in das die [!DNL Google Sheets]-Dateien konvertiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Slides] Dateien in Format konvertieren] </td> 
   <td> <p>Wählen Sie das Format aus, in das die [!DNL Google Slides]-Dateien konvertiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Drawings] Dateien in Format konvertieren] </td> 
   <td> <p>Wählen Sie das Format aus, in das die [!DNL Google Drawings]-Dateien konvertiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei-ID]</td> 
   <td> <p> Geben Sie die Kennung der Datei ein, die Sie abrufen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Abrufen einer Dateiliste]

Ruft Dateien und/oder Ordnerdetails basierend auf dem Suchbegriff ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Team Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Wählen Sie das freigegebene Laufwerk aus, von dem Sie Dateien auflisten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie den Ordner aus, aus dem Sie Dateien auflisten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Suche] </td> 
   <td> <p>Wählen Sie den gewünschten Suchtyp aus (siehe unten).</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Abfrage]</p> </td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>[!UICONTROL Suche in Dateinamen]</p> <p style="font-weight: normal;">Geben Sie den Dateinamen (einschließlich der Dateierweiterung) ein, wenn die Option [!UICONTROL Suche nach dem genauen Begriff Suche] ausgewählt ist, oder geben Sie den Teil des Namens ein, wenn die Option [!UICONTROL Suche nach Namen, die den gesuchten Begriff enthalten] ausgewählt ist.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Volltextsuche]</p> <p>Geben Sie den Suchbegriff ein, um nach Dateinamen, Beschreibungen und Inhalten zu suchen.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Benutzerdefinierte Suchabfrage]</p> <p>Geben Sie den Suchabfragebegriff [!DNL Google] ein. Weitere Informationen finden Sie in der <a href="https://developers.google.com/drive/api/v2/ref-search-terms">Dokumentation zu Suchabfragen</a> von [!DNL Google]. Beispiel: <code>fullText contains '"Hello world"'</code></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Retrieve]</td> 
   <td>Wählen Sie aus, ob Sie Dateien, Ordner oder beides abrufen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl an zurückgegebenen Ergebnissen]</td> 
   <td> <p> Legen Sie die maximale Anzahl von Dateien oder Ordnern fest, die [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgibt.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Erstellen eines Ordners]

Erstellt einen neuen Ordner.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Team Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Wählen Sie das freigegebene Laufwerk aus, auf dem Sie einen Ordner erstellen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie den Ordner aus, in dem Sie einen Ordner erstellen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Der Name des neuen Ordners]</td> 
   <td> <p> Geben Sie den Namen des neuen Ordners ein.</p> </td> 
  </tr> 
 </tbody> 
</table>
