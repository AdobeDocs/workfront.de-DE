---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Archivmodule
description: In einem [!DNL Adobe Workfront Fusion] Szenario können Sie ein Archiv, z. B. eine komprimierte Datei, mit mehreren Anwendungen und Diensten von Drittanbietern verbinden. Sie können beispielsweise ein Szenario konfigurieren, bei dem
author: Becky
feature: Workfront Fusion
exl-id: e29b6d39-3666-4d6d-a178-1983ae9f3aa9
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# [!UICONTROL Archive] -Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie in Ihrem Szenario ein Archiv, z. B. eine komprimierte Datei, verwenden, um es in Ihren Automatisierungen oder Integrationen verwenden zu können.

Wenn Sie Anweisungen zum Erstellen eines Szenarios benötigen, finden Sie weitere Informationen unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## [!UICONTROL Archivieren] -Module und ihre Felder

Wenn Sie die Module [!UICONTROL Archivieren] konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche Felder für [!UICONTROL Archivieren] angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Archiv extrahieren]](#extract-an-archive)
* [[!UICONTROL Erstellen eines Archivs]](#create-an-archive)
* [[!UICONTROL inflate]](#inflate)
* [[!UICONTROL Deflate]](#deflate)

## [!UICONTROL Archiv extrahieren]

Dieses Aktionsmodul extrahiert eine Datei, die Sie aus einem Archiv identifizieren.

Das Modul gibt die Kennung der Datei und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source-Datei]</td> 
   <td> <p> Wählen Sie die zu extrahierende Datei aus. Diese Datei kann von einem vorherigen Modul zugeordnet werden (z. B. dem Modul "[!DNL Workfront]"&gt; "[!UICONTROL Dokument herunterladen").</p>  </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Beispiel:** Rufen Sie die ZIP-Datei aus dem definierten Ordner [!DNL Dropbox] ab (z. B. Archive), extrahieren Sie sie mit dem Modul [!UICONTROL Archiv] und senden Sie extrahierte Dateien als Anhänge mit dem Modul [!UICONTROL E-Mail] oder [!DNL Gmail] an die gewünschte E-Mail-Adresse.
>
>![](assets/example-dropbox-350x134.png)

## [!UICONTROL Erstellen eines Archivs]

Dieses Aggregatormodul fügt die gewünschten Dateien einem [!UICONTROL ZIP] - oder [!UICONTROL TAR] -Archiv hinzu.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source-Modul]</td> 
   <td> <p> Wählen Sie das Modul aus, aus dem Sie die Dateien abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Typ] </td> 
   <td> <p>Wählen Sie aus, ob Sie Dateien zu einem [!UICONTROL ZIP]-Archiv oder einem [!UICONTROL TAR]-Archiv hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kommentar]</td> 
   <td>Geben Sie einen Kommentar ein, den Sie dem Archiv hinzufügen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gruppe nach]</td> 
   <td> <p>Definieren Sie einen Ausdruck, nach dem Sie die aggregierte Ausgabe gruppieren möchten. Dieser Ausdruck kann ein oder mehrere zugeordnete Elemente enthalten. Die aggregierten Daten werden dann mithilfe des Werts dieses Ausdrucks in Gruppen unterteilt. Jede Gruppe gibt als separates Bundle mit einem Schlüssel (dem ausgewerteten Ausdruck) und einem Wert (dem aggregierten Text) aus. Sie können den Schlüssel als Filter in nachfolgenden Modulen verwenden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Verarbeitung nach einer leeren Aggregation stoppen]</td> 
   <td>Wählen Sie diese Option, um das Szenario zu stoppen, wenn keine Ergebnisse vorliegen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Archivname]</td> 
   <td> <p> Geben Sie einen Namen für das erstellte Archiv ein. Fügen Sie keine Erweiterung hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Beispiel:** Sehen Sie eingehende E-Mails mithilfe des Moduls [!DNL Gmail] >[!UICONTROL E-Mails ansehen] an. Wenn eine E-Mail empfangen wird, werden ihre Anhänge in einzelne Bundles iteriert, dann in der Datei [!DNL ZIP] archiviert und im definierten Dropbox-Ordner gespeichert.
>
>![](assets/example-gmail-350x102.png)

## [!UICONTROL inflate]

Dieses Transformatormodul dekomprimiert Binärdaten mithilfe eines Inflationsalgorithmus.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Daten] </td> 
   <td> <p>Geben Sie die Daten ein oder ordnen Sie sie mithilfe der Aufblähung-Funktion zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL Deflate]

Dieses Transformatormodul komprimiert Binärdaten mithilfe eines Deflationsalgorithmus.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Daten] </td> 
   <td> <p>Geben Sie die Daten, die Sie komprimieren möchten, mithilfe der deflate -Funktion ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>
