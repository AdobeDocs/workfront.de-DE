---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Übersicht über berechnete Datenausdrücke
description: Sie können Datenausdrücke verwenden, um berechnete benutzerdefinierte Datenfelder in Adobe Workfront zu definieren. Berechnete Ausdrücke verbinden vorhandene Workfront-Felder in Anweisungen, die ein neues Feld generieren.
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: fe9d3cfbb50bfda672360b918d971cc77b0b8b0a
workflow-type: tm+mt
source-wordcount: '2463'
ht-degree: 2%

---

# Übersicht über berechnete Datenausdrücke

<!--Audited: 12/2023-->

Sie können Datenausdrücke verwenden, um berechnete benutzerdefinierte Felder in Adobe Workfront zu definieren. Berechnete Ausdrücke verbinden vorhandene Workfront-Felder in Anweisungen, die ein neues Feld generieren.

Berechnete Datenausdrücke können in folgenden Bereichen verwendet werden:

* Ein berechnetes benutzerdefiniertes Feld in einem benutzerdefinierten Formular

  Weitere Informationen zum Erstellen berechneter benutzerdefinierter Felder in benutzerdefinierten Formularen in Workfront finden Sie unter [Hinzufügen berechneter Felder zu einem Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

* Eine berechnete benutzerdefinierte Spalte in einem Bericht oder einer Liste, wenn Sie den Textmodus verwenden

  Weitere Informationen zur Verwendung des Textmodus in Berichten und Ansichten finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Syntax von berechneten benutzerdefinierten Feldern im Vergleich zu berechneten benutzerdefinierten Spalten

Obwohl die von Ihnen verwendeten Funktionen identisch sind, kann sich die Syntax zum Erstellen eines Ausdrucks in einem berechneten benutzerdefinierten Feld von der Syntax zum Erstellen einer berechneten benutzerdefinierten Spalte unterscheiden.

Die Unterschiede zwischen den beiden Syntaxen sind:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Berechnetes benutzerdefiniertes Feld</strong></td> 
   <td><strong>Berechnetes benutzerdefiniertes Berichterstellungselement</strong></td> 
  </tr> 
   <td>Schließen Sie Feldnamen in geschweifte Klammern ein</td> 
   <td>Schließen Sie Feldnamen nicht in Klammern oder Klammern ein, wenn Sie sie in einer <p><code>valuefield </code></p>Zeile. <p>Schließen Sie Feldnamen in geschweifte Klammern ein, wenn Sie sie in einer <p><code>valueexpression</code></p> Zeile.</p> </td> 
  </tr> 
  <tr> 
   <td>Felder durch Punkte trennen</td> 
   <td> <p>Trennen Sie die Felder bei Verwendung in einem <p><code>valuefield </code></p>Zeile</p> <p>Trennen Sie die Felder bei Verwendung in einem <p><code>valueexpression </code></p>Zeile. </p> </td> 
  </tr> 
 </tbody> 
</table>

Beispiel:

* In einem benutzerdefinierten Feld in einem benutzerdefinierten Formular für Aufgaben würden Sie Folgendes verwenden, um den Namen des übergeordneten Projekts der Aufgabe zu generieren, an das das benutzerdefinierte Formular angehängt ist:


  ` {project}.{name}`


* In einer benutzerdefinierten Spalte in einem Bericht würden Sie Folgendes verwenden, um eine benutzerdefinierte Spalte „Projektname“ zu einem Aufgabenbericht hinzuzufügen:


  `valuefield=project:name`


  Oder

  `valueexpression={project}.{name}`


  >[!TIP]
  >
  >Die gleiche Syntax gilt für alle Berichtselemente im Textmodus, in denen berechnete Ausdrücke verwendet werden: Ansichten, Filter, Gruppierungen, Eingabeaufforderungen.

Weitere Informationen zur Syntax, die Sie in einer berechneten benutzerdefinierten Spalte verwenden müssen, finden Sie unter [Übersicht über den Textmodus](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Datenausdrücke, die Sie verwenden können

In den folgenden Listen werden die verfügbaren Ausdrücke definiert, die Sie beim Erstellen eines der drei verschiedenen Arten von berechneten benutzerdefinierten Feldern in Workfront verwenden können:

* [Berechnete benutzerdefinierte Felder für Datum und Uhrzeit](#date-time-calculated-custom-fields)
* [Mathematisch berechnete benutzerdefinierte Felder](#mathematical-calculated-custom-fields)
* [Berechnete benutzerdefinierte Textfelder](#text-calculated-custom-fields)

Sie können die unten aufgeführten Ausdrücke verwenden, um berechnete benutzerdefinierte Spalten zu erstellen. Sie müssen jedoch die richtige Syntax für eine berechnete benutzerdefinierte Spalte verwenden, wie im Abschnitt [Syntax berechneter benutzerdefinierter Felder vs. berechneter benutzerdefinierter Spalten](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) in diesem Artikel beschrieben.

### Berechnete benutzerdefinierte Felder für Datum und Uhrzeit {#date-time-calculated-custom-fields}

>[!NOTE]
>
>Wenn Sie eine Datums- und Uhrzeitberechnung erstellen, die keinen Zeitanteil enthält oder die Datums-Platzhalter $$TODAY oder $$NOW verwendet, verwendet das System das Datum in der UTC-Zone (Coordinated Universal Time) und nicht in der Zeitzone Ihrer lokalen Zeitzone. Dies kann zu einem unerwarteten Datumsergebnis führen.

Sie können ein berechnetes benutzerdefiniertes Feld für Datum oder Uhrzeit mithilfe der folgenden Ausdrücke erstellen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Ausdruck</th> 
   <th>Erklärung und Beispiel</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ADDDAYS</strong> </td> 
   <td> <p>Addiert die Anzahl der Tage zum Datum. Der Zahlenwert kann Teiltage enthalten. Mit 1.5 werden dem Datum beispielsweise anderthalb Tage hinzugefügt.</p> <p>Der Ausdruck ist wie folgt formatiert:</p>

<p><code>ADDDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>Addiert die Anzahl der Wochentage zum Datum. Dieser Ausdruck fügt dem Datum nur ganze Ganzzahlwerte hinzu, die abgerundet werden. </p> <p>Der Ausdruck ist wie folgt formatiert:</p>

<p><code>ADDWEEKDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>Addiert die Anzahl der Monate zum Datum und ist wie folgt formatiert:

</p><p><code>ADDMONTHS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>Addiert die Anzahl der Jahre zum Datum und ist wie folgt formatiert:</p>

<p><code>ADDYEARS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDHOURS</strong> </td> 
   <td> <p>Addiert die Anzahl der Stunden zum Datum und ist wie folgt formatiert:</p>

<p><code>ADDHOUR(date, number)</code></p>
   <p>Hinweis: Dieser Ausdruck wird in Workfront Planning nicht unterstützt.</p></td> 
  </tr>
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>Löscht den Zeitabschnitt eines Datums und ist wie folgt formatiert. In diesem Beispiel ist das Datum das Eingabedatum für ein Arbeitsobjekt.</p>

<p><code>CLEARTIME({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATE</strong> </td> 
   <td> <p>Konvertiert eine Zeichenfolge in ein Datum und ist wie folgt formatiert:</p>

<p><code>DATE(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>Gibt die Anzahl der Tage zwischen den beiden Datumsangaben zurück, wobei die Anfangs- und Endtage des ausgewählten Zeitraums sowie die Zeitstempel an diesen Tagen berücksichtigt werden. Wenn beispielsweise die Startzeit des Startdatums 15 Uhr ist, wird der Starttag nicht als ganzer Tag gezählt.</p> <p>Der Ausdruck ist wie folgt formatiert:</p>

<p><code>DATEDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>Gibt den Tag des Monats für das Datum als eine Zahl zwischen 1 und 31 zurück.</p> <p>Der Ausdruck ist wie folgt formatiert. In diesem Beispiel ist das Datum das Eingabedatum für ein Arbeitsobjekt.</p>

<p><code>DAYOFMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>Gibt den Wochentag für das Datum als eine Zahl zwischen 1 (Sonntag) und 7 (Samstag) zurück.</p> <p>Der Ausdruck ist wie folgt formatiert. In diesem Beispiel ist das Datum das Eingabedatum für ein Arbeitsobjekt.</p>

<p><code>DAYOFWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>Gibt die Gesamtzahl von Tagen im Monat des Datums als Zahl zurück und ist wie folgt formatiert. In diesem Beispiel ist das Datum das Eingabedatum für ein Arbeitsobjekt.</p>

<p><code>DAYSINMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>Gibt die Gesamtzahl von Wochentagen zwischen dem Datum und dem Ende der Woche oder des Monats zurück, je nachdem, was zuerst eintritt. In diesem Beispiel ist das Datum das Eingabedatum für ein Arbeitsobjekt.</p> <p>Der Ausdruck ist wie folgt formatiert:</p>

<p><code>DAYSINSPLITWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>Gibt die Gesamtzahl von Tagen im Jahr des Datums als Zahl zurück und ist wie folgt formatiert. In diesem Beispiel ist das Datum das Eingabedatum für ein Arbeitsobjekt.</p>

<p><code>DAYSINYEAR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>Gibt das letzte Datum in der Liste zurück und ist wie folgt formatiert:</p>

<p><code>DMAX(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>Gibt das früheste Datum in der Liste zurück und ist wie folgt formatiert:</p>

<p><code>DMIN(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>STUNDE</strong> </td> 
   <td> <p>Gibt die Stunde des Datums als eine Zahl zwischen 0 und 23 zurück.</p> <p>Der Ausdruck ist wie folgt formatiert. In diesem Beispiel ist das Datum das Eingabedatum für ein Arbeitsobjekt.</p>

<p><code>HOUR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUTE</strong> </td> 
   <td> <p>Gibt die Minute des Datums als eine Zahl zwischen 0 und 60 zurück, die wie folgt formatiert ist. In diesem Beispiel ist das Datum das Eingabedatum für ein Arbeitsobjekt.</p>

<p><code>MINUTE({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MONAT</strong> </td> 
   <td> <p>Gibt den Monat des Datums als eine Zahl zwischen 1 und 12 zurück, die wie folgt formatiert ist. In diesem Beispiel ist das Datum das Eingabedatum für ein Arbeitsobjekt.</p>

<p><code>MONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SECOND</strong> </td> 
   <td> <p>Gibt die Sekunde des Datums als eine Zahl zwischen 0 und 60 zurück, die wie folgt formatiert ist. In diesem Beispiel ist das Datum das Eingabedatum für ein Arbeitsobjekt.</p>

<p><code>SECOND({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>Gibt die Anzahl der Wochentage zwischen zwei Terminen zurück, wobei der Anfangs- und der Endtag des ausgewählten Zeitraums sowie die Zeitstempel an diesen Tagen berücksichtigt werden. Wenn beispielsweise die Startzeit des Startdatums 15 Uhr ist, wird der Starttag nicht als ganzer Tag gezählt.</p> <p>Der Ausdruck ist wie folgt formatiert:</p>

<p><code>WEEKDAYDIFF(date2, date1)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>Gibt die Anzahl geplanter Minuten zwischen den Datumsangaben gemäß Standardzeitplan zurück.</p> <p>Der Ausdruck ist wie folgt formatiert:</p>

<p><code>WORKMINUTESDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>YEAR</strong> </td> 
   <td> <p>Gibt das Jahr des Datums als 4-stellige Zahl zurück, wie folgt formatiert. In diesem Beispiel ist das Datum das Eingabedatum für ein Arbeitsobjekt.</p>

<p><code>YEAR({entryDate})</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### Mathematisch berechnete benutzerdefinierte Felder {#mathematical-calculated-custom-fields}

Sie können ein berechnetes benutzerdefiniertes Feld erstellen, das einige der folgenden mathematischen Ausdrücke verwendet:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Ausdruck</th> 
   <th>Erklärung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ABS</strong> </td> 
   <td>Gibt den absoluten Wert der Zahl zurück und ist wie folgt formatiert. In diesem Beispiel wird die Anzahl der Objekte unter dem Objekt verwendet, an das das benutzerdefinierte Formular angehängt ist.

<p><code>ABS({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>DURCHSCHNITT</strong> </td> 
   <td>Gibt den Zahlendurchschnitt zurück und ist wie folgt formatiert:

<p><code>AVERAGE(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>Rundet eine Zahl auf die nächste Ganzzahl auf und ist wie folgt formatiert. In diesem Beispiel wird die Anzahl der Objekte unter dem Objekt verwendet, an das das benutzerdefinierte Formular angehängt ist.

<p><code>CEIL({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>Dividiert alle Zahlen in der angegebenen Reihenfolge und ist wie folgt formatiert:

<p><code>DIV(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>Rundet eine Zahl auf die nächste Ganzzahl herunter und wird wie folgt formatiert. In diesem Beispiel wird die Anzahl der Objekte unter dem Objekt verwendet, an das das benutzerdefinierte Formular angehängt ist.

<p><code>FLOOR({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>Gibt den natürlichen Logarithmus der Zahl zurück und ist wie folgt formatiert:

<p><code>LN({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>Gibt den Logarithmus der Zahl2 zur Basis der Zahl1 zurück und ist wie folgt formatiert:

<p><code>LOG(number1, number2)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>MAX</strong> </td> 
   <td>Gibt das größte Element in der Liste zurück und ist wie folgt formatiert:

<p><code>MAX(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>MIN</strong> </td> 
   <td>Gibt das kleinste Element in der Liste zurück und ist wie folgt formatiert:

<p><code>MIN(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>NUMBER</strong> </td> 
   <td>Konvertiert eine Zeichenfolge in eine Zahl und ist wie folgt formatiert:<p><code>NUMBER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>Gibt eine Potenz einer Zahl zurück und ist wie folgt formatiert:

<p><code>POWER(number, power)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>Multipliziert alle Zahlen und ist wie folgt formatiert:

<p><code>PROD(number1, number2, ....)</code></p>
   <p><b>NOTIZ</b></p>

<p>Stellen Sie beim Multiplizieren von Feldern, die Stunden enthalten, sicher, dass Sie verstehen, ob die Datenbank die Stunden in ausgewählten Feldern in Minuten, Stunden oder Sekunden speichert. Wenn die Stunden in Minuten oder Sekunden gespeichert werden, aber in der Workfront-Benutzeroberfläche in Stunden angezeigt werden, müssen Sie beim Schreiben eines Ausdrucks mit dieser Berechnung möglicherweise die Konvertierung von Minuten oder Sekunden in Stunden berücksichtigen. </p>
   </td> 
  </tr> 
  <tr> 
   <td><strong>RUND</strong> </td> 
   <td>Rundet die Zahl auf eine angegebene Dezimalgenauigkeit auf und ist wie folgt formatiert:

<p><code>ROUND(number, precision)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> Bestellt die Zahlen in aufsteigender Reihenfolge und ist wie folgt formatiert:</p>

<p><code>SORTASCNUM(number1,number2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>Bestellt die Zahlen in absteigender Reihenfolge und ist wie folgt formatiert:

<p><code>SORTDESCNUM(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>Gibt die Quadratwurzel einer Zahl zurück und ist wie folgt formatiert. In diesem Beispiel wird die Anzahl der Objekte unter dem Objekt verwendet, an das das benutzerdefinierte Formular angehängt ist.</p>

<p><code>SQRT({numberOfChildren})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>Subtrahiert alle Zahlen in der angegebenen Reihenfolge und ist wie folgt formatiert:

<p><code>SUB(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SUM</strong> </td> 
   <td>Addiert alle Zahlen und ist wie folgt formatiert:

<p><code>SUM(number1, number2, ...)</code></p></td> 
  </tr> 
 </tbody> 
</table>

### Berechnete benutzerdefinierte Textfelder {#text-calculated-custom-fields}

Sie können ein berechnetes benutzerdefiniertes Feld erstellen, das einen textformatierten Wert anzeigt, indem Sie die folgenden Ausdrücke verwenden:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Ausdruck</th> 
   <th>Erklärung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ARRAY</strong> </td> 
   <td> <p>Konvertiert eine Zeichenfolge in ein Array. Das Trennzeichen kann eine beliebige Zeichenfolge sein.</p> 
   <p>Der Ausdruck ist wie folgt formatiert:</p>
   <p><code>ARRAY(string1, "delimiter")</code></p> 
   </td> 
  </tr>

<tr> 
   <td><strong>ARRAYCONTAINS</strong> </td> 
   <td> <p>Sucht nach einem bestimmten Wert in einer Liste oder einem Array. Wenn der Wert gefunden wird, gibt die Funktion True zurück, andernfalls gibt sie False zurück. </p> 
   <p>Der Ausdruck ist wie folgt formatiert:</p>
   <p><code>ARRAYCONTAINS(array, value)</code></p> 
   </td> 
  </tr>


<tr> 
   <td><strong>ARRAYLENGTH</strong> </td> 
   <td> <p>Gibt die Anzahl der Elemente im Array zurück und ist wie folgt formatiert:</p>
   <p><code>ARRAYLENGTH(array)</code></p> 
   </td> 
  </tr>
  <tr> 
   <td><strong>ARRAYELEMENT</strong> </td> 
   <td> <p>Gibt das Element unter der im Array angegebenen Nummer zurück. Wenn der Index außerhalb des zulässigen Bereichs liegt, wird ein leerer Wert zurückgegeben.</p> 
   <p>Der Ausdruck ist wie folgt formatiert:</p>
   <p><code>ARRAYELEMENT(array, number)</code></p> 
   </td> 
  </tr>
  <tr> 
   <td><strong>SORTASCARRAY</strong> </td> 
   <td> <p>Sortiert die Array-Elemente in aufsteigender Reihenfolge und konvertiert sie in den Typ des ersten Elements.</p>
   <p>Der Ausdruck ist wie folgt formatiert:</p>
   <p><code>SORTASCARRAY(array)</code></p>
   <p>Beispielsweise wird ["-12.6“, -13.0] zu ["-12.6“, "-13“].</p>
   <p>Hinweis: Dieser Ausdruck wird in Workfront Planning nicht unterstützt.</p></td> 
  </tr>
  <tr> 
   <td><strong>SORTDESCARRAY</strong> </td> 
   <td> <p>Sortiert die Array-Elemente in absteigender Reihenfolge und konvertiert sie in den Typ des ersten Elements.</p>
   <p>Der Ausdruck ist wie folgt formatiert:</p>
   <p><code>SORTDESCARRAY(array)</code></p>
   <p>Beispielsweise wird ["-12.6“, -13.0] zu ["-13“, "-12.6“].</p>
   <p>Hinweis: Dieser Ausdruck wird in Workfront Planning nicht unterstützt.</p></td> 
  </tr>
  <tr>   
   <td><strong>CASE</strong> </td> 
   <td> <p>Wird mit anderen Ausdrücken verwendet, um einen Wert basierend auf einer Indexnummer aus einer Liste auszuwählen. </p>
   <p>Eine Indexnummer ist ein Feld oder eine Funktion, die einen numerischen Wert (normalerweise in einem bekannten Bereich) zurückgibt.</p> 
   <p>Der Ausdruck ist wie folgt formatiert:</p>
   <p><code>CASE(indexNumber, value1, value2, ...)</code></p>

<p>Beispielsweise gibt der folgende Ausdruck den Namen des Wochentags in einer berechneten Spalte zurück, wobei 1=Sonntag, 2=Montag usw. ist:</p>

<p><code>CASE(DAYOFWEEK({entryDate}),"Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday")</code></p>

<p>Funktioniert am besten mit anderen Ausdrücken, die eine Zahl zurückgeben, z. B. DAYOFWEEK, DAYOFMONTH und MONTH.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>Verkettet die Zeichenfolge und ist wie folgt formatiert:</p><p><code>CONCAT(string1,"separator", string2)</code></p> <p>Im Folgenden finden Sie Beispiele für Trennzeichen, die Sie einschließen können:</p> 
    <ul> 
     <li>ein Leerzeichen: ""</li> 
     <li>Ein Bindestrich: "-"</li> 
     <li>Ein Schrägstrich: "/"</li> 
     <li>ein Komma: ",“</li> 
     <li>Ein Wort: „OR“, „AND“</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>ENTHÄLT</strong> </td> 
   <td>Gibt „true“ zurück, wenn die Zeichenfolge „findText“ im String „withinText“ gefunden wird und wie folgt formatiert ist:

<p><code>CONTAINS(findText, withinText)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>Setzt alle Sonderzeichen in der Zeichenfolge in Escape-Zeichen, damit sie in ein URL-Argument aufgenommen werden können.<p>Der Ausdruck ist wie folgt formatiert:</p>

<p><code>ENCODEURL(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>FORMAT</strong> </td> 
   <td><p>Gibt formatierten Text zurück. Nur die hier aufgeführten Parameteroptionen sind im FORMAT zulässig.</p>
   <p>Die Farboptionen sind $$POSITIVE, $$INFORMATIVE, $$NEGATIVE, $$NOTICE und die anderen Formatierungsoptionen sind $$BOLD, $$ITALIC, $$UNDERLINE. Es ist nur eine Farboption zusammen mit bis zu drei anderen Formatierungsoptionen zulässig. Wenn keine Farboption festgelegt ist, wird die Standardfarbe des Systems angewendet.</p>
   <p>Der Ausdruck ist wie folgt formatiert:</p>
   <p><code>FORMAT($$POSITIVE, $$BOLD, $$ITALIC)</code></p>
   <p>Hinweis: Dieser Ausdruck wird in Workfront Planning nicht unterstützt.</p></td> 
  </tr>   
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>Wertet eine von Ihnen angegebene Bedingung aus und gibt den Wert von „trueExpression“ zurück, wenn „true“ festgelegt ist, oder den Wert von „falseExpression“, wenn „false“ festgelegt ist.</p>

<p>Der Ausdruck ist wie folgt formatiert:</p>

<p><code>IF(condition, trueExpression, falseExpression)</code></p>

<p>Sie können beispielsweise zwei verschiedene Datumsfelder und anschließend ein Ergebnis „true/false“ als Datenzeichenfolge vergleichen:</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","On Track")</code></p>

<p>In der Alltagssprache bedeutet diese Aussage: „Wenn das voraussichtliche Abschlussdatum meines Objekts „größer als“ das geplante Abschlussdatum meines gleichen Objekts ist, dann zeigen Sie in diesem Feld die Wörter „Aus dem Kurs“ an; andernfalls zeigen Sie die Wörter „Auf dem Kurs“ an.“</p>

<p>Wenn Sie die Ausdrücke „true“ oder „false“ nicht kennzeichnen möchten, müssen Sie eine leere Kennzeichnung in Ihre Anweisung einfügen, z. B.:</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"","On Track")</code></p> 
   <p>Oder</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","")</code></p>

<p>Weitere Informationen zum Erstellen von „IF“-Anweisungen finden Sie unter <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref"> „IF“-Anweisungen - Übersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>Ermöglicht die Suche nach einem bestimmten Wert in einer Zeichenfolge möglicher Werte. Wenn der gesuchte Wert einem der angegebenen Werte entspricht, gibt der Ausdruck den Wert „trueExpression“ zurück. Andernfalls gibt er den Wert „falseExpression“ zurück.</p> 
   <p>Der Ausdruck ist wie folgt formatiert:</p>

<p><code>IFIN(value, value1, value2,..., trueExpression, falseExpression)</code></p>

<p>Sie können beispielsweise einen bestimmten Projektbesitzer suchen und diese Projekte mit einem bestimmten Tag in einer Projektansicht markieren: <br><p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")
   </code></p>
    <p> In der täglichen Rede bedeutet diese Aussage: „Wenn die Projektbesitzerin Jennifer Campbell oder Rick Kuvec ist, markieren Sie dieses Projekt mit „Marketing-Team“; andernfalls markieren Sie es mit „Andere Teams“.“</p> 
    <p> Wenn Sie die Ausdrücke „true“ oder „false“ nicht kennzeichnen möchten, müssen Sie eine leere Kennzeichnung in Ihre Anweisung einfügen, z. B.: </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> 
    <p>Oder </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","")</code></p> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>IN</strong> </td> 
   <td> <p>Gibt „true“ zurück, wenn der Wert einem der angegebenen Werte entspricht; andernfalls gibt der Ausdruck „false“ zurück.</p> <p>Der Ausdruck ist wie folgt formatiert:

</p><p><code>IN(value, value1[, value2...])</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>Gibt „true“ zurück, wenn der Wert null oder leer ist; andernfalls gibt der Ausdruck „false“ zurück.</p> <p>Der Ausdruck ist wie folgt formatiert:

</p><p><code>ISBLANK(value)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LINKS</strong> </td> 
   <td> <p>Gibt eine angegebene Anzahl von Zeichen auf der linken Seite einer Zeichenfolge zurück und ist wie folgt formatiert:</p>

<p><code>LEFT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>Gibt die Länge einer Zeichenfolge zurück und ist wie folgt formatiert:</p>

<p><code>LEN(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>UNTEN</strong> </td> 
   <td>Gibt die Zeichenfolge in Kleinbuchstaben zurück und ist wie folgt formatiert:

<p><code>LOWER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>ERSETZEN</strong> </td> 
   <td> <p>Ersetzt in Zeichenfolge1 alle Vorkommen von Zeichenfolge2 durch Zeichenfolge3.</p> <p>Der Ausdruck ist wie folgt formatiert:</p>

<p><code>REPLACE(string1, string2, string3)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>RIGHT</strong> </td> 
   <td> <p>Gibt eine bestimmte Anzahl von Zeichen rechts von einer Zeichenfolge zurück und ist wie folgt formatiert:</p>

<p><code>RIGHT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUCHE</strong> </td> 
   <td> <p>Gibt den Index des ersten Vorkommens von findText in der Zeichenfolge withinText zurück, beginnend mit der angegebenen Startposition, oder gibt -1 zurück, wenn der Text nicht gefunden wird.</p> <p>Der Ausdruck ist wie folgt formatiert:</p>

<p><code>SEARCH(findText, withinText, start)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ZEICHENFOLGE</strong> </td> 
   <td> <p>Konvertiert eine Zahl in eine Zeichenfolge und ist wie folgt formatiert:</p>

<p><code>STRING(number)</code></p> </td> 
  </tr>
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>Sortiert eine Liste mit Zeichenfolgen in aufsteigender Reihenfolge und ist wie folgt formatiert:</p>
   <p><code>SORTASCSTRING(string1, string2, ...)</code></p> </td> 
  </tr>
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> Sortiert eine Liste mit Zeichenfolgen in absteigender Reihenfolge und ist wie folgt formatiert:</p>
   <p><code>SORTDESCSTRING(string1, string2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>Gibt Zeichen einer Zeichenfolge basierend auf dem angegebenen Start- und Endindex zurück und ist wie folgt formatiert:</p>

<p><code>SUBSTR({string}, number of start position, number of end position)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SWITCH</strong> </td> 
   <td> <p>Wertet den Ausdruck anhand einer Liste von Werten aus und gibt das Ergebnis zurück, das dem ersten übereinstimmenden Wert entspricht.</p>
   <p>Der Ausdruck ist wie folgt formatiert:</p>
   <p><code>SWITCH(expression, value1, result1, [value2, result2], ...)</code></p>
   <p>Dieser Ausdruck wird in Workfront Planning nicht unterstützt.</p></td> 
  </tr>   
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>Entfernt Leerzeichen vom Anfang und Ende einer Zeichenfolge und ist wie folgt formatiert:</p>

<p><code>TRIM(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>Gibt eine Zeichenfolge in Großbuchstaben zurück und ist wie folgt formatiert:</p>

<p><code>UPPER(string)</code></p> </td> 
  </tr> 
 </tbody> 
</table>
