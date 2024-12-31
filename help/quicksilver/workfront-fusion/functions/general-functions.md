---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Allgemeine Funktionen in Adobe Workfront Fusion
description: Die folgenden allgemeinen Funktionen sind im Bedienfeld "Adobe Workfront Fusion-Zuordnung“ verfügbar.
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

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] Lizenz**</td> 
   <td>
   <p>Aktuelle Lizenzanforderung: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!DNL Adobe Workfront] [!UICONTROL Select] oder [!UICONTROL Prime] verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu nutzen. [!DNL Workfront Fusion] ist im [!DNL Workfront] [!UICONTROL Ultimate] enthalten.</p>
   <p>Oder</p>
   <p>Legacy-Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL GET (Objekt oder Array; Pfad)]

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

Gibt die `value1` zurück, wenn der Ausdruck als „true“ ausgewertet wird. Andernfalls wird die `value2` zurückgegeben.

Um eine if-Anweisung zu erstellen, die einen Wert nur dann zurückgibt, wenn zwei oder mehr Ausdrücke als „true“ ausgewertet werden, verwenden Sie das `and`-Schlüsselwort.

Um `if` Anweisungen zu kombinieren, verwenden Sie die Operatoren `and` und `or` .

![UND-Operator](/help/quicksilver/workfront-fusion/functions/assets/and-in-if-statement.png)

>[!INFO]
>
>**Beispiele:**
>
>* `if( 1 = 1 ; A ; B )`
>
>    Gibt einen
>
>* `if( 1 = 2 ; A ; B )`
>
>   Gibt B zurück
>
>* `if( 1 = 2 and 1 = 2 ; A ; B )`
>
>    Gibt B zurück
>   

## [!UICONTROL IfEmpty (value1; value2)]

Gibt den `value1` zurück, wenn dieser Wert nicht leer ist. Andernfalls wird der `value2` zurückgegeben.

>[!INFO]
>
>**Beispiele:**
>
>* `ifempty(` `A` `;` `B` )
>
>   Gibt einen
>
>* `ifempty(` `unknown` `;` `B` )
>
>   Gibt B zurück
>
>* `ifempty(` `""` `;` `B` )
>
>   Gibt B zurück

## [!UICONTROL switch (Ausdruck; Wert1; Ergebnis1; [Wert2; Ergebnis2; …]; [else])]

Wertet einen Wert (den Ausdruck) anhand einer Werteliste aus und gibt das Ergebnis zurück, das dem ersten übereinstimmenden Wert entspricht. Um einen `else` Wert einzuschließen, fügen Sie ihn nach dem endgültigen Ausdruck oder Wert hinzu.

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
>   In dieser Funktion ist 4 der Wert, der zurückgegeben werden soll, wenn keine Ausdrücke gelten (der `else`).

## [!UICONTROL OMIT(Objekt; Schlüssel1; [Schlüssel2; …])]

Lässt die angegebenen Schlüssel des -Objekts aus und gibt den Rest zurück.

>[!INFO]
>
>**Beispiel:**
>
>`omit(` Benutzer `;` Passwort `)`
>
>Gibt eine Sammlung der Benutzerinformationen zurück, mit Ausnahme des Kennworts.

## [!UICONTROL PICK(Objekt; Schlüssel1; [Schlüssel2; …])]

Wählt nur die angegebenen Schlüssel aus dem Objekt aus.

>[!INFO]
>
>**Beispiel:**
>
>`pick(` Benutzer `;` Passwort `;` E-Mail-`)`
>
>Gibt nur eine Sammlung von Passwort und E-Mail-Adresse der Benutzenden zurück.

## mergeCollections(collection1 ; collection2)

Führt zwei Sammlungen durch Kombinieren ihrer Schlüssel-Wert-Paare zusammen. Wenn beide Sammlungen denselben Schlüssel enthalten, überschreibt der Wert aus der zweiten Sammlung diesen Wert aus der ersten Sammlung.

