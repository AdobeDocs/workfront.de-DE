---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;agile-and-teams;user-management
keywords: Steckverbinder
navigation-topic: apps-and-their-modules
title: Google Team Drive-Module
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 8b4c057f-bb98-44d1-9b71-cbeaa402a1c3
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1353'
ht-degree: 0%

---

# [!DNL Google Team Drive]

Die [!DNL Adobe Workfront Fusion] [!DNL Google Team Drive] ermöglichen es Ihnen, Dateien zu überwachen, hochzuladen, zu aktualisieren, zu kopieren, zu löschen oder abzurufen und Ordner in Ihrem [!DNL Google Shared Drive] zu erstellen.

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Google Team Drive-Module](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-team-drive-modules.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Um [!DNL Google Team Drive] mit [!DNL Adobe Workfront Fusion] verwenden zu können, muss ein [!DNL Google Workspace] Konto vorhanden sein. Wenn Sie noch kein solches Konto haben, können Sie ein [!DNL Google Workspace] Konto bei der [[!DNL Google Workspace] Anmeldeseite“ ](https://workspace.google.com/business/signup/welcome).

In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die [!DNL Google Team Drive] verwenden, und sie mit mehreren Anwendungen und Services von Drittanbietern verbinden.

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

## Voraussetzungen

Um [!DNL Google Team Drive] Module verwenden zu können, müssen Sie über eine [!DNL Google Team Drive] verfügen.

## [!DNL Google Team Drive] Module und ihre Felder

Beim Konfigurieren [!DNL Google Team Drive] Module zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder dem Service weitere [!DNL Google Team Drive] angezeigt werden. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

Die Dialogfelder für Module, die in **fett** angezeigt werden (im [!DNL Workfront Fusion] Szenario **nicht** diesem Dokumentationsartikel), sind obligatorisch.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Trigger

#### [!UICONTROL Dateien ansehen]

Gibt Dateidetails zurück, wenn eine neue Datei im angegebenen Ordner hinzugefügt und/oder geändert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Team Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Teamlaufwerk]</td> 
   <td> <p> Wählen Sie das freigegebene Laufwerk aus, das Sie überwachen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Ordner] </td> 
   <td> <p>Wählen Sie den Ordner im freigegebenen Laufwerk aus.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Welche Dateien beobachtet werden]</td> 
   <td> <p> Wählen Sie den Typ der Dateien aus, die Sie beobachten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Documents] Dateien ins Format konvertieren] </td> 
   <td> <p>Wählen Sie das Format aus, in das die überwachten [!DNL Google Documents] konvertiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Sheets] Dateien ins Format konvertieren] </td> 
   <td> <p>Wählen Sie das Format aus, in das die überwachten [!DNL Google Sheets] konvertiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Slides] Dateien ins Format konvertieren] </td> 
   <td> <p>Wählen Sie das Format aus, in das die überwachten [!DNL Google Slides] konvertiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Drawings] Dateien ins Format konvertieren] </td> 
   <td> <p>Wählen Sie das Format aus, in das die überwachten [!DNL Google Drawings] konvertiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Uhr]</td> 
   <td> <p> Wählen Sie aus, ob Sie den Ordner auf neue und geänderte Dateien oder nur auf neue Dateien überwachen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl heruntergeladener Dateien]</td> 
   <td> <p> Legen Sie die maximale Anzahl von Dateien fest, die [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgeben.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL Datei hochladen]](#upload-a-file)
* [[!UICONTROL Aktualisieren einer Datei]](#update-a-file)
* [[!UICONTROL Kopieren einer Datei]](#copy-a-file)
* [[!UICONTROL Datei löschen]](#delete-a-file)
* [[!UICONTROL Verschieben einer Datei in den Papierkorb]](#move-a-file-to-trash)
* [[!UICONTROL Datei abrufen]](#get-a-file)
* [[!UICONTROL Dateiliste abrufen]](#get-a-file-list)
* [[!UICONTROL Ordner erstellen]](#create-a-folder)

#### [!UICONTROL Datei hochladen]

Lädt eine Datei auf das angegebene freigegebene Laufwerk hoch.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Team Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Teamlaufwerk] </td> 
   <td> <p>Wählen Sie das freigegebene Laufwerk aus, auf das Sie eine Datei hochladen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Ordner] </td> 
   <td> <p>Wählen Sie den Ordner im freigegebenen Laufwerk aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Source-Datei]</p> </td> 
   <td> <p>Geben Sie die Datei an, die Sie auf das freigegebene Laufwerk hochladen möchten.</p> <p>Ordnen Sie die Datei zu, die Sie aus dem vorherigen Modul (z. B. [!UICONTROL HTTP] &gt;[!UICONTROL Datei abrufen] oder [!UICONTROL Dropbox] &gt;[!UICONTROL (Datei abrufen)]], oder geben Sie den Dateinamen und die Dateidaten manuell ein.</p> </td> 
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

#### [!UICONTROL Aktualisieren einer Datei]

Ermöglicht das Ändern des Dateinamens und/oder des Dateiinhalts.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Team Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Teamlaufwerk]</td> 
   <td> <p> Wählen Sie das freigegebene Laufwerk aus, das die zu aktualisierende Datei enthält.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Ordner] </td> 
   <td> <p>Wählen Sie den Ordner im freigegebenen Laufwerk aus.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei-ID]</td> 
   <td> <p> Geben Sie die ID der Datei ein, die Sie aktualisieren möchten (zuordnen).</p> </td> 
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
   <td> <p> Aktivieren Sie diese Option, um die Datei in das entsprechende [!DNL Google] in Ihrem freigegebenen Ordner zu konvertieren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kopieren einer Datei]

Kopiert eine angegebene Datei in den ausgewählten Ordner.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Team Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Teamlaufwerk]</td> 
   <td> <p> Wählen Sie das freigegebene Laufwerk aus, das die zu kopierende Datei enthält.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Ordner] </td> 
   <td> <p>Wählen Sie den Zielordner aus, in den Sie die Datei kopieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei-ID]</td> 
   <td> <p> Geben Sie die ID der Datei ein, die Sie kopieren möchten (zuordnen).</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Der Name der Kopierdatei]</p> </td> 
   <td> <p>Geben Sie den neuen Dateinamen ein, wenn er am Zielspeicherort geändert werden soll.</p> </td> 
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
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Team Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei-ID]</td> 
   <td> <p> Geben Sie die ID der Datei ein, die Sie löschen möchten, oder mappen Sie sie.</p> </td> 
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
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Team Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei-ID]</td> 
   <td> <p> Geben Sie die ID der Datei ein, die Sie in den Papierkorb verschieben möchten, oder mappen Sie sie.</p> </td> 
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
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Team Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Documents] Dateien ins Format konvertieren] </td> 
   <td> <p>Wählen Sie das Format aus, in das die [!DNL Google Documents] konvertiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Sheets] Dateien ins Format konvertieren] </td> 
   <td> <p>Wählen Sie das Format aus, in das die [!DNL Google Sheets] konvertiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Slides] Dateien ins Format konvertieren] </td> 
   <td> <p>Wählen Sie das Format aus, in das die [!DNL Google Slides] konvertiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Google Drawings] Dateien ins Format konvertieren] </td> 
   <td> <p>Wählen Sie das Format aus, in das die [!DNL Google Drawings] konvertiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei-ID]</td> 
   <td> <p> Geben Sie die ID der Datei ein, die Sie abrufen möchten, oder mappen Sie sie.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Dateiliste abrufen]

