---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connector
navigation-topic: apps-and-their-modules
title: Dropbox-Module
description: In einem [!DNL Adobe Workfront Fusion] szenario können Sie Workflows automatisieren, die Dropbox verwenden, und sie mit mehreren Drittanbieteranwendungen und -diensten verbinden. Dies ermöglicht Ihnen die Automatisierung von Aktivitäten wie Überwachung, Suche, Abrufen, Auflisten, Erstellen und Bearbeiten von Dateien und Ordnern in Ihrer Dropbox.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: a35631d7-40ac-4e7f-9a37-ad3879c0b6a2
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '3230'
ht-degree: 0%

---

# [!DNL Dropbox] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!UICONTROL Dropbox] oder [!DNL Dropbox Business] verwenden, und sie mit mehreren Drittanbieteranwendungen und -diensten verbinden. Dies ermöglicht Ihnen die Automatisierung von Aktivitäten wie Überwachung, Suche, Abrufen, Auflisten, Erstellen und Bearbeiten von Dateien und Ordnern in Ihrer [!UICONTROL Dropbox].

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

* Um [!DNL Dropbox] -Module zu verwenden, müssen Sie über ein [!DNL Dropbox] -Konto verfügen.

>[!IMPORTANT]
>
>Dropbox muss Anwendungen mit mehr als 50 Nutzern genehmigen.
>
>Weitere Informationen finden Sie unter &quot;Produktionsgenehmigung&quot;im Dropbox-Entwicklerhandbuch.

## Dropbox-API-Informationen

Der Dropbox-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Basis-URL</td> 
   <td> https://api.dropboxapi.com/2    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Version</td> 
   <td> 2 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td><ul><li><p>Dropbox</p><p>v5.3.9</p></li><li><p>Dropbox Business</p><p>v1.0.12</p></li></ul></td> 
  </tr>
 </tbody> 
 </table>


## Erstellen einer Verbindung zu [!DNL Dropbox]

So erstellen Sie eine Verbindung für Ihre [!DNL Dropbox] -Module:

1. Klicken Sie neben dem Feld Verbindung auf **[!UICONTROL Hinzufügen]** .

1. Füllen Sie die folgenden Felder aus:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[!UICONTROL Verbindungsname]</td>
        <td>
          <p>Geben Sie einen Namen für diese Verbindung ein.</p>
        </td>
        <tr>
        <td role="rowheader">[!UICONTROL Umgebung]</td>
        <td>Wählen Sie aus, ob diese Verbindung für eine Produktions- oder Nicht-Produktionsumgebung vorgesehen ist.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Typ]</td>
        <td>Wählen Sie aus, ob Sie eine Verbindung zu einem Dienstkonto oder einem persönlichen Konto herstellen möchten.</td>
        </tr>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client-ID]</td>
        <td>Geben Sie Ihre [!UICONTROL Dropbox] [!UICONTROL Client ID] ein. </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Geben Sie Ihren [!DNL Dropbox] [!UICONTROL Client Secret] ein. </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Kontotyp]</td>
        <td>Wählen Sie aus, ob Sie eine Verbindung zu einem persönlichen Dropbox-Konto oder einem geschäftlichen Konto (Dropbox Business) herstellen.</td>
        </tr>
      </tbody>
    </table>

1. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindung zu speichern und zum Modul zurückzukehren.## [!DNL Dropbox] Module und ihre Felder

## [!DNL Dropbox] Module und ihre Felder

