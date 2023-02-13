---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Hinzufügen eines Filters zu einem Szenario in [!DNL Adobe] Workfront Fusion
description: In einigen Szenarien müssen Sie nur mit Bundles arbeiten, die bestimmte Kriterien erfüllen. Mit Filtern können Sie diese Bundles auswählen.
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

# Hinzufügen eines Filters zu einem Szenario in [!DNL Adobe Workfront Fusion]

In einigen Szenarien müssen Sie nur mit Bundles arbeiten, die bestimmte Kriterien erfüllen. Mit Filtern können Sie diese Bundles auswählen.

<!--

For example, you could create a scenario with the [!UICONTROL Watch records] trigger for [!DNL Salesforce] to capture only records containing a specific word written by a specific author.

-->

Sie können einen Filter zwischen zwei Modulen hinzufügen und überprüfen, ob von den vorherigen Modulen erhaltene Bundles bestimmte Filterbedingungen erfüllen:

* Wenn dies der Fall ist, werden die Bundles im Szenario an das nächste Modul übergeben.
* Ist dies nicht der Fall, wird die Verarbeitung für die Bundles beendet.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p><p>[!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung] </p>  </td>    </tr> 
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

Sie müssen beide Module zu einem Szenario hinzufügen, bevor Sie einen Filter zwischen ihnen hinzufügen können.

## Fügen Sie einen Filter zwischen zwei Modulen hinzu:

1. Klicken **[!UICONTROL Szenarien]** ![](assets/scenarios-icon.png) Wählen Sie im linken Bereich das Szenario aus, um es zu öffnen.
1. Klicken Sie oben rechts im Fenster auf **[!UICONTROL Bearbeiten]**.
1. Klicken Sie auf die Verbindungslinie zwischen den Modulen.
1. Geben Sie in das angezeigte Feld einen **[!UICONTROL Titel]** für den Filter.
1. Filter definieren **[!UICONTROL Bedingung]**.

   Sie können ein oder zwei Operanden in die beiden Felder eingeben. Wenn Sie Operanden in beide Felder eingeben, können Sie im Dropdown-Menü zwischen ihnen einen Operator auswählen, um die Beziehung zwischen ihnen festzulegen.

   >[!TIP]
   >
   >In den Operandenfeldern können Sie Werte auf die gleiche Weise eingeben wie bei der Zuordnung, wie in [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

   Wenn der Filter beispielsweise Dateien in finden soll [!DNL Adobe Workfront] endet mit XML und übergibt sie an [!DNL Dropbox]eingeben **[!UICONTROL Dateiname]** im ersten Feld und .**[!UICONTROL xml]** in das zweite Feld ein. Im Dropdown-Menü zwischen ihnen wählen Sie **[!UICONTROL Endet in (nicht von Schreibweise abhängig)]**. Dieser Filter würde für eingehende Bundles aus dem ersten Modul (Workfront) gelten. Nur Pakete mit XML-Dateien werden an das nächste Modul ([!DNL Dropbox]).

   ![](assets/set-up-filter-box-350x368.jpg)

1. Klicken **[!DNL OK]**.

## Filter kopieren

Derzeit enthält der Szenario-Editor keine Funktion zum Kopieren eines Filters.

>[!NOTE]
>
>Wenn Sie die Module auf beiden Seiten des Filters kopieren, wird der Filter ebenfalls kopiert.
>
>Weitere Informationen zum Kopieren von Modulen finden Sie unter [Kopieren Sie Module oder Szenarien in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)

Um einen Filter zu kopieren, ohne Module zu kopieren, können Sie [!DNL Google] Chrome für die folgende Problemumgehung:

1. Installieren Sie die [!UICONTROL [!DNL Adobe Workfront Fusion] DevTool Chrome] -Erweiterung.
1. In [!DNL Workfront Fusion], öffnen Sie das Szenario.
1. Klicken Sie auf das Drei-Punkte-Menü von Chrome und dann auf **[!UICONTROL Weitere Tools*]* > **[!UICONTROL Entwicklertools]**.

1. Im [!UICONTROL Entwicklertools] -Bedienfeld, das oben in der Menüleiste angezeigt wird, klicken Sie auf das [!UICONTROL Workfront Fusion] Registerkarte.

   ![](assets/copy-a-filter-350x174.png)

1. Klicken Sie auf **[!UICONTROL Instrumente]** icon ![](assets/devtools-tools-icon.png) in der linken Seitenleiste.

1. Klicken **[!UICONTROL Filter kopieren]**, konfigurieren Sie dann die **[!UICONTROL Filter kopieren]** im rechten Seitenbereich:

   1. Legen Sie die **[!UICONTROL Quellmodul]** als Modul direkt nach dem Filter, den Sie kopieren möchten.
   1. Legen Sie die **[!UICONTROL Zielmodul]** als Modul direkt vor dem Filter, den Sie kopieren möchten.

1. Klicken **[!UICONTROL Ausführen]**.
