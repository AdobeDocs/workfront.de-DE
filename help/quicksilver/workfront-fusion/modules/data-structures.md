---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Datenstrukturen in [!DNL Adobe Workfront Fusion]
description: Eine Datenstruktur ist ein Dokument, in dem das Format der an Adobe Workfront Fusion übertragenen Daten detailliert beschrieben wird. Basierend auf diesem Dokument kann der Szenario-Editor herausfinden, welches Modul welche Daten zurückgibt oder empfängt. Die Datenstrukturdokumente werden meist zum Serialisieren/Parsen von Datenformaten wie JSON, XML, CSV und anderen verwendet.
author: Becky
feature: Workfront Fusion
exl-id: 35a7e906-7ca2-433d-87a9-bbb01babffb0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Datenstrukturen in [!DNL Adobe Workfront Fusion]

Eine Datenstruktur ist ein Dokument, in dem das Format der an [!DNL Adobe Workfront Fusion] übertragenen Daten detailliert beschrieben wird. Basierend auf diesem Dokument kann der Szenario-Editor herausfinden, welches Modul welche Daten zurückgibt oder empfängt. Die Datenstrukturdokumente werden meist zum Serialisieren/Parsen von Datenformaten wie JSON, XML, CSV und anderen verwendet.

Sie können eine Datenstruktur erstellen, indem Sie im Abschnitt [!UICONTROL Datenstrukturübersicht] auf die Schaltfläche [!UICONTROL Neue Datenstruktur erstellen] klicken oder in den Einstellungen des Moduls, für das eine Datenstrukturspezifikation erforderlich ist.

Die unterstützten Datentypen werden im Artikel [[!UICONTROL Modultypen]](../../workfront-fusion/modules/module-types.md) beschrieben.

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

## Datenstrukturgenerator

Datenstrukturen müssen nicht immer erstellt werden. Mithilfe einer Vorlage aus unserem integrierten Generator können Sie dies vereinfachen. Durch die Bereitstellung eines Datenbeispiels erstellt der Generator automatisch eine Datenstruktur, die auf dem von Ihnen eingegebenen Datenmuster basiert. Die erstellte Datenstruktur kann dann manuell geändert werden.

![](assets/data-structure-generator-350x341.jpg)
