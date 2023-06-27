---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;agile-and-teams;user-management
keywords: Connector
navigation-topic: apps-and-their-modules
title: Google Team Drive-Module
description: Die [!DNL Adobe Workfront Fusion Google Team Drive] -Module ermöglichen es Ihnen, Dateien zu überwachen, hochzuladen, zu aktualisieren, zu kopieren, zu löschen oder abzurufen und Ordner in Ihren [!DNL Google Shared] Fahren Sie.
author: Becky
feature: Workfront Fusion
exl-id: 8b4c057f-bb98-44d1-9b71-cbeaa402a1c3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1306'
ht-degree: 0%

---

# [!DNL Google Team Drive]-Module

Die [!DNL Adobe Workfront Fusion] [!DNL Google Team Drive] -Module ermöglichen es Ihnen, Dateien zu überwachen, hochzuladen, zu aktualisieren, zu kopieren, zu löschen oder abzurufen und Ordner in Ihren [!DNL Google Shared Drive].

Zur Verwendung [!DNL Google Team Drive] mit [!DNL Adobe Workfront Fusion], muss ein [!DNL G Suite] -Konto. Wenn Sie noch keine haben, können Sie eine [!DNL G Suite] -Konto [[!DNL G Suite] Website anmelden](https://gsuite.google.com/signup/businessstarter/welcome).

In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL Google Team Drive], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.

Informationen zum Erstellen eines Szenarios finden Sie unter [Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Ältere Lizenzanforderungen: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderungen: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Ältere Produktanforderungen: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Verwendung [!DNL Google Team Drive] -Module, müssen Sie über eine [!DNL Google Team Drive].

## [!DNL Google Team Drive] Module und ihre Felder

Bei der Konfiguration [!DNL Google Team Drive] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Google Team Drive] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Die Dialogfelder für das Modul, die in **fett** (im [!DNL Workfront Fusion] Szenario, **not** in diesem Dokumentationsartikel) sind obligatorisch.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Trigger

#### [!UICONTROL Überwachungsdateien]

Gibt Dateidetails zurück, wenn eine neue Datei im angegebenen Ordner hinzugefügt und/oder geändert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google Team Drive] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
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
   <td>[!UICONTROL Convert [!DNL Google Documents] zu formatierende Dateien] </td> 
   <td> <p>Wählen Sie das Format aus, in dem die Uhr ausgeführt werden soll [!DNL Google Documents] -Dateien in konvertiert.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Sheets] zu formatierende Dateien] </td> 
   <td> <p>Wählen Sie das Format aus, in dem die Uhr ausgeführt werden soll [!DNL Google Sheets] -Dateien in konvertiert.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Slides] zu formatierende Dateien] </td> 
   <td> <p>Wählen Sie das Format aus, in dem die Uhr ausgeführt werden soll [!DNL Google Slides] -Dateien in konvertiert.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Drawings] zu formatierende Dateien] </td> 
   <td> <p>Wählen Sie das Format aus, in dem die Uhr ausgeführt werden soll [!DNL Google Drawings] -Dateien in konvertiert.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p> Wählen Sie aus, ob Sie den Ordner auf neue und geänderte Dateien oder nur auf neue Dateien überwachen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl heruntergeladener Dateien]</td> 
   <td> <p> Maximale Dateianzahl festlegen [!DNL Workfront Fusion] wird während eines Ausführungszyklus zurückgegeben.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL Datei hochladen]](#upload-a-file)
* [[!UICONTROL Datei aktualisieren]](#update-a-file)
* [[!UICONTROL Eine Datei kopieren]](#copy-a-file)
* [[!UICONTROL Datei löschen]](#delete-a-file)
* [[!UICONTROL Verschieben einer Datei in den Papierkorb]](#move-a-file-to-trash)
* [[!UICONTROL Datei abrufen]](#get-a-file)
* [[!UICONTROL Dateiliste abrufen]](#get-a-file-list)
* [[!UICONTROL Erstellen eines Ordners]](#create-a-folder)

#### [!UICONTROL Datei hochladen]

Lädt eine Datei auf das angegebene freigegebene Laufwerk hoch.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google Team Drive] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
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
   <td> <p>[!UICONTROL Quelldatei]</p> </td> 
   <td> <p>Geben Sie die Datei an, die Sie auf das freigegebene Laufwerk hochladen möchten.</p> <p>Ordnen Sie die Datei zu, die Sie vom vorherigen Modul hochladen möchten (z. B. [!UICONTROL HTTP] &gt; [!UICONTROL Datei abrufen] oder [!UICONTROL Dropbox] &gt;[!UICONTROL Datei abrufen)] oder geben Sie den Dateinamen und die Dateidaten manuell ein.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden der [!DNL Google Team Drive] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
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
   <td> <p>[!UICONTROL Quelldatei]</p> </td> 
   <td>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Titel] </td> 
   <td> <p>Geben Sie den neuen Titel für die aktualisierte Datei ein.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei konvertieren]</td> 
   <td> <p> Aktivieren Sie diese Option, um die Datei in die entsprechende [!DNL Google] in Ihrem freigegebenen Ordner speichern.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden der [!DNL Google Team Drive] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
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
   <td> <p>Anweisungen zum Verbinden der [!DNL Google Team Drive] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
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
   <td> <p>Anweisungen zum Verbinden der [!DNL Google Team Drive] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
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
   <td> <p>Anweisungen zum Verbinden der [!DNL Google Team Drive] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Documents] zu formatierende Dateien] </td> 
   <td> <p>Wählen Sie das gewünschte Format aus. [!DNL Google Documents] -Dateien in konvertiert.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Sheets] zu formatierende Dateien] </td> 
   <td> <p>Wählen Sie das gewünschte Format aus. [!DNL Google Sheets] -Dateien in konvertiert.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Slides] zu formatierende Dateien] </td> 
   <td> <p>Wählen Sie das gewünschte Format aus. [!DNL Google Slides] -Dateien in konvertiert.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Drawings] zu formatierende Dateien] </td> 
   <td> <p>Wählen Sie das gewünschte Format aus. [!DNL Google Drawings] -Dateien in konvertiert.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei-ID]</td> 
   <td> <p> Geben Sie die Kennung der Datei ein, die Sie abrufen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Dateiliste abrufen]

Ruft Dateien und/oder Ordnerdetails basierend auf dem Suchbegriff ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google Team Drive] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
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
     <li> <p style="font-weight: bold;">[!UICONTROL Benutzerdefinierte Suchabfrage]</p> <p>Geben Sie die [!DNL Google] Suchabfragebegriff. Weitere Informationen finden Sie unter [!DNL Google]s <a href="https://developers.google.com/drive/api/v2/ref-search-terms">Dokumentation zu Suchabfragen</a>. Beispiel: <code>fullText contains '"Hello world"'</code></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Retrieve]</td> 
   <td>Wählen Sie aus, ob Sie Dateien, Ordner oder beides abrufen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl an zurückgegebenen Ergebnissen]</td> 
   <td> <p> Maximale Anzahl von Dateien oder Ordnern festlegen [!DNL Workfront Fusion] wird während eines Ausführungszyklus zurückgegeben.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden der [!DNL Google Team Drive] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
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
