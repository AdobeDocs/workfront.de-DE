---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Mathematische Funktionen in Adobe Workfront Fusion
description: Die folgenden mathematischen Funktionen sind im Bereich Adobe Workfront Fusion-Zuordnung verfügbar.
author: Becky
feature: Workfront Fusion
exl-id: 8a3c7a89-62b5-45e9-b857-8beedd0e5af4
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 1%

---

# Mathematische Funktionen in [!DNL Adobe Workfront Fusion]

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

## [!UICONTROL Durchschnitt ([Array von Werten]) average(value1; [value2], ...)]

Gibt den Durchschnittswert der numerischen Werte in einem bestimmten Array oder den Durchschnittswert der einzelnen eingegebenen numerischen Werte zurück.

## [!UICONTROL ceil (Zahl)]

Gibt die kleinste Ganzzahl zurück, die größer oder gleich einer angegebenen Zahl ist.

>[!INFO]
>
>**Beispiele:**
>
>* `ceil(` `1.2` `)`
   >
   >   Gibt 2 zurück
>
>* `ceil(` `4` `)`
   >
   >   Gibt 4 zurück


## [!UICONTROL floor (number)]

Gibt die größte Ganzzahl zurück, die kleiner oder gleich einer angegebenen Zahl ist.

>[!INFO]
>
>**Beispiele:**
>
>* `floor(` `1.2` `)`
   >
   >   Gibt 1 zurück
>
>* `floor(` `1.9` `)`
   >
   >   Gibt 1 zurück
>
>* `floor(` `4` `)`
   >
   >   Gibt 4 zurück


## [!UICONTROL formatNumber (Zahl) decimalPOINTS; [decimalSeparator]; [Tausendertrennzeichen])]

Gibt eine Zahl im angeforderten Format zurück. Standardmäßig ist der Dezimalpunkt ein Komma (,) und das Tausendertrennzeichen ein Punkt (.).

>[!INFO]
>
>**Beispiel:**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>Gibt 123.456.789.000 zurück

## [!UICONTROL max ([Array von Werten]), max(value1;value2; ...)]

Gibt die größte Zahl in einem angegebenen Array oder die größte Zahl unter den einzeln eingegebenen Zahlen zurück.

## [!UICONTROL min ([Array von Werten]), min(value1; Wert 2; ...)]

Gibt die kleinste Zahl in einem angegebenen Array oder die kleinste Zahl unter den einzeln eingegebenen Zahlen zurück.

## [!UICONTROL parseNumber (Zahl) Dezimaltrennzeichen)]

Analysiert eine Zeichenfolge mit einer Zahl und gibt die Zahl zurück. Beispiel: parseNumber(1 756,456;,)

## [!UICONTROL round (Zahl)]

Kürzt den numerischen Wert auf die nächste Ganzzahl.

>[!INFO]
>
>**Beispiele:**
>
>* `round(` `1.2` `)`
   >
   >   Gibt 1 zurück
>
>* `round(` `1.5` `)`
   >
   >   Gibt 2 zurück
>
>* `round(` `1.7` `)`
   >
   >   Gibt 2 zurück
> 
>* `round(` `2` `)`
   >
   >   Gibt 2 zurück


## [!UICONTROL sum ([Array von Werten]), sum(value1; Wert 2; ...)]

Gibt die Summe der Werte in einem angegebenen Array oder die Summe der einzelnen eingegebenen Zahlen zurück.