Wenn Sie [!DNL Dropbox] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Dropbox] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Trigger-Module](#trigger-modules)
* [Module zum Abrufen von [!DNL Dropbox] Dateien und Ordnern](#modules-for-getting-dropbox-files-and-folders)
* [Module zum Erstellen und Bearbeiten von [!DNL Dropbox] Dateien und Ordnern](#modules-for-creating-and-editing-dropbox-files-and-folders)
* [Sonstige Module](#other-modules)

### Trigger-Module

#### [!UICONTROL Dateien ansehen]

Dieses Trigger-Typ-Modul gibt Dateidetails zurück, wenn die Datei in einem angegebenen Ordner geändert wird.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Dropbox]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-dropbox" class="MCXref xref">Erstellen einer Verbindung mit [!DNL Dropbox]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie den Ordner aus, den Sie auf Änderungen überwachen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Überwacht auch Unterordner]</td> 
   <td> <p> Aktivieren Sie diese Option, um auch die Unterordner im ausgewählten Ordner auf geänderte Dateien zu überwachen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit] </td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Module zum Abrufen von [!DNL Dropbox]-Dateien und -Ordnern

* [[!UICONTROL Dateien/Ordner durchsuchen]](#search-filesfolders)
* [[!UICONTROL Datei herunterladen]](#download-a-file)
* [[!UICONTROL Abrufen von Ordnermetadaten]](#get-a-folder-metadata)
* [[!UICONTROL Alle Dateien/Unterordner in einem Ordner auflisten]](#list-all-filessubfolders-in-a-folder)
* [[!UICONTROL Listendateiüberarbeitungen]](#list-file-revisions)

#### [!UICONTROL Dateien/Ordner durchsuchen]

Dieses Suchmodul sucht nach Datensätzen in einem Objekt in [!DNL Dropbox], die mit der von Ihnen angegebenen Suchabfrage übereinstimmen.

Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Dropbox]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-dropbox" class="MCXref xref">Erstellen einer Verbindung mit [!DNL Dropbox]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Suche] </td> 
   <td> <p>Geben Sie den Suchbegriff ein.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie den Ordner aus, den Sie suchen möchten. Dieses Modul durchsucht den gesamten [!DNL Dropbox] , wenn Sie keinen Ordner auswählen.</p> </td> 
  </tr> 
  <tr> 
   <td>Dateistatus</td> 
   <td> <p> Wählen Sie den Dateistatus aus, um die Suche auf den ausgewählten Dateistatus zu beschränken.</p> </td> 
  </tr> 
  <tr> 
   <td>Dateikategorien</td> 
   <td> <p> Wählen Sie die Dateikategorien aus, um die Suche auf die ausgewählten Kategorien zu beschränken.</p> </td> 
  </tr> 
  <tr> 
   <td>Dateierweiterungen</td> 
   <td> <p> Wählen Sie die Dateierweiterungen aus, nach denen Sie suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>Limit </td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei herunterladen]

Dieses Aktionsmodul lädt eine Datei aus einem Ordner herunter.

Sie geben die Datei und ihren Speicherort an.

Das Modul gibt die Kennung der Datei und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

>[!NOTE]
>
>Dieses Modul ist nützlich, um Dateien für nachfolgende Module bereitzustellen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Dropbox]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-dropbox" class="MCXref xref">Erstellen einer Verbindung mit [!DNL Dropbox]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>Dateiauswahl</td> 
   <td> <p> Wählen Sie aus, ob Sie den Dateipfad zuordnen oder die Datei manuell auswählen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dateipfad/Datei</p> </td> 
   <td> <p style="font-weight: bold;">Dateipfad</p> <p>Geben Sie den Zielpfad der Datei ein oder ordnen Sie ihn zu.</p> <p style="font-weight: bold;">Datei</p> <p>Wählen Sie die Datei aus dem Menü aus.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Abrufen von Ordnermetadaten]

Dieses Aktionsmodul ruft Details zu freigegebenen Ordnern ab.

Sie geben die Kennung des Ordners an.

Das Modul gibt die Kennung des Ordners sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Dropbox]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-dropbox" class="MCXref xref">Erstellen einer Verbindung mit [!DNL Dropbox]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>Freigegebene Ordner-ID</td> 
   <td> <p> Geben Sie die Kennung des Ordners ein, zu dem Sie Details abrufen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Alle Dateien/Unterordner in einem Ordner auflisten]

Dieses Aktionsmodul listet Dateien oder Ordner in einem bestimmten Ordner auf.

Sie geben die Kennung des Ordners an.

Das Modul gibt die IDs der Dateien oder Ordner und der zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Dropbox]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-dropbox" class="MCXref xref">Erstellen einer Verbindung mit [!DNL Dropbox]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>Liste </td> 
   <td> <p>Wählen Sie aus, ob Sie Dateien oder Ordner abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>Nur herunterladbare Dateien anzeigen</td> 
   <td> <p> Aktivieren Sie diese Option, um nur herunterladbare Dateien zurückzugeben. Einige Dateitypen, z. B. Google-Dokumente, können nicht heruntergeladen werden.</p> </td> 
  </tr> 
  <tr> 
   <td>Ordner </td> 
   <td> <p>Geben Sie den Ordner ein oder ordnen Sie ihn zu, aus dem Sie Dateien oder Ordner abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>Limit </td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während des Ausführungszyklus eines Szenarios auflisten soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listendateiüberarbeitungen]

Dieses Aktionsmodul ruft alle Dateirevisionen (einen Versionsverlauf) einer bestimmten Datei ab.\
Sie geben die Kennung der Datei an.

