---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Auswählen, wo ein Trigger-Modul in Adobe Workfront Fusion gestartet wird
description: Einige Trigger-Module ermöglichen es Ihnen, das erste Bundle auszuwählen, aus dem das Abrufen von Bundles beginnen soll.
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 1%

---

# Festlegen, wo ein Trigger-Modul in [!DNL Adobe Workfront Fusion] beginnt

Einige Trigger-Module ermöglichen es Ihnen, das erste Bundle auszuwählen, aus dem das Abrufen von Bundles beginnen soll.

Sie können auch angeben, ob Sie alle Bundles oder nur die Bundles von nach einem bestimmten Datum abrufen möchten.

Weitere Informationen zu Trigger-Modulen finden Sie im Abschnitt [Trigger-Module](../../workfront-fusion/modules/module-types.md#triggers) im Artikel [Modultypen](../../workfront-fusion/modules/module-types.md).

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

## Festlegen, wo ein Trigger-Modul beginnt

1. Speichern Sie ein Trigger-Modul.

   Oder

   Ändern Sie die Einstellungen des Trigger-Moduls wie unter [Moduleinstellungen in [!UICONTROL Adobe Workfront Fusion konfigurieren]](../../workfront-fusion/modules/configure-a-modules-settings.md) beschrieben.

   Oder

   Klicken Sie mit der rechten Maustaste auf das Symbol für das Trigger-Modul im [!UICONTROL Szenario-Editor], wie unter [Szenario in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) erstellen beschrieben.

1. Wählen Sie eine Option im angezeigten Feld **[!UICONTROL Festlegen, wo der Start erfolgen soll]** aus.

   ![](assets/choose-where-to-start-350x346.jpg)

   Die angezeigten Optionen hängen von den Möglichkeiten eines bestimmten Dienstes ab. Sie können Folgendes umfassen:

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL Von jetzt an] (Standard)</td>
            <td>Ruft alle von jetzt an hinzugefügten oder aktualisierten Bundles ab (je nach Einstellungen).</td>
        </tr>
        <tr>
            <td>[!UICONTROL Von nach einem bestimmten Datum]</td>
            <td>Ruft alle Pakete ab, die (je nach Einstellungen) nach einem bestimmten Datum/einer bestimmten Uhrzeit hinzugefügt oder aktualisiert wurden</td>
        </tr>
        <tr>
            <td>[!UICONTROL Mit Kennung, die größer oder gleich einem bestimmten Wert ist]</td>
            <td>Ruft alle Bundles mit einer ID ab, die größer oder gleich einer angegebenen ID ist</td> 
        </tr>
        <tr>
            <td>[!UICONTROL Alle Pakete]</td>
            <td>Ruft alle verfügbaren Pakete ab</td>
        </tr>
        <tr>
            <td>[!UICONTROL Das erste Bundle auswählen]</td>
            <td>Ermöglicht die Auswahl des ersten Bundles, aus dem der Abruf von Bundles beginnen soll</td>
        </tr>
   </table>
