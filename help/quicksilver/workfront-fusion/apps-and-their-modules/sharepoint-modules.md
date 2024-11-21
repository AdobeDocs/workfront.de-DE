---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: SharePoint-Module
description: In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die SharePoint verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 16d49031-06d2-4c86-bac4-f58cd9b2f1f5
source-git-commit: 2e91e9a4c691430f3c98e3cbddb30706ea57f84a
workflow-type: tm+mt
source-wordcount: '2877'
ht-degree: 0%

---

# [!DNL SharePoint] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL SharePoint] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

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

Um [!DNL SharePoint] -Module zu verwenden, müssen Sie über ein [!DNL SharePoint] -Konto verfügen.

## SharePoint-API-Informationen

Der SharePoint-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Basis-URL</td> 
   <td> https://graph.microsoft.com/v1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Version</td> 
   <td> v1.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v1.14.2</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL SharePoint] mit [!DNL Workfront Fusion] verbinden {#connect-sharepoint-to-workfront-fusion}

* [Verbinden von [!DNL SharePoint] mit [!DNL Workfront Fusion] mithilfe eines [!DNL Microsoft] Kontos](#connect-sharepoint-to-workfront-fusion-using-a-microsoft-account)
* [ [!DNL SharePoint] mit erweiterten Einstellungen an [!DNL Workfront Fusion] verbinden](#connect-sharepoint-to-workfront-fusion-using-advanced-settings)

### [!DNL SharePoint] mit einem [!DNL Microsoft]-Konto an [!DNL Workfront Fusion] anschließen

Sie können Ihr [!DNL Microsoft]-Konto verwenden, um eine Verbindung zu [!DNL SharePoint] herzustellen. Anweisungen zum Verbinden Ihres [!DNL Sharepoint]-Kontos mit [!DNL Workfront Fusion] finden Sie unter [Erstellen einer Verbindung zu  [!DNL Adobe Workfront Fusion]  - Grundlegende Anweisungen](../../workfront-fusion/connections/connect-to-fusion-general.md)

### [!DNL SharePoint] mit [!DNL Workfront Fusion] über erweiterte Einstellungen verbinden

Um [!DNL SharePoint] mit [!DNL Workfront Fusion] ohne ein [!DNL Microsoft] -Konto zu verbinden, benötigen Sie eine Client-ID, einen Client-Geheimnisschlüssel und eine Mandantenkennung.

1. Klicken Sie oben im Feld **[!DNL SharePoint]** auf **[!UICONTROL Hinzufügen]** , um das Feld **[!UICONTROL Verbindung erstellen]** zu öffnen.

1. (Optional) Ändern Sie den standardmäßigen **[!UICONTROL Verbindungsnamen]**.
1. Klicken Sie auf **[!UICONTROL Erweiterte Einstellungen anzeigen]**.
1. Geben Sie die [!DNL SharePoint] **[!UICONTROL Client-ID]** und den **[!UICONTROL Client-Geheimnis]** ein.

1. Klicken Sie auf **[!UICONTROL Weiter]**.
1. Geben Sie im angezeigten Anmeldefenster Ihre Anmeldedaten ein, um sich bei der App anzumelden, falls noch nicht geschehen.
1. (Bedingt) Wenn die Schaltfläche **[!UICONTROL Zulassen]** angezeigt wird, klicken Sie auf die Schaltfläche , um die App mit [!DNL Workfront Fusion] zu verbinden.

## [!DNL SharePoint] Module und ihre Felder

Wenn Sie [!DNL SharePoint] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL SharePoint] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Laufwerkselement](#drive-item)
* [Element](#item)
* [Liste](#list)
* [Seite (Beta)](#page-beta)
* [Site](#site)
* [Sonstige](#other)

### Laufwerkselement

* [Datei erstellen](#create-a-file)
* [Ordner erstellen](#create-a-folder)
* [Datei abrufen](#get-a-file)
* [Ordnerelemente überwachen](#watch-folder-items)

#### Abrufen von Änderungen

Dieses Modul gibt Änderungen zurück, die in SharePoint vorgenommen wurden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL SharePoint]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL SharePoint] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eingabe von Site-, Drive- und Ordner-IDs]</td> 
   <td> <p>Wählen Sie aus, wie Sie den Speicherort des Ordners identifizieren möchten, in dem Sie Änderungen abrufen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie die <strong>[!UICONTROL Site ID]</strong>, die <strong>[!UICONTROL List ID]</strong> und die <strong>[!UICONTROL Folder ID]</strong> in die angezeigten Felder ein oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Wählen Sie aus der Liste aus, der Sie folgen]</strong> </p> <p>Wählen Sie den Speicherort aus, an dem Sie Änderungen abrufen möchten. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Token]</td> 
   <td> </td> 
  </tr>  </tbody> 
</table>

#### Ordner erstellen

Dieses Aktionsmodul erstellt einen neuen Ordner in SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL SharePoint]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL SharePoint] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eingabe von Site-, Drive- und Ordner-IDs]</td> 
   <td> <p>Wählen Sie aus, wie Sie den Speicherort des Ordners identifizieren möchten, den Sie erstellen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie die <strong>[!UICONTROL Site ID]</strong>, die <strong>[!UICONTROL List ID]</strong> und die <strong>[!UICONTROL Folder ID]</strong> in die angezeigten Felder ein oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Wählen Sie aus der Liste aus, der Sie folgen]</strong> </p> <p>Wählen Sie den Speicherort aus, an dem Sie den Ordner erstellen möchten. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordnername]</td> 
   <td>Geben Sie einen Namen für den neuen Ordner ein oder ordnen Sie ihn zu.</td> 
  </tr>
  </tbody> 
</table>

#### Datei abrufen

Dieses Aktionsmodul ruft die angegebene SharePoint-Datei ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL SharePoint]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL SharePoint] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eingabe von Site-, Drive- und Ordner-IDs]</td> 
   <td> <p>Wählen Sie aus, wie Sie den Speicherort der Datei identifizieren möchten, die Sie abrufen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie die <strong>[!UICONTROL Site ID]</strong>, die <strong>[!UICONTROL List ID]</strong> und die <strong>[!UICONTROL File ID]</strong> in die angezeigten Felder ein oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Wählen Sie aus der Liste aus, der Sie folgen]</strong> </p> <p>Wählen Sie den Speicherort der Datei aus. </p> </li> 
    </ul> </td> 
  </tr> 
