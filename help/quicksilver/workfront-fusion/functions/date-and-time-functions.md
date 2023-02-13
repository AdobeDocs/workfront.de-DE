---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Datums- und Uhrzeitfunktionen in Adobe Workfront Fusion
description: Die folgenden Datums- und Uhrzeitfunktionen sind im Zuordnungsfenster von Adobe Workfront Fusion verfügbar.
author: Becky
feature: Workfront Fusion
exl-id: 76c63afc-4bb6-4895-9bba-6b3913ecbcf6
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '1867'
ht-degree: 1%

---

# Datums- und Uhrzeitfunktionen in [!DNL Adobe Workfront Fusion]

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

## [!UICONTROL formatDate (date; Format; [timezone])]

Verwenden Sie diese Funktion, wenn Sie einen Datumswert haben, z. B. `12-10-2021 20:30`, die Sie als Textwert formatieren möchten, z. B. `Dec 10, 2021 8:30 PM`.

Dies ist beispielsweise nützlich, wenn Sie das Datumsformat einer App oder eines Webdiensts in das einer verbundenen App oder eines Webdiensts ändern müssen.

Weitere Informationen finden Sie unter [Datum](../../workfront-fusion/mapping/item-data-types.md#date) und [Text](../../workfront-fusion/mapping/item-data-types.md#text) im Artikel [Elementdatentypen in Adobe Workfront Fusion](../../workfront-fusion/mapping/item-data-types.md).

### Parameter

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Parameter</th> 
   <th>Erwarteter Datentyp* </th> 
   <th>Funktion</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Datum] </td> 
   <td>Datum </td> 
   <td> <p>Konvertiert einen Datumswert in einen Textwert. </p> </td> 
  </tr> 
  <tr> 
   <td>Format [!UICONTROL] </td> 
   <td>Text </td> 
   <td> <p>Ermöglicht die Angabe eines Formats mithilfe von Token zur Datums-/Uhrzeitformatierung. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md" class="MCXref xref">Token für die Datums- und Uhrzeitformatierung in [!DNL Adobe Workfront Fusion]</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>DD.MM.YYYY HH:mm</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL timezone] </td> 
   <td>Text </td> 
   <td> <p>(Optional) Hier können Sie die Zeitzone angeben, die für die Konvertierung verwendet wird. </p> <p>Eine Liste der erkannten Zeitzonen finden Sie in der Spalte "Name der TZ-Datenbank"in der Wikipedia <a href="https://en.wikipedia.org/wiki/List_of_tz_database_time_zones">Liste der Zeitzonen der tz-Datenbank</a>. Nur die in dieser Spalte aufgeführten Werte werden von der Funktion als gültige Zeitzone erkannt. Jeder andere Wert wird ignoriert und stattdessen die in Ihrem Profil angegebene Zeitzone Szenarios verwendet. Weitere Informationen finden Sie im Artikel <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">Profileinstellungen ändern in [!DNL Adobe Workfront Fusion]</a>.</p> <p>Wenn Sie diesen Parameter weglassen, wird die in Ihren Profileinstellungen angegebene Zeitzone Szenarios angewendet. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>Europe/Prague</code>, <code>UTC</code></p> </td> 
  </tr> 
 </tbody> 
</table>

