---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: JSON-Module
description: Die Adobe Workfront Fusion JSON-App bietet Module zur Verarbeitung von Daten im JSON-Format, sodass Adobe Workfront Fusion mit dem Dateninhalt weiter arbeiten oder neue JSON-Inhalte erstellen kann.
author: Becky
feature: Workfront Fusion
exl-id: 60540608-9d2e-4e10-9fb2-5388dda64784
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1205'
ht-degree: 0%

---

# [!UICONTROL JSON] -Module

Die App [!DNL Adobe Workfront Fusion] [!UICONTROL JSON] stellt Module zur Verarbeitung von Daten im JSON-Format bereit, sodass [!DNL Adobe Workfront Fusion] mit dem Dateninhalt weiterarbeiten oder neue JSON-Inhalte erstellen kann.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
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

## Parse JSON

* [Datenstruktur](#data-structure)
* [Sammlung vs. Array](#collection-vs-array)

### Datenstruktur

Die Datenstruktur beschreibt, wie die JSON-Daten organisiert sind, und ermöglicht die Zuordnung einzelner JSON-Elemente zu anderen Modulen in Ihrem Szenario. Wenn Sie die Datenstruktur nicht angeben, können Sie das Modul manuell ausführen und [!DNL Workfront Fusion] erstellt die Struktur aus der bereitgestellten JSON:

1. Fügen Sie das Modul [!UICONTROL JSON analysieren] zu einem Szenario hinzu.
1. Geben Sie im Feld **[!UICONTROL JSON-Zeichenfolge]** die JSON-Datei ein, aus der Sie eine Datenstruktur erstellen möchten.
1. Verbinden Sie noch keine anderen Module mit dem Modul [!UICONTROL JSON analysieren] . Da [!DNL Workfront Fusion] die Struktur der JSON-Daten noch nicht kennt, ist es noch nicht möglich, Daten aus dem Modul [!UICONTROL JSON analysieren] anderen Modulen in Ihrem Szenario zuzuordnen.
1. Führen Sie das Szenario manuell aus. Dadurch kann das Modul [!UICONTROL JSON analysieren] die JSON-Struktur aus der von Ihnen bereitgestellten JSON identifizieren.
1. Sie können jetzt die folgenden Module verbinden. Die Elemente aus dem JSON-Modul &quot;Parse&quot;sind jetzt für die Zuordnung verfügbar.

Weitere Informationen finden Sie unter [Datenstrukturen in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-structures.md).

### Sammlung vs. Array

Wenn das Feld JSON-Zeichenfolge eine Sammlung `{ ... }` enthält, ist die Ausgabe ein einzelnes Bundle, das die Elemente der Sammlung enthält.

>[!INFO]
>
>**Beispiel:**
>
>```
>{
>       "name" : "Peter",
>
>    
   "ID" : 1
>}
>```
>
>![](assets/json-collection.png)

Wenn das JSON-Zeichenfolgenfeld ein Array `[ ... ]` enthält, ist die Ausgabe eine Reihe von Bundles. Jedes Bundle enthält ein Element des Arrays.

>[!INFO]
>
>**Beispiel:**
>
>```
>[
>   {
>       "name" : "Peter",
>       "ID" : 1
>   },
>
>  
> {
>       "name" : "Mike",
>       "ID" : 2
>   }
>]
>```
>
>![](assets/json-array.png)

## [!UICONTROL JSON] -Module und ihre Felder

Wenn Sie [!DNL JSON] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche JSON-Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Aggregat zu JSON](#aggregate-to-json)
* [JSON in XML konvertieren](#convert-json-to-xml)
* [JSON analysieren](#parse-json)
* [JSON erstellen](#create-json)
* [JSON transformieren](#transform-json)

### [!UICONTROL Aggregat zu JSON]

Dieses Aggregatormodul aggregiert die Ausgabe eines vorherigen Moduls in JSON.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Modul] </td> 
   <td> <p>Wählen Sie das Modul aus, das die Daten ausgibt, die Sie in JSON aggregieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datenstruktur]</td> 
   <td> <p>Wählen Sie die Datenstruktur aus, die Sie zum Erstellen von JSON verwenden möchten. Die Datenstruktur bestimmt, welche anderen Felder in diesem Modul verfügbar sind. Weitere Informationen finden Sie unter <a href="#data-structure" class="MCXref xref">Datenstruktur</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Einzug]</td> 
   <td> <p> Wählen Sie aus, ob Sie die JSON mit Registerkarten, zwei Leerzeichen oder vier Leerzeichen einbeziehen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Gruppe nach]</td> 
   <td>Definieren Sie einen Ausdruck, nach dem Sie die aggregierte Ausgabe gruppieren möchten. Dieser Ausdruck kann ein oder mehrere zugeordnete Elemente enthalten. Die aggregierten Daten werden dann mithilfe des Werts dieses Ausdrucks in Gruppen unterteilt. Jede Gruppe gibt als separates Bundle mit einem Schlüssel (dem ausgewerteten Ausdruck) und einem Wert (dem aggregierten Text) aus. Sie können den Schlüssel als Filter in nachfolgenden Modulen verwenden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verarbeitung nach einer leeren Aggregation stoppen]</td> 
   <td>Aktivieren Sie diese Option, um das Szenario zu stoppen, wenn keine Ergebnisse vorliegen.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL JSON in XML konvertieren]