</tbody> 
</table>

#### Ordnerelemente überwachen

Dieses Trigger-Modul startet ein Szenario, wenn ein Element in einem von Ihnen ausgewählten Ordner aktualisiert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL SharePoint]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL SharePoint] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eingabe von Site-, Drive- und Ordner-IDs]</td> 
   <td> <p>Wählen Sie aus, wie Sie den Speicherort der Datei identifizieren möchten, die Sie abrufen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie die <strong>[!UICONTROL Site ID]</strong>, die <strong>[!UICONTROL List ID]</strong> und die <strong>[!UICONTROL Ordner-ID]</strong> in die angezeigten Felder ein oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Wählen Sie aus der Liste aus, der Sie folgen]</strong> </p> <p>Wählen Sie den Speicherort des Ordners aus, den Sie überwachen möchten. </p> </li> 
    </ul> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Geben Sie die maximale Anzahl von Elementen ein, die [!DNL Workfront Fusion] während eines Szenario-Ausführungszyklus zurückgeben soll.</td> 
  <tr>
  </tr>
</tbody> 
</table>

### Element

* [[!UICONTROL Element kopieren]](#copy-an-item)
* [[!UICONTROL Element erstellen]](#create-an-item)
* [[!UICONTROL Löschen eines Elements]](#delete-an-item)
* [[!UICONTROL Element abrufen]](#get-an-item)
* [[!UICONTROL Listenelemente]](#list-items)
* [[!UICONTROL Element verschieben]](#move-an-item)
* [[!UICONTROL Aktualisieren eines Elements]](#update-an-item)
* [[!UICONTROL Elemente ansehen] (geplant)](#watch-items-scheduled)


#### [!UICONTROL Element kopieren]

Dieses Aktionsmodul kopiert ein vorhandenes Element in einer SharePoint-Liste.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL SharePoint]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL SharePoint] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Eingabe von Site-, Laufwerk- und Ordner-IDs</td> 
   <td> <p>Wählen Sie aus, wie Sie die Site und die Liste identifizieren möchten, die das zu kopierende Element enthalten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie die <strong>[!UICONTROL Site ID]</strong>, die <strong>[!UICONTROL List ID]</strong> und die <strong>[!UICONTROL Item ID]</strong> in die angezeigten Felder ein oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Wählen Sie aus der Liste aus, der Sie folgen]</strong> </p> <p>Wählen Sie im Feld Elementtyp aus, ob Sie ein Feld oder einen Ordner verschieben möchten.  Wählen Sie die Site aus, die das zu kopierende Element enthält, wählen Sie dann die Liste aus und wählen Sie dann das Element aus. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ziel-ID]</td> 
   <td> Geben Sie die Kennung des Ordners ein, in den Sie das Element kopieren möchten, oder ordnen Sie sie zu. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Neuer Name]</td> 
   <td>Geben Sie einen Namen für die neue Kopie des Elements ein oder ordnen Sie ihn zu. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Element erstellen]

Dieses Aktionsmodul erstellt ein neues Element in einer SharePoint-Liste.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL SharePoint]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL SharePoint] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Element erstellen]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Site identifizieren möchten, und geben Sie an, wo Sie ein Element erstellen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie die <strong>[!UICONTROL Site ID]</strong> und die <strong>[!UICONTROL List ID]</strong> in die angezeigten Felder ein oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Auswahl aus der Liste]</strong> </p> <p>Wählen Sie die Site mit der Liste aus, in der Sie ein Element erstellen möchten, und wählen Sie dann die Liste aus. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Felder]</td> 
   <td>Geben Sie für jedes Feld, das Sie für das neue Element festlegen möchten, den Schlüssel des Felds (identifiziert das Feld) und den Wert ein, den das neue Element für dieses Feld aufweisen soll.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Löschen eines Elements]

