---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Hinzufügen eines Filters zu einem Szenario in  [!DNL Adobe] Workfront Fusion
description: In einigen Szenarien müssen Sie nur mit Bundles arbeiten, die bestimmte Kriterien erfüllen. Mit Filtern können Sie diese Bundles auswählen.
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# Filter zu einem Szenario in [!DNL Adobe Workfront Fusion] hinzufügen

In einigen Szenarien müssen Sie nur mit Bundles arbeiten, die bestimmte Kriterien erfüllen. Mit Filtern können Sie diese Bundles auswählen.

<!--

For example, you could create a scenario with the [!UICONTROL Watch records] trigger for [!DNL Salesforce] to capture only records containing a specific word written by a specific author.

-->

Sie können einen Filter zwischen zwei Modulen hinzufügen und überprüfen, ob von den vorherigen Modulen erhaltene Bundles bestimmte Filterbedingungen erfüllen:

* Wenn dies der Fall ist, werden die Bundles im Szenario an das nächste Modul übergeben.
* Ist dies nicht der Fall, wird die Verarbeitung für die Bundles beendet.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz*</td> 
  <td>
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
   </td>    </tr> 
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

Sie müssen beide Module zu einem Szenario hinzufügen, bevor Sie einen Filter zwischen ihnen hinzufügen können.

## Fügen Sie einen Filter zwischen zwei Modulen hinzu:

1. Klicken Sie im linken Bereich auf **[!UICONTROL Szenarios]** ![](assets/scenarios-icon.png) und wählen Sie dann das Szenario aus, um es zu öffnen.
1. Klicken Sie in der oberen rechten Ecke des Fensters auf **[!UICONTROL Bearbeiten]**.
1. Klicken Sie auf die Verbindungslinie zwischen den Modulen.
1. Geben Sie in das angezeigte Feld einen **[!UICONTROL Titel]** für den Filter ein.
1. Definieren Sie einen Filter **[!UICONTROL Bedingung]**.

   Sie können ein oder zwei Operanden in die beiden Felder eingeben. Wenn Sie Operanden in beide Felder eingeben, können Sie im Dropdown-Menü zwischen ihnen einen Operator auswählen, um die Beziehung zwischen ihnen festzulegen.

   >[!TIP]
   >
   >In den Operandenfeldern können Sie Werte auf dieselbe Weise eingeben wie bei der Zuordnung, wie unter [Informationen von einem Modul einem anderen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) zuordnen beschrieben.

   Wenn Sie beispielsweise möchten, dass der Filter Dateien in [!DNL Adobe Workfront] findet, die mit XML enden, und sie an [!DNL Dropbox] übergibt, geben Sie in das erste Feld und den Dateinamen **[!UICONTROL 3} ein.]****[!UICONTROL xml]** im zweiten Feld. Im Dropdown-Menü zwischen ihnen wählen Sie **[!UICONTROL Ends with (case not ensitive)]** aus. Dieser Filter würde für eingehende Bundles aus dem ersten Modul (Workfront) gelten. Nur Pakete mit XML-Dateien werden an das nächste Modul ([!DNL Dropbox]) übergeben.

   ![](assets/set-up-filter-box-350x368.jpg)

1. Klicken Sie auf **[!DNL OK]**.

## Filter kopieren

Derzeit enthält der Szenario-Editor keine Funktion zum Kopieren eines Filters.

>[!NOTE]
>
>Wenn Sie die Module auf beiden Seiten des Filters kopieren, wird der Filter ebenfalls kopiert.
>
>Weitere Informationen zum Kopieren von Modulen finden Sie unter [Kopieren von Modulen oder Szenarien in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)

Um einen Filter zu kopieren, ohne Module zu kopieren, können Sie für die folgende Problemumgehung [!DNL Google] Chrome verwenden:

1. Installieren Sie die Erweiterung [!UICONTROL [!DNL Adobe Workfront Fusion] DevTool Chrome] .
1. Öffnen Sie in [!DNL Workfront Fusion] das Szenario.
1. Klicken Sie auf das Drei-Punkte-Menü von Chrome und dann auf **[!UICONTROL Weitere Tools*]* > **[!UICONTROL Entwicklertools]**.

1. Klicken Sie im Bereich [!UICONTROL Entwicklertools] , der oben in der Menüleiste angezeigt wird, auf die Registerkarte [!UICONTROL Workfront Fusion] .

   ![](assets/copy-a-filter-350x174.png)

1. Klicken Sie in der linken Seitenleiste auf das Symbol **[!UICONTROL Tools]** ![](assets/devtools-tools-icon.png) .

1. Klicken Sie auf **[!UICONTROL Filter kopieren]** und konfigurieren Sie dann das Tool **[!UICONTROL Filter kopieren]** im rechten Seitenbereich:

   1. Legen Sie das **[!UICONTROL Source-Modul]** als Modul direkt nach dem Filter fest, den Sie kopieren möchten.
   1. Legen Sie das **[!UICONTROL Zielmodul]** als Modul direkt vor dem Filter fest, den Sie kopieren möchten.

1. Klicken Sie auf **[!UICONTROL Ausführen]**.