Dieses Aktionsmodul konvertiert eine JSON-Zeichenfolge in XML.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON-Zeichenfolge] </td> 
   <td> <p>Geben Sie die JSON-Datei ein oder ordnen Sie sie zu, die Sie in XML konvertieren möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL JSON analysieren]

Dieses Aktionsmodul analysiert eine JSON-Zeichenfolge in einer Datenstruktur, mit der Sie auf die Daten in der JSON-Zeichenfolge zugreifen können.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datenstruktur]</td> 
   <td> <p>Wählen Sie die Datenstruktur aus, die Sie zum Erstellen von JSON verwenden möchten. Weitere Informationen finden Sie unter <a href="#data-structure" class="MCXref xref">Datenstruktur</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON-Zeichenfolge] </td> 
   <td> <p>Geben Sie die JSON-Datei ein oder ordnen Sie sie zu, die Sie analysieren möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL JSON erstellen]

Dieses Aktionsmodul erstellt JSON aus einer Datenstruktur.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">Datenstruktur</td> 
   <td> <p>Wählen Sie die Datenstruktur aus, die Sie zum Erstellen von JSON verwenden möchten. Weitere Informationen finden Sie unter <a href="#data-structure" class="MCXref xref">Datenstruktur</a> in diesem Artikel.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL JSON transformieren]

Dieses Aktionsmodul wandelt ein Objekt in eine JSON-Zeichenfolge um.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Objekt]</td> 
   <td> <p>Geben Sie das Objekt ein oder ordnen Sie es zu, das Sie in JSON umwandeln möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Datendatensätze in JSON umwandeln

