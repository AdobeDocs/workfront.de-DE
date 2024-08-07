---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Kopieren von Modulen oder Szenarien in [!DNL Adobe Workfront Fusion]
description: Kopieren von Modulen oder Szenarien in [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 24e77a56-d676-4cf1-a801-1c328ffd0c4e
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 0%

---

# Kopieren von Modulen oder Szenarien in [!DNL Adobe Workfront Fusion]

Sie können Module, Gruppen von Modulen oder ganze Szenarien in [!DNL Adobe Workfront Fusion] kopieren. Mit dieser Funktion können Sie Szenarien oder Teile von Szenarien wiederverwenden, ohne sie erneut erstellen zu müssen

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

Sie müssen einem Szenario Module hinzufügen, bevor Sie sie kopieren können.

## Kopieren von Modulen oder Modulgruppen

Wenn Sie ein Modul kopieren, behält die Kopie alle Feldwerte und Einstellungen des ursprünglichen Moduls bei.

Sie können das Modul oder die Module in einen anderen Bereich desselben Szenarios oder in ein anderes Szenario einfügen.

Beachten Sie beim Einfügen von Modulen in ein anderes Szenario Folgendes.

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>If you paste the modules into another scenario, any fields that pull information from a module that you did not copy must be set to pull information from a module in the new scenario.</p> </li>
  -->

* Feldwerte, die Informationen von einem anderen Modul abrufen, das Sie nicht kopiert haben, können nicht mehr auf diese Informationen zugreifen. Sie müssen diese Felder so einstellen, dass Informationen aus dem neuen Szenario abgerufen werden.
* Wenn Sie die Module in ein Szenario einfügen, das einem anderen Team oder einer anderen Organisation gehört, müssen alle Verbindungen auf Verbindungen aktualisiert werden, die der Gruppe oder Organisation gehören, der das neue Szenario gehört.

### Module kopieren

Das Kopieren einer Modulgruppe ähnelt dem Kopieren eines einzelnen Moduls.

1. Klicken Sie mit der rechten Maustaste auf das Modul, das Sie kopieren möchten.

   >[!NOTE]
   >
   >Sie können mehr als ein Modul auswählen, indem Sie [!UICONTROL shift] gedrückt halten und auf die Module klicken, die Sie kopieren möchten. Beim Kopieren einer Modulgruppe werden auch alle Verbindungslinien, Filter oder Routing-Logiken zwischen ihnen kopiert.

1. Wählen Sie **[!UICONTROL Modul kopieren]** aus.
1. Verschieben Sie den Cursor in den Bereich des Szenarios, in dem Sie die Kopie des Szenarios erstellen möchten.
1. Klicken Sie mit der rechten Maustaste und wählen Sie **[!UICONTROL Einfügen]** aus.
1. Verbinden Sie die eingefügten Module mit dem Szenario, indem Sie sie an die gewünschte Position im Szenario ziehen.

   Sie können auch Tastaturbefehle zum Kopieren und Einfügen verwenden.

## Kopieren eines Szenarios durch Klonen

Durch das Klonen eines Szenarios wird eine Kopie des Szenarios erstellt, die Sie dann bearbeiten können.

1. Öffnen Sie die Detailseite des Szenarios:

   1. Klicken Sie im linken Bereich auf die Registerkarte **[!UICONTROL Szenario]** und dann auf ein Szenario, für das Sie Details anzeigen möchten.

      Oder

      Wenn Sie mit dem Szenario im [Szenario-Editor in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md) arbeiten, klicken Sie auf den linken Pfeil ![](assets/exit-editing-arrow.png) in der oberen linken Ecke des Fensters.

1. Klicken Sie mit der rechten Maustaste oben rechts auf der Seite auf **[!UICONTROL Optionen]** .
1. Wählen Sie **[!UICONTROL Klonen]** aus.
1. (Optional) Geben Sie einen Namen für das neue Szenario ein.
1. (Optional) Aktivieren Sie **[!UICONTROL Behalten Sie die Status aller neuen Module mit den Duplizierungsstatus bei]**, um sicherzustellen, dass das kopierte Szenario auch Informationen zu den neuesten Datensätzen enthält, die vom ursprünglichen Szenario verarbeitet wurden.
1. Klicken Sie auf **[!UICONTROL Speichern]** , um das Szenario zu erstellen.

## Kopieren eines Szenarios mithilfe von Blueprints

Szenario-Blueprints stellen die Anordnung, Zuordnung und Feldwerte eines bestimmten Szenarios zu einem bestimmten Zeitpunkt dar. Sie können einen Szenario-Blueprint in eine JSON-Datei auf Ihrem Computer exportieren und ihn dann beim Erstellen eines neuen Szenarios importieren. Aus einem Szenario-Blueprint importierte Szenarien können bearbeitet werden.

Ein Szenario-Blueprint stellt das gesamte Szenario dar. Wenn Sie nur bestimmte Module aus einem Szenario kopieren möchten, finden Sie weitere Informationen unter [Kopieren eines Moduls oder einer Modulgruppe](#copy-a-module-or-a-group-of-modules) in diesem Artikel.

>[!NOTE]
>
>Informationen zu Blueprints im Kontext von [!DNL Adobe Workfront] finden Sie unter [Blueprints - Übersicht](../../administration-and-setup/blueprints/blueprints-overview.md).

### Exportieren eines Szenario-Blueprints

1. Klicken Sie im Szenario auf das Menü **[!UICONTROL Mehr]** im Einstellungsbereich des Szenarios.
1. Klicken Sie auf **[!UICONTROL Blueprint exportieren]**.

   Eine JSON-Datei wird erstellt und auf Ihren Computer heruntergeladen. Sie können diese Datei in Ihrem Ordner &quot;[!DNL Downloads]&quot;finden.

### Importieren eines Blueprints

>[!IMPORTANT]
>
>Wenn Sie einen Blueprint in ein vorhandenes Szenario importieren, ersetzt der Szenario-Blueprint das vorhandene Szenario. Sie können einen Blueprint nicht an ein vorhandenes Szenario anhängen.

1. Beginnen Sie mit der Erstellung eines neuen Szenarios.
1. Klicken Sie im Szenario auf das Menü **[!UICONTROL Mehr]** im Einstellungsbereich des Szenarios.
1. Klicken Sie auf **[!UICONTROL Blueprint importieren]**.
1. Klicken Sie im angezeigten Dialogfeld auf **[!UICONTROL Durchsuchen]** .
1. Navigieren Sie zum Blueprint, den Sie importieren möchten, und klicken Sie auf **[!UICONTROL Öffnen]**.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Eine JSON-Datei wird erstellt und auf Ihren Computer heruntergeladen. Sie finden diese Datei im Ordner [!UICONTROL Downloads] .

## Kopieren und Wiederverwenden von Szenarien mithilfe von Vorlagen

Sie können Vorlagen als Ausgangspunkt für Ihre [!DNL Workfront Fusion]-Szenarien erstellen. Wenn Sie ein Szenario aus einer Vorlage erstellen, können Sie das Szenario ändern, ohne die Vorlage zu ändern. Feldwerte werden nicht in Vorlagen gespeichert.

Weitere Informationen zum Erstellen und Verwenden von Vorlagen finden Sie unter [Szenario-Vorlagen](../../workfront-fusion/scenarios/templates/fusion-templates.md).
