---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connector
navigation-topic: apps-and-their-modules
title: Dropbox Module
description: In [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die Dropbox verwenden, und sie mit mehreren Drittanbieteranwendungen und -diensten verbinden. Dies ermöglicht Ihnen die Automatisierung von Aktivitäten wie Überwachung, Suche, Abrufen, Auflisten, Erstellen und Bearbeiten von Dateien und Ordnern in Ihrer Dropbox.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: a35631d7-40ac-4e7f-9a37-ad3879c0b6a2
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3013'
ht-degree: 0%

---

# [!DNL Dropbox]-Module

In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!UICONTROL Dropbox], und verbinden Sie es mit mehreren Drittanbieteranwendungen und -diensten. Dies ermöglicht Ihnen die Automatisierung von Aktivitäten wie Überwachung, Suche, Abrufen, Auflisten, Erstellen und Bearbeiten von Dateien und Ordnern in Ihren [!UICONTROL Dropbox].

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Verwendung [!DNL Dropbox] -Module, müssen Sie über eine [!DNL Dropbox] -Konto.

## [!DNL Dropbox] Module und ihre Felder

Bei der Konfiguration [!DNL Dropbox] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Dropbox] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Trigger-Module](#trigger-modules)
* [Zu erhaltende Module [!DNL Dropbox] Dateien und Ordner](#modules-for-getting-dropbox-files-and-folders)
* [Module zum Erstellen und Bearbeiten [!DNL Dropbox] Dateien und Ordner](#modules-for-creating-and-editing-dropbox-files-and-folders)
* [Sonstige Module](#other-modules)

### Trigger-Module

#### [!UICONTROL Überwachungsdateien]

Dieses Trigger-Modul gibt Dateidetails zurück, wenn die Datei in einem angegebenen Ordner geändert wird.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Dropbox] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
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

### Zu erhaltende Module [!DNL Dropbox] Dateien und Ordner

* [[!UICONTROL Suchdateien/Ordner]](#search-filesfolders)
* [[!UICONTROL Datei herunterladen]](#download-a-file)
* [[!UICONTROL Abrufen von Ordnermetadaten]](#get-a-folder-metadata)
* [[!UICONTROL Alle Dateien/Unterordner in einem Ordner auflisten]](#list-all-filessubfolders-in-a-folder)
* [[!UICONTROL Dateiüberarbeitungen auflisten]](#list-file-revisions)

#### [!UICONTROL Suchdateien/Ordner]

Dieses Suchmodul sucht nach Datensätzen in einem Objekt in [!DNL Dropbox] die mit der angegebenen Suchabfrage übereinstimmen.

Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Dropbox] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Suche] </td> 
   <td> <p>Geben Sie den Suchbegriff ein.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie den Ordner aus, den Sie suchen möchten. Dieses Modul durchsucht die gesamte [!DNL Dropbox] wenn Sie keinen Ordner auswählen.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden der [!DNL Dropbox] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>Dateiauswahl</td> 
   <td> <p> Wählen Sie aus, ob Sie den Dateipfad zuordnen möchten, oder wählen Sie die Datei manuell aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dateipfad/Datei</p> </td> 
   <td> <p style="font-weight: bold;">Dateipfad</p> <p>Geben oder ordnen Sie den Zielpfad der Datei zu.</p> <p style="font-weight: bold;">Datei</p> <p>Wählen Sie die Datei aus dem Menü aus.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden der [!DNL Dropbox] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
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
   <td> <p>Anweisungen zum Verbinden der [!DNL Dropbox] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
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

#### [!UICONTROL Dateiüberarbeitungen auflisten]

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
   <td> <p>Anweisungen zum Verbinden der [!DNL Dropbox] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>Dateiauswahl</td> 
   <td> <p> Wählen Sie aus, ob Sie den Dateipfad zuordnen möchten, oder wählen Sie die Datei manuell aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dateipfad/Datei</p> </td> 
   <td> <p style="font-weight: bold;">Dateipfad</p> <p>Geben oder ordnen Sie den Zielpfad der Datei zu.</p> <p style="font-weight: bold;">Datei</p> <p>Wählen Sie die Datei aus dem Menü aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Limit</p> </td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während des Ausführungszyklus eines Szenarios auflisten soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Module zum Erstellen und Bearbeiten [!DNL Dropbox] Dateien und Ordner

* [[!UICONTROL Hochladen] eine Datei](#upload-a-file)
* [[!UICONTROL Erstellen eines Ordners]](#create-a-folder)
* [[!UICONTROL Erstellen/Überschreiben einer Textdatei]](#createoverwrite-a-text-file)
* [[!UICONTROL Link zur Freigabe erstellen/aktualisieren]](#createupdate-a-share-link)
* [[!UICONTROL Wiederherstellen einer Datei]](#restore-a-file)
* [[!UICONTROL Verschieben einer Datei/eines Ordners]](#move-a-filefolder)
* [[!UICONTROL Eine Datei/einen Ordner umbenennen]](#rename-a-filefolder)
* [[!UICONTROL Datei/Ordner löschen]](#delete-a-filefolder)

#### [!UICONTROL Datei hochladen]

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
   <td> <p>Anweisungen zum Verbinden der [!DNL Dropbox] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner]</td> 
   <td> <p> Wählen Sie den Ordner Ihrer [!DNL Dropbox] Sie die Datei in hochladen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Quelldatei]</p> </td> 
   <td> <p>Geben Sie die Datei ein oder ordnen Sie sie zu der Datei zu, die Sie hinzufügen möchten. [!DNL Dropbox] Ordner, der oben ausgewählt wurde.</p> <p style="font-weight: bold;">[!UICONTROL Dateiname]</p> <p>Geben Sie den Dateinamen einschließlich der Dateierweiterung ein oder ordnen Sie ihn zu.</p> <p style="font-weight: bold;">[!UICONTROL Dateidaten]</p> <p>Geben Sie die Dateidaten ein oder ordnen Sie sie zu (aus dem vorherigen Modul wie [!UICONTROL Google Drive] &gt;[!UICONTROL Datei abrufen)).</p> <p>Hinweis: Die maximale Größe der hochgeladenen Datei beträgt 150 MB.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden der [!DNL Dropbox] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordnername] </td> 
   <td> <p>Geben Sie den Namen für den neuen Ordner ein.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Ordner]</p> </td> 
   <td> <p>Geben Sie den Pfad ein oder ordnen Sie ihn zu, in dem Sie einen neuen Ordner erstellen möchten.</p> <p>Notiz:   <p>Wenn Sie eine [!DNL Dropbox Business] -Konto (mit Teamräumen), müssen Sie den Schrägstrich entfernen <code>/</code>oder klicken Sie nicht auf <strong>[!UICONTROL Klicken Sie hier, um Ordner auszuwählen.</strong> , um einen Team-Ordner im Stammverzeichnis zu erstellen.</p> <p>Wenn der Schrägstrich nicht entfernt wird, wird ein Fehler ausgegeben <code>[409] path/malformed_path/..</code> zurückgegeben.</p> </p> </td> 
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
   <td> <p>Anweisungen zum Verbinden der [!DNL Dropbox] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
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
   <td> <p>[!UICONTROL Quelldatei]</p> </td> 
   <td> <p>Geben Sie die Datei ein oder ordnen Sie sie zu der Datei zu, die Sie hinzufügen möchten. [!DNL Dropbox] Ordner.</p> <p style="font-weight: bold;">Dateiname</p> <p>Geben Sie den Dateinamen für die neue DOC-Datei ein (ohne Erweiterung).</p> <p style="font-weight: bold;">Dateiinhalt</p> <p>Geben Sie den Textinhalt der DOC-Datei ein.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Link zur Freigabe erstellen/aktualisieren]

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
   <td> <p>Anweisungen zum Verbinden der [!DNL Dropbox] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Methode zur Dateiauswahl]</td> 
   <td> <p> Wählen Sie aus, ob Sie eine Zuordnung vornehmen möchten, geben Sie den Dateipfad ein oder wählen Sie die Datei manuell aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Dateipfad/Datei]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Dateipfad]</p> <p>Geben oder ordnen Sie den Zielpfad der Datei zu.</p> <p style="font-weight: bold;">[!UICONTROL Datei]</p> <p>Wählen Sie die Datei aus dem Menü aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Angeforderte Sichtbarkeit]</p> </td> 
   <td> <p>Wählen Sie aus, ob der Link öffentlich, für Teams oder Kennworteinschränkungen ist.</p> <p>Hinweis: Die Optionen Nur [!UICONTROL Team] und [!UICONTROL Zugriff mit Kennwort] stehen nur Benutzern zur Verfügung, die [!DNL Dropbox Pro] oder höher.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Link's Expiration Date]</td> 
   <td> <p> Geben Sie das Datum und die Uhrzeit ein, zu der der Link abläuft und nicht mehr verfügbar sein wird. Wenn dieses Feld leer gelassen wird, läuft der Link nicht ab. Eine Liste der unterstützten Datums- und Uhrzeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Typenkonvertierung in [!DNL Adobe Workfront Fusion]</a>.</p> <p>Hinweis: Die Optionen [!UICONTROL Team] und [!UICONTROL Zugriff mit Passwort] stehen nur Benutzern mit [!UICONTROL Dropbox Pro] oder höheren Versionen zur Verfügung.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Link's Access Level]</p> </td> 
   <td> <p>Legen Sie die Berechtigung für den Link-Empfänger fest.</p> <p><strong>[!UICONTROL Viewer]</strong> Benutzer, die den Link verwenden, können den Inhalt anzeigen und kommentieren.</p> <p><strong>[!UICONTROL Editor]</strong> Benutzer, die den Link verwenden, können den Inhalt bearbeiten, anzeigen und kommentieren.</p> <p><strong>[!UICONTROL Max]</strong> Benutzer, die den Link verwenden, erhalten die maximale Zugriffsstufe, auf die Sie den Link festlegen können.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Wiederherstellen einer Datei]

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
   <td> <p>Anweisungen zum Verbinden der [!DNL Dropbox] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Methode zur Dateiauswahl]</td> 
   <td> <p> Wählen Sie aus, ob Sie eine Zuordnung vornehmen möchten, geben Sie den Dateipfad ein oder wählen Sie die Datei manuell aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Dateipfad] / [!UICONTROL Datei]</p> </td> 
   <td> <p><strong>[!UICONTROL Dateipfad]</strong> </p> <p>Geben oder ordnen Sie den Zielpfad der Datei zu.</p> <p><strong>[!UICONTROL Datei]</strong> </p> <p>Wählen Sie die Datei aus dem Menü aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Revision]</p> </td> 
   <td> <p>Geben Sie die Revisionsnummer der Revisionsnummer ein, die Sie wiederherstellen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Verschieben einer Datei/eines Ordners]

Dieses Aktionsmodul verschiebt eine Datei oder einen Ordner an einen anderen Speicherort.

Sie geben die Datei bzw. den Ordner an und geben an, wie und wo sie verschoben werden soll.

Das Modul gibt die ID der Datei oder des Ordners sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Dropbox] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
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

