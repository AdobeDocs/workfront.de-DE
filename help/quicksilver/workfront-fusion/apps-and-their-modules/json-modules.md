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

# [!UICONTROL JSON] Module

Die [!DNL Adobe Workfront Fusion] [!UICONTROL JSON] App stellt Module zur Verarbeitung von Daten im JSON-Format bereit, sodass [!DNL Adobe Workfront Fusion] kann mit dem Dateninhalt weiter arbeiten oder neue JSON-Inhalte erstellen.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Ältere Lizenzanforderungen: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderungen: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Ältere Produktanforderungen: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Parse JSON

* [Datenstruktur](#data-structure)
* [Sammlung vs. Array](#collection-vs-array)

### Datenstruktur

Die Datenstruktur beschreibt, wie die JSON-Daten organisiert sind, und ermöglicht die Zuordnung einzelner JSON-Elemente zu anderen Modulen in Ihrem Szenario. Wenn Sie die Datenstruktur nicht angeben, können Sie das Modul manuell ausführen und [!DNL Workfront Fusion] erstellt die Struktur aus der bereitgestellten JSON:

1. Fügen Sie die [!UICONTROL Parse JSON] zu einem Szenario.
1. Im **[!UICONTROL JSON-Zeichenfolge]** Geben Sie die JSON-Datei ein, aus der Sie eine Datenstruktur erstellen möchten.
1. Verbinden Sie keine anderen Module mit dem [!UICONTROL Parse JSON] -Modul hinzugefügt. weil [!DNL Workfront Fusion] die Struktur der JSON-Daten noch nicht kennt, ist es noch nicht möglich, Daten aus der [!UICONTROL Parse JSON] -Modul zu anderen Modulen in Ihrem Szenario.
1. Führen Sie das Szenario manuell aus. Dies ermöglicht die [!UICONTROL Parse JSON] -Modul, um die JSON-Struktur aus der von Ihnen bereitgestellten JSON zu identifizieren.
1. Sie können jetzt die folgenden Module verbinden. Die Elemente aus dem JSON-Modul &quot;Parse&quot;sind jetzt für die Zuordnung verfügbar.

Weitere Informationen finden Sie unter [Datenstrukturen in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-structures.md).

### Sammlung vs. Array

Wenn das JSON-Zeichenfolgenfeld eine Sammlung enthält `{ ... }`, ist die Ausgabe ein einzelnes Bundle, das die Elemente der Sammlung enthält.

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

Wenn das JSON-Zeichenfolgenfeld ein Array enthält `[ ... ]`, ist die Ausgabe eine Reihe von Bundles. Jedes Bundle enthält ein Element des Arrays.

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
 {
>       "name" : "Mike",
>       "ID" : 2
>   }
>]
>```
>
>![](assets/json-array.png)

## [!UICONTROL JSON] Module und ihre Felder

Bei der Konfiguration [!DNL JSON] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche JSON-Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Aggregieren zu JSON](#aggregate-to-json)
* [Konvertieren von JSON in XML](#convert-json-to-xml)
* [Parse JSON](#parse-json)
* [JSON erstellen](#create-json)
* [JSON transformieren](#transform-json)

### [!UICONTROL Aggregieren zu JSON]

Dieses Aggregatormodul aggregiert die Ausgabe eines vorherigen Moduls in JSON.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quellmodul] </td> 
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

### [!UICONTROL Konvertieren von JSON in XML]

Dieses Aktionsmodul konvertiert eine JSON-Zeichenfolge in XML.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON string] </td> 
   <td> <p>Geben Sie die JSON-Datei ein oder ordnen Sie sie zu, die Sie in XML konvertieren möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Parse JSON]

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
   <td role="rowheader">[!UICONTROL JSON string] </td> 
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
>**Beispiel:** Das folgende Beispiel zeigt, wie Datensätze aus [!DNL Google Sheets] im JSON-Format:
>
>1. Platzieren Sie die [!DNL Google Sheets] > [!UICONTROL Zeilen auswählen] -Modul in Ihrem Szenario verwenden, um die Daten abzurufen. Richten Sie das Modul ein, um Zeilen aus Ihrem [!DNL Google] Tabelle. Festlegen des &#x200B;**[!UICONTROL Maximale Anzahl an zurückgegebenen Zeilen]** auf eine kleine Zahl, jedoch zu Testzwecken größer als 1 (Beispiel: 3). Führen Sie die [!DNL Google Sheets] -Modul durch Rechtsklick darauf und Auswahl von &quot;**[!UICONTROL Nur dieses Modul ausführen]**.&quot; Überprüfen Sie die Ausgabe des Moduls.
>
1. Verbinden Sie die [!UICONTROL Array-Aggregator] -Modul nach [!DNL Google Sheets] -Modul. Wählen Sie in der Moduleinrichtung die [!DNL Google Sheets] -Modul im **[!UICONTROL Quellknoten]** -Feld. Lassen Sie die anderen Felder unverändert.
>
1. Verbinden [!UICONTROL JSON] > [!UICONTROL JSON erstellen] -Modul nach [!UICONTROL Array-Aggregator] -Modul. Die Einrichtung des Moduls erfordert eine Datenstruktur, die das JSON-Format beschreibt. Klicken **[!UICONTROL Hinzufügen]** , um die Einrichtung der Datenstruktur zu öffnen. Die einfachste Möglichkeit, diese Datenstruktur zu erstellen, besteht darin, sie automatisch aus einem JSON-Beispiel zu generieren. Klicken **[!UICONTROL Generator]** und fügen Sie Ihr JSON-Beispiel in die **[!UICONTROL Beispieldaten]** -Feld:
>
**Beispiel:**
>
>```
>{
>
>"books": [
>
>{
>
>"id": "ID",
>
>"title": "Title",
>
>"author": "Author"
>
>}
>
>]
>
>}
>```
>
1. Klicken Sie auf **[!UICONTROL Speichern]**. Die [!UICONTROL Spezifikation] -Feld in der Datenstruktur enthält nun die generierte Struktur.
1. Ändern Sie den Namen Ihrer Datenstruktur in einen spezifischeren Namen und klicken Sie auf **[!UICONTROL Speichern]**. Ein Feld, das dem Root-Array-Attribut entspricht, wird als zuordnbares Feld in der Einrichtung des JSON-Moduls angezeigt.
>
1. Klicken Sie auf **[!UICONTROL Zuordnung]** neben dem Feld klicken und die `Array[]` -Element aus der Array-Aggregator-Ausgabe an.
>
1. Klicken **[!UICONTROL OK]** zum Schließen der [!UICONTROL JSON] -Moduleinstellungen.
>
1. Öffnen Sie die Einrichtung der [!UICONTROL Array-Aggregator] -Modul. Ändern Sie die **[!UICONTROL Zielstruktur]** von [!UICONTROL Benutzerdefiniert] der [!UICONTROL JSON] -Feld des -Moduls, das dem Attribut des Stamm-Array entspricht. Zuordnen von Elementen aus [!DNL Google Sheets] in die entsprechenden Felder ein.
>
1. Klicken **[!UICONTROL OK]** zum Schließen der [!UICONTROL Array-Aggregator] -Moduleinstellungen.
>
1. Führen Sie das Szenario aus.
>
Die [!UICONTROL JSON] gibt das richtige JSON-Format aus.
>
1. Öffnen Sie die Einrichtung der [!DNL Google Sheets] und erhöhen Sie die [!UICONTROL Maximale Anzahl an zurückgegebenen Zeilen] -Zahl größer als die Anzahl der Zeilen in Ihrem Arbeitsblatt sein, um alle Daten zu verarbeiten.

## Fehlerbehebung

### Es können keine Daten aus dem [!UICONTROL Parse JSON] Modul

Vergewissern Sie sich, dass der JSON-Inhalt der [!UICONTROL Parse JSON] und dass die Datenstruktur korrekt definiert ist. Weitere Informationen finden Sie unter [Datendatensätze in JSON umwandeln](#transforming-data-records-to-json) in diesem Artikel.

### Das -Modul schlägt bei der Verwendung von bedingten Anweisungen in JSON fehl

Bei Verwendung von bedingten Anweisungen wie `if` Fügen Sie die Anführungszeichen in Ihre JSON-Datei außerhalb der bedingten Anweisung ein.

>[!INFO]
>
**Beispiel:**
>
![](assets/quotes-in-json-350x120.png)
