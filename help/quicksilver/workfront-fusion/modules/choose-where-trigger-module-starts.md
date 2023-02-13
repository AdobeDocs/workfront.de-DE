---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Auswählen, wo ein Trigger-Modul in Adobe Workfront Fusion gestartet wird
description: Einige Trigger-Module ermöglichen es Ihnen, das erste Bundle auszuwählen, aus dem das Abrufen von Bundles beginnen soll.
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Festlegen, wo ein Trigger-Modul beginnt [!DNL Adobe Workfront Fusion]

Einige Trigger-Module ermöglichen es Ihnen, das erste Bundle auszuwählen, aus dem das Abrufen von Bundles beginnen soll.

Sie können auch angeben, ob Sie alle Bundles oder nur die Bundles von nach einem bestimmten Datum abrufen möchten.

Weitere Informationen zu Trigger-Modulen finden Sie im Abschnitt . [Trigger-Module](../../workfront-fusion/modules/module-types.md#triggers) im Artikel [Modultypen](../../workfront-fusion/modules/module-types.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Festlegen, wo ein Trigger-Modul beginnt

1. Speichern Sie ein Trigger-Modul.

   Oder

   Ändern Sie die Einstellungen des Trigger-Moduls wie unter [Konfigurieren Sie die Einstellungen eines Moduls in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

   Oder

   Klicken Sie mit der rechten Maustaste auf das Symbol für das Trigger-Modul im [!UICONTROL Szenario-Editor]wie in [Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Wählen Sie eine Option im **[!UICONTROL Festlegen, wo der Start beginnen soll]** angezeigt.

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
            <td>[!UICONTROL Alle Bundles]</td>
            <td>Ruft alle verfügbaren Bundles ab</td>
        </tr>
        <tr>
            <td>[!UICONTROL Das erste Bundle auswählen]</td>
            <td>Ermöglicht die Auswahl des ersten Bundles, aus dem der Abruf von Bundles beginnen soll</td>
        </tr>
   </table>
