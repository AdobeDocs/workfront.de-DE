---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Allgemeine Funktionen in Adobe Workfront Fusion
description: Die folgenden allgemeinen Funktionen sind im Bedienfeld Adobe Workfront Fusion-Zuordnung verfügbar.
author: Becky
feature: Workfront Fusion
exl-id: 74bfda4e-5690-4b8c-ac58-20cf261f188d
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 2%

---

# Allgemeine Funktionen in [!DNL Adobe Workfront Fusion]

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

## [!UICONTROL get (Objekt oder Array) path)]

Gibt den Wertpfad eines Objekts oder Arrays zurück. Verwenden Sie Punktnotation, um auf verschachtelte Objekte zuzugreifen. Das erste Element in einem Array ist Index 1.

>[!INFO]
>
>**Beispiele:**
>
>* `get( array ; 1 + 1 )`
>* `get( array ; 5.raw_name )`
>* `get( object ; raw_name )`
>* `get( object ; raw_name.sub_raw_name )`


## [!UICONTROL if (Ausdruck) value1; value2)]

Gibt die `value1` wenn der Ausdruck als &quot;true&quot;ausgewertet wird; Andernfalls wird `value2`.

>[!INFO]
>
>**Beispiele:**
>
>* `if( 1 = 1 ; A ; B )`
   >
   >    Gibt eine
>
>* `if( = 2 ; A ; B )`
   >
   >   Gibt B zurück


## [!UICONTROL ifempty (value1) value2)]

Gibt die `value1` wenn dieser Wert nicht leer ist; Andernfalls wird `value2`.

>[!INFO]
>
>**Beispiele:**
>
>* `ifempty(` `A` `;` `B` )
   >
   >   Gibt eine
>
>* `ifempty(` `unknown` `;` `B` )
   >
   >   Gibt B zurück
>
>* `ifempty(` `""` `;` `B` )
   >
   >   Gibt B zurück


## [!UICONTROL switch (Ausdruck) value1; result1; [Wert 2; result2; ...]; [else])]

Wertet einen Wert (den so genannten Ausdruck) mit einer Werteliste aus; gibt das Ergebnis zurück, das dem ersten übereinstimmenden Wert entspricht.

>[!INFO]
>
>**Beispiele:**
>
>* `switch( B ; A ; 1 ; B ; 2 ; C ; 3 )`
   >
   >   Gibt 2 zurück
>
>* `switch( C ; A ; 1 ; B ; 2 ; C ; 3 )`
   >
   >   Gibt 3 zurück
>
>* `switch( X ; A ; 1 ; B ; 2 ; C ; 3 ; 4 )`
>
>  Gibt 4 zurück

## [!UICONTROL omit(object) key1; [key2; ...])]

Löst die angegebenen Schlüssel des Objekts aus und gibt den Rest zurück.

>[!INFO]
>
>**Beispiel:**
>
>`omit(` Benutzer `;` password `)`
>
>Gibt eine Sammlung der Benutzerinformationen zurück, mit Ausnahme des Kennworts.

## [!UICONTROL pick(object) key1; [key2; ...])]

Wählt nur die angegebenen Schlüssel aus dem Objekt aus.

>[!INFO]
>
>**Beispiel:**
>
>`pick(` Benutzer `;` password `;` email `)`
>
>Gibt nur eine Sammlung des Kennworts und der E-Mail-Adresse des Benutzers zurück.
