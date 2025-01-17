---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Kopieren Sie Module oder Szenarien in [!DNL Adobe Workfront Fusion]
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 24e77a56-d676-4cf1-a801-1c328ffd0c4e
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# Kopieren von Modulen oder Szenarien in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Module oder Szenarien kopieren](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/copy-modules-or-scenarios.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Sie können Module, Modulgruppen oder ganze Szenarien in [!DNL Adobe Workfront Fusion] kopieren. Mit dieser Funktion können Sie Szenarien oder Teile von Szenarien wiederverwenden, ohne sie erneut erstellen zu müssen

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

Sie müssen Module zu einem Szenario hinzufügen, bevor Sie sie kopieren können.

## Kopieren eines Moduls oder einer Gruppe von Modulen

Beim Kopieren eines Moduls behält die Kopie alle Feldwerte und Einstellungen des ursprünglichen Moduls bei.

Sie können das Modul oder die Module in einen anderen Bereich desselben Szenarios oder in ein anderes Szenario einfügen.

Beachten Sie beim Einfügen von Modulen in ein anderes Szenario Folgendes.

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>If you paste the modules into another scenario, any fields that pull information from a module that you did not copy must be set to pull information from a module in the new scenario.</p> </li>
  -->

* Feldwerte, die Informationen aus einem anderen Modul abrufen, das Sie nicht kopiert haben, können nicht mehr auf diese Informationen zugreifen. Sie müssen diese Felder festlegen, um Informationen aus dem neuen Szenario abzurufen.
* Wenn Sie die Module in ein Szenario einfügen, das einem anderen Team oder einer anderen Organisation gehört, müssen alle Verbindungen zu Verbindungen aktualisiert werden, die der Gruppe oder Organisation gehören, die das neue Szenario besitzt.

### Module kopieren

Das Kopieren einer Gruppe von Modulen ähnelt dem Kopieren eines einzelnen Moduls.

1. Klicken Sie mit der rechten Maustaste auf das Modul, das Sie kopieren möchten.

   >[!NOTE]
   >
   >Sie können mehrere Module auswählen, indem Sie die [!UICONTROL Umschalt]-Taste gedrückt halten und auf die Module klicken, die Sie kopieren möchten. Beim Kopieren einer Gruppe von Modulen werden auch alle Verbindungsleitungen, Filter oder Routing-Logiken zwischen ihnen kopiert.

1. Wählen Sie **[!UICONTROL Modul kopieren]** aus.
1. Bewegen Sie den Cursor in den Bereich des Szenarios, in dem die Kopie des Szenarios erstellt werden soll.
1. Klicken Sie mit der rechten Maustaste und wählen Sie **[!UICONTROL Einfügen]**.
1. Verbinden Sie die eingefügten Module mit dem Szenario, indem Sie sie an die entsprechende Position im Szenario ziehen.

   Sie können auch Tastaturbefehle zum Kopieren und Einfügen verwenden.

## Szenario durch Klonen kopieren

Beim Klonen eines Szenarios wird eine Kopie des Szenarios erstellt, die Sie dann bearbeiten können.

1. Öffnen Sie die Seite mit den Szenario-Details:

   1. Klicken Sie **[!UICONTROL linken Panel auf]** Registerkarte „Szenario“ und dann auf ein Szenario, zu dem Sie Details anzeigen möchten.

      Oder

      Wenn Sie an dem Szenario im [Der Szenario-Editor in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md) arbeiten, klicken Sie auf den Pfeil nach links ![](assets/exit-editing-arrow.png) in der oberen linken Ecke des Fensters.

1. Klicken Sie **[!UICONTROL rechts oben]** der Seite mit der rechten Maustaste auf „Optionen“.
1. Wählen Sie **[!UICONTROL Klonen]** aus.
1. (Optional) Geben Sie einen Namen für das neue Szenario ein.
1. (Optional) Aktivieren Sie **[!UICONTROL Halten Sie die Status aller neuen Module dieselben wie die duplizierten]**, um sicherzustellen, dass das kopierte Szenario auch Informationen zu den neuesten Datensätzen enthält, die vom ursprünglichen Szenario verarbeitet wurden.
1. Klicken Sie auf **[!UICONTROL Speichern]**, um das Szenario zu erstellen.

## Kopieren eines Szenarios mithilfe von Blueprints

Szenario-Blueprints stellen die Anordnung, Zuordnung und Feldwerte eines bestimmten Szenarios zu einem bestimmten Zeitpunkt dar. Sie können einen Szenario-Blueprint in eine JSON-Datei auf Ihrem Computer exportieren und sie dann beim Erstellen eines neuen Szenarios importieren. Aus einem Szenario-Blueprint importierte Szenarien können bearbeitet werden.

Ein Szenario-Blueprint stellt das gesamte Szenario dar. Wenn Sie nur bestimmte Module aus einem Szenario kopieren möchten, finden Sie weitere Informationen unter [Kopieren eines Moduls oder einer Gruppe von Modulen](#copy-a-module-or-a-group-of-modules) in diesem Artikel.

>[!NOTE]
>
>Informationen zu Blueprints im Zusammenhang mit [!DNL Adobe Workfront] finden Sie unter [Blueprints - Übersicht](../../administration-and-setup/blueprints/blueprints-overview.md).

### Szenario-Blueprint exportieren

1. Klicken Sie im Szenario auf das Menü **[!UICONTROL Mehr]** im Bereich Szenario-Einstellungen.
1. Klicken Sie **[!UICONTROL Blueprint exportieren]**.

   Eine JSON-Datei wird erstellt und auf Ihren Computer heruntergeladen. Sie können diese Datei in Ihrem [!DNL Downloads] Ordner finden.

### Blueprint importieren

>[!IMPORTANT]
>
>Wenn Sie eine Blueprint in ein vorhandenes Szenario importieren, ersetzt die Szenario-Blueprint das vorhandene Szenario. Sie können keine Blueprint an ein vorhandenes Szenario anhängen.

1. Beginnen Sie mit der Erstellung eines neuen Szenarios.
1. Klicken Sie im Szenario auf das Menü **[!UICONTROL Mehr]** im Bereich Szenario-Einstellungen.
1. Klicken Sie **[!UICONTROL Blueprint importieren]**.
1. Klicken Sie im angezeigten Dialogfeld auf **[!UICONTROL Durchsuchen]**
1. Navigieren Sie zu der Blueprint, die Sie importieren möchten, und klicken Sie auf **[!UICONTROL Öffnen]**.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Eine JSON-Datei wird erstellt und auf Ihren Computer heruntergeladen. Sie können diese Datei in Ihrem Ordner [!UICONTROL Downloads] finden.

## Kopieren und Wiederverwenden von Szenarien mithilfe von Vorlagen

Sie können Vorlagen als Ausgangspunkt für Ihre [!DNL Workfront Fusion] erstellen. Wenn Sie ein Szenario aus einer Vorlage erstellen, können Sie das Szenario ändern, ohne die Vorlage zu ändern. Feldwerte werden nicht in Vorlagen gespeichert.

Weitere Informationen zum Erstellen und Verwenden von Vorlagen finden Sie unter [Szenariovorlagen](../../workfront-fusion/scenarios/templates/fusion-templates.md).
