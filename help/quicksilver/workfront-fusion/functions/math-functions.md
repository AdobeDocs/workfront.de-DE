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
source-git-commit: c325e16ba0cde4cd48fc3e40358a9ea9ed310659
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 1%

---

# Mathematische Funktionen in [!DNL Adobe Workfront Fusion]

<!--Audited: 4/2024-->

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td>  
   <td> <p>Alle</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td>  
   <td> <p>Neu: [!UICONTROL Standard]</p><p>Oder</p><p>Aktuell: [!UICONTROL Arbeit] oder höher</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td>  
   <td> 
   <p>Aktuell: Keine [!DNL Workfront Fusion] Lizenzanforderung.</p> 
   <p>Oder</p> 
   <p>Veraltet: Beliebig </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Produkt</td>  
   <td> 
   <p>Neu:</p> <ul><li>[!UICONTROL Select] oder [!UICONTROL Prime] [!DNL Workfront] Plan: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben.</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] ist enthalten.</li></ul> 
   <p>Oder</p> 
   <p>Aktuell: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] kaufen.</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Durchschnitt ([Array der Werte]) average(value1; [value2], ...)]

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

## [!UICONTROL max ([Array der Werte]), max(value1;value2; ...)]

Gibt die größte Zahl in einem angegebenen Array oder die größte Zahl unter den einzeln eingegebenen Zahlen zurück.

## [!UICONTROL min ([Array der Werte]), min(value1; value2; ...)]

Gibt die kleinste Zahl in einem angegebenen Array oder die kleinste Zahl unter den einzeln eingegebenen Zahlen zurück.

## [!UICONTROL round (number)]

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

## [!UICONTROL sum ([Array der Werte]), sum(value1; value2; ...)]

Gibt die Summe der Werte in einem angegebenen Array oder die Summe der einzelnen eingegebenen Zahlen zurück.

## [!UICONTROL parseNumber (Zahl; Dezimaltrennzeichen)]

Analysiert eine Zeichenfolge mit einer Zahl und gibt die Zahl zurück. Beispiel: parseNumber(1 756,456;,)

## [!UICONTROL formatNumber (Zahl; decimalPOINTS; [decimalSeparator]; [Tausendertrennzeichen])]

Gibt eine Zahl im angeforderten Format zurück. Standardmäßig ist der Dezimalpunkt ein Komma (,) und das Tausendertrennzeichen ein Punkt (.).

>[!INFO]
>
>**Beispiel:**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>Gibt 123 456 789 000 zurück
