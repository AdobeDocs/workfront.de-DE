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
source-git-commit: a5130e551ad73717796bfac206d99799efc7987d
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---

# Allgemeine Funktionen in [!DNL Adobe Workfront Fusion]

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
   <p>Aktuelle Lizenzanforderungen: nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL get (Objekt oder Array; Pfad)]

Gibt den Wertpfad eines Objekts oder Arrays zurück. Verwenden Sie Punktnotation, um auf verschachtelte Objekte zuzugreifen. Das erste Element in einem Array ist Index 1.

>[!INFO]
>
>**Beispiele:**
>
>* `get( array ; 1 + 1 )`
>* `get( array ; 5.raw_name )`
>* `get( object ; raw_name )`
>* `get( object ; raw_name.sub_raw_name )`

## [!UICONTROL if (Ausdruck; Wert1; Wert2)]

Gibt die `value1` wenn der Ausdruck als &quot;true&quot;ausgewertet wird; gibt andernfalls den `value2`.

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

## [!UICONTROL ifempty (value1; value2)]

Gibt die `value1` Wenn dieser Wert nicht leer ist, wird andernfalls der Wert `value2`.

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

## [!UICONTROL switch (expression; value1; result1) [value2; result2; ...]; [else])]

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

## [!UICONTROL omit(object; key1) [key2; ...])]

Löst die angegebenen Schlüssel des Objekts aus und gibt den Rest zurück.

>[!INFO]
>
>**Beispiel:**
>
>`omit(` Benutzer `;` password `)`
>
>Gibt eine Sammlung der Benutzerinformationen zurück, mit Ausnahme des Kennworts.

## [!UICONTROL pick(object; key1) [key2; ...])]

Wählt nur die angegebenen Schlüssel aus dem Objekt aus.

>[!INFO]
>
>**Beispiel:**
>
>`pick(` Benutzer `;` password `;` email `)`
>
>Gibt nur eine Sammlung des Kennworts und der E-Mail-Adresse des Benutzers zurück.
