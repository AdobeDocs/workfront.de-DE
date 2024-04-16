---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Array-Funktionen in Adobe Workfront Fusion
description: Die folgenden Array-Funktionen sind im Bereich Adobe Workfront Fusion-Zuordnung verfügbar.
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
source-git-commit: 033a9f4aa1f191e5e3cabd0c0f232128fa6bce5d
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 1%

---

# Array-Funktionen in Adobe Workfront Fusion

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
   <p>Aktuell: Nein [!DNL Workfront Fusion] Lizenzanforderungen.</p> 
   <p>Oder</p> 
   <p>Veraltet: Beliebig </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Produkt</td>  
   <td> 
   <p>Neu:</p> <ul><li>[!UICONTROL Select] oder [!UICONTROL Prime] [!DNL Workfront] Plan: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] ist enthalten.</li></ul> 
   <p>Oder</p> 
   <p>Aktuell: Ihr Unternehmen muss Einkäufe tätigen [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Funktionen

* [join](#join-array-separator)
* [length](#length-array)
* [keys](#keys-object)
* [Slice](#slice-array-start-end)
* [merge](#merge-array1-array2)
* [enthält](#contains-array-value)
* [remove](#remove-array-value1-value2)
* [add](#add-array-value1-value2)
* [map](#map-complex-array-keykey-for-filteringpossible-values-for-filtering)
* [shuffle]
* [sort](#sort-array-order-key)
* [reverse](#reverse-array)
* [flatten](#flatten-array)
* [distinct](#distinct-array-key)
* [toCollection]
* [toArray](#toarray)
* [arrayDifference](#arraydifference-array1-array2-mode)
* [deduplizieren]

### [!UICONTROL join (array; separator)]

Verkettet alle Elemente eines Arrays mithilfe des angegebenen Trennzeichens zwischen den einzelnen Elementen in einer Zeichenfolge.

### [!UICONTROL length (Array)]

Gibt die Anzahl der Elemente in einem Array zurück.

### [!UICONTROL keys (object)]

Gibt ein Array der Eigenschaften eines angegebenen Objekts oder Arrays zurück.

### [!UICONTROL slice (array; start; [end])]

Gibt ein neues Array zurück, das nur ausgewählte Elemente enthält.

### [!UICONTROL merge (array1; array2; ...)]

Führt ein oder mehrere Arrays in einem Array zusammen.

### [!UICONTROL contains (array; value)]

Überprüft, ob ein Array den Wert enthält.

### [!UICONTROL remove (Array; Wert1; Wert2; ...)]

Entfernt die in den Parametern eines Arrays angegebenen Werte. Diese Funktion ist nur bei primitiven Arrays von Text oder Zahlen wirksam.

### [!UICONTROL add (Array; Wert1; Wert2; ...)]

Fügt in Parametern angegebene Werte zu einem Array hinzu und gibt dieses Array zurück.

### [!UICONTROL map (komplexes Array; Schlüssel)[Filterschlüssel];[mögliche Filterwerte])]

Gibt ein primitives Array zurück, das die Werte eines komplexen Arrays enthält. Diese Funktion ermöglicht das Filtern von Werten. Verwenden Sie unformatierte Variablennamen für Schlüssel.

>[!INFO]
>
>**Beispiele:**
>
>* `map(Emails[];email)`
>
>  Gibt ein primitives Array mit E-Mails zurück
>
>* `map(Emails[];email;label;work;home)`
>
>  Gibt ein primitives Array mit E-Mails zurück, deren Beschriftung gleich &quot;Arbeit&quot;oder &quot;Zuhause&quot;ist

Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)

### shuffle

### [!UICONTROL sort (Array); [bestellen]; [key])]

Sortiert Werte eines Arrays. Die gültigen Werte der `order` -Parameter sind:

* `asc`

  (Standard) - aufsteigende Reihenfolge: 1, 2, 3, ... für den Typ Zahl. A, B, C, a, b, c, ... für den Typ Text

* `desc`

  Absteigende Reihenfolge: ..., 3, 2, 1 für Typ &quot;Number&quot;. ..., c, b, a, C, B, A für den Typ Text.

* `asc ci`

  nicht von Schreibweise abhängig aufsteigende Reihenfolge: A, a, B, b, C, c, ... für den Typ Text.

* `desc ci`

  nicht von Schreibweise abhängig absteigende Reihenfolge: ..., C, c, B, b, A, a für den Typ Text.

Verwenden Sie die `key` -Parameter, um auf Eigenschaften in komplexen Objekten zuzugreifen.

Verwenden Sie unformatierte Variablennamen für Schlüssel.

Verwenden Sie Punktnotation, um auf verschachtelte Eigenschaften zuzugreifen.

Das erste Element in einem Array ist Index 1.

>[!INFO]
>
>**Beispiele:**
>
>* `sort(Contacts[];name)`
>
>    Sortiert eine Gruppe von Kontakten nach der Eigenschaft &quot;name&quot;in aufsteigender Standardreihenfolge
>
>* `sort(Contacts[];desc;name)`
>
>   Sortiert ein Kontaktarray nach der Eigenschaft &quot;name&quot;in absteigender Reihenfolge
>
>* `sort(Contacts[];asc ci;name)`
>
>    Sortiert eine Gruppe von Kontakten nach der Eigenschaft &quot;name&quot;in aufsteigender Reihenfolge, in der nicht zwischen Groß- und Kleinschreibung unterschieden wird
>
>* `sort(Emails[];sender.name)`
>
>    Sortiert ein Array von E-Mails nach der Eigenschaft &quot;sender.name&quot;

### [!UICONTROL reverse (Array)]

Das erste Element des Arrays wird zum letzten Element, das zweite zum letzten usw.

### [!UICONTROL flatten (Array)]

Erstellt ein neues Array mit allen Unter-Array-Elementen, die bis zur angegebenen Tiefe rekursiv darin verkettet sind.

### [!UICONTROL distinct (Array) [key])]

Entfernt Duplikate in einem Array. Verwenden Sie die[!UICONTROL key]&quot;-Argument, um auf Eigenschaften in komplexen Objekten zuzugreifen. Verwenden Sie Punktnotation, um auf verschachtelte Eigenschaften zuzugreifen. Das erste Element in einem Array ist Index 1.

>[!INFO]
>
>**Beispiel:** `distinct(Contacts[];name)`
>
>Entfernt Dubletten in einem Array von Kontakten durch Vergleich der Eigenschaft &quot;name&quot;

### toCollection

### toArray

Diese Funktion konvertiert eine Sammlung in ein Array von Schlüssel-Wert-Paaren.

>[!INFO]
>
>**Beispiele:**
>
>Aufgrund der Kollektion
>
>`{ key1: "value1", key2: "value2:}`
>
>Die Funktion
>
>`toArray({ key1: "value1", key2: "value2:})`
>
>Gibt das Array von Schlüssel-Wert-Paaren aus
>
>`[{ key1: "value1"}, { key2: "value2"}]`

### [!UICONTROL arrayDifference [array1, array2, mode]]

Gibt die Differenz zwischen zwei Arrays zurück.

Geben Sie für die `mode` -Parameter.

* `classic`: Gibt ein neues Array zurück, das alle Elemente von enthält `array1` , die nicht in `array2`.

* `symmetric`: Gibt ein Array von Elementen zurück, die nicht für beide Arrays gelten.

  Mit anderen Worten, die Funktion gibt ein Array zurück, das alle Elemente von `array1` , die nicht in `array2`und alle Elemente von `array2` , die nicht in `array1`.

  >[!INFO]
  >
  >**Beispiele:**
  >
  >Bei den folgenden Arrays:
  >
  >```
  >myArray = [1,2,3,4,5]
  >```
  >
  >```
  >yourArray = [3,4,5,6,7]
  >```
  >
  >* `arrayDifference [myArray, yourArray, classic]`
  >
  >    Rückgabe `[1,2]`
  >
  >* `arrayDifference [yourArray, myArray, classic]`
  >
  >    Rückgabe `[6,7]`
  >
  >* `arrayDifference [myArray, yourArray, symmetric]`
  >
  >    Rückgabe `[1,2,6,7]`

### deDuplicate

## Schlüsselwörter

### emptyarray