Dieses Aktionsmodul löscht ein vorhandenes Element in einer SharePoint-Liste.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL SharePoint]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL SharePoint] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Element aktualisieren]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Site und die Liste identifizieren möchten, die das zu löschende Element enthalten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie die <strong>[!UICONTROL Site ID]</strong>, die <strong>[!UICONTROL List ID]</strong> und die <strong>[!UICONTROL Item ID]</strong> in die angezeigten Felder ein oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Auswahl aus der Liste]</strong> </p> <p>Wählen Sie die Site aus, die das zu löschende Element enthält, wählen Sie dann die Liste aus und wählen Sie dann das Element aus. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Element abrufen]

Dieses Aktionsmodul gibt die Daten eines angegebenen Elements zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL SharePoint]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL SharePoint] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Element abrufen]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Site und die Liste identifizieren möchten, die das gewünschte Element enthalten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie die <strong>[!UICONTROL Site ID]</strong>, die <strong>[!UICONTROL List ID]</strong> und die <strong>[!UICONTROL Item ID]</strong> in die angezeigten Felder ein oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Auswahl aus der Liste]</strong> </p> <p>Wählen Sie die Site aus, die die Liste enthält, aus der Sie ein Element abrufen möchten, wählen Sie die Liste aus und wählen Sie dann das Element aus. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listenelemente]

Dieses Aktionsmodul ruft eine Liste aller Elemente in einer angegebenen Liste ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL SharePoint]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL SharePoint] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listenelemente]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Liste identifizieren möchten, aus der Elemente abgerufen werden sollen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie die <strong>[!UICONTROL Site ID]</strong> und die <strong>[!UICONTROL List ID]</strong> in die angezeigten Felder ein oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Auswahl aus der Liste]</strong> </p> <p>Wählen Sie die Site mit der Liste aus, aus der Sie Elemente abrufen möchten, und wählen Sie dann die Liste aus. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Elementen ein oder ordnen Sie sie zu, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Verschieben eines Elements]

Dieses Aktionsmodul kopiert ein vorhandenes Element in einer SharePoint-Liste.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL SharePoint]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL SharePoint] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Eingabe von Site-, Laufwerk- und Ordner-IDs</td> 
   <td> <p>Wählen Sie aus, wie Sie die Site und die Liste identifizieren möchten, die das zu verschiebende Element enthalten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie die <strong>[!UICONTROL Site ID]</strong>, die <strong>[!UICONTROL List ID]</strong> und die <strong>[!UICONTROL Item ID]</strong> in die angezeigten Felder ein oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Wählen Sie aus der Liste aus, der Sie folgen]</strong> </p> <p>Wählen Sie im Feld Elementtyp aus, ob Sie ein Feld oder einen Ordner verschieben möchten. Wählen Sie die Site aus, die das zu kopierende Element enthält, wählen Sie dann die Liste aus und wählen Sie dann das Element aus. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ziel-ID]</td> 
   <td> Geben Sie die Kennung des Ordners ein, in den Sie das Element verschieben möchten, oder ordnen Sie sie zu. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Neuer Name]</td> 
   <td>Geben Sie einen Namen für das verschobene Element ein oder ordnen Sie ihn zu. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aktualisieren eines Elements]

