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

Eine Datenstruktur ist ein Dokument, in dem das Format der zu übertragenden Daten detailliert beschrieben wird. [!DNL Adobe Workfront Fusion]. Basierend auf diesem Dokument kann der Szenario-Editor herausfinden, welches Modul welche Daten zurückgibt oder empfängt. Die Datenstrukturdokumente werden meist zum Serialisieren/Parsen von Datenformaten wie JSON, XML, CSV und anderen verwendet.

Sie können eine Datenstruktur erstellen, indem Sie auf die [!UICONTROL Neue Datenstruktur erstellen] im [!UICONTROL Datenstruktur - Übersicht] oder in den Einstellungen des Moduls, für das eine Datenstrukturspezifikation erforderlich ist.

Die unterstützten Datentypen werden im Abschnitt [[!UICONTROL Modultypen]](../../workfront-fusion/modules/module-types.md) Artikel.

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
   <td>
   <p>Aktuelle Lizenzanforderungen: Nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Ältere Lizenzanforderungen: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderungen: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Ältere Produktanforderungen: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Datenstrukturgenerator

Datenstrukturen müssen nicht immer erstellt werden. Mithilfe einer Vorlage aus unserem integrierten Generator können Sie dies vereinfachen. Durch die Bereitstellung eines Datenbeispiels erstellt der Generator automatisch eine Datenstruktur, die auf dem von Ihnen eingegebenen Datenmuster basiert. Die erstellte Datenstruktur kann dann manuell geändert werden.

![](assets/data-structure-generator-350x341.jpg)