Ruft Dateien- und/oder Ordnerdetails basierend auf dem Suchbegriff ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Team Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Teamlaufwerk]</td> 
   <td> <p> Wählen Sie das freigegebene Laufwerk aus, dessen Dateien aufgelistet werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Ordner] </td> 
   <td> <p>Wählen Sie den Ordner aus, aus dem Sie Dateien auflisten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Suche] </td> 
   <td> <p>Wählen Sie die Art der Suche aus, die Sie durchführen möchten - siehe unten.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL-Abfrage]</p> </td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>[!UICONTROL Innerhalb von Dateinamen suchen]</p> <p style="font-weight: normal;">Geben Sie den Dateinamen (einschließlich der Dateierweiterung) ein, wenn die Option [!UICONTROL Suche nach exaktem Begriff] ausgewählt ist, oder geben Sie den Teil des Namens ein, wenn die Option [!UICONTROL Suche nach Namen, die den gesuchten Begriff enthalten] ausgewählt ist.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Volltextsuche]</p> <p>Geben Sie den Suchbegriff ein, um die Dateinamen, Beschreibungen und Inhalte zu durchsuchen.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Benutzerdefinierte Suchabfrage]</p> <p>Geben Sie den [!DNL Google] Suchabfragebegriff ein. Weitere Informationen finden Sie in der [!DNL Google]-<a href="https://developers.google.com/drive/api/v2/ref-search-terms"> (Dokumentation zu Suchanfragen</a>. Beispiel: <code>fullText contains '"Hello world"'</code></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL abrufen]</td> 
   <td>Wählen Sie aus, ob Sie Dateien, Ordner oder beides abrufen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl der zurückgegebenen Ergebnisse]</td> 
   <td> <p> Legen Sie die maximale Anzahl von Dateien oder Ordnern fest, die [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgeben.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ordner erstellen]

Erstellt einen neuen Ordner.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Team Drive]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Teamlaufwerk]</td> 
   <td> <p> Wählen Sie das freigegebene Laufwerk aus, auf dem Sie einen Ordner erstellen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Ordner] </td> 
   <td> <p>Wählen Sie den Ordner aus, in dem Sie einen Ordner erstellen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Der Name des neuen Ordners]</td> 
   <td> <p> Geben Sie den Namen des neuen Ordners ein.</p> </td> 
  </tr> 
 </tbody> 
</table>
