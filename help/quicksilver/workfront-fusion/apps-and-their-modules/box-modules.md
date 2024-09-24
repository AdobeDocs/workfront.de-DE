---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connector
navigation-topic: apps-and-their-modules
title: Box-Module
description: In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die Box verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden. überwacht einen angegebenen Ordner, um nach Dateiänderungen zu suchen, vorhandene Dateien zu ändern und zu löschen oder neue Dateien in einen Ordner hochzuladen.
author: Becky
feature: Workfront Fusion
exl-id: 965ce570-40bf-474d-b318-0d2de8be6b9d
source-git-commit: 16cd5dee183153540bcccea8ce469a461d0e8562
workflow-type: tm+mt
source-wordcount: '1070'
ht-degree: 0%

---

# Box-Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL Box] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden. überwacht einen angegebenen Ordner, um nach Dateiänderungen zu suchen, vorhandene Dateien zu ändern und zu löschen oder neue Dateien in einen Ordner hochzuladen.

Wenn Sie Anweisungen zum Erstellen eines Szenarios benötigen, finden Sie weitere Informationen unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Um [!DNL Box] -Module zu verwenden, müssen Sie über ein [!DNL Box] -Konto verfügen.

## [!DNL Box] Module und ihre Felder

Wenn Sie [!DNL Box] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Box] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Trigger

* [[!UICONTROL Neues Ereignis]](#new-event)
* [[!UICONTROL Dateien ansehen]](#watch-files)

#### [!UICONTROL Neues Ereignis]

Dieses Instant Trigger-Modul startet ein Szenario, wenn eine Datei hinzugefügt, verschoben, kopiert, gelöscht, gesperrt oder entsperrt wird.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Wählen Sie den Webhook aus, den Sie zum Anzeigen ausgehender Nachrichten verwenden möchten. Um einen Webhook hinzuzufügen, klicken Sie auf <strong>[!UICONTROL Add]</strong> und geben Sie den Namen und die Verbindung des Webhooks ein.</p> <p> Anweisungen zum Verbinden Ihres [!UICONTROL Box]-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der App oder des Webdiensts des Moduls mit [!UICONTROL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Maximale Anzahl an zurückgegebenen Ereignissen]</p> </td> 
   <td> <p>Geben Sie die höchste Anzahl von Ereignissen ein, die das Modul während der Ausführung jedes Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Dateien ansehen]

Dieses Trigger-Modul startet ein Szenario, wenn eine neue Datei hinzugefügt oder eine bestehende Datei in einem überwachten Ordner aktualisiert wird.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Box]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  <tr> 
   <td role="rowheader">Watch</td> 
   <td> <p>Wählen Sie den Dateityp aus, den Sie sehen möchten.</p> 
    <ul> 
     <li> <p><strong>Nur neue Dateien</strong> </p> <p>Das Szenario beginnt mit dem Hinzufügen einer neuen Datei.</p> </li> 
     <li> <p><strong>Neue Dateien und alle Änderungen</strong> </p> <p>Das Szenario beginnt, wenn eine Datei hinzugefügt oder der Dateiinhalt oder ein Dateiattribut (z. B. sein Name) geändert wird.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Maximale Anzahl heruntergeladener Dateien</p> </td> 
   <td> <p>Geben Sie die höchste Anzahl von Dateien ein, die das Modul während der Ausführung jedes Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL  Hochladen] einer Datei](#upload-a-file)
* [[!UICONTROL Aktualisieren einer Datei]](#update-a-file)
* [[!UICONTROL Datei löschen]](#delete-a-file)
* [[!UICONTROL Datei abrufen]](#get-a-file)

#### [!UICONTROL  Datei hochladen]

Dieses Aktionsmodul lädt eine Datei hoch.

Sie geben die Datei an. Sie können auch einen neuen Dateinamen für die Datei angeben.

Das Modul gibt die Kennung der Datei und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Box]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Wenn dieses Modul nicht erfolgreich ist, sollten Sie Folgendes beachten:
>
>* Die Dateigröße kann die maximale Dateigrößenbeschränkung für Ihren [!DNL Box]-Plan überschreiten, oder Sie haben möglicherweise das Speicherkontingent Ihres [!DNL Box]-Kontos verwendet. Um mehr Speicherplatz zu erhalten, löschen Sie vorhandene Dateien aus [!DNL Box] oder aktualisieren Sie Ihr [!DNL Box] -Konto.
>* [!DNL Box] lädt nicht mehr als eine Datei mit demselben Namen in einen einzelnen Ordner hoch. Wenn der Zielordner eine Datei mit demselben Namen wie die hochgeladene Datei enthält, wird die Ausführung des Szenarios mit einem Fehler beendet. Benennen Sie die Datei um, um dies zu vermeiden. Wenn Sie die Datei aktualisieren möchten, verwenden Sie das Modul **[!UICONTROL Datei aktualisieren]** .

#### [!UICONTROL Aktualisieren einer Datei]

Dieses Aktionsmodul aktualisiert eine Datei.

Sie geben die Kennung der Datei an.

Das Modul gibt die Kennung der Datei und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Box]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datei-ID]</td> 
   <td>Geben Sie die eindeutige ID der Datei ein oder ordnen Sie sie zu, die das Modul aktualisieren soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei löschen]

Dieses Aktionsmodul löscht eine Datei.

Sie geben die Kennung der Datei an.

Das Modul gibt die Kennung der Datei und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Box]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datei-ID]</td> 
   <td>Geben Sie die eindeutige ID der Datei ein oder ordnen Sie sie zu, die das Modul aktualisieren soll.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei abrufen]

Dieses Aktionsmodul lädt eine Datei herunter.

Sie geben die Kennung der Datei an.

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
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Box]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datei-ID]</td> 
   <td>Geben Sie die eindeutige ID der Datei ein oder ordnen Sie sie zu, die das Modul aktualisieren soll.</td> 
  </tr> 
 </tbody> 
</table>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Possible problems</h2>
-->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This is drafted out because we don't have a download module for Box yet</p>
-->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Watch files trigger module doesn't download a file contained in the folder.</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">There are several situations when downloading a file fails:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The current file lock setting does not allow the file to be downloaded or the downloading of the file is disabled. In this case, the file is ignored.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">When the scenario started, the file was being uploaded to the server and was not ready to be downloaded. The scenario run gets stopped and Workfront Fusion tries downloading the file again during the next execution of the scenario.</li>
  -->