Das Modul gibt alle mit dem Datensatz verknüpften Standardfelder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Dropbox]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-dropbox" class="MCXref xref">Erstellen einer Verbindung mit [!DNL Dropbox]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>Dateiauswahl</td> 
   <td> <p> Wählen Sie aus, ob Sie den Dateipfad zuordnen oder die Datei manuell auswählen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dateipfad/Datei</p> </td> 
   <td> <p style="font-weight: bold;">Dateipfad</p> <p>Geben Sie den Zielpfad der Datei ein oder ordnen Sie ihn zu.</p> <p style="font-weight: bold;">Datei</p> <p>Wählen Sie die Datei aus dem Menü aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Limit</p> </td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während des Ausführungszyklus eines Szenarios auflisten soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Module zum Erstellen und Bearbeiten von [!DNL Dropbox]-Dateien und -Ordnern

* [[!UICONTROL Eine Datei hochladen]](#upload-a-file)
* [[!UICONTROL Erstellen eines Ordners]](#create-a-folder)
* [[!UICONTROL Erstellen/Überschreiben einer Textdatei]](#createoverwrite-a-text-file)
* [[!UICONTROL Erstellen/Aktualisieren eines Freigabe-Links]](#createupdate-a-share-link)
* [[!UICONTROL Datei wiederherstellen]](#restore-a-file)
* [[!UICONTROL Verschieben einer Datei/eines Ordners]](#move-a-filefolder)
* [[!UICONTROL Umbenennen einer Datei/eines Ordners]](#rename-a-filefolder)
* [[!UICONTROL Datei/Ordner löschen]](#delete-a-filefolder)

#### [!UICONTROL  Datei hochladen]

Dieses Aktionsmodul lädt eine Datei in einen Ordner hoch.

Sie geben Informationen wie den Speicherort der Datei, die Datei, die Sie hochladen möchten, und einen optionalen neuen Namen für die Datei an.

Das Modul gibt die Kennung der Datei und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Dropbox]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-dropbox" class="MCXref xref">Erstellen einer Verbindung mit [!DNL Dropbox]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner]</td> 
   <td> <p> Wählen Sie den Ordner Ihres [!DNL Dropbox] aus, in den Sie die Datei hochladen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Source-Datei]</p> </td> 
   <td> <p>Geben Sie die Datei ein oder ordnen Sie sie dem oben ausgewählten Ordner [!DNL Dropbox] zu.</p> <p style="font-weight: bold;">[!UICONTROL Dateiname]</p> <p>Geben Sie den Dateinamen einschließlich der Dateierweiterung ein oder ordnen Sie ihn zu.</p> <p style="font-weight: bold;">[!UICONTROL Dateidaten]</p> <p>Geben Sie die Dateidaten ein oder ordnen Sie sie zu (aus dem vorherigen Modul wie [!UICONTROL Google Drive] &gt;[!UICONTROL Datei abrufen)).</p> <p>Hinweis: Die maximale Größe der hochgeladenen Datei beträgt 150 MB.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vorhandene Datei überschreiben]</td> 
   <td> <p> Aktivieren Sie diese Option, um die vorhandene Datei durch die neue zu ersetzen. Wenn diese Option deaktiviert bleibt, wird die hochgeladene Datei umbenannt.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Erstellen eines Ordners]

Dieses Aktionsmodul erstellt einen neuen Ordner.

Sie geben den Pfad und einen Namen für den Ordner an.

Das Modul gibt die Kennung des Ordners sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Dropbox]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-dropbox" class="MCXref xref">Erstellen einer Verbindung mit [!DNL Dropbox]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordnername] </td> 
   <td> <p>Geben Sie den Namen für den neuen Ordner ein.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Ordner]</p> </td> 
   <td> <p>Geben Sie den Pfad ein oder ordnen Sie ihn zu, in dem Sie einen neuen Ordner erstellen möchten.</p> <p>Hinweis:   <p>Wenn Sie ein [!DNL Dropbox Business] -Konto (mit Teamräumen) verwenden, müssen Sie den Schrägstrich <code>/</code> entfernen oder nicht auf <strong>[!UICONTROL Klicken Sie hier] klicken, um den Ordner</strong> auszuwählen, um einen Teamordner im Stammordner zu erstellen.</p> <p>Wenn der Schrägstrich nicht entfernt wird, wird der Fehler <code>[409] path/malformed_path/..</code> zurückgegeben.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Auto-Umbenennung]</td> 
   <td> <p> Aktivieren Sie diese Option, um den neuen Ordner umzubenennen, wenn bereits ein Ordner mit demselben Namen im Zielspeicherort vorhanden ist.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Erstellen/Überschreiben einer Textdatei]

