---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Übersicht über berechnete Datenausdrücke
description: Sie können Datenausdrücke verwenden, um berechnete benutzerdefinierte Datenfelder in Adobe Workfront zu definieren. Berechnete Ausdrücke verbinden vorhandene Workfront-Felder in Anweisungen, die ein neues Feld generieren.
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: 6f026590f0030b564f0d110afead9ade1acd7896
workflow-type: tm+mt
source-wordcount: '2166'
ht-degree: 0%

---

# Übersicht über berechnete Datenausdrücke

<!--Audited: 12/2023-->

Sie können Datenausdrücke verwenden, um berechnete benutzerdefinierte Felder in Adobe Workfront zu definieren. Berechnete Ausdrücke verbinden vorhandene Workfront-Felder in Anweisungen, die ein neues Feld generieren.

Sie können berechnete Datenausdrücke in folgenden Bereichen verwenden:

* Ein berechnetes benutzerdefiniertes Feld in einem benutzerdefinierten Formular

  Weitere Informationen zum Erstellen berechneter benutzerdefinierter Felder in benutzerdefinierten Formularen in Workfront finden Sie unter [Hinzufügen berechneter Daten zu einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* Eine berechnete benutzerdefinierte Spalte in einem Bericht oder einer Liste, wenn Sie den Textmodus verwenden

  Weitere Informationen zur Verwendung des Textmodus in Berichten und Ansichten finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Syntax von berechneten benutzerdefinierten Feldern im Vergleich zu berechneten benutzerdefinierten Spalten

Die von Ihnen verwendeten Funktionen sind zwar identisch, die Syntax zum Erstellen eines Ausdrucks in einem berechneten benutzerdefinierten Feld kann sich jedoch von der Syntax zum Erstellen einer berechneten benutzerdefinierten Spalte unterscheiden.

Die Unterschiede zwischen den beiden Syntaxen sind:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Berechnetes benutzerdefiniertes Feld</strong></td> 
   <td><strong>Berechnetes benutzerdefiniertes Berichtselement</strong></td> 
  </tr> 
   <td>Feldnamen in geschweifte Klammern setzen</td> 
   <td>Schließen Sie Feldnamen nicht in Klammern oder Klammern ein, wenn Sie sie in einer <p><code>valuefield </code></p>Linie. <p>Fügen Sie Feldnamen in geschweifte Klammern bei der Verwendung in einer <p><code>valueexpression</code></p> Linie.</p> </td> 
  </tr> 
  <tr> 
   <td>Trennen Sie die Felder durch Punkte.</td> 
   <td> <p>Trennen Sie die Felder bei Verwendung in einer <p><code>valuefield </code></p>line</p> <p>Trennen Sie die Felder bei der Verwendung in einer <p><code>valueexpression </code></p>Linie. </p> </td> 
  </tr> 
 </tbody> 
</table>

Beispiel:

* In einem benutzerdefinierten Feld würden Sie in einem benutzerdefinierten Formular für Aufgaben den Namen des übergeordneten Projekts der Aufgabe generieren, an das das benutzerdefinierte Formular angehängt ist:


  ` {project}.{name}`


* In einer benutzerdefinierten Spalte in einem Bericht können Sie wie folgt eine benutzerdefinierte Spalte für den Projektnamen zu einem Aufgabenbericht hinzufügen:


  `valuefield=project:name`


  Oder

  `valueexpression={project}.{name}`


  >[!TIP]
  >
  >Dieselbe Syntax gilt für alle Berichterstellungselemente im Textmodus, in denen berechnete Ausdrücke verwendet werden: Ansichten, Filter, Gruppierungen, Eingabeaufforderungen.

Weitere Informationen zur Syntax, die Sie in einer berechneten benutzerdefinierten Spalte verwenden müssen, finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Sie können Datenausdrücke verwenden

In den folgenden Listen werden die verfügbaren Ausdrücke definiert, die Sie verwenden können, wenn Sie in Workfront einen der drei Typen berechneter benutzerdefinierter Felder erstellen:

* [Datum und Uhrzeit der Berechnung benutzerdefinierter Felder](#date-time-calculated-custom-fields)
* [Mathematisch berechnete benutzerdefinierte Felder](#mathematical-calculated-custom-fields)
* [Benutzerdefinierte Textfelder](#text-calculated-custom-fields)

Sie können die unten aufgeführten Ausdrücke verwenden, um berechnete benutzerdefinierte Spalten zu erstellen. Sie müssen jedoch die richtige Syntax für eine berechnete benutzerdefinierte Spalte verwenden, wie im Abschnitt [Syntax berechneter benutzerdefinierter Felder vs. berechneter benutzerdefinierter Spalten](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) in diesem Artikel beschrieben.

### Benutzerdefinierte Felder für Datum und Uhrzeit mit Datum und Uhrzeit {#date-time-calculated-custom-fields}

>[!NOTE]
>
>Wenn Sie eine Datums- und Uhrzeitberechnung erstellen, die keinen Zeitabschnitt enthält oder die Datumsfelder $$TODAY oder $$NOW verwendet, verwendet das System das Datum gemäß der UTC-Zone (Coordinated Universal Time), nicht gemäß Ihrer lokalen Zeitzone. Dies kann zu einem unerwarteten Datumsergebnis führen.

Sie können ein benutzerdefiniertes Datums- oder Uhrzeitfeld mithilfe der folgenden Ausdrücke erstellen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Ausdruck</th> 
   <th>Erläuterung und Beispiel</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ADDDAYS</strong> </td> 
   <td> <p>Fügt die Anzahl der Tage zum Datum hinzu. Der Zahlenwert kann Teiltage enthalten. Beispielsweise fügt 1.5 dem Datum anderthalb Tage hinzu.</p> <p>Der Ausdruck ist wie folgt formatiert:</p>

<p><code>ADDDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>Fügt die Anzahl der Wochentage zum Datum hinzu. Dieser Ausdruck fügt nur ganze ganzzahlige Werte zum Datum hinzu und rundet es ab. </p> <p>Der Ausdruck ist wie folgt formatiert:</p>

<p><code>ADDWEEKDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>Fügt die Anzahl der Monate zum Datum hinzu und ist wie folgt formatiert:

</p><p><code>ADDMONTHS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>Fügt die Anzahl der Jahre zum Datum hinzu und ist wie folgt formatiert:</p>

<p><code>ADDYEARS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>Löscht den Zeitabschnitt eines Datums und ist wie folgt formatiert. In diesem Beispiel ist das Datum das Datum der Einsendung für ein Arbeitsobjekt.</p>

<p><code>CLEARTIME({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATE</strong> </td> 
   <td> <p>Konvertiert eine Zeichenfolge in ein Datum und ist wie folgt formatiert:</p>

<p><code>DATE(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>Gibt die Anzahl der Tage zwischen den beiden Daten unter Berücksichtigung des Start- und Endtages des ausgewählten Zeitraums sowie der Zeitstempel dieser Tage zurück. Wenn die Startzeit des Startdatums beispielsweise 15 Uhr beträgt, wird der Starttag nicht als vollständiger Tag gezählt.</p> <p>Der Ausdruck ist wie folgt formatiert:</p>

<p><code>DATEDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>Gibt den Tag des Monats für das Datum als Zahl zwischen 1 und 31 zurück.</p> <p>Der Ausdruck ist wie folgt formatiert: In diesem Beispiel ist das Datum das Datum der Einsendung für ein Arbeitsobjekt.</p>

<p><code>DAYOFMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>Gibt den Wochentag für das Datum als Zahl zwischen 1 (Sonntag) und 7 (Samstag) zurück.</p> <p>Der Ausdruck ist wie folgt formatiert: In diesem Beispiel ist das Datum das Datum der Einsendung für ein Arbeitsobjekt.</p>

<p><code>DAYOFWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>Gibt die Gesamtanzahl der Tage im Monat des Datums als Zahl aus und ist wie folgt formatiert: In diesem Beispiel ist das Datum das Datum der Einsendung für ein Arbeitsobjekt.</p>

<p><code>DAYSINMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>Gibt die Gesamtwochentage zwischen dem Datum und dem Ende der Woche bzw. dem Ende des Monats zurück, je nachdem, was zuerst eintritt. In diesem Beispiel ist das Datum das Datum der Einsendung für ein Arbeitsobjekt.</p> <p>Der Ausdruck ist wie folgt formatiert:</p>

<p><code>DAYSINSPLITWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>Gibt die Gesamtanzahl der Tage im Jahr des Datums als Zahl aus und ist wie folgt formatiert: In diesem Beispiel ist das Datum das Datum der Einsendung für ein Arbeitsobjekt.</p>

<p><code>DAYSINYEAR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>Gibt das neueste Datum in der Liste zurück und ist wie folgt formatiert:</p>

<p><code>DMAX(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>Gibt das früheste Datum in der Liste zurück und ist wie folgt formatiert:</p>

<p><code>DMIN(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>STUNDE</strong> </td> 
   <td> <p>Gibt die Stunde des Datums als Zahl zwischen 0 und 23 zurück.</p> <p>Der Ausdruck ist wie folgt formatiert: In diesem Beispiel ist das Datum das Datum der Einsendung für ein Arbeitsobjekt.</p>

<p><code>HOUR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUTE</strong> </td> 
   <td> <p>Gibt die Minute des Datums als Zahl zwischen 0 und 60 zurück, formatiert wie folgt. In diesem Beispiel ist das Datum das Datum der Einsendung für ein Arbeitsobjekt.</p>

<p><code>MINUTE({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MONTH</strong> </td> 
   <td> <p>Gibt den Monat des Datums als Zahl zwischen 1 und 12 zurück, formatiert wie folgt. In diesem Beispiel ist das Datum das Datum der Einsendung für ein Arbeitsobjekt.</p>

<p><code>MONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SECOND</strong> </td> 
   <td> <p>Gibt die Sekunde des Datums als Zahl zwischen 0 und 60 zurück, formatiert wie folgt. In diesem Beispiel ist das Datum das Datum der Einsendung für ein Arbeitsobjekt.</p>

<p><code>SECOND({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>Gibt die Anzahl der Wochentage zwischen zwei Daten unter Berücksichtigung des Start- und Endtages des ausgewählten Zeitraums sowie der Zeitstempel dieser Tage zurück. Wenn die Startzeit des Startdatums beispielsweise 15 Uhr beträgt, wird der Starttag nicht als voller Tag gezählt.</p> <p>Der Ausdruck ist wie folgt formatiert:</p>

<p><code>WEEKDAYDIFF(date2, date1)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>Gibt die Anzahl der geplanten Minuten zwischen den Daten gemäß dem Standardzeitplan zurück.</p> <p>Der Ausdruck ist wie folgt formatiert:</p>

<p><code>WORKMINUTESDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>JAHR</strong> </td> 
   <td> <p>Gibt das Jahr des Datums als vierstellige Zahl zurück, die wie folgt formatiert ist: In diesem Beispiel ist das Datum das Datum der Einsendung für ein Arbeitsobjekt.</p>

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
   <td>Gibt den absoluten Wert der Zahl zurück und ist wie folgt formatiert: In diesem Beispiel wird die Anzahl der Objekte unter dem Objekt verwendet, an das das benutzerdefinierte Formular angehängt ist.

<p><code>ABS({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>DURCHSCHNITT</strong> </td> 
   <td>Gibt den Durchschnittswert der Zahlen zurück und ist wie folgt formatiert:

<p><code>AVERAGE(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>Kürzt die Zahl auf die nächste Ganzzahl und wird wie folgt formatiert: In diesem Beispiel wird die Anzahl der Objekte unter dem Objekt verwendet, an das das benutzerdefinierte Formular angehängt ist.

<p><code>CEIL({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>Teilt alle Zahlen in der angegebenen Reihenfolge und ist wie folgt formatiert:

<p><code>DIV(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>Kürzt die Zahl auf die nächste Ganzzahl und wird wie folgt formatiert: In diesem Beispiel wird die Anzahl der Objekte unter dem Objekt verwendet, an das das benutzerdefinierte Formular angehängt ist.

<p><code>FLOOR({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>Gibt den natürlichen Logarithmuswert der Zahl zurück und ist wie folgt formatiert:

<p><code>LN({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>Gibt den Logarithmuswert von number2 zur Basisnummer 1 zurück und ist wie folgt formatiert:

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
   <td>Gibt eine Zahl zurück, die auf einen Strom erhöht wird und wie folgt formatiert ist:

<p><code>POWER(number, power)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>Multipliziert alle Zahlen und ist wie folgt formatiert:

<p><code>PROD(number1, number2, ....)</code></p>
   <p><b>NOTIZ</b></p>

<p>Stellen Sie beim Multiplizieren von Feldern, die Stunden enthalten, sicher, dass Sie verstehen, ob die Datenbank die Stunden in ausgewählten Feldern in Minuten, Stunden oder Sekunden speichert. Wenn die Stunden in Minuten oder Sekunden gespeichert, aber in Stunden auf der Workfront-Oberfläche angezeigt werden, müssen Sie beim Schreiben eines Ausdrucks mithilfe dieser Berechnung möglicherweise die Konvertierung von Minuten oder Sekunden in Stunden berücksichtigen. </p>
   </td> 
  </tr> 
  <tr> 
   <td><strong>ROUND</strong> </td> 
   <td>Rundet die Zahl auf eine angegebene Dezimalzahl und ist wie folgt formatiert:

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
   <td> <p>Gibt eine Quadratwurzel einer Zahl zurück und ist wie folgt formatiert: In diesem Beispiel wird die Anzahl der Objekte unter dem Objekt verwendet, an das das benutzerdefinierte Formular angehängt ist.</p>

<p><code>SQRT({numberOfChildren})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>Zieht alle Zahlen in der angegebenen Reihenfolge ab und ist wie folgt formatiert:

<p><code>SUB(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SUM</strong> </td> 
   <td>Fügt alle Zahlen hinzu und ist wie folgt formatiert:

<p><code>SUM(number1, number2, ...)</code></p></td> 
  </tr> 
 </tbody> 
</table>

### Benutzerdefinierte Textfelder {#text-calculated-custom-fields}

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
   <td><strong>CASE</strong> </td> 
   <td> <p>Wird mit anderen Ausdrücken verwendet, um einen Wert aus einer Liste basierend auf einer Indexnummer auszuwählen. </p>
   <p>Eine Indexnummer ist ein Feld oder eine Funktion, das bzw. die einen numerischen Wert zurückgibt (normalerweise in einem bekannten Bereich).</p> 
   <p>Der Ausdruck ist wie folgt formatiert:</p>
   <p><code>CASE(indexNumber, value1, value2, ...)</code></p>

<p>Der folgende Ausdruck gibt beispielsweise den Namen des Wochentags zurück, wobei 1=Sonntag, 2=Montag usw. in einer berechneten Spalte enthalten ist:</p>

<p><code>CASE(DAYOFWEEK({entryDate}),"Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday")</code></p>

<p>Funktioniert am besten mit anderen Ausdrücken, die eine Zahl zurückgeben, z. B. DAYOFWEEK, DAYOFMONTH und MONTH.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>Verkettet die Zeichenfolge und ist wie folgt formatiert:</p><p><code>CONCAT(string1,"separator", string2)</code></p> <p>Im Folgenden finden Sie Beispiele für Trennzeichen, die Sie einfügen können:</p> 
    <ul> 
     <li>ein Leerzeichen: " "</li> 
     <li>ein Bindestrich: "-"</li> 
     <li>einen Schrägstrich: "/"</li> 
     <li>ein Komma: ","</li> 
     <li>ein Wort: "or", "and"</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>ENTHÄLT</strong> </td> 
   <td>Gibt "true"zurück, wenn die Zeichenfolge findText in der Zeichenfolge in WithinText gefunden und wie folgt formatiert wird:

<p><code>CONTAINS(findText, withinText)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>Maskiert alle Sonderzeichen in der Zeichenfolge, damit sie in ein URL-Argument aufgenommen werden können.<p>Der Ausdruck ist wie folgt formatiert:</p>

<p><code>ENCODEURL(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>Wertet eine von Ihnen angegebene Bedingung aus und gibt den Wert von trueExpression (wahr) bzw. den Wert von falseExpression (falsch) zurück.</p>

<p>Der Ausdruck ist wie folgt formatiert:</p>

<p><code>IF(condition, trueExpression, falseExpression)</code></p>

<p>Sie können beispielsweise zwei verschiedene Datumsfelder vergleichen, gefolgt von einem True-/False-Ergebnis als Datenzeichenfolge:</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","On Track")</code></p>

<p>In der alltäglichen Rede bedeutet diese Aussage: "Wenn das geplante Abschlussdatum meines Objekts "größer als"ist, das geplante Abschlussdatum meines gleichen Objekts, zeigen Sie in diesem Feld die Wörter "Off Track"an; andernfalls zeigen Sie die Wörter "On Track"an."</p>

<p>Wenn Sie die Ausdrücke "true"und "false"nicht beschriften möchten, müssen Sie eine leere Bezeichnung in Ihre Anweisung einfügen, z. B.:</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"","On Track")</code></p> 
   <p>Oder</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","")</code></p>

<p>Weitere Informationen zum Erstellen von "IF"-Anweisungen finden Sie unter <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">"IF"-Anweisungen - Übersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>Ermöglicht die Suche nach einem bestimmten Wert in einer Zeichenfolge möglicher Werte. Wenn der Wert, den Sie suchen, einem der bereitgestellten Werte entspricht, gibt der Ausdruck "trueExpression"zurück. Andernfalls wird "falseExpression"zurückgegeben.</p> 
   <p>Der Ausdruck ist wie folgt formatiert:</p>

<p><code>IFIN(value, value1, value2,..., trueExpression, falseExpression)</code></p>

<p>Sie können beispielsweise einen bestimmten Projekteigentümer finden und diese Projekte mit einem bestimmten Tag in einer Projektansicht markieren: <br><p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")
   </code></p>
    <p> In alltäglicher Rede bedeutet diese Aussage: "Wenn der Projektinhaber Jennifer Campbell oder Rick Kuvec ist, markieren Sie dieses Projekt mit "Marketing-Team"; andernfalls markieren Sie es mit "Andere Teams"."</p> 
    <p> Wenn Sie die Ausdrücke "true"und "false"nicht beschriften möchten, müssen Sie eine leere Bezeichnung in Ihre Anweisung einfügen, z. B.: </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> 
    <p>Oder </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","")</code></p> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>IN</strong> </td> 
   <td> <p>Gibt "true"zurück, wenn der Wert einem der angegebenen Werte entspricht; andernfalls gibt der Ausdruck "false"zurück.</p> <p>Der Ausdruck ist wie folgt formatiert:

</p><p><code>IN(value, value1[, value2...])</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>Gibt "true"zurück, wenn der Wert null oder leer ist. Andernfalls gibt der Ausdruck "false"zurück.</p> <p>Der Ausdruck ist wie folgt formatiert:

</p><p><code>ISBLANK(value)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LINKS</strong> </td> 
   <td> <p>Gibt eine angegebene Anzahl von Zeichen von der linken Seite einer Zeichenfolge zurück und ist wie folgt formatiert:</p>

<p><code>LEFT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>Gibt die Länge einer Zeichenfolge zurück und ist wie folgt formatiert:</p>

<p><code>LEN(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>NIEDRIGER</strong> </td> 
   <td>Gibt die Zeichenfolge in Kleinbuchstaben zurück und ist wie folgt formatiert:

<p><code>LOWER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>ERSETZEN</strong> </td> 
   <td> <p>Ersetzt alle Vorkommen von string2 durch string3 in string1.</p> <p>Der Ausdruck ist wie folgt formatiert:</p>

<p><code>REPLACE(string1, string2, string3)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>RIGHT</strong> </td> 
   <td> <p>Gibt eine angegebene Anzahl von Zeichen von der rechten Seite einer Zeichenfolge zurück und ist wie folgt formatiert:</p>

<p><code>RIGHT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SEARCH</strong> </td> 
   <td> <p>Gibt den Index des ersten Vorkommens von findText in der Zeichenfolge in der Zeichenfolge inText zurück, beginnend bei der angegebenen Startposition, oder -1, wenn der Text nicht gefunden wird.</p> <p>Der Ausdruck ist wie folgt formatiert:</p>

<p><code>SEARCH(findText, withinText, start)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>STRING</strong> </td> 
   <td> <p>Konvertiert eine Zahl in eine Zeichenfolge und ist wie folgt formatiert:</p>

<p><code>STRING(number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>Sortiert eine Liste von Zeichenfolgen in aufsteigender Reihenfolge und ist wie folgt formatiert:</p>

<p><code>SORTASCSTRING(string1, string2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> Sortiert eine Liste von Zeichenfolgen in absteigender Reihenfolge und ist wie folgt formatiert:</p>

<p><code>SORTDESCSTRING(string1, string2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>Gibt Zeichen einer Zeichenfolge basierend auf dem angegebenen Anfangs- und Endindex zurück und ist wie folgt formatiert:</p>

<p><code>SUBSTR({string}, number of start position, number of end position)</code></p> </td> 
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
