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
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '293'
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

## Datenstrukturgenerator

Datenstrukturen müssen nicht immer erstellt werden. Mithilfe einer Vorlage aus unserem integrierten Generator können Sie dies vereinfachen. Durch die Bereitstellung eines Datenbeispiels erstellt der Generator automatisch eine Datenstruktur, die auf dem von Ihnen eingegebenen Datenmuster basiert. Die erstellte Datenstruktur kann dann manuell geändert werden.

![](assets/data-structure-generator-350x341.jpg)