Dieses Aktionsmodul erstellt eine DOC-Datei oder überschreibt den Inhalt einer vorhandenen Datei.

Sie geben die Quelldatei und den Ordner an.

Das Modul gibt die Kennung des Ordners sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Dropbox]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-dropbox" class="MCXref xref">Erstellen einer Verbindung mit [!DNL Dropbox]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Auswählen bis]</td> 
   <td> <p> Wählen Sie aus, ob Sie eine DOC-Datei erstellen oder überschreiben möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie den Zielspeicherort aus, an dem Sie eine Datei erstellen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Source-Datei]</p> </td> 
   <td> <p>Geben Sie die Datei ein oder ordnen Sie sie dem Ordner [!DNL Dropbox] zu.</p> <p style="font-weight: bold;">Dateiname</p> <p>Geben Sie den Dateinamen für die neue DOC-Datei ein (ohne Erweiterung).</p> <p style="font-weight: bold;">Dateiinhalt</p> <p>Geben Sie den Textinhalt der DOC-Datei ein.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Erstellen/Aktualisieren eines Freigabe-Links]

Dieses Aktionsmodul erstellt einen öffentlichen Link zu einer Datei.

Sie geben die Datei und Informationen zum Link an.

Das Modul gibt die Kennung des Links und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Dropbox]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-dropbox" class="MCXref xref">Erstellen einer Verbindung mit [!DNL Dropbox]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Methode zur Dateiauswahl]</td> 
   <td> <p> Wählen Sie aus, ob Sie eine Zuordnung vornehmen möchten, geben Sie den Dateipfad ein oder wählen Sie die Datei manuell aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Dateipfad/Datei]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Dateipfad]</p> <p>Geben Sie den Zielpfad der Datei ein oder ordnen Sie ihn zu.</p> <p style="font-weight: bold;">[!UICONTROL Datei]</p> <p>Wählen Sie die Datei aus dem Menü aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Angeforderte Sichtbarkeit]</p> </td> 
   <td> <p>Wählen Sie aus, ob der Link öffentlich, für Teams oder Kennworteinschränkungen ist.</p> <p>Hinweis: Die Optionen [!UICONTROL Team] und [!UICONTROL Zugriff mit Passwort] stehen nur Benutzern mit der Version [!DNL Dropbox Pro] oder höher zur Verfügung.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ablaufdatum]</td> 
   <td> <p> Geben Sie das Datum und die Uhrzeit ein, zu der der Link abläuft und nicht mehr verfügbar sein wird. Wenn dieses Feld leer gelassen wird, läuft der Link nicht ab. Eine Liste der unterstützten Datums- und Uhrzeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Typerzwingung in [!DNL Adobe Workfront Fusion]</a>.</p> <p>Hinweis: Die Optionen [!UICONTROL Team] und [!UICONTROL Access with password] stehen nur Benutzern mit [!UICONTROL Dropbox Pro] oder höheren Versionen zur Verfügung.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Link's Access Level]</p> </td> 
   <td> <p>Legen Sie die Berechtigung für den Link-Empfänger fest.</p> <p><strong>[!UICONTROL Viewer]</strong> Benutzer, die den Link verwenden, können den Inhalt anzeigen und kommentieren.</p> <p><strong>[!UICONTROL Editor]</strong> Benutzer, die den Link verwenden, können den Inhalt bearbeiten, anzeigen und kommentieren.</p> <p><strong>[!UICONTROL Max]</strong> Benutzer, die den Link verwenden, erhalten die maximale Zugriffsstufe, auf die Sie den Link setzen können.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei wiederherstellen]

Dieses Aktionsmodul stellt eine frühere Version einer Datei wieder her.

Sie geben die Datei und die Nummer der gewünschten Revision an.

Das Modul gibt die ID der Version und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Dropbox]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-dropbox" class="MCXref xref">Erstellen einer Verbindung mit [!DNL Dropbox]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Methode zur Dateiauswahl]</td> 
   <td> <p> Wählen Sie aus, ob Sie eine Zuordnung vornehmen möchten, geben Sie den Dateipfad ein oder wählen Sie die Datei manuell aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Dateipfad] / [!UICONTROL Datei]</p> </td> 
   <td> <p><strong>[!UICONTROL Dateipfad]</strong> </p> <p>Geben Sie den Zielpfad der Datei ein oder ordnen Sie ihn zu.</p> <p><strong>[!UICONTROL Datei]</strong> </p> <p>Wählen Sie die Datei aus dem Menü aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Revision]</p> </td> 
   <td> <p>Geben Sie die Revisionsnummer der Revisionsnummer ein, die Sie wiederherstellen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Verschieben einer Datei/eines Ordners]

