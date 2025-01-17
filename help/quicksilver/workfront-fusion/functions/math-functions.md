---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Mathematische Funktionen in Adobe Workfront Fusion
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 8a3c7a89-62b5-45e9-b857-8beedd0e5af4
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 1%

---

# Mathematische Funktionen in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Mathematische Funktionen](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/mapping-panel/functions/math-functions.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

<!--Audited: 4/2024-->

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td>  
   <td> <p>Beliebig</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td>  
   <td> <p>Neu: [!UICONTROL Standard]</p><p>Oder</p><p>Aktuell: [!UICONTROL Work] oder höher</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Lizenz **</td>  
   <td> 
   <p>Aktuell: Keine [!DNL Workfront Fusion].</p> 
   <p>Oder</p> 
   <p>Legacy: Beliebig </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Produkt</td>  
   <td> 
   <p>Neu:</p> <ul><li>[!UICONTROL Select] oder [!UICONTROL Prime] [!DNL Workfront] Plan: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] kaufen.</li><li>[!UICONTROL Ultimate] [!DNL Workfront]: [!DNL Workfront Fusion] ist enthalten.</li></ul> 
   <p>Oder</p> 
   <p>Aktuell: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben.</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL average ([Array von Werten]) average(Wert1; [Wert2], …)]

Gibt den Durchschnittswert der numerischen Werte in einem bestimmten Array oder den Durchschnittswert einzeln eingegebener numerischer Werte zurück.

## [!UICONTROL CELL (Zahl)]

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

## [!UICONTROL FLOOR (number)]

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

## [!UICONTROL max ([Array von Werten]), max(Wert1;Wert2; …)]

Gibt die größte Zahl in einem angegebenen Array oder die größte Zahl einzeln eingegebener Zahlen zurück.

## [!UICONTROL min ([Array von Werten]), min(Wert1; Wert2; …)]

Gibt die kleinste Zahl in einem angegebenen Array oder die kleinste Zahl unter einzeln eingegebenen Zahlen zurück.

## [!UICONTROL round (number)]

Rundet einen numerischen Wert auf die nächste Ganzzahl.

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

## [!UICONTROL SUM ([Array von Werten]), SUM(Wert1; Wert2; …)]

Gibt die Summe der Werte in einem angegebenen Array oder die Summe der einzeln eingegebenen Zahlen zurück.

## [!UICONTROL parseNumber (Zahl; Dezimaltrennzeichen)]

Analysiert eine Zeichenfolge mit einer Zahl und gibt die Zahl zurück. Beispiel: parseNumber(1 756,456;,)

## [!UICONTROL formatNumber (Zahl; decimalPOINTS; [decimalSeparator]; [thousandsSeparator])]

Gibt eine Zahl im angeforderten Format zurück. Standardmäßig ist der Dezimalpunkt ein Komma (,) und das Tausendertrennzeichen ein Punkt (.).

>[!INFO]
>
>**Beispiel:**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>Gibt 123.456.789.000 zurück
