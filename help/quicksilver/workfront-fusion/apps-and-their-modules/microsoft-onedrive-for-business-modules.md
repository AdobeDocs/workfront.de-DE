---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connector
navigation-topic: apps-and-their-modules
title: Microsoft OneDrive für Geschäftsmodule
description: In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL Microsoft OneDrive for Business], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.
author: Becky
feature: Workfront Fusion
exl-id: b7175cb9-aade-49b7-a28b-25fc9805a078
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive for Business]-Module

In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL Microsoft OneDrive for Business], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.

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

Verwendung [!DNL Microsoft OneDrive for Business] mit [!DNL Adobe Workfront Fusion]benötigen Sie [!DNL Microsoft] -Konto.

Anweisungen zum Verbinden der [!DNL OneDrive for Business] Konto [!DNL Workfront Fusion], siehe [Verbindung zur Adobe erstellen [!DNL Workfront Fusion] - Grundlegende Anweisungen](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Microsoft OneDrive for Business] Module und ihre Felder

Bei der Konfiguration [!DNL Microsoft OneDrive for Business] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Microsoft OneDrive for Business] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Trigger](#triggers)
* [Aktionen](#actions)

### Trigger

* [[!UICONTROL Dateien überwachen]](#watch-files)
* [[!UICONTROL Ordner überwachen]](#watch-folders)

#### [!UICONTROL Dateien überwachen]

Dieses Trigger-Modul wird aktiviert, wenn eine neue Datei in einem überwachten Ordner hinzugefügt oder aktualisiert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Drive ID]</p> </td> 
   <td> <p>Wählen Sie das Laufwerk aus, das Sie sehen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner]</td> 
   <td> <p> Wählen Sie den Ordner aus, den Sie sehen möchten. In einem Szenario können Sie nur einen Ordner überwachen.</p> <p>Tipp: Um mehrere Ordner zu verfolgen, erstellen Sie für jeden Ordner ein unabhängiges Szenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Ich möchte sehen]</p> </td> 
   <td> <p>Wählen Sie aus, ob Sie neue Dateien und alle Änderungen oder nur neue Dateien sehen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl der zurückgegebenen Zeilen]</td> 
   <td> <p> Legen Sie die maximale Anzahl von Ergebnissen fest, die [!DNL Workfront Fusion] wird während eines Zyklus mit arbeiten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ordner überwachen]

Dieses Ordnermodul wird aktiviert, wenn dem überwachten Trigger ein neuer Ordner hinzugefügt wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Drive ID]</p> </td> 
   <td> <p>Wählen Sie das Laufwerk aus, das Sie sehen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner]</td> 
   <td> <p> Wählen Sie den Ordner aus, den Sie sehen möchten. In einem Szenario können Sie nur einen Ordner überwachen.</p> <p>Tipp: Um mehrere Ordner zu verfolgen, erstellen Sie für jeden Ordner ein unabhängiges Szenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Ich möchte sehen]</p> </td> 
   <td> <p>Wählen Sie aus, ob Sie neue Ordner und alle Änderungen oder nur neue Ordner sehen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl der zurückgegebenen Zeilen]</td> 
   <td> <p> Legen Sie die maximale Anzahl von Ergebnissen fest, die [!DNL Workfront Fusion] wird während eines Zyklus mit arbeiten.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL Datei hochladen]](#upload-a-file)
* [[!UICONTROL Datei löschen]](#delete-a-file)
* [[!UICONTROL Datei abrufen]](#get-a-file)
* [[!UICONTROL Ordner erstellen]](#create-a-folder)
* [[!UICONTROL Ordner löschen]](#delete-a-folder)
* [[!UICONTROL Freigabe-Link abrufen]](#get-a-sharing-link)

#### [!UICONTROL Datei hochladen]

Dieses Aktionsmodul lädt eine Binär- oder Textdatei in einen angegebenen Ordner hoch

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>Wählen Sie das Laufwerk aus, auf das Sie eine Datei hochladen möchten.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie den Ordner im Laufwerk aus.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Quelldatei]</p> </td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Wenn die Datei mit demselben Namen vorhanden ist]</td> 
   <td> <p> Wählen Sie aus, was Sie tun möchten, wenn bereits eine Datei mit demselben Namen wie die Datei vorhanden ist, die Sie hochladen möchten.</p> 
    <ul> 
     <li>[!UICONTROL Vorhandene Datei ersetzen]</li> 
     <li>[!UICONTROL Neue Datei umbenennen]</li> 
     <li>[!UICONTROL Mit Fehler beenden]</li> 
    </ul> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei löschen]

Dieses Aktionsmodul verschiebt die angegebene Datei in den Papierkorb.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>Wählen Sie das Laufwerk aus, aus dem Sie eine Datei löschen möchten.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei-ID]</td> 
   <td> <p>Geben Sie die Kennung der Datei ein, die Sie löschen möchten. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei abrufen]

Dieses Aktionsmodul ruft die Datei mit der angegebenen ID ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>Wählen Sie das Laufwerk aus, von dem Sie eine Datei abrufen möchten.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datei-ID]</td> 
   <td> <p>Geben Sie die Kennung der Datei ein, die Sie abrufen möchten. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ordner erstellen]

Erstellt einen Ordner innerhalb des angegebenen übergeordneten Ordners.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL Verbindung]</strong> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Drive ID]</strong> </td> 
   <td> <p>Wählen Sie das Laufwerk aus, auf dem Sie einen neuen Ordner erstellen möchten.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Ordner]</strong> </td> 
   <td> <p>Wählen Sie den Ordner aus, in dem Sie einen neuen Ordner erstellen möchten.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Ordnername]</strong> </td> 
   <td>Geben Sie einen Namen für den neuen Ordner ein oder ordnen Sie ihn zu.</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ordner löschen]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>Wählen Sie das Laufwerk aus, aus dem Sie eine Datei löschen möchten.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner-ID]</td> 
   <td> <p>Geben Sie die Kennung des Ordners ein, den Sie löschen möchten, oder ordnen Sie sie zu. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Freigabe-Link abrufen]

Dieses Modul ruft einen Link ab, den Sie freigeben können, um Zugriff auf die angegebene Datei zu gewähren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>Wählen Sie das Laufwerk aus, auf das Sie eine Datei hochladen möchten.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Eingabe]</td> 
   <td> <p>Wählen Sie mithilfe der Datei-ID oder des Dateipfads aus, ob Sie eine Datei auswählen möchten. Geben Sie die Datei-ID oder den Pfad in das Feld ein, das angezeigt wird.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Berechtigungstyp]</p> </td> 
   <td> <p>Wählen Sie aus, ob Personen, die den Link erhalten, Lese-/Schreibberechtigungen erhalten oder nur Lese-/Schreibberechtigungen erhalten sollen.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Umfang]</td> 
   <td> <p> Wählen Sie aus, ob die Datei für alle Benutzer zugänglich sein soll, die über den Link verfügen oder nur für Mitglieder Ihrer Organisation zugänglich sind.</p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