Dieses Aktionsmodul aktualisiert ein vorhandenes Element in einer SharePoint-Liste.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL SharePoint]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL SharePoint] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Element aktualisieren]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Site und die Liste identifizieren möchten, die das zu aktualisierende Element enthalten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie die <strong>[!UICONTROL Site ID]</strong>, die <strong>[!UICONTROL List ID]</strong> und die <strong>[!UICONTROL Item ID]</strong> in die angezeigten Felder ein oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Auswahl aus der Liste]</strong> </p> <p>Wählen Sie die Site aus, die das zu aktualisierende Element enthält, wählen Sie dann die Liste aus und wählen Sie dann das Element aus. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Felder]</td> 
   <td>Geben Sie für jedes Feld, das Sie für das neue Element aktualisieren möchten, den Schlüssel des Felds (identifiziert das Feld) und den neuen Wert ein, den das Element für dieses Feld aufweisen soll.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Elemente ansehen] (geplant)

Dieses Trigger-Modul startet ein Szenario, wenn ein Element erstellt oder geändert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL SharePoint]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL SharePoint] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Überwachungslisten]</td> 
   <td>Wählen Sie aus, ob Sie Listen nach Erstellungszeit (neue Elemente) oder Änderungszeitpunkt (aktualisierte Elemente) überwachen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eingabe der Site- und Listen-ID]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Site und die Liste identifizieren möchten, die Sie sehen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie die <strong>[!UICONTROL Site ID]</strong> und die <strong>[!UICONTROL List ID]</strong> in die angezeigten Felder ein oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Wählen Sie aus der Liste aus, der Sie folgen]</strong> </p> <p>Wählen Sie die Website aus, die Sie ansehen möchten, und wählen Sie dann die Liste aus. Diese Dropdown-Listen rufen nur die folgenden Sites ab.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Elementen ein oder ordnen Sie sie zu, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Liste

* [[!UICONTROL Erstellen einer Liste]](#create-a-list)
* [[!UICONTROL Liste abrufen]](#get-a-list)
* [[!UICONTROL Listenlisten]](#list-lists)
* [[!UICONTROL Listen ansehen]](#watch-lists)

#### [!UICONTROL Erstellen einer Liste]

Dieses Aktionsmodul erstellt eine neue Liste in SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL SharePoint]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL SharePoint] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eingabe einer Site-ID]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Site identifizieren möchten, und geben Sie an, wo Sie eine Liste erstellen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie die <strong>[!UICONTROL Site ID]</strong> ein oder ordnen Sie sie zu, in der Sie eine Liste erstellen möchten.</p> </li> 
     <li> <p><strong>[!UICONTROL Auswahl aus der Liste]</strong> </p> <p>Wählen Sie die Site aus, auf der Sie eine Liste erstellen möchten. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anzeigename]</td> 
   <td>Geben Sie einen Namen für die neue Liste ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Beschreibung]</td> 
   <td>Geben Sie eine Beschreibung für die neue Liste ein oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Spalten hinzufügen]</td> 
   <td>Geben Sie für jede Spalte, die Sie für die neue Liste festlegen möchten, einen <strong>[!UICONTROL Namen]</strong> für das Feld ein und wählen Sie den Wert <strong>[!UICONTROL Type]</strong> aus, den die neue Spalte aufweisen soll.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Liste abrufen]

Dieses Aktionsmodul gibt die Daten einer angegebenen Liste zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL SharePoint]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL SharePoint] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Liste abrufen]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Site und die Liste identifizieren möchten, die das gewünschte Element enthalten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie die <strong>[!UICONTROL Site ID]</strong> und die <strong>Listen-ID</strong> in die angezeigten Felder ein oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Auswahl aus der Liste]</strong> </p> <p>Wählen Sie die Site aus, die die Liste enthält, die Sie abrufen möchten, und wählen Sie dann die Liste aus. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listenlisten]

Dieses Aktionsmodul ruft eine Liste aller Elemente in einer angegebenen Liste ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL SharePoint]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL SharePoint] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listen]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Site identifizieren möchten, von der Sie Listen abrufen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie die <strong>[!UICONTROL Site ID]</strong> ein oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Auswahl aus der Liste]</strong> </p> <p>Wählen Sie die Site aus, die die Listen enthält, die Sie abrufen möchten. Über das Dropdown-Menü werden nur die folgenden Sites abgerufen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Listen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungsperioden zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listen ansehen]

