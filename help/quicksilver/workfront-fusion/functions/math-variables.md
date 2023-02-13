---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Mathematische Variablen in [!DNL Adobe Workfront Fusion]
description: Die folgenden mathematischen Variablen sind in der [!DNL Adobe Workfront Fusion mapping] Bereich.
author: Becky
feature: Workfront Fusion
exl-id: 2fb561d2-0780-4fd6-87b3-5360a02df177
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---

# Mathematische Variablen in [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p><p>[!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL random]

Gibt eine Gleitkommazahl-Zufallszahl im Bereich aus [`0`,`1`] (einschließlich `0`, aber nicht `1`).

Verwenden Sie die folgende Formel, um eine Integer-Pseudo-Zufallszahl im Bereich zu generieren [`min`,`max`] (einschließlich `min` und `max`):

![](assets/math-variable-random-350x61.png)

```
{{floor(random * (1.max - 1.min + 1)) + 1.min}}
```
