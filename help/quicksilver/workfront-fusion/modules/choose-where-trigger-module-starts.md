---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Startpunkt eines Trigger-Moduls in Adobe Workfront Fusion auswählen
description: Bei einigen Trigger-Modulen können Sie das erste Bundle auswählen, von dem aus das Abrufen von Bundles beginnen soll.
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: 489ed23fe0d7945753b59810ff9da084bd3e92e4
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---

# Auswählen, wo ein Trigger-Modul in [!DNL Adobe Workfront Fusion] beginnt

Bei einigen Trigger-Modulen können Sie das erste Bundle auswählen, von dem aus das Abrufen von Bundles beginnen soll.

Sie können auch angeben, ob Sie alle Bundles oder nur die Bundles von nach einem bestimmten Datum abrufen möchten.

Trigger Trigger Weitere Informationen zu Modulen finden Sie im Abschnitt [Modulmodule](../../workfront-fusion/modules/module-types.md#triggers) im Artikel [Modultypen](../../workfront-fusion/modules/module-types.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
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

+++

## Startseite eines Trigger-Moduls auswählen

1. Speichern Sie ein Trigger-Modul.

   Oder

   Ändern Sie die Einstellungen des Moduls Trigger wie unter [Konfigurieren der Moduleinstellungen in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md) beschrieben.

   Oder

   Trigger Klicken Sie mit der rechten Maustaste auf das Symbol für das Szenario[!UICONTROL Modul im ], wie unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) beschrieben.

1. Wählen Sie eine Option im **[!UICONTROL Startpunkt auswählen]** aus.

   ![](assets/choose-where-to-start-350x346.jpg)

   Die angezeigten Optionen hängen von den Möglichkeiten eines bestimmten Service ab. Sie können Folgendes umfassen:

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL Von jetzt an] (Standard)</td>
            <td>Ruft alle (je nach Einstellungen) ab jetzt hinzugefügten oder aktualisierten Bundles ab</td>
        </tr>
        <tr>
            <td>[!UICONTROL Ab nach einem bestimmten Datum]</td>
            <td>Ruft alle hinzugefügten oder aktualisierten Pakete (je nach Einstellungen) nach einem bestimmten Datum/einer bestimmten Uhrzeit ab</td>
        </tr>
        <tr>
            <td>[!UICONTROL mit ID größer oder gleich einem bestimmten Wert]</td>
            <td>Ruft alle Bundles mit einer ID ab, die größer oder gleich einer angegebenen ID ist</td> 
        </tr>
        <tr>
            <td>[!UICONTROL Alle Bundles]</td>
            <td>Ruft alle verfügbaren Bundles ab</td>
        </tr>
        <tr>
            <td>[!UICONTROL Erstes Bundle auswählen]</td>
            <td>Ermöglicht die Auswahl des ersten Bundles, von dem aus der Abruf der Bundles beginnen soll</td>
        </tr>
   </table>
