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
source-git-commit: 5860e75d0a6521abbe082668749f78058fe7a114
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---

# Array-Funktionen in Adobe Workfront Fusion

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

## [!UICONTROL add (Array; Wert1; Wert2; ...)]

Fügt in Parametern angegebene Werte zu einem Array hinzu und gibt dieses Array zurück.

## [!UICONTROL contains (array; value)]

Überprüft, ob ein Array den Wert enthält.

## [!UICONTROL distinct (Array) [key])]

Entfernt Duplikate in einem Array. Verwenden Sie die[!UICONTROL key]&quot;-Argument, um auf Eigenschaften in komplexen Objekten zuzugreifen. Verwenden Sie Punktnotation, um auf verschachtelte Eigenschaften zuzugreifen. Das erste Element in einem Array ist Index 1.

>[!INFO]
>
>**Beispiel:** `distinct(Contacts[];name)`
>
>Entfernt Dubletten in einem Array von Kontakten durch Vergleich der Eigenschaft &quot;name&quot;

## [!UICONTROL flatten (Array)]

Erstellt ein neues Array mit allen Unter-Array-Elementen, die bis zur angegebenen Tiefe rekursiv darin verkettet sind.


## [!UICONTROL join (array; separator)]

Verkettet alle Elemente eines Arrays mithilfe des angegebenen Trennzeichens zwischen den einzelnen Elementen in einer Zeichenfolge.

## [!UICONTROL keys (object)]

Gibt ein Array der Eigenschaften eines angegebenen Objekts oder Arrays zurück.

## [!UICONTROL length (Array)]

Gibt die Anzahl der Elemente in einem Array zurück.

## [!UICONTROL map (komplexes Array; Schlüssel)[Filterschlüssel];[mögliche Filterwerte])]

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


## [!UICONTROL merge (array1; array2; ...)]

Führt ein oder mehrere Arrays in einem Array zusammen.

## [!UICONTROL remove (Array; Wert1; Wert2; ...)]

Entfernt die in den Parametern eines Arrays angegebenen Werte. Diese Funktion ist nur bei primitiven Arrays von Text oder Zahlen wirksam.

## [!UICONTROL reverse (Array)]

Das erste Element des Arrays wird zum letzten Element, das zweite zum letzten usw.

## [!UICONTROL slice (array; start; [end])]

Gibt ein neues Array zurück, das nur ausgewählte Elemente enthält.

## [!UICONTROL sort (Array); [bestellen]; [key])]

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

## [!UICONTROL arrayDifference [array1, array2, mode]]

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

## toArray

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
