---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Archivierungsmodule
description: In  [!DNL Adobe Workfront Fusion]  Szenario können Sie ein Archiv, z. B. eine ZIP-Datei, mit mehreren Anwendungen und Services von Drittanbietern verbinden. Sie können beispielsweise ein Szenario konfigurieren, das
author: Becky
feature: Workfront Fusion
exl-id: e29b6d39-3666-4d6d-a178-1983ae9f3aa9
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# [!UICONTROL Archivieren] Module

In einem [!DNL Adobe Workfront Fusion] Szenario können Sie ein Archiv, z. B. eine ZIP-Datei, in Ihrem Szenario verwenden, sodass Sie es in Ihren Automatisierungen oder Integrationen verwenden können.

Anweisungen zum Erstellen eines Szenarios finden Sie unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## [!UICONTROL Archivieren] Module und ihre Felder

Beim Konfigurieren von [!UICONTROL Archiv]-Modulen zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können zusätzliche [!UICONTROL Archivieren]-Felder angezeigt werden, abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder dem Service. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Entpacken Sie ein Archiv]](#extract-an-archive)
* [[!UICONTROL Erstellen eines Archivs]](#create-an-archive)
* [[!UICONTROL aufblasen]](#inflate)
* [[!UICONTROL Entlüften]](#deflate)

## [!UICONTROL Entpacken Sie ein Archiv]

Dieses Aktionsmodul extrahiert eine identifizierte Datei aus einem Archiv.

Das Modul gibt die ID der Datei und aller zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source-Datei]</td> 
   <td> <p> Wählen Sie die zu extrahierende Datei aus. Diese Datei kann von einem vorherigen Modul (z. B. dem Modul [!DNL Workfront] &gt;[!UICONTROL Dokument herunterladen]) zugeordnet werden.</p>  </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Beispiel** Rufen Sie die ZIP-Datei aus dem definierten [!DNL Dropbox]-Ordner ab (z. B. „Archive„), extrahieren Sie sie mithilfe des [!UICONTROL Archive]-Moduls und senden Sie die extrahierten Dateien als Anhänge mit dem [!UICONTROL Email]- oder [!DNL Gmail]-Modul an die gewünschte E-Mail-Adresse.
>
>![](assets/example-dropbox-350x134.png)

## [!UICONTROL Erstellen eines Archivs]

Dieses Aggregator-Modul fügt die gewünschten Dateien zu einem [!UICONTROL ZIP]- oder [!UICONTROL TAR]-Archiv hinzu.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source-Modul]</td> 
   <td> <p> Wählen Sie das Modul aus, von dem Sie die Dateien abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Typ] </td> 
   <td> <p>Wählen Sie aus, ob Sie Dateien zu einem [!UICONTROL ZIP]-Archiv oder einem [!UICONTROL TAR]-Archiv hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Kommentar]</td> 
   <td>Geben Sie einen Kommentar ein, den Sie dem Archiv hinzufügen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gruppieren nach]</td> 
   <td> <p>Definieren Sie einen Ausdruck, nach dem die aggregierte Ausgabe gruppiert werden soll. Dieser Ausdruck kann ein oder mehrere zugeordnete Elemente enthalten. Die aggregierten Daten werden dann mithilfe des Werts dieses Ausdrucks in Gruppen aufgeteilt. Jede Gruppe gibt als separates Bundle mit einem Schlüssel (dem ausgewerteten Ausdruck) und einem Wert (dem aggregierten Text) aus. Sie können den Schlüssel als Filter in nachfolgenden Modulen verwenden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Verarbeitung nach einer leeren Aggregation anhalten]</td> 
   <td>Wählen Sie diese Option, um das Szenario anzuhalten, wenn keine Ergebnisse vorliegen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Archivname]</td> 
   <td> <p> Geben Sie einen Namen für das erstellte Archiv ein. Keine Erweiterung hinzufügen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Beispiel:** eingehende E-Mails mit dem Modul [!DNL Gmail] > [!UICONTROL E-Mails ]. Wenn eine E-Mail empfangen wird, werden ihre Anhänge in einzelne Bundles iteriert, dann in der [!DNL ZIP] archiviert und im definierten Dropbox-Ordner gespeichert.
>
>![](assets/example-gmail-350x102.png)

## [!UICONTROL aufblasen]

Dieses Transformatormodul dekomprimiert Binärdaten mithilfe eines Inflationsalgorithmus.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Daten] </td> 
   <td> <p>Geben Sie die Daten, die Sie dekomprimieren möchten, mithilfe der Inflate-Funktion ein oder mappen Sie sie.</p> </td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL Entlüften]

Dieses Transformatormodul komprimiert Binärdaten mit einem Deflationsalgorithmus.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Daten] </td> 
   <td> <p>Geben Sie die Daten, die Sie komprimieren möchten, mit der Deflate-Funktion ein oder mappen Sie sie.</p> </td> 
  </tr> 
 </tbody> 
</table>