Dieses Trigger-Modul startet ein Szenario, wenn eine Liste erstellt oder geändert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL SharePoint]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL SharePoint] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Überwachungslisten]</td> 
   <td>Wählen Sie aus, ob Sie Listen nach Erstellungszeit (neue Elemente) oder Änderungszeitpunkt (aktualisierte Elemente) überwachen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eingabe der Site- und Listen-ID]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Site und die Liste identifizieren möchten, die Sie sehen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie die <strong>[!UICONTROL Site ID]</strong> ein oder ordnen Sie sie zu, wo sich die Liste befindet, die Sie sehen möchten.</p> </li> 
     <li> <p><strong>[!UICONTROL Wählen Sie aus der Liste aus, der Sie folgen]</strong> </p> <p>Wählen Sie die Website aus, die Sie ansehen möchten. Über die Dropdown-Liste werden nur die von Ihnen verfolgte Site abgerufen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Listen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungsperioden zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Seite (Beta)

>[!NOTE]
>
>APIs in der Version `beta` in [!DNL Microsoft Graph] können sich ändern. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

#### [!UICONTROL Abrufen einer Seite]

Dieses Aktionsmodul gibt die Daten einer angegebenen Seite zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL SharePoint]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL SharePoint] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seite abrufen]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Seite identifizieren möchten, die Sie abrufen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie die <strong>[!UICONTROL Site ID]</strong>und die <strong>[!UICONTROL Seiten-ID]</strong> ein oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Auswahl aus der Liste]</strong> </p> <p>Wählen Sie die Site mit der Seite aus, die Sie abrufen möchten, und wählen Sie dann die Seite aus.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Site

* [[!UICONTROL Eine Site abrufen]](#get-a-site)
* [[!UICONTROL Suchseiten]](#search-sites)

#### [!UICONTROL Eine Site abrufen]

Dieses Aktionsmodul gibt die Daten einer angegebenen Site zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL SharePoint]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL SharePoint] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eine Site abrufen]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Seite identifizieren möchten, die Sie abrufen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie die <strong>[!UICONTROL Site ID]</strong> ein oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Auswahl aus der Liste]</strong> </p> <p>Wählen Sie die Site aus, die Sie abrufen möchten.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suchseiten]

Dieses Aktionsmodul sucht nach Sites anhand eines von Ihnen angegebenen Parameters.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL SharePoint]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL SharePoint] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Schlüsselwort des Anzeigenamens]</td> 
   <td> <p>Geben Sie den Suchbegriff ein oder ordnen Sie ihn zu, nach dem Sie die Sites suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Sites ein oder ordnen Sie sie zu, die das Modul während der einzelnen Szenario-Ausführungszyklen zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Sonstige

* [Abrufen von Änderungen](#get-changes)
* [API-Aufruf durchführen](#make-an-api-call)
* [Ereignisse beobachten](#watch-events)

#### Abrufen von Änderungen

Dieses Modul ruft Ergänzungen, Aktualisierungen und Löschungen ab, die im Ordner &quot;SharePoint&quot;vorgenommen wurden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL SharePoint]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL SharePoint] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eingabe von Site-, Drive- und Ordner-IDs]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Site und die Liste identifizieren möchten, die das zu aktualisierende Element enthalten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie die <strong>[!UICONTROL Site ID]</strong>, die <strong>[!UICONTROL Drive ID]</strong> und die <strong>[!UICONTROL Folder ID]</strong> in die angezeigten Felder ein oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Auswahl aus der Liste]</strong> </p> <p>Wählen Sie die Site aus, die das zu aktualisierende Element enthält, wählen Sie dann das Laufwerk aus und wählen Sie dann den Ordner aus. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Token]</td> 
   <td> Das Token gibt an, ab welchem Punkt das Modul mit dem Abrufen von Änderungen beginnen soll.  </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL API-Aufruf durchführen]

Mit diesem Modul können Sie einen benutzerdefinierten API-Aufruf ausführen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL SharePoint]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL SharePoint] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Geben Sie einen Pfad relativ zu <code>https://graph.microsoft.com</code> ein. Beispiel:<code> /beta/sites</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Methode]</p> </td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu, z. B. <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] fügt die Autorisierungskopfzeilen für Sie hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p> Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Typ]</td> 
   <td>Wählen Sie im API-Aufruf den Datentyp aus, den Sie senden möchten.</td> 
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

#### Ereignisse beobachten

Dieses Instant Trigger-Modul startet ein Szenario, wenn ein Element in SharePoint hinzugefügt, aktualisiert oder gelöscht wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
  <!--
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront Fusion], see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  -->
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Wählen Sie einen vorhandenen Webhook aus oder klicken Sie auf Hinzufügen , um einen neuen Webhook zu erstellen.</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

