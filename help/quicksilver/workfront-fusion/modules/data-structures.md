---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Datenstrukturen in [!DNL Adobe Workfront Fusion]
description: Eine Datenstruktur ist ein Dokument, in dem das Format der an Adobe Workfront Fusion zu übertragenden Daten detailliert beschrieben wird. Basierend auf diesem Dokument kann der Szenario-Editor herausfinden, welches Modul welche Art von Daten zurückgibt oder erhält. Die Datenstrukturdokumente werden am häufigsten zum Serialisieren/Analysieren von Datenformaten wie JSON, XML, CSV und anderen verwendet.
author: Becky
feature: Workfront Fusion
exl-id: 35a7e906-7ca2-433d-87a9-bbb01babffb0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Datenstrukturen in [!DNL Adobe Workfront Fusion]

Eine Datenstruktur ist ein Dokument, in dem das Format der an [!DNL Adobe Workfront Fusion] zu übertragenden Daten detailliert beschrieben wird. Basierend auf diesem Dokument kann der Szenario-Editor herausfinden, welches Modul welche Art von Daten zurückgibt oder erhält. Die Datenstrukturdokumente werden am häufigsten zum Serialisieren/Analysieren von Datenformaten wie JSON, XML, CSV und anderen verwendet.

Sie können eine Datenstruktur erstellen, indem Sie auf die Schaltfläche [!UICONTROL Neue Datenstruktur erstellen] im Abschnitt [!UICONTROL Datenstruktur - Übersicht] oder in den Einstellungen des Moduls klicken, für das eine Datenstrukturspezifikation erforderlich ist.

Unterstützte Datentypen werden im Artikel [[!UICONTROL Typen von Modulen]](../../workfront-fusion/modules/module-types.md) beschrieben.

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

## Datenstrukturgenerator

Nicht immer müssen Datenstrukturen erstellt werden. Sie können es einfacher machen, indem Sie eine Vorlage aus unserem integrierten Generator verwenden. Durch die Bereitstellung eines Datenmusters erstellt der Generator automatisch eine Datenstruktur basierend auf der von Ihnen eingegebenen Stichprobe. Die erstellte Datenstruktur kann dann manuell geändert werden.

![](assets/data-structure-generator-350x341.jpg)