Dieses Aktionsmodul verschiebt eine Datei oder einen Ordner an einen anderen Speicherort.

Sie geben die Datei bzw. den Ordner an und geben an, wie und wohin Sie sie verschieben möchten.

Das Modul gibt die ID der Datei oder des Ordners sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Dropbox]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-dropbox" class="MCXref xref">Erstellen einer Verbindung mit [!DNL Dropbox]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Methode zur Dateiauswahl] </td> 
   <td> <p>Wählen Sie aus, ob Sie eine Zuordnung vornehmen möchten, geben Sie den Dateipfad ein oder wählen Sie die Datei manuell aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Datei-/Ordnerpfad] / [!UICONTROL Datei/Ordner]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Datei-/Ordnerpfad]</p> <p>Geben Sie den Zielpfad der Datei oder des Ordners ein oder ordnen Sie ihn zu.</p> <p style="font-weight: bold;">[!UICONTROL Datei/Ordner]</p> <p>Wählen Sie die Datei oder den Ordner aus dem Menü aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL To Folder]</p> </td> 
   <td> <p>Geben Sie den Zielspeicherort für die Datei oder den Ordner ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Neuer Name]</p> </td> 
   <td> <p>Geben Sie den neuen Namen für die Datei oder den Ordner am neuen Speicherort ein.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Automatisches Umbenennen]</p> </td> 
   <td> <p>Aktivieren Sie diese Option, um sicherzustellen, dass das Modul die neue Datei oder den Ordner umbenennt, indem es ([!UICONTROL NUMBER]) nach dem Datei- oder Ordnernamen hinzufügt. Andernfalls wird die Datei oder der Ordner im Zielspeicherort überschrieben.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Eigentumsübertragung zulassen]</p> </td> 
   <td> <p>Aktivieren Sie diese Option, um Bewegungen nach Eigentümer zuzulassen, selbst wenn dies zu einer Eigentumsübertragung für den verschobenen Inhalt führen würde.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Umbenennen einer Datei/eines Ordners]

Dieses Aktionsmodul benennt eine Datei oder einen Ordner um.

Sie geben die Datei oder den Ordner und den neuen Namen an.

Das Modul gibt die ID der Datei oder des Ordners sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Dropbox]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-dropbox" class="MCXref xref">Erstellen einer Verbindung mit [!DNL Dropbox]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>Dateiauswahl</td> 
   <td> <p> Wählen Sie aus, ob Sie eine Zuordnung vornehmen möchten, geben Sie den Dateipfad ein oder wählen Sie die Datei manuell aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Datei/Ordnerpfad/Datei/Ordner</p> </td> 
   <td> <p style="font-weight: bold;">Datei-/Ordnerpfad</p> <p>Geben Sie den Zielpfad der Datei oder des Ordners ein oder ordnen Sie ihn zu.</p> <p style="font-weight: bold;">Datei/Ordner</p> <p>Wählen Sie die Datei oder den Ordner aus dem Menü aus.</p> </td> 
  </tr> 
  <tr> 
   <td>Umbenennen </td> 
   <td> <p>Geben Sie den [!UICONTROL Zielnamen] für die Datei ein, einschließlich der Dateierweiterung.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei/Ordner löschen]

Dieses Aktionsmodul löscht eine Datei oder einen Ordner.

Sie geben die Datei oder den Ordner an.

Das Modul gibt die Kennung des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Dropbox]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-dropbox" class="MCXref xref">Erstellen einer Verbindung mit [!DNL Dropbox]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Methode zur Dateiauswahl]</td> 
   <td> <p> Wählen Sie aus, ob Sie eine Zuordnung vornehmen möchten, geben Sie den Dateipfad ein oder wählen Sie die Datei manuell aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Dateipfad] / [!UICONTROL Datei]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Dateipfad]</p> <p>Geben Sie den Zielpfad der Datei ein oder ordnen Sie ihn zu.</p> <p style="font-weight: bold;">[!UICONTROL Datei]</p> <p>Wählen Sie die Datei aus dem Menü aus.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Sonstige Module