#### [!UICONTROL Eine Datei/einen Ordner umbenennen]

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
   <td> <p>Anweisungen zum Verbinden der [!DNL Dropbox] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
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
   <td> <p>Anweisungen zum Verbinden der [!DNL Dropbox] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Methode zur Dateiauswahl]</td> 
   <td> <p> Wählen Sie aus, ob Sie eine Zuordnung vornehmen möchten, geben Sie den Dateipfad ein oder wählen Sie die Datei manuell aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Dateipfad] / [!UICONTROL Datei]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Dateipfad]</p> <p>Geben oder ordnen Sie den Zielpfad der Datei zu.</p> <p style="font-weight: bold;">[!UICONTROL Datei]</p> <p>Wählen Sie die Datei aus dem Menü aus.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Sonstige Module

#### [!UICONTROL API-Aufruf durchführen]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Dropbox] API. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von der anderen nicht durchgeführt werden kann [!DNL Dropbox] Module.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Dropbox] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Geben Sie einen Pfad relativ zum Pfad ein, der relativ zu <code>https://api.dropboxapi.com</code>. Beispiel: <code>/2/files/list_folder</code></p> <p>Hinweis: Eine Liste der verfügbaren Endpunkte finden Sie unter <a href="https://www.dropbox.com/developers/documentation/http/documentation">Dokumentation zur Dropbox API v2</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Methode]</p> </td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Header] </td> 
   <td> <p>Geben Sie die gewünschten Anforderungsheader ein. [!DNL Workfront Fusion] fügt automatisch Autorisierungskopfzeilen hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p> Geben Sie die Abfragezeichenfolge der Anfrage ein.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body] </td> 
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Notiz:   <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> Fügen Sie die Anführungszeichen in Ihre JSON-Datei außerhalb der bedingten Anweisung ein.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Beispiel:** Der folgende API-Aufruf gibt die ersten 10 Dateien aus der [!DNL /Text files] Ordner in [!DNL Dropbox] Konto:
>
>URL: `/2/files/list_folder`
>
>Text:
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
>Treffer der Suche finden Sie in der Ausgabe des Moduls unter [!UICONTROL Bundle] > [!UICONTROL body] > Einträge.
>
>In unserem Beispiel wurden 10 Tickets zurückgegeben:

## Häufige Probleme

* [Datei kann nicht hochgeladen oder aktualisiert werden](#unable-to-upload-or-update-a-file)
* [Bild, auf das über einen freigegebenen Link verwiesen wird, wird nicht gerendert](#image-referenced-via-a-shared-link-does-not-render)

### Datei kann nicht hochgeladen oder aktualisiert werden

Es gibt mehrere Situationen, in denen das Hochladen oder Aktualisieren einer Datei fehlschlägt:

* Die hochgeladene Datei ist zu groß und überschreitet die für Ihre [!DNL Dropbox] Plan, oder Sie haben alle Ihre [!DNL Dropbox] Speicherkontingent des Kontos. Sie müssen vorhandene Dateien aus Ihrem [!DNL Dropbox] -Konto zu erstellen oder Ihren Plan zu aktualisieren.
* Der zuvor ausgewählte Ordner, in den die Datei hochgeladen wird, existiert nicht mehr. Das Szenario wird gestoppt und Sie müssen den Zielordner erneut auswählen.

### Bild, auf das über einen freigegebenen Link verwiesen wird, wird nicht gerendert

Die von der [!UICONTROL Dropbox] >[!UICONTROL Freigegebenen Link erstellen] nicht direkt mit einem Bild verknüpft, sondern mit einem [!DNL Dropbox] Seite. Um das Herunterladen des Bildes zu erzwingen, ersetzen Sie das nachfolgende `?dl=0` mit `?dl=1`. Um die Wiedergabe des Bildes zu erzwingen (z. B. in einem Webbrowser oder in Facebook Messenger), hängen Sie `&raw=1` zur URL.

Wenn Sie den direkten oder Rohlink Ihres Bildes für Ihre Website oder für andere [!DNL Workfront Fusion] -Module verwenden, müssen Sie die ursprüngliche freigegebene URL wie folgt ändern:

Ursprüngliche URL:

`https://www.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png?dl=0`

1. Ersetzen `www` mit `dl`.
1. Entfernen `?dl=0`.

Endgültige URL:

`https://dl.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png`

Um die URL automatisch zu ändern, können Sie die `replace()` Funktion zweimal:

* Ersetzen von www durch dl

   ![](assets/www-to-dl-350x32.png)

* Und um ?dl=0 zu entfernen

   ![](assets/remove-dl0-350x33.png)

Um dies in einem Schritt zu tun, kombinieren Sie die folgenden Funktionen:

![](assets/replace-both-350x47.png)

Sie können sie auch kopieren und in das Feld einfügen. Ersetzen `1.url` mit der URL.

```
{{replace(replace(1.url; "?dl=0"; ""); "www"; "dl")}}
```