>[!INFO]
>
>**Beispiel:** Das folgende Beispiel zeigt, wie Datendatensätze aus [!DNL Google Sheets] in das JSON-Format umgewandelt werden:
>
>1. Platzieren Sie das Modul [!DNL Google Sheets] > [!UICONTROL Zeilen auswählen] in Ihrem Szenario, um die Daten abzurufen. Richten Sie das -Modul ein, um Zeilen aus Ihrer [!DNL Google] -Tabelle abzurufen. Stellen Sie die &#x200B;**[!UICONTROL Maximale Anzahl der zurückgegebenen Zeilen]** auf eine kleine Zahl ein, die zu Testzwecken jedoch größer als eine ist (Beispiel: 3). Führen Sie das Modul [!DNL Google Sheets] aus, indem Sie mit der rechten Maustaste darauf klicken und &quot;**[!UICONTROL Nur dieses Modul ausführen]**&quot;auswählen. Überprüfen Sie die Ausgabe des Moduls.
>
1. Verbinden Sie das Modul [!UICONTROL Array Aggregator] nach dem Modul [!DNL Google Sheets] . Wählen Sie im Setup des Moduls das Modul [!DNL Google Sheets] im Feld **[!UICONTROL Source node]** aus. Lassen Sie die anderen Felder unverändert.
>
1. Verbinden Sie das Modul [!UICONTROL JSON] > [!UICONTROL JSON] nach dem Modul [!UICONTROL Array Aggregator] . Die Einrichtung des Moduls erfordert eine Datenstruktur, die das JSON-Format beschreibt. Klicken Sie auf **[!UICONTROL Hinzufügen]** , um die Einrichtung der Datenstruktur zu öffnen. Die einfachste Möglichkeit, diese Datenstruktur zu erstellen, besteht darin, sie automatisch aus einem JSON-Beispiel zu generieren. Klicken Sie auf **[!UICONTROL Generator]** und fügen Sie Ihr JSON-Beispiel in das Feld **[!UICONTROL Beispieldaten]** ein:
>
**Beispiel:**
>   
```
{

"books": [

{

"id": "ID",

"title": "Title",

"author": "Author"

}

]

}
```
>
1. Klicken Sie auf **[!UICONTROL Speichern]**. Das Feld [!UICONTROL Spezifikation] in der Datenstruktur enthält jetzt die generierte Struktur.
1. Ändern Sie den Namen Ihrer Datenstruktur in etwas spezifischeres und klicken Sie auf **[!UICONTROL Speichern]**. Ein Feld, das dem Root-Array-Attribut entspricht, wird als zuordnbares Feld in der Einrichtung des JSON-Moduls angezeigt.
>
1. Klicken Sie auf die Schaltfläche **[!UICONTROL Zuordnung]** neben dem Feld und ordnen Sie ihm das Element `Array[]` aus der Array-Aggregatorausgabe zu.
>
1. Klicken Sie auf **[!UICONTROL OK]** , um das Setup des Moduls [!UICONTROL JSON] zu schließen.
>
1. Öffnen Sie die Einrichtung des Moduls [!UICONTROL Array Aggregator] . Ändern Sie die **[!UICONTROL Zielstruktur]** von [!UICONTROL Benutzerdefiniert] in das Feld des Moduls [!UICONTROL JSON] , das dem Stammarray-Attribut entspricht. Ordnen Sie Elemente aus dem Modul [!DNL Google Sheets] den entsprechenden Feldern zu.
>
1. Klicken Sie auf **[!UICONTROL OK]** , um das Setup des [!UICONTROL Array Aggregator] -Moduls zu schließen.
>
1. Führen Sie das Szenario aus.
>
Das Modul [!UICONTROL JSON] gibt das richtige JSON-Format aus.
>
1. Öffnen Sie die Einrichtung des Moduls [!DNL Google Sheets] und erhöhen Sie die Zahl der maximal zurückgegebenen Zeilen] auf die Anzahl der Zeilen in Ihrer Tabelle, um alle Daten zu verarbeiten.[!UICONTROL 

## Fehlerbehebung

### Daten des Moduls [!UICONTROL Parse JSON] können nicht zugeordnet werden

Stellen Sie sicher, dass der JSON-Inhalt ordnungsgemäß dem Modul [!UICONTROL JSON analysieren] zugeordnet ist und dass die Datenstruktur korrekt definiert ist. Weitere Informationen finden Sie unter [Transformieren von Datendatensätzen in JSON](#transforming-data-records-to-json) in diesem Artikel.

### Das -Modul schlägt bei der Verwendung von bedingten Anweisungen in JSON fehl

Bei Verwendung von bedingten Anweisungen wie `if` in Ihrer JSON platzieren Sie die Anführungszeichen außerhalb der bedingten Anweisung.

>[!INFO]
>
**Beispiel:**
>
![](assets/quotes-in-json-350x120.png)