#### [!UICONTROL API-Aufruf durchführen]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Dropbox] -API durchführen. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von anderen [!DNL Dropbox] -Modulen nicht ausgeführt werden kann.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Dropbox]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-dropbox" class="MCXref xref">Erstellen einer Verbindung mit [!DNL Dropbox]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Geben Sie einen Pfad relativ zum Pfad relativ zu <code>https://api.dropboxapi.com</code> ein. Beispiel: <code>/2/files/list_folder</code></p> <p>Hinweis: Die Liste der verfügbaren Endpunkte finden Sie in der Dokumentation zur <a href="https://www.dropbox.com/developers/documentation/http/documentation">Dropbox API v2-Dokumentation</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Methode]</p> </td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Header] </td> 
   <td> <p>Geben Sie die gewünschten Anforderungsheader ein. [!DNL Workfront Fusion] fügt Autorisierungskopfzeilen automatisch hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p> Geben Sie die Abfragezeichenfolge der Anfrage ein.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body] </td> 
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:   <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> in Ihrer JSON platzieren Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Beispiel:** Der folgende API-Aufruf gibt die ersten 10 Dateien aus dem Ordner [!DNL /Text files] in Ihrem [!DNL Dropbox]-Konto zurück:
>
>URL: `/2/files/list_folder`
>
>Hauptteil:
> 
>`{`
>
>`"path": "/Text files",`
>
>`"limit": 10,`
>
>`"recursive": false,`
>
>`"include_deleted": false`
>
>`}`
>
>Übereinstimmungen der Suche finden Sie in der Ausgabe des Moduls unter [!UICONTROL Bundle] > [!UICONTROL Hauptteil] > Einträgen.
>
>In unserem Beispiel wurden 10 Tickets zurückgegeben:

## Häufige Probleme

* [Datei kann nicht hochgeladen oder aktualisiert werden](#unable-to-upload-or-update-a-file)
* [Über einen freigegebenen Link referenziertes Bild wird nicht gerendert](#image-referenced-via-a-shared-link-does-not-render)

### Datei kann nicht hochgeladen oder aktualisiert werden

Es gibt mehrere Situationen, in denen das Hochladen oder Aktualisieren einer Datei fehlschlägt:

* Die hochgeladene Datei ist zu groß und überschreitet die für Ihren [!DNL Dropbox]-Plan maximal zulässige Dateigröße, oder Sie haben das Speicherkontingent Ihres [!DNL Dropbox]-Kontos verwendet. Sie müssen vorhandene Dateien aus Ihrem [!DNL Dropbox] -Konto löschen oder Ihren Plan aktualisieren.
* Der zuvor ausgewählte Ordner, in den die Datei hochgeladen wird, existiert nicht mehr. Das Szenario wird gestoppt und Sie müssen den Zielordner erneut auswählen.

### Über einen freigegebenen Link referenziertes Bild wird nicht gerendert

Die von [!UICONTROL Dropbox] >[!UICONTROL Geteilten Link erstellen] zurückgegebene URL verlinkt nicht direkt zu einem Bild, sondern zu einer [!DNL Dropbox] -Seite. Um das Herunterladen des Bildes zu erzwingen, ersetzen Sie die nachfolgende `?dl=0` durch `?dl=1`. Um die Wiedergabe des Bildes zu erzwingen (z. B. in einem Webbrowser oder in Facebook Messenger), hängen Sie `&raw=1` an die URL an.

Wenn Sie den direkten oder Rohlink Ihres Bildes für Ihre Website oder andere [!DNL Workfront Fusion]-Module abrufen müssen, müssen Sie die ursprünglich freigegebene URL wie folgt ändern:

Ursprüngliche URL:

`https://www.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png?dl=0`

1. Ersetzen Sie `www` durch `dl`.
1. Entfernen Sie `?dl=0`.

Endgültige URL:

`https://dl.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png`

Um die URL automatisch zu ändern, können Sie die Funktion `replace()` zweimal verwenden:

* Ersetzen von www durch dl

  ![](assets/www-to-dl-350x32.png)

* Und um ?dl=0 zu entfernen

  ![](assets/remove-dl0-350x33.png)

Um dies in einem Schritt zu tun, kombinieren Sie die folgenden Funktionen:

![](assets/replace-both-350x47.png)

Sie können sie auch kopieren und in das Feld einfügen. Ersetzen Sie `1.url` durch die URL.

```
{{replace(replace(1.url; "?dl=0"; ""); "www"; "dl")}}
```
