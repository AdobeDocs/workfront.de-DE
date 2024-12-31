---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Array-Funktionen in Adobe Workfront Fusion
description: Die folgenden Array-Funktionen sind im Bedienfeld "Adobe Workfront Fusion-Zuordnung“ verfügbar.
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

## Funktionen

* [beitreten](#join-array-separator)
* [length](#length-array)
* [Schlüssel](#keys-object)
* [Scheibe](#slice-array-start-end)
* [Fusionieren](#merge-array1-array2)
* [enthält](#contains-array-value)
* [entfernen](#remove-array-value1-value2)
* [hinzufügen](#add-array-value1-value2)
* [kartieren](#map-complex-array-keykey-for-filteringpossible-values-for-filtering)
* [Mischen]
* [sortieren](#sort-array-order-key)
* [Rückwärtsgang](#reverse-array)
* [abflachen](#flatten-array)
* [distinct](#distinct-array-key)
* [toCollection]
* [toArray](#toarray)
* [arrayDifference](#arraydifference-array1-array2-mode)
* [deduplizieren]

### [!UICONTROL Join (Array;Trennzeichen)]

Verkettet alle Elemente eines Arrays in einer Zeichenfolge, wobei zwischen den einzelnen Elementen das angegebene Trennzeichen verwendet wird.

### [!UICONTROL length (Array)]

Gibt die Anzahl der Elemente in einem Array zurück.

### [!UICONTROL keys (Objekt)]

Gibt ein Array der Eigenschaften eines bestimmten Objekts oder Arrays zurück.

### [!UICONTROL slice (Array; Start; [end])]

Gibt ein neues Array zurück, das nur ausgewählte Elemente enthält.

### [!UICONTROL Zusammenführen (Array1; Array2; …)]

Führt ein oder mehrere Arrays in einem Array zusammen.

### [!UICONTROL Enthält (Array; Wert)]

Prüft, ob ein Array den Wert enthält.

### [!UICONTROL Entfernen (Array; Wert1; Wert2; …)]

Entfernt die in den Parametern eines Arrays angegebenen Werte. Diese Funktion ist nur bei primitiven Text- oder Zahlenfeldern wirksam.

### [!UICONTROL add (Array; Wert1; Wert2; …)]

Fügt die in den Parametern angegebenen Werte zu einem Array hinzu und gibt dieses Array zurück.

### [!UICONTROL Map (komplexes Array; Schlüssel; [Schlüssel zum Filtern]; [mögliche Werte zum Filtern])]

Gibt ein primitives Array mit Werten eines komplexen Arrays zurück. Diese Funktion ermöglicht das Filtern von Werten. Verwenden Sie unformatierte Variablennamen für Schlüssel.

>[!INFO]
>
>**Beispiele:**
>
>* `map(Emails[];email)`
>
>  Gibt ein primitives Array mit E-Mails zurück.
>
>* `map(Emails[];email;label;work;home)`
>
>  Gibt ein primitives Array mit E-Mails mit einer Kennzeichnung wie Arbeit oder Startseite zurück.

Weitere Informationen finden Sie unter [Zuordnen von Informationen von einem Modul zu einem anderen in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)

### schlurfen

### [!UICONTROL sort (Array; [order]; [key])]

Sortiert die Werte eines Arrays. Die gültigen Werte des `order` sind:

* `asc`

  (Standard) - aufsteigende Reihenfolge: 1, 2, 3, … für Typ Nummer. A, B, C, a, b, c, … für den Typ Text

* `desc`

  Absteigende Reihenfolge: …, 3, 2, 1 für Typ Nummer. …, c, b, a, C, B, A für den Typ Text.

* `asc ci`

  Aufsteigende Reihenfolge ohne Unterscheidung der Groß- und Kleinschreibung: A, a, B, b, C, c, … für den Typ Text.

* `desc ci`

  Groß-/Kleinschreibung wird nicht in absteigender Reihenfolge beachtet: …, C, c, B, b, A, a für Typ Text.

Verwenden Sie den `key`-Parameter, um auf Eigenschaften in komplexen Objekten zuzugreifen.

Verwenden Sie unformatierte Variablennamen für Schlüssel.

Verwenden Sie Punktnotation, um auf verschachtelte Eigenschaften zuzugreifen.

Das erste Element in einem Array ist Index 1.

>[!INFO]
>
>**Beispiele:**
>
>* `sort(Contacts[];name)`
>
>    Sortiert ein Array von Kontakten nach der Eigenschaft „name“ in aufsteigender Standardreihenfolge.
>
>* `sort(Contacts[];desc;name)`
>
>   Sortiert ein Array von Kontakten nach der Eigenschaft „name“ in absteigender Reihenfolge
>
>* `sort(Contacts[];asc ci;name)`
>
>    Sortiert ein Array von Kontakten nach der Eigenschaft „name“ in aufsteigender Reihenfolge ohne Berücksichtigung der Groß-/Kleinschreibung
>
>* `sort(Emails[];sender.name)`
>
>    Sortiert ein Array von E-Mails nach der Eigenschaft „sender.name“

### [!UICONTROL reverse (Array)]

Das erste Element des Arrays wird zum letzten Element, das zweite zum vorletzten Element usw.

### [!UICONTROL reduzieren (Array)]

Erstellt ein neues Array, in dem alle Unterarray-Elemente rekursiv bis zur angegebenen Tiefe verkettet sind.

### [!UICONTROL distinct (Array; [key])]

Entfernt Duplikate innerhalb eines Arrays. Verwenden Sie das [!UICONTROL key]-Argument, um auf Eigenschaften in komplexen Objekten zuzugreifen. Verwenden Sie Punktnotation, um auf verschachtelte Eigenschaften zuzugreifen. Das erste Element in einem Array ist Index 1.

>[!INFO]
>
>**Beispiel:** `distinct(Contacts[];name)`
>
>Entfernt Duplikate innerhalb eines Arrays von Kontakten, indem die Eigenschaft „name“ verglichen wird.

### toCollection

### toArray

Diese Funktion wandelt eine Sammlung in ein Array von Schlüssel-Wert-Paaren um.

>[!INFO]
>
>**Beispiele:**
>
>Angegeben an die Sammlung
>
>`{ key1: "value1", key2: "value2:}`
>
>Die Funktion
>
>`toArray({ key1: "value1", key2: "value2:})`
>
>Gibt das Array von Schlüssel-Wert-Paaren zurück.
>
>`[{ key1: "value1"}, { key2: "value2"}]`

### [!UICONTROL arrayDifference [array1, array2, mode]]

Gibt die Differenz zwischen zwei Arrays zurück.

Geben Sie einen der folgenden Werte für den `mode` ein.

* `classic`: Gibt ein neues Array zurück, das alle Elemente der `array1` enthält, die nicht in `array2` vorhanden sind.

* `symmetric`: Gibt ein Array von Elementen zurück, die nicht in beiden Arrays enthalten sind.

  Mit anderen Worten: Die Funktion gibt ein -Array zurück, das alle Elemente von `array1` enthält, die nicht in `array2` vorhanden sind, sowie alle Elemente von `array2`, die nicht in `array1` vorhanden sind.

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
  >    Gibt `[1,2]`
  >
  >* `arrayDifference [yourArray, myArray, classic]`
  >
  >    Gibt `[6,7]`
  >
  >* `arrayDifference [myArray, yourArray, symmetric]`
  >
  >    Gibt `[1,2,6,7]`

### deduplizieren

## Schlüsselwörter

### emptyarray