Wenn ein anderer Typ angegeben wird, wird die Typerzwingung angewendet. Weitere Informationen finden Sie unter [Typenkonvertierung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

### Rückgabewert und Typ

Die `formatDate` gibt eine Textdarstellung des angegebenen Datumswerts entsprechend dem angegebenen Format und der angegebenen Zeitzone zurück. Der Datentyp ist Text.

>[!INFO]
>
>**Beispiele:** Sowohl das Szenario als auch die Web-Zeitzone wurden auf `Europe/Prague` in diesen Beispielen.
>
>![](assets/date&time-functions-examples-350x61.png)
>
>* `formatDate(1. Date created;MM/DD/YYYY)`
   >
   >    Gibt 10.01.2018 zurück
>
>* `formatDate(1. Date created; YYYY-MM-DD hh:mm A)`
   >
   >   Gibt 2018-10-01 09:32 Uhr zurück
>
>* `formatDate(1. Date created;DD.MM.YYYY HH:mm;UTC)`
   >
   >    Gibt 01.10.2018 07:32 zurück
>
>* `formatDate(now;DD.MM.YYYY HH:mm)`
   >
   >    Gibt 19.03.2019 15:30 Uhr zurück


## [!UICONTROL parseDate (text; Format; [timezone])]

Verwenden Sie diese Funktion, wenn Sie einen Textwert haben, der ein Datum darstellt (z. B. `12-10-2019 20:30` oder `Aug 18, 2019 10:00 AM`) und Sie möchten sie in einen Datumswert (eine binäre, maschinenlesbare Darstellung) konvertieren (analysieren). Weitere Informationen finden Sie unter [Datum](../../workfront-fusion/mapping/item-data-types.md#date) und [Text](../../workfront-fusion/mapping/item-data-types.md#text) im Artikel [Elementdatentypen in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

### Parameter

Die zweite Spalte zeigt den erwarteten Typ an. Wenn ein anderer Typ angegeben wird, wird die Typerzwingung angewendet. Weitere Informationen finden Sie unter [Typenkonvertierung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Parameter</th> 
   <th>Erwarteter Datentyp* </th> 
   <th>Funktion</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td>Text </td> 
   <td> <p>Konvertiert einen Datumswert in einen Textwert. </p> </td> 
  </tr> 
  <tr> 
   <td>Format [!UICONTROL] </td> 
   <td>Text </td> 
   <td> <p>Ermöglicht die Angabe eines Formats mithilfe von Token zur Datums-/Uhrzeitformatierung. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md" class="MCXref xref">Token für die Datums- und Uhrzeitformatierung in Adobe Workfront Fusion</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>DD.MM.YYYY HH:mm</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL timezone] </td> 
   <td>Text </td> 
   <td> <p>(Optional) Hier können Sie die Zeitzone angeben, die für die Konvertierung verwendet wird. </p> <p>Eine Liste der erkannten Zeitzonen finden Sie in der Spalte "Name der TZ-Datenbank"in der Wikipedia <a href="https://en.wikipedia.org/wiki/List_of_tz_database_time_zones">Liste der Zeitzonen der tz-Datenbank</a>. Nur die in dieser Spalte aufgeführten Werte werden von der Funktion als gültige Zeitzone erkannt. Jeder andere Wert wird ignoriert und stattdessen die in Ihrem Profil angegebene Zeitzone Szenarios verwendet. Weitere Informationen finden Sie im Artikel <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">Profileinstellungen in Adobe Workfront Fusion ändern</a>.</p> <p>Wenn Sie diesen Parameter weglassen, wird die in Ihren Profileinstellungen angegebene Zeitzone Szenarios angewendet.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>Europe/Prague</code>, <code>UTC</code></p> </td> 
  </tr> 
 </tbody> 
</table>

Wenn ein anderer Typ angegeben wird, wird die Typerzwingung angewendet. Weitere Informationen finden Sie unter [Typenkonvertierung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

### Rückgabewert und Typ

Diese Funktion konvertiert eine Textzeichenfolge entsprechend dem angegebenen Format und der angegebenen Zeitzone in ein Datum. Der Datentyp des Werts ist Datum.

>[!INFO]
>
>**Beispiele:** In den folgenden Beispielen wird der zurückgegebene Datumswert gemäß ISO 8601 ausgedrückt, der Datentyp des Ergebnisses ist jedoch Datum.
>
>* `parseDate(2016-12-28;YYYY-MM-DD)`
   >
   >    Gibt 2016-12-28T00 zurück:00:00.000Z
>
>* `parseDate(2016-12-28 16:03;YYYY-MM-DD HH:mm)`
   >
   >    Gibt 2016-12-28T16 zurück:03:00.000Z
>
>* `parseDate(2016-12-28 04:03 pm; YYYY-MM-DD hh:mm a)`
   >
   >    Gibt 2016-12-28T16 zurück:03:06.000Z
>
>* `parseDate(1482940986;X)`
>
>  Gibt 2016-12-28T16 zurück:03:06.000Z

## [!UICONTROL addDays (date; number)] {#adddays-date-number}

Gibt infolge des Hinzufügens einer bestimmten Anzahl von Tagen zu einem Datum ein neues Datum zurück. Um Tage zu subtrahieren, geben Sie eine negative Zahl ein.

>[!INFO]
>
>**Beispiele:**
>
>* `addDays(2016-12-08T15:55:57.536Z;2)`
   >
   >    Gibt 2016-12-10T15 zurück:55:57.536 Z
>
>* `addDays(2016-12-08T15:55:57.536Z;-2)`
   >
   >    Gibt 2016-12-6T15 zurück:55:57.536 Z


## [!UICONTROL addHours (date; number)] {#addhours-date-number}

Gibt infolge des Hinzufügens einer bestimmten Anzahl von Stunden zu einem Datum ein neues Datum zurück. Geben Sie eine negative Zahl ein, um Stunden zu subtrahieren.

>[!INFO]
>
>**Beispiele:**
>
>* `addHours(2016-12-08T15:55:57.536Z; 2)`
   >
   >    Gibt 2016-12-08T17 zurück:55:57.536 Z
>
>* `addHours(2016-12-08T15:55:57.536Z;-2)`
   >
   >    Gibt 2016-12-08T13 zurück:55:57.536 Z


## [!UICONTROL addMinutes (date; number)] {#addminutes-date-number}

Gibt infolge des Hinzufügens einer bestimmten Anzahl von Minuten zu einem Datum ein neues Datum zurück. Geben Sie eine negative Zahl ein, um Minuten zu subtrahieren.

>[!INFO]
>
>**Beispiele:**
>
>* `addMinutes(2016-12-08T15:55:57.536Z;2)`
   >
   >    Gibt 2016-12-08T15 zurück:57:57.536 Z
>
>* `addMinutes(2016-12-08T15:55:57.536Z;-2)`
   >
   >    Gibt 2016-12-08T15 zurück:53:57.536 Z


## [!UICONTROL addMonths (date; number)] {#addseconds-date-number}

Gibt infolge des Hinzufügens einer bestimmten Anzahl von Monaten zu einem Datum ein neues Datum zurück. Um Monate abzuziehen, geben Sie eine negative Zahl ein.

>[!INFO]
>
>**Beispiele:**
>
>* `addMonths(2016-08-08T15:55:57.536Z;2)`
   >
   >    Gibt 2016-10-08T15 zurück:55:57.536 Z
>
>* `addMonths(2016-08-08T15:55:57.536Z;-2)`
   >
   >    Gibt 2016-06-08T15 zurück:55:57.536 Z


## [!UICONTROL addSeconds (date; number)]

Gibt infolge des Hinzufügens einer bestimmten Anzahl von Sekunden zu einem Datum ein neues Datum zurück. Geben Sie eine negative Zahl ein, um Sekunden abzuziehen.

>[!INFO]
>
>**Beispiele:**
>
>* `addSeconds(2016-12-08T15:55:57.536Z;2)`
   >
   >   Gibt 2016-12-08T15 zurück:55:59.536 Z
>
>* `addSeconds(2016-12-08T15:55:57.536Z;-2)`
   >
   >   Gibt 2016-12-08T15 zurück:55:55.536 Z


## [!UICONTROL addYears (date; number)]

Gibt infolge des Hinzufügens einer bestimmten Anzahl von Jahren zu einem Datum ein neues Datum zurück. Um Jahre abzuziehen, geben Sie eine negative Zahl ein.

>[!INFO]
>
>**Beispiele:**
>
>* `addYears(2016-08-08T15:55:57.536Z;2)`
   >
   >    Gibt 2018-08-08T15 zurück:55:57.536 Z
>
>* `addYears(2016-12-08T15:55:57.536Z; -2)`
   >
   >    Gibt 2014-08-08T15 zurück:55:57.536 Z


## [!UICONTROL setSecond (date; number)]

Diese Funktion gibt ein neues Datum mit den in den Parametern angegebenen Sekunden zurück.

Geben Sie eine Zahl zwischen 0 und 59 an. Wenn die Zahl außerhalb dieses Bereichs liegt, gibt die Funktion eine Sekunde aus der vorherigen Minute (für eine negative Zahl) oder aus der darauf folgenden Minute (für eine positive Zahl) zurück.

Wenn Sie eine Zahl außerhalb des Bereichs angeben müssen, empfehlen wir,[!UICONTROL  addSeconds], wie oben im Abschnitt beschrieben [addSeconds (date; number)](#addseconds-date-number).

>[!INFO]
>
>**Beispiele:**
>
>* `setSecond(2015-10-07T11:36:39.138Z;10)`
   >
   >    Gibt 2015-10-07T11 zurück:36:10.138 Z
>
>* `setSecond(2015-10-07T11:36:39.138Z; 6)`
   >
   >    Gibt 2015-10-07T11 zurück:37:01.138 Z


## [!UICONTROL setMinute (Datum) number)]

Diese Funktion gibt ein neues Datum mit den in den Parametern angegebenen Minuten zurück.

Geben Sie eine Zahl zwischen 0 und 59 an. Wenn die Zahl außerhalb dieses Bereichs liegt, gibt die Funktion eine Minute von der vorherigen Stunde (für eine negative Zahl) oder der nachfolgenden Stunde (für eine positive Zahl) zurück.

Wenn Sie eine Zahl außerhalb des Bereichs angeben müssen, empfehlen wir die Verwendung von addMinutes, wie oben unter [addMinutes (date; number)](#addminutes-date-number).

>[!INFO]
>
>**Beispiele:**
>
>* `setMinute(2015-10-07T11:36:39.138Z;10)`
   >
   >    Gibt 2015-10-07T11 zurück:10:39.138 Z
>
>* `setMinute(2015-10-07T11:36:39.138Z;61)`
   >
   >    Gibt 2015-10-07T12 zurück:01:39.138 Z


## [!UICONTROL setHour (date; number)]

Diese Funktion gibt ein neues Datum mit der in den Parametern angegebenen Stunde zurück.

Geben Sie eine Zahl zwischen 0 und 23 an. Wenn die Zahl außerhalb dieses Bereichs liegt, gibt die Funktion eine Stunde vom vorherigen Tag (für eine negative Zahl) oder vom darauf folgenden Tag (für eine positive Zahl) zurück.

Wenn Sie eine Zahl außerhalb des Bereichs angeben müssen, empfehlen wir die Verwendung von addHours, wie oben unter [addHours (date; number)](#addhours-date-number).

>[!INFO]
>
>**Beispiele:**
>
>* `setHour(2015-08-07T11:36:39.138Z;6)`
   >
   >   Gibt 2015-08-07T06 zurück:36:39.138 Z
>
>* `setHour(2015-08-07T11:36:39.138;-6)`
   >
   >    Gibt 2015-08-06T18 zurück:36:39.138 Z


## [!UICONTROL setDay (date; Anzahl/Name des Tages (in englischer Sprache)]

Diese Funktion gibt ein neues Datum mit dem in den Parametern angegebenen Tag zurück.

Sie können diese Funktion verwenden, um den Wochentag mit Sonntag auf 1 und Samstag auf 7 festzulegen. Wenn Sie eine Zahl zwischen 1 und 7 angeben, liegt das resultierende Datum in der aktuellen (Sonntag bis Samstag) Woche. Wenn die Zahl außerhalb dieses Bereichs liegt, gibt die Funktion einen Tag aus der vorherigen Woche (für eine negative Zahl) oder aus der darauffolgenden Woche (für eine positive Zahl) zurück.

Wenn Sie eine Zahl außerhalb des Bereichs angeben müssen, empfehlen wir die Verwendung von addDays, wie oben unter [addDays (date; number)](#adddays-date-number).

>[!INFO]
>
>**Beispiele:**
>
>* `setDay(2018-06-27T11:36:39.138Z;Monday)`
   >
   >   Gibt 2018-06-25T11 zurück:36:39.138 Z
>
>* `setDay(2018-06-27T11:36:39.138Z;1)`
   >
   >   Gibt 2018-06-24T11 zurück:36:39.138 Z
>
>* `setDay(2018-06-27T11:36:39.138Z;7)`
   >
   >   Gibt 2018-06-30T11 zurück:36:39.138 Z


## [!UICONTROL setDate (Datum; number)]

Diese Funktion gibt ein neues Datum mit dem in den Parametern angegebenen Tag des Monats zurück.

Geben Sie eine Zahl zwischen 1 und 31 an. Wenn die Zahl außerhalb dieses Bereichs liegt, gibt die Funktion einen Tag aus dem vorherigen Monat (für eine negative Zahl) oder aus dem darauf folgenden Monat (für eine positive Zahl) zurück.

>[!INFO]
>
>**Beispiele:**
>
>* `setDate(2015-08-07T11:36:39.138Z;5)`
   >
   >   Gibt 2015-08-05T11 zurück:36:39.138 Z
>
>* `setDate(2015-08-07T11:36:39.138Z;32)`
   >
   >   Gibt 2015-09-01T11 zurück:36:39.138 Z


## [!UICONTROL setMonth (date; Zahl/Name des Monats in englischer Sprache)]

Diese Funktion gibt ein neues Datum mit dem in den Parametern angegebenen Monat zurück.

Geben Sie eine Zahl zwischen 1 und 12 an. Wenn die Zahl außerhalb dieses Bereichs liegt, gibt die Funktion den Monat im Vorjahr (für eine negative Zahl) oder im darauf folgenden Jahr (für eine positive Zahl) zurück.

>[!INFO]
>
>**Beispiele:**
>
>* `setMonth(2015-08-07T11:36:39.138Z;5)`
   >
   >   Gibt 2015-05-07T11 zurück:36:39.138 Z
>
>* `setMonth(2015-08-07T11:36:39.138Z;17)`
   >
   >   Gibt 2016-05-07T11 zurück:36:39.138 Z
>
>* `setMonth(2015-08-07T11:36:39.138Z;january)`
   >
   >   Gibt 2015-01-07T12 zurück:36:39.138 Z


## [!UICONTROL setYear (date; number)]

Gibt ein neues Datum mit dem in den Parametern angegebenen Jahr zurück.

>[!INFO]
>
>**Beispiel:**
>
>* `setYear(2015-08-07T11:36:39.138Z;2017)`
   >
   >   Gibt 2017-08-07T11 zurück:36:39.138 Z


## [!UICONTROL dateDifference (Date1; Datum 2; Einheit)]

Gibt eine Zahl zurück, die die Differenz der beiden Daten in der angegebenen Einheit darstellt.

Date2 wird von Date1 subtrahiert.

Verwenden Sie einen der folgenden Zeitwerte für die `unit` Parameter:

* Millisekunden
* Sekunden
* Minuten
* Stunden
* Tage
* Wochen
* Monate

Wenn keine Einheit angegeben ist, gibt die Funktion die Differenz in Millisekunden zurück.

>[!INFO]
>
>**Beispiele:**
>
>* `dateDifference(2021-05-11T18:10:00.000Z;2021-05-11T18:00:00.000Z)`
   >
   >    Rückgabe `600,000`
>
>* `dateDifference(2021-05-11T18:10:00.000Z;2021-05-11T18:00:00.000Z;hours)`
   >
   >    Rückgabe `4`
>
>* `dateDifference2021-06-11T18:10:00.000Z;2021-05-11T18:00:00.000Z;months)`
   >
   >    Rückgabe `1`


## Zusätzliche Beispiele

### Berechnung des n. Wochentags im Monat

Dieser Abschnitt wurde für [!DNL Workfront Fusion] von [!DNL Exceljet] -Webseite, auf der erklärt wird, wie der n-te Wochentag in einem Monat erreicht wird.

Wenn Sie ein Datum berechnen müssen, das dem n. Wochentag im Monat entspricht (z. B. erster Dienstag, dritter Freitag usw.), können Sie die folgende Formel verwenden:

![](assets/date&time-functions-calc-nth-day-350x31.png)

```
{{addDays(setDate(1.date; 1); 1.n * 7 - formatDate(addDays(setDate(1.date; 1); "-" + 1.dow); "E"))}}
```

Die Formel enthält die folgenden Elemente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>1.n</code> </td> 
   <td> <p> n. Tag:</p> 
    <ul> 
     <li><code>1</code> für den 1. Dienstag</li> 
     <li><code>2</code> für den zweiten Dienstag</li> 
     <li><code>3</code> für den 3. Dienstag usw.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><code>2.dow</code> </td> 
   <td> <p> Wochentag:</p> 
    <ul> 
     <li><code>1</code> für Montag</li> 
     <li><code>2</code> für Dienstag</li> 
     <li><code>3</code> für Mittwoch</li> 
     <li><code>4</code> für Donnerstag</li> 
     <li><code>5</code> für Freitag</li> 
     <li><code>6</code> für Samstag</li> 
     <li><code>7</code> für Sonntag</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><code>1.date</code> </td> 
   <td> <p> Das Datum bestimmt den Monat. Um den n. Wochentag im aktuellen Monat zu berechnen, verwenden Sie die <code>now</code> -Variable.</p> </td> 
  </tr> 
 </tbody> 
</table>

Wenn Sie nur einen bestimmten Fall berechnen möchten, z. B. jeden zweiten Mittwoch, können Sie die Elemente ersetzen `1.n` und `2.dow` in der Formel mit entsprechenden Zahlen. Für den zweiten Mittwoch im aktuellen Monat würden Sie die folgenden Werte verwenden:

* `1.n` = `2`
* `1.dow` = `3`
* `1.date` = `now`

![](assets/nth-day-variable-value-350x33.png)

### Erklärung:

* `setDate(now;1)` gibt den ersten Tag des aktuellen Monats aus
* `formatDate(....;E)` gibt den Wochentag zurück (1, 2, ... 6)

## So berechnen Sie Tage zwischen Datumsangaben

Eine Möglichkeit besteht darin, den folgenden Ausdruck zu verwenden:

![](assets/calculate-days-between-dates-350x68.png)

```
{{round((2.value - 1.value) / 1000 / 60 / 60 / 24)}}
```

>[!NOTE]
>
>* Werte von `D1`und `D2` haben Datumstypwerte. Wenn es sich um Werte vom Typ String handelt (z. B. 20.10.2018), verwenden Sie die `parseDate()` -Funktion, um sie in Werte vom Typ Datum zu konvertieren.
>
>* Die `round()` -Funktion wird für Fälle verwendet, in denen eines der Daten unter den Sommerzeit-Zeitraum fällt und das andere nicht. In diesen Fällen beträgt die Differenz in Stunden mindestens eine Stunde. Sie können ihn durch 24 für ein Ergebnis ohne Ganzzahl teilen. Sie verlieren eine stündliche Sommerzeit. Rund reduziert es, sodass Sie keinen Prozentsatz haben


### Berechnung des letzten Tages/der Millisekunde des Monats

Wenn Sie einen Datumsbereich angeben, z. B. in einem Suchmodul, müssen Sie den letzten Tag des Monats berechnen, wenn der Bereich den gesamten vorherigen Monat als geschlossenes Intervall umfasst (das Intervall, das beide Begrenzungspunkte enthält).

2019-09-01 ≤ D ≤ 2019-09-30

Die folgende Formel zeigt eine Methode zur Berechnung des letzten Tages des vorherigen Monats:

![](assets/last-day-prev-month.png)

```
{{addDays(setDate(now; 1); -1)}}
```

In einigen Fällen müssen Sie nicht nur den letzten Tag des Monats berechnen, sondern buchstäblich die letzte Millisekunde:

09.09.2019 T00:00:00.000Z ≤ D ≤ 2019-09-30T23:59:59.999 Z

Diese Formel zeigt eine Methode zur Berechnung der letzten Millisekunde des Vormonats:

![](assets/last-millisecond-prev-month-350x45.png)

```
{{parseDate(parseDate(formatDate(now; "YYYYMM01"); "YYYYMMDD"; "UTC") - 1; "x")}}
```

Wenn Sie das Ergebnis benötigen, um Ihre Zeitzoneneinstellung zu verwenden, lassen Sie das UTC-Argument weg:

![](assets/omit-utc-argument-350x45.png)

`{{parseDate(parseDate(formatDate(now; "YYYYMM01"); "YYYYMMDD") - 1; "x")}}`

Es ist jedoch vorzuziehen, stattdessen das halboffene Intervall zu verwenden (das Intervall, das einen seiner Grenzpunkte ausschließt), stattdessen den ersten Tag des folgenden Monats anzugeben und den Operator &quot;kleiner oder gleich&quot;wie folgt durch &quot;kleiner als&quot;zu ersetzen:

`2019-09-01 ≤ D < 2019-10-01`

`2019-09-01T00:00:00.000Z ≤ D < 2019-10-01T00:00:00.000Z`
