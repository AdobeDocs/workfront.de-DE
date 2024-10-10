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
source-git-commit: 5cd1cbd1976d5574668098be53daee780a9cc1fb
workflow-type: tm+mt
source-wordcount: '395'
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

## [!UICONTROL if (expression; value1; value2)]

Gibt die `value1` zurück, wenn der Ausdruck als &quot;true&quot;ausgewertet wird; sonst wird die `value2` zurückgegeben.

Verwenden Sie das Schlüsselwort `and` , um eine if -Anweisung zu erstellen, die nur dann einen Wert zurückgibt, wenn zwei oder mehr Ausdrücke als &quot;true&quot;ausgewertet werden.

Verwenden Sie die Operatoren `and` und `or`, um `if` -Anweisungen zu kombinieren.

![ und operator](/help/quicksilver/workfront-fusion/functions/assets/and-in-if-statement.png)

>[!INFO]
>
>**Beispiele:**
>
>* `if( 1 = 1 ; A ; B )`
>
>    Gibt eine
>
>* `if( 1 = 2 ; A ; B )`
>
>   Gibt B zurück
>
>* `if( 1 = 2 and 1 = 2 ; A ; B )`
>
>    Gibt B zurück
>   

## [!UICONTROL ifempty (value1; value2)]

Gibt den Wert `value1` zurück, wenn dieser Wert nicht leer ist. Andernfalls wird der Wert `value2` zurückgegeben.

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

## [!UICONTROL switch (expression; value1; result1; [value2; result2; ...]; [else])]

Wertet einen Wert (den so genannten Ausdruck) mit einer Werteliste aus; gibt das Ergebnis zurück, das dem ersten übereinstimmenden Wert entspricht. Um einen `else` -Wert einzuschließen, fügen Sie ihn nach dem letzten Ausdruck oder Wert hinzu.

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
>   Gibt 4 zurück
>   
>   In dieser Funktion ist 4 der Wert, der zurückgegeben wird, wenn keine Ausdrücke zutreffen (der Wert `else` ).

## [!UICONTROL omit(object; key1; [key2; ...])]

Löst die angegebenen Schlüssel des Objekts aus und gibt den Rest zurück.

>[!INFO]
>
>**Beispiel:**
>
>`omit(` Benutzer `;` Kennwort `)`
>
>Gibt eine Sammlung der Benutzerinformationen zurück, mit Ausnahme des Kennworts.

## [!UICONTROL pick(object; key1; [key2; ...])]

Wählt nur die angegebenen Schlüssel aus dem Objekt aus.

>[!INFO]
>
>**Beispiel:**
>
>`pick(` Benutzer `;` Kennwort `;` E-Mail `)`
>
>Gibt nur eine Sammlung des Kennworts und der E-Mail-Adresse des Benutzers zurück.

## mergeCollections(collection1 ; collection2)

Führt zwei Sammlungen durch Kombination ihrer Schlüssel-Wert-Paare zusammen. Wenn beide Sammlungen denselben Schlüssel enthalten, überschreibt der Wert aus der zweiten Sammlung diesen Wert aus der ersten Sammlung.

