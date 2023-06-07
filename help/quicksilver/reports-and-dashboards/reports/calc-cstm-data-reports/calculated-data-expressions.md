---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Berechnete Datenausdrücke
description: Sie können Datenausdrücke verwenden, um berechnete benutzerdefinierte Datenfelder in Adobe Workfront zu definieren. Sie verbinden vorhandene Workfront-Felder in Anweisungen, die ein neues Feld generieren.
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: 18f26f976a47af003817f2f82f8550bdfbc0ab90
workflow-type: tm+mt
source-wordcount: '2368'
ht-degree: 5%

---

# Berechnete Datenausdrücke

Sie können Datenausdrücke verwenden, um berechnete benutzerdefinierte Datenfelder in Adobe Workfront zu definieren. Sie verbinden vorhandene Workfront-Felder in Anweisungen, die ein neues Feld generieren.

Sie können berechnete Datenausdrücke in folgenden Bereichen verwenden:

* Ein benutzerdefiniertes Formular

   Weitere Informationen zum Erstellen von berechneten benutzerdefinierten Datenfeldern für benutzerdefinierte Formulare in Workfront finden Sie unter [Hinzufügen errechneter Daten zu einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* Eine berechnete benutzerdefinierte Spalte in einem Bericht oder einer Liste, wenn Sie den Textmodus verwenden

   Weitere Informationen zur Verwendung des Textmodus in Berichten und Ansichten finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Syntax von berechneten benutzerdefinierten Feldern im Vergleich zu berechneten benutzerdefinierten Spalten

Die von Ihnen verwendeten Funktionen sind zwar identisch, die Syntax für die Erstellung eines Ausdrucks in einem berechneten benutzerdefinierten Feld kann sich jedoch von der für die Erstellung einer berechneten benutzerdefinierten Spalte unterscheiden.

Beispiel:

* In einem benutzerdefinierten Feld würden Sie in einem benutzerdefinierten Formular für Aufgaben den Namen des übergeordneten Projekts der Aufgabe generieren, an das das benutzerdefinierte Formular angehängt ist:

   ```
   {project}.{name}
   ```

* In einer benutzerdefinierten Spalte in einem Bericht können Sie wie folgt eine benutzerdefinierte Spalte für den Projektnamen zu einem Aufgabenbericht hinzufügen:

   ```
   valuefield=project:name
   ```

   Oder

   ```
   valueexpression={project}.{name}
   ```

   >[!TIP]
   >
   >Dieselbe Syntax gilt für alle Berichterstellungselemente im Textmodus, in denen berechnete Ausdrücke verwendet werden: Ansichten, Filter, Gruppierungen, Eingabeaufforderungen.

Die Unterschiede zwischen den beiden Syntaxen sind:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Berechnetes benutzerdefiniertes Feld</strong></td> 
   <td><strong>Berechnetes benutzerdefiniertes Berichtselement</strong></td> 
  </tr> 
   <td>Schließen Sie die Feldnamen in geschweifte Klammern ein.</td> 
   <td>Schließen Sie Feldnamen nicht in Klammern oder Klammern ein, wenn Sie sie in einer <code>valuefield </code>Linie. <p>Fügen Sie Feldnamen in geschweifte Klammern ein, wenn Sie sie in einer <code>valueexpression</code> Linie.</p> </td> 
  </tr> 
  <tr> 
   <td>Trennen Sie die Felder durch Punkte.</td> 
   <td> <p>Trennen Sie die Felder bei Verwendung in einer <code>valuefield </code>line</p> <p>Trennen Sie die Felder bei der Verwendung in einer <code>valueexpression </code>Linie. </p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zur Syntax, die Sie in einer berechneten benutzerdefinierten Spalte verwenden müssen, finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Datenausdrücke, die Sie verwenden können

In den folgenden Listen werden die verfügbaren Ausdrücke definiert, die Sie verwenden können, wenn Sie in Workfront einen der drei Typen berechneter benutzerdefinierter Felder erstellen:

* [Berechnete benutzerdefinierte Felder für Datum und Uhrzeit](#date-time-calculated-custom-fields)
* [Mathematisch berechnete benutzerdefinierte Felder](#mathematical-calculated-custom-fields)
* [Benutzerdefinierte Textfelder](#text-calculated-custom-fields)

### Berechnete benutzerdefinierte Felder für Datum und Uhrzeit {#date-time-calculated-custom-fields}

>[!NOTE]
>
>Wenn Sie eine Datums- und Uhrzeitberechnung erstellen, die keinen Zeitabschnitt enthält oder die Datumsfelder $$TODAY oder $$NOW verwendet, verwendet das System das Datum gemäß der UTC-Zone (Coordinated Universal Time), nicht gemäß Ihrer lokalen Zeitzone. Dies kann zu einem unerwarteten Datumsergebnis führen.

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
   <td> <p>Dieser Ausdruck fügt die Anzahl der Tage zum Datum hinzu. Der Zahlenwert kann Teiltage enthalten (z. B. fügt 1,5 dem Datum anderthalb Tage hinzu).</p> <p>Der Ausdruck ist wie folgt formatiert:</p><pre>ADDDAYS(Datum, Zahl)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>Dieser Ausdruck fügt die Anzahl der Wochentage zum Datum hinzu. Dieser Ausdruck fügt nur ganze ganzzahlige Werte zum Datum hinzu und rundet es ab. </p> <p>Der Ausdruck ist wie folgt formatiert:</p><pre>ADDWEEKDAYS(Datum, Zahl)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>Dieser Ausdruck fügt die Anzahl der Monate zum Datum hinzu und ist wie folgt formatiert:</p><pre>ADDMONTHS(Datum, Zahl)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>Dieser Ausdruck fügt die Anzahl der Jahre zum Datum hinzu und ist wie folgt formatiert:</p><pre>ADDYEARS(Datum, Zahl)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>Dieser Ausdruck löscht den Zeitabschnitt eines Datums und wird wie folgt formatiert: In diesem Beispiel ist das Datum das Eintragsdatum für ein Arbeitsobjekt.</p><pre>CLEARTIME({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATE</strong> </td> 
   <td> <p>Dieser Ausdruck konvertiert eine Zeichenfolge in ein Datum und ist wie folgt formatiert:</p><pre>DATE(Zeichenfolge)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>Dieser Ausdruck gibt die Anzahl der Tage zwischen den beiden Daten zurück, wobei der Start- und Endtag des ausgewählten Zeitraums sowie die Zeitstempel dieser Tage berücksichtigt werden. Wenn die Startzeit des Startdatums beispielsweise 15 Uhr beträgt, wird der Starttag nicht als voller Tag gezählt.</p> <p>Der Ausdruck ist wie folgt formatiert:</p><pre>DATEDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>Dieser Ausdruck gibt den Tag des Monats für das Datum als Zahl zwischen 1 und 31 zurück.</p> <p>Der Ausdruck ist wie folgt formatiert: In diesem Beispiel ist das Datum das Eintragsdatum für ein Arbeitsobjekt.</p><pre>DAYOFMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>Dieser Ausdruck gibt den Wochentag für das Datum als Zahl zwischen 1 (Sonntag) und 7 (Samstag) zurück.</p> <p>Der Ausdruck ist wie folgt formatiert: In diesem Beispiel ist das Datum das Eintragsdatum für ein Arbeitsobjekt.</p><pre>DAYOFWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>Dieser Ausdruck gibt die Gesamtanzahl der Tage im Monat des Datums als Zahl zurück und wird wie folgt formatiert: In diesem Beispiel ist das Datum das Eintragsdatum für ein Arbeitsobjekt.</p><pre>DAYSINMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>Dieser Ausdruck gibt die Gesamtwochentage zwischen dem Datum und dem Ende der Woche bzw. dem Ende des Monats zurück, je nachdem, was zuerst eintritt. In diesem Beispiel ist das Datum das Eintragsdatum für ein Arbeitsobjekt.</p> <p>Der Ausdruck ist wie folgt formatiert:</p><pre>DAYSINSPLITWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>Dieser Ausdruck gibt die Gesamtanzahl der Tage im Jahr des Datums als Zahl zurück und ist wie folgt formatiert: In diesem Beispiel ist das Datum das Eintragsdatum für ein Arbeitsobjekt.</p><pre>DAYSINYEAR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>Dieser Ausdruck gibt das neueste Datum in der Liste zurück und ist wie folgt formatiert:</p><pre>DMAX(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>Dieser Ausdruck gibt das früheste Datum in der Liste zurück und ist wie folgt formatiert:</p><pre>DMIN(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>HOUR</strong> </td> 
   <td> <p>Dieser Ausdruck gibt die Stunde des Datums als Zahl zwischen 0 und 23 zurück.</p> <p>Der Ausdruck ist wie folgt formatiert: In diesem Beispiel ist das Datum das Eintragsdatum für ein Arbeitsobjekt.</p><pre>HOUR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUTE</strong> </td> 
   <td> <p>Dieser Ausdruck gibt die Minute des Datums als Zahl zwischen 0 und 60 zurück, die wie folgt formatiert ist. In diesem Beispiel ist das Datum das Eintragsdatum für ein Arbeitsobjekt.</p><pre>MINUTE({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MONAT</strong> </td> 
   <td> <p>Dieser Ausdruck gibt den Monat des Datums als Zahl zwischen 1 und 12 zurück, formatiert wie folgt. In diesem Beispiel ist das Datum das Eintragsdatum für ein Arbeitsobjekt.</p><pre>MONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SECOND</strong> </td> 
   <td> <p>Dieser Ausdruck gibt die Sekunde des Datums als Zahl zwischen 0 und 60 zurück, die wie folgt formatiert ist. In diesem Beispiel ist das Datum das Eintragsdatum für ein Arbeitsobjekt.</p><pre>SECOND({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>Dieser Ausdruck gibt die Anzahl der Wochentage zwischen zwei Daten zurück, wobei der Start- und Endtag des ausgewählten Zeitraums sowie die Zeitstempel dieser Tage berücksichtigt werden. Wenn die Startzeit des Startdatums beispielsweise 15 Uhr beträgt, wird der Starttag nicht als voller Tag gezählt.</p> <p>Der Ausdruck ist wie folgt formatiert:</p><pre>WEEKDAYDIFF(date2, date1)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>Dieser Ausdruck gibt die Anzahl der geplanten Minuten zwischen den Daten gemäß dem Standardzeitplan zurück.</p> <p>Der Ausdruck ist wie folgt formatiert:</p><pre>WORKMINUTESDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>JAHR</strong> </td> 
   <td> <p>Dieser Ausdruck gibt das Jahr des Datums als vierstellige Zahl zurück, die wie folgt formatiert ist. In diesem Beispiel ist das Datum das Eintragsdatum für ein Arbeitsobjekt.</p><pre>YEAR({entryDate})</pre> </td> 
  </tr> 
 </tbody> 
</table>

### Mathematisch berechnete benutzerdefinierte Felder {#mathematical-calculated-custom-fields}

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
   <td>Dieser Ausdruck gibt den absoluten Wert der Zahl zurück und ist wie folgt formatiert. In diesem Beispiel wird die Anzahl der Objekte unter dem Objekt verwendet, an das das benutzerdefinierte Formular angehängt ist.<pre>ABS({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>AVERAGE</strong> </td> 
   <td>Dieser Ausdruck gibt den Durchschnitt der Zahlen zurück und ist wie folgt formatiert:<pre>DURCHSCHNITT(Zahl1, Zahl2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>Dieser Ausdruck rundet eine Zahl auf die nächste Ganzzahl auf und ist wie folgt formatiert: In diesem Beispiel wird die Anzahl der Objekte unter dem Objekt verwendet, an das das benutzerdefinierte Formular angehängt ist.<pre>CEIL({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>Dieser Ausdruck teilt alle Zahlen in der angegebenen Reihenfolge und ist wie folgt formatiert:<pre>DIV(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>Dieser Ausdruck rundet eine Zahl auf die nächste Ganzzahl ab und ist wie folgt formatiert: In diesem Beispiel wird die Anzahl der Objekte unter dem Objekt verwendet, an das das benutzerdefinierte Formular angehängt ist.<pre>FLOOR({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>Dieser Ausdruck gibt den natürlichen Logarithmuswert der Zahl zurück und ist wie folgt formatiert:<pre>LN({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>Dieser Ausdruck gibt den Logarithmuswert von number2 an die Basisnummer1 zurück und ist wie folgt formatiert:<pre>LOG(Zahl1, Zahl2)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>MAX</strong> </td> 
   <td>Dieser Ausdruck gibt das größte Element in der Liste zurück und ist wie folgt formatiert:<pre>MAX(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>MIN</strong> </td> 
   <td>Dieser Ausdruck gibt das kleinste Element in der Liste zurück und ist wie folgt formatiert:<pre>MIN(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ZAHL</strong> </td> 
   <td>Dieser Ausdruck konvertiert eine Zeichenfolge in eine Zahl und ist wie folgt formatiert:<pre>NUMBER(Zeichenfolge)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>Dieser Ausdruck gibt eine Zahl zurück, die an einen Strom erhöht wird, und ist wie folgt formatiert:<pre>POWER(Zahl, Potenz)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>Dieser Ausdruck multipliziert alle Zahlen und ist wie folgt formatiert:<pre>PROD(number1, number2, ....</pre>
   <b>NOTIZ</b>

Stellen Sie beim Multiplizieren von Feldern, die Stunden enthalten, sicher, dass Sie verstehen, ob die Stunden in den ausgewählten Feldern in Minuten, Stunden oder Sekunden in der Datenbank gespeichert werden. Wenn die Stunden in Minuten oder Sekunden gespeichert, aber in Stunden auf der Workfront-Oberfläche angezeigt werden, müssen Sie beim Schreiben eines Ausdrucks mithilfe dieser Berechnung möglicherweise die Konvertierung von Minuten oder Sekunden in Stunden berücksichtigen.
</td> 
  </tr> 
  <tr> 
   <td><strong>ROUND</strong> </td> 
   <td>Dieser Ausdruck rundet die Zahl auf eine angegebene Dezimalzahl auf und ist wie folgt formatiert:<p>ROUND(Zahl, Genauigkeit)</p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> Dieser Ausdruck ordnet die Zahlen in aufsteigender Reihenfolge an und ist wie folgt formatiert:</p><pre>SORTASCNUM(number1,number2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>Dieser Ausdruck ordnet die Zahlen in absteigender Reihenfolge an und ist wie folgt formatiert:<pre>SORTDESCNUM(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>Dieser Ausdruck gibt eine Quadratwurzel einer Zahl zurück und ist wie folgt formatiert: In diesem Beispiel wird die Anzahl der Objekte unter dem Objekt verwendet, an das das benutzerdefinierte Formular angehängt ist.</p><pre>SQRT({numberOfChildren})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>Dieser Ausdruck subtrahiert alle Zahlen in der angegebenen Reihenfolge und ist wie folgt formatiert:<pre>SUB(Zahl1, Zahl2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SUM</strong> </td> 
   <td>Dieser Ausdruck fügt alle Zahlen hinzu und ist wie folgt formatiert:<pre>SUM(number1, number2, ...)</pre></td> 
  </tr> 
 </tbody> 
</table>

### Benutzerdefinierte Textfelder {#text-calculated-custom-fields}

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
   <td> <p>Dieser Ausdruck wird zusammen mit anderen Ausdrücken verwendet, um einen Wert aus einer Liste basierend auf einer Indexnummer auszuwählen. Eine Indexnummer ist ein Feld oder eine Funktion, das bzw. die einen numerischen Wert zurückgibt (normalerweise in einem bekannten Bereich).</p> <p>Der Ausdruck ist wie folgt formatiert:</p><pre>CASE(indexNumber, value1, value2, ...)</pre> <p>Der folgende Ausdruck gibt beispielsweise den Namen des Wochentags zurück, wobei 1=Sonntag, 2=Montag usw. in einer berechneten Spalte enthalten ist:</p><pre>CASE(DAYOFWEEK({entryDate}),"Sunday","Monday","Dienstag","Mittwoch","Donnerstag","Freitag","Samstag")</pre> <p>Dieser Ausdruck eignet sich am besten für andere Ausdrücke, die eine Zahl zurückgeben, z. B. DAYOFWEEK, DAYOFMONTH und MONTH.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>ZUSAMMENFÜGEN</strong> </td> 
   <td> <p>Dieser Ausdruck verkettet die Zeichenfolge und ist wie folgt formatiert:</p><pre>CONCAT(string1,"separator", string2)</pre> <p>Im Folgenden finden Sie Beispiele für Trennzeichen, die Sie einfügen können:</p> 
    <ul> 
     <li>ein Leerzeichen: " " "</li> 
     <li>einen Bindestrich: "-"</li> 
     <li>einen Schrägstrich: "/"</li> 
     <li>ein Komma: ","</li> 
     <li>ein Wort: "or", "and"</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>CONTAINS</strong> </td> 
   <td>Dieser Ausdruck gibt "true"zurück, wenn die Zeichenfolge "findText"in der Zeichenfolge in WithinText gefunden und wie folgt formatiert wird:<pre>CONTAINS(findText, withinText)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>Dieser Ausdruck maskiert alle Sonderzeichen in der Zeichenfolge, sodass sie in ein URL-Argument aufgenommen werden können.<p>Der Ausdruck ist wie folgt formatiert:</p><pre>ENCODEURL(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>Dieser Ausdruck wertet eine von Ihnen angegebene Bedingung aus und gibt den Wert von trueExpression (wahr) bzw. den Wert von falseExpression (falsch) zurück.</p> <p>Der Ausdruck ist wie folgt formatiert:</p><pre>IF(condition, trueExpression, falseExpression)</pre> <p>Sie können beispielsweise zwei verschiedene Datumsfelder vergleichen, gefolgt von einem True-/False-Ergebnis als Datenzeichenfolge:</p><pre>IF({forecastCompletionDate}&gt;{scheduledCompletionDate},"Off Track","On Track")</pre> <p>Diese Aussage bedeutet im Alltag: "Wenn das geplante Abschlussdatum meines Objekts "größer als"das geplante Abschlussdatum meines Objekts ist, zeigen Sie in diesem Feld die Wörter "Off Track"an. andernfalls die Wörter "Auf Track"anzeigen.</p> <p>Wenn Sie die Ausdrücke "true"und "false"nicht beschriften möchten, müssen Sie eine leere Bezeichnung in Ihre Anweisung einfügen, z. B.:</p><pre>IF({estimatedCompletionDate}&gt;{scheduledCompletionDate},"","On Track")</pre> <p>Oder</p><pre>IF({forecastCompletionDate}&gt;{scheduledCompletionDate},"Off Track","")</pre> <p>Weitere Informationen zum Erstellen von "IF"-Anweisungen finden Sie unter <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">Übersicht über "IF"-Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>Mit diesem Ausdruck können Sie in einer Zeichenfolge möglicher Werte nach einem bestimmten Wert suchen. Wenn der gesuchte Wert einem der bereitgestellten Werte entspricht, gibt der Ausdruck "trueExpression"zurück. Andernfalls wird falseExpression zurückgegeben.</p> <p>Der Ausdruck ist wie folgt formatiert:</p><pre>IFIN(value, value1, value2,..., trueExpression, falseExpression)</pre> <p>Sie können beispielsweise einen bestimmten Projekteigentümer finden und diese Projekte mit einem bestimmten Tag in einer Projektansicht markieren: <br><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")</code></p> <p> Diese Aussage bedeutet im Alltag: "Wenn der Projektinhaber Jennifer Campbell oder Rick Kuvec ist, markieren Sie dieses Projekt mit "Marketing-Team". andernfalls markieren Sie es mit "Andere Teams".</p> <p> Wenn Sie die Ausdrücke "true"und "false"nicht beschriften möchten, müssen Sie eine leere Bezeichnung in Ihre Anweisung einfügen, z. B.: </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> <p>Oder </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team",""</code> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>IN</strong> </td> 
   <td> <p>Dieser Ausdruck gibt "true"zurück, wenn der Wert einem der bereitgestellten Werte entspricht. sonst gibt der Ausdruck "false"zurück.</p> <p>Der Ausdruck ist wie folgt formatiert:</p><pre>IN(Wert, Wert1[, Wert2...])</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>Dieser Ausdruck gibt "true"zurück, wenn der Wert null oder leer ist. sonst gibt der Ausdruck "false"zurück.</p> <p>Der Ausdruck ist wie folgt formatiert:</p><pre>ISBLANK(value)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LINKS</strong> </td> 
   <td> <p>Dieser Ausdruck gibt eine angegebene Anzahl von Zeichen von der linken Seite einer Zeichenfolge zurück und ist wie folgt formatiert:</p><pre>LEFT(Zeichenfolge, Länge)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>Dieser Ausdruck gibt die Länge einer Zeichenfolge zurück und ist wie folgt formatiert:</p><pre>LEN(Zeichenfolge)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LOWER</strong> </td> 
   <td>Dieser Ausdruck gibt die Zeichenfolge in Kleinbuchstaben zurück und ist wie folgt formatiert:<pre>LOWER(Zeichenfolge)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ERSETZEN</strong> </td> 
   <td> <p>Dieser Ausdruck ersetzt alle Vorkommen von string2 durch string3 in string1.</p> <p>Der Ausdruck ist wie folgt formatiert:</p><pre>REPLACE(Zeichenfolge1, Zeichenfolge2, Zeichenfolge3)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>RECHTS</strong> </td> 
   <td> <p>Dieser Ausdruck gibt eine angegebene Anzahl von Zeichen von der rechten Seite einer Zeichenfolge zurück und ist wie folgt formatiert:</p><pre>RIGHT(Zeichenfolge, Länge)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SEARCH</strong> </td> 
   <td> <p>Dieser Ausdruck gibt den Index des ersten Vorkommens von findText in der Zeichenfolge innerhalbText zurück, beginnend bei der angegebenen Startposition, oder -1, wenn der Text nicht gefunden wird.</p> <p>Der Ausdruck ist wie folgt formatiert:</p><pre>SEARCH(findText, inText, start)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ZEICHENFOLGE</strong> </td> 
   <td> <p>Dieser Ausdruck konvertiert eine Zahl in eine Zeichenfolge und ist wie folgt formatiert:</p><pre>STRING(number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>Dieser Ausdruck sortiert eine Liste von Zeichenfolgen in aufsteigender Reihenfolge und ist wie folgt formatiert:</p><pre>SORTASCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> Dieser Ausdruck sortiert eine Liste von Zeichenfolgen in absteigender Reihenfolge und ist wie folgt formatiert:</p><pre>SORTDESCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>Dieser Ausdruck gibt Zeichen einer Zeichenfolge basierend auf dem angegebenen Anfangs- und Endindex zurück und ist wie folgt formatiert:</p><pre>SUBSTRG({string}, Anzahl der Startposition, Anzahl der Endposition)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>Dieser Ausdruck entfernt Leerzeichen vom Anfang und Ende einer Zeichenfolge und ist wie folgt formatiert:</p><pre>TRIM(Zeichenfolge)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>Dieser Ausdruck gibt eine Zeichenfolge in Großbuchstaben zurück und ist wie folgt formatiert:</p><pre>UPPER(Zeichenfolge)</pre> </td> 
  </tr> 
 </tbody> 
</table>
