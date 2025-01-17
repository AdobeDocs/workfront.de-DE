---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Hinzufügen eines Filters zu einem Szenario in  [!DNL Adobe] Workfront Fusion
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---

# Hinzufügen eines Filters zu einem Szenario in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Hinzufügen eines Filters zu einem Szenario](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/add-a-filter-to-a-scenario.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

In einigen Szenarien müssen Sie nur mit Bundles arbeiten, die bestimmte Kriterien erfüllen. Mit Filtern können Sie diese Bundles auswählen.

<!--

For example, you could create a scenario with the [!UICONTROL Watch records] trigger for [!DNL Salesforce] to capture only records containing a specific word written by a specific author.

-->

Sie können einen Filter zwischen zwei Modulen hinzufügen und überprüfen, ob die von den vorherigen Modulen empfangenen Pakete bestimmte Filterbedingungen erfüllen:

* Wenn dies der Fall ist, werden die Bundles an das nächste Modul im Szenario weitergegeben.
* Ist dies nicht der Fall, wird die Verarbeitung für die Bundles beendet.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] Lizenz**</td> 
  <td>
   <p>Aktuelle Lizenzanforderung: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!DNL Adobe Workfront] [!UICONTROL Select] oder [!UICONTROL Prime] verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu nutzen. [!DNL Workfront Fusion] ist im [!DNL Workfront] [!UICONTROL Ultimate] enthalten.</p>
   <p>Oder</p>
   <p>Legacy-Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Sie müssen beide Module zu einem Szenario hinzufügen, bevor Sie einen Filter zwischen ihnen hinzufügen können.

## Fügen Sie einen Filter zwischen zwei Modulen hinzu:

1. Klicken Sie **[!UICONTROL linken Bedienfeld auf]** Szenarien![](assets/scenarios-icon.png) und wählen Sie dann das Szenario aus, um es zu öffnen.
1. Klicken Sie oben rechts im Fenster auf **[!UICONTROL Bearbeiten]**.
1. Klicken Sie auf die Verbindungslinie zwischen den Modulen.
1. Geben Sie in das angezeigte Feld einen **[!UICONTROL Titel]** für den Filter ein.
1. Definieren Sie einen Filter **[!UICONTROL Bedingung]**.

   Sie können in die beiden Felder einen oder zwei Operanden eingeben. Wenn Sie in beide Felder Operanden eingeben, können Sie im Dropdown-Menü zwischen den Feldern einen Operator auswählen, um die Beziehung zwischen ihnen anzugeben.

   >[!TIP]
   >
   >In die Operandenfelder können Sie Werte auf die gleiche Weise eingeben, wie Sie sie zuordnen würden, wie in [Zuordnen von Informationen von einem Modul zu einem anderen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) beschrieben.

   Wenn der Filter beispielsweise Dateien in [!DNL Adobe Workfront] suchen soll, die auf XML enden, und sie an [!DNL Dropbox] weitergeben soll, geben Sie **[!UICONTROL Dateiname]** in das erste Feld ein und .**[!UICONTROL xml]** im zweiten Feld an. Im Dropdown-Menü zwischen ihnen wählen Sie **[!UICONTROL Endet mit (Groß-/Kleinschreibung wird nicht beachtet)]**. Dieser Filter würde für eingehende Bundles des ersten Moduls (Workfront) gelten. Nur Bundles mit XML-Dateien würden an das nächste Modul ([!DNL Dropbox]) weitergegeben.

   ![](assets/set-up-filter-box-350x368.jpg)

1. Klicken Sie auf **[!DNL OK]**.

## Kopieren von Filtern

Derzeit enthält der Szenario-Editor keine Funktion zum Kopieren eines Filters.

>[!NOTE]
>
>Wenn Sie die Module auf beiden Seiten des Filters kopieren, wird der Filter ebenfalls kopiert.
>
>Weitere Informationen zum Kopieren von Modulen finden Sie unter [Module oder Szenarien kopieren in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)

Um einen Filter zu kopieren, ohne Module zu kopieren, können Sie [!DNL Google] Chrome für die folgende Problemumgehung verwenden:

1. Installieren Sie die [!UICONTROL [!DNL Adobe Workfront Fusion] DevTool Chrome]-Erweiterung.
1. Öffnen Sie in [!DNL Workfront Fusion] das Szenario.
1. Klicken Sie auf das Chrome-Dreipunkt-Menü und dann auf **[!UICONTROL Weitere Tools*]* > **[!UICONTROL Entwickler-Tools]**.

1. Klicken Sie [!UICONTROL  angezeigten Bedienfeld ]Entwickler-Tools“ in der Menüleiste am oberen Rand auf die Registerkarte [!UICONTROL Workfront Fusion] .

   ![](assets/copy-a-filter-350x174.png)

1. Klicken Sie auf **[!UICONTROL Symbol]** Tools![](assets/devtools-tools-icon.png) in der linken Seitenleiste.

1. Klicken Sie **[!UICONTROL Filter kopieren]** und konfigurieren Sie dann das **[!UICONTROL Filter kopieren]**-Tool im rechten Seitenbereich:

   1. Legen Sie das **[!UICONTROL Source]** Modul direkt nach dem Filter, den Sie kopieren möchten, als Modul fest.
   1. Legen Sie das **[!UICONTROL Target-Modul]** als Modul direkt vor dem Filter fest, den Sie kopieren möchten.

1. Klicken Sie auf **[!UICONTROL Ausführen]**.
