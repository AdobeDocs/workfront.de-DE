---
product-area: reporting
navigation-topic: text-mode-reporting
title: Übersicht über die Syntax der Textmodi
description: Sie können die Textmodus-Oberfläche verwenden, um komplexere Ansichten, Filter, Gruppierungen und benutzerdefinierte Eingabeaufforderungen in Listen und Berichten zu erstellen. Mithilfe des Textmodus können Sie auf Felder und deren Attribute zugreifen, die in der Benutzeroberfläche des Standardmodus nicht verfügbar sind.
author: Nolan
feature: Reports and Dashboards
role: User
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '1862'
ht-degree: 0%

---

# Übersicht über die Syntax der Textmodi

<!--Audited: 12/2023-->

Sie können die Textmodus-Oberfläche verwenden, um komplexere Ansichten, Filter, Gruppierungen und benutzerdefinierte Eingabeaufforderungen in Listen und Berichten zu erstellen. Mithilfe des Textmodus können Sie auf Felder und deren Attribute zugreifen, die in der Benutzeroberfläche des Standardmodus nicht verfügbar sind.

Informationen und Überlegungen zum Textmodus vor dem Start finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Eine vollständige Liste aller unserer berichtspflichtigen Felder und ihrer Attribute finden Sie in der [API-Explorer](../../../wf-api/general/api-explorer.md).

Weitere Informationen zum Erstellen von Berichten im Textmodus, einschließlich Klassen, Videos und Tutorials, finden Sie im Abschnitt &quot;Lernen&quot;auf der Adobe Experience League-Site.

## Überlegungen zur Syntax des Textmodus

* Sie müssen die Adobe Workfront-Syntax verstehen, bevor Sie mit der Erstellung von Berichterstellungselementen im Textmodus beginnen können. Die Workfront-Syntax für den Textmodus ist für diese Anwendung eindeutig und weist eindeutige Merkmale auf, mit denen Sie vertraut sein müssen.
* Bevor Sie mit der Verwendung des Textmodus in Ihren Berichten beginnen, empfehlen wir dringend, unsere Klassen für erweiterte Berichte zu verwenden, um ein tieferes Verständnis unserer Textmodussprache zu erhalten. <!--outdated link: For training materials on reporting see [Workfront Reports and Dashboards Learning Paths](https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ).-->
* Sie können Ansichten, Filter und Gruppierungen mithilfe der Benutzeroberfläche des Standardmodus anpassen. Sie können jedoch nur im Textmodus benutzerdefinierte Eingabeaufforderungen erstellen.

## Allgemeine Richtlinien zum Erstellen von Berichterstellungselementen im Textmodus

Die folgenden allgemeinen Richtlinien gelten beim Erstellen von Berichterstellungs- oder Listenelementen im Textmodus:

* Verwenden Sie beim Referenzieren von Objekten oder Attributen in der Workfront-Datenbank immer die Binnenmajuskel-Schreibweise.
* Beachten Sie die Hierarchie der Objekte in Workfront. Die folgenden Unterschiede bestehen zwischen Ansichten, Filtern und Gruppierungen:

   * Sie können ein Objekt anzeigen, das sich in einer Ansicht aus drei Objekten außerhalb des Berichts oder Listenobjekts befindet.
   * Sie können in einer Gruppierungs-, Filter- oder benutzerdefinierten Eingabeaufforderung nicht auf Objekte verweisen, die mehr als zwei Objekte vom Hauptobjekt entfernt sind.

  **Beispiel:** Sie können den Namen oder die GUID des Portfolio-Eigentümers in einer Aufgabenansicht anzeigen:


  `valuefield=project:portfolio:ownerID`

  Sie können in einer Aufgabenansicht keine Portfolio Owner gruppieren, filtern oder auffordern:

  `project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa`


  In diesen Beispielen befindet sich die Portfolio Owner ID drei Objekte vom Listenobjekt entfernt.

  Informationen zur Hierarchie von Objekten in Workfront finden Sie unter:

   * [Objekte in Adobe Workfront verstehen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
   * [API-Explorer](../../../wf-api/general/api-explorer.md)

* Verwenden Sie nach Möglichkeit Platzhalter, um Ihre Berichte und Listen dynamischer zu gestalten und zu vermeiden, dass sie für verschiedene Benutzer und ähnliche Zeitpläne dupliziert werden.

## Überblick über Fälle in Camel

Beim Referenzieren von Workfront-Feldern oder ihren Attributen im Textmodus müssen Sie in Workfront deren Namen in Binnenmajuskel-Schreibweise eingeben. In diesem Fall werden die Felder mit einem Namen in Kleinbuchstaben geschrieben. Zusammengesetzte Felder werden nach folgendem Muster geschrieben:

`camelCaseSyntax`

>[!IMPORTANT]
>
>Alle Berichterstellungselemente folgen diesem Groß-/Kleinschreibung.

Die Eigenschaften des Kamelschachtes sind:

* Das erste Wort beginnt immer mit einem Kleinbuchstaben.
* Die folgenden Wörter beginnen immer mit einem Großbuchstaben.
* Zwischen den Wörtern gibt es keine Leerzeichen.

**Beispiel:** Um auf das tatsächliche Abschlussdatum eines Projekts zu verweisen, lautet der Name des Felds, das Sie beim Erstellen von Berichterstellungselementen im Textmodus verwenden würden:

`actualCompletionDate`

## Textmodussyntax für verschiedene Berichterstellungselemente

Die folgenden Syntaxsätze der unten aufgeführten Berichterstellungselemente weisen bei ihrer Erstellung im Textmodus Ähnlichkeiten auf:

* Die Zeilen des Codes und der Syntax sind für Ansichten und Gruppierungen ähnlich.

  Informationen zu den wichtigsten Codezeilen für Ansichten und Gruppierungen beim Erstellen im Textmodus finden Sie unter:

   * [Bearbeiten einer Ansicht im Textmodus](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
   * [Textmodus in einer Gruppierung bearbeiten](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* Die Codezeilen und die Syntax sind für Filter und benutzerdefinierte Eingabeaufforderungen ähnlich.

  Weitere Informationen finden Sie unter

   * [Filter im Textmodus bearbeiten](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
   * [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### Syntax für Ansichten und Gruppierungen

Die Codezeilen beim Erstellen von Ansichten und Gruppierungen sind ähnlich.

Informationen zum Erstellen von Ansichten und Gruppierungen finden Sie in den folgenden Artikeln:

* [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Gruppierungsübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

Die wichtigste Codezeile für eine Ansicht oder Gruppierung ist die Zeile, die das in der Ansichtsspalte oder in der Gruppierung referenzierte Objekt angibt. Diese Codezeile kann mit `valuefield` oder `valueexpression` je nachdem, ob dieses Feld eine direkte Referenz zu einem Workfront-Datenbankfeld oder eine Berechnung zwischen mehreren Feldern ist.

In der folgenden Tabelle sind die gängigsten Codezeilen in einer Ansicht oder Gruppierung aufgeführt:

| Codezeile | Beschreibung |
|-----------------|------------------------------------------------------------------------------------------------------------------------------|
| `valuefield` | Identifiziert das in der Ansichtsspalte oder Gruppierung referenzierte Objekt. Dies ist ein direkter Verweis auf das referenzierte Objekt. |
| `valueexpression` | Identifiziert das in der Ansichtsspalte oder Gruppierung referenzierte Objekt. Dies ist eine Berechnung zwischen mehreren Feldern. |
| `valueformat` | Gibt das Format an, in dem Workfront den Wert zurückgibt, der in den Ausdruckszeilen &quot;value&quot;oder &quot;value&quot;angegeben ist. |
| `width` | Gibt die Breite einer Spalte in Pixel an. |
| `stretch` | Gibt an, welche Spalten zusätzlichen Speicherplatz belegen, der für die Ansicht nicht benötigt wird. |

>[!TIP]
>
>* Obwohl die Codezeilen in den Beispielen unten zwischen Ansichten und Gruppierungen ähnlich sind, sollten Sie immer daran denken, dass jede Codezeile für eine Gruppierung mit der Gruppierungsnummer beginnt.
>
>  Um in einer Projektliste oder einem Bericht nach Projektname zu gruppieren, verwenden Sie die folgende Zeile für die Gruppierung der ersten Ebene:
>
>  `group.0.valuefield=name`
>  
>* Wenn Sie mehrere Spalten in einer Ansicht in derselben Spalte bearbeiten (wie es bei gemeinsamen Spalten der Fall ist), beachten Sie, dass jede Codezeile für jede Spalte mit der Spaltennummer beginnt.
>
>  Verwenden Sie das folgende Format, um die erste Spalte einer Ansicht zu identifizieren:
>
>  `column.0.valuefield=name`
>  
>  Informationen zum Freigeben von Spalten finden Sie unter [Ansicht: Zusammenführen von Informationen aus mehreren Spalten in einer gemeinsamen Spalte](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).
>

#### `Valuefield` Syntaxübersicht für Ansichten und Gruppierungen

`Valuefield=` ist eine Schlüsselzeile des Codes in Ansichten und Gruppierungen, die das Objekt identifiziert, auf das Sie direkt verweisen.

Die Syntax für direkt referenzierende Felder ist für Gruppierungen und Ansichten identisch.

Die folgenden Regeln gelten für das Referenzieren von Workfront-Objekten mithilfe eines `valuefield` Linie:

* Verwenden Sie die Binnenmajuskel-Groß-/Kleinschreibung, um direkt auf Felder zu verweisen.

  **Beispiel:** Verwenden Sie die folgende Zeile, um auf das tatsächliche Abschlussdatum der Aufgabe in einer Aufgabenansicht zu verweisen:

  `valuefield=actualCompletionDate`

* Verwenden Sie die Groß-/Kleinschreibung und Doppelpunkte, um Felder zu trennen, die für dasselbe Objekt miteinander in Beziehung stehen.

  **Beispiel:** Verwenden Sie die folgende Zeile, um auf das geplante Abschlussdatum des Projekts in einer Aufgabenansicht zu verweisen:

  `valuefield=project:plannedCompletionDate`

  Informationen dazu, wie Objekte in der Workfront-Datenbank aufeinander verweisen, finden Sie in der [API-Explorer](../../../wf-api/general/api-explorer.md).

* Verwenden Sie beim Referenzieren eines benutzerdefinierten Felds den Namen des Felds genau so, wie er in der Benutzeroberfläche angezeigt wird.

  **Beispiel:** Verwenden Sie die folgende Zeile, um auf ein benutzerdefiniertes Projekt mit der Bezeichnung Zusätzliche Details in einer Aufgabenansicht zu verweisen:

  `valuefield=project:Additional Details`

#### `Valueexpression` Syntaxübersicht für Ansichten und Gruppierungen

Sie können die `valuefield=` Codezeile mit `valueexpression=` beim Erstellen von Ansichten und Gruppierungen im Textmodus, wenn Sie eine Berechnung zwischen zwei oder mehr Feldern referenzieren möchten.

>[!TIP]
>
>Sie können berechnete Felder erstellen, die in Berichten angezeigt werden können. Berechnete Ansichten und Gruppierungen sind jedoch dynamischer. Berechnete Ansichten und Gruppierungen werden jedes Mal, wenn Sie den Bericht ausführen oder eine Liste anzeigen, mit neuen Informationen aktualisiert.
>
>Informationen zum Erstellen berechneter Spalten in einer Ansicht finden Sie unter [Berechnete benutzerdefinierte Felder vs. berechnete Spalten](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Das Erstellen einer berechneten Gruppierung ähnelt dem Erstellen einer berechneten Spalte in einer Ansicht.

Die folgenden Regeln gelten für das Referenzieren von Workfront-Objekten mithilfe eines `valueexpression` Linie:

* Verwenden Sie die Binnenmajuskel-Schreibweise, um direkt auf Felder zu verweisen und jedes Feld in geschweifte Klammern einzuschließen.

  **Beispiel:** So zeigen Sie das Feld &quot;Task Name&quot;in einer Aufgabenspalte an: `valueexpression`verwenden Sie die folgende Zeile:

  `valueexpression={name}`


* Verwenden Sie Kamelgehäuse und Punkte, um miteinander verknüpfte Felder voneinander zu trennen.

  **Beispiel:** Verwenden Sie die folgenden Zeilen, um den Namen eines mit dem Namen der Aufgabe verknüpften Projekts in einem Aufgabenbericht anzuzeigen:

   * In einer Ansicht:

     `valueexpression=CONCAT({project}.{name},' - ',{name})`

   * Gruppierung:

     `group.0.valueexpression=CONCAT({project}.{name},' - ',{name})`

  Informationen dazu, wie Objekte in der Workfront-Datenbank aufeinander verweisen, finden Sie in der [API-Explorer](../../../wf-api/general/api-explorer.md).

* Verwenden Sie beim Referenzieren eines benutzerdefinierten Felds die folgenden Regeln:

   * Verwenden Sie den Namen des Felds genau so, wie er in der Benutzeroberfläche angezeigt wird.
   * Stellen Sie dem Namen des Felds &quot;DE:&quot;voran.
   * Schließen Sie das Feld in geschweifte Klammern ein.
   * Trennen Sie die mit dem Objekt verknüpften Felder durch Punkte.

  **Beispiel:** Verwenden Sie die folgende Zeile, um das benutzerdefinierte Feld für das Projekt &quot;Zusätzliche Details&quot;in einer Aufgabenansicht in einer Ausdruckszeile für Werte anzuzeigen:

  `valueexpression={project}.{DE:Additional Details}`

* Sie können einen Platzhalter in einem `valueexpression` aber nicht in `valuefield` Linie.

  Weitere Informationen zu Platzhaltern finden Sie unter [Übersicht über Wildcard-Filtervariablen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).


#### `Valueformat` Übersicht über Ansichten und Gruppierungen

Die zweitwichtigste Codezeile in einer Ansicht oder Gruppierung ist die `valueformat=` Linie. Dies teilt Workfront mit, in welchem Format Sie den Wert zurückgeben möchten, den Sie im `valuefield` oder `valueexpression` Zeilen. Sie können zwar verschiedene Formate für die `valueformat` empfiehlt es sich, bei der Verwendung von `valueexpression`:

`valueformat=HTML`

Für zusätzliche `valueformat` -Werte, siehe auch die folgenden Artikel:

* [Datumsangaben in Textmodusberichten formatieren](../../reports/text-mode/format-dates-in-text-mode-reports.md)
* [Formatnummern, Währungs- und Prozentwerte in Textmodusberichten](../../reports/text-mode/format-numbers-in-text-mode-reports.md)

#### `width` Übersicht über Ansichten

`width=` ist die Codezeile, in der Sie die Breite jeder Spalte in Pixel angeben können. Workfront bietet für jedes Feld eine empfohlene Breite. Je nach Feldtyp und -format können Sie jedoch Anpassungen vornehmen.

Sie müssen die zusätzliche `usewidths=true` Codezeile, um die für die Spalte angegebene Breite zu erzwingen.

**Beispiel:** Verwenden Sie die folgenden Zeilen, um eine Spalte mit einer Breite von 80 Pixel anzuzeigen:

`width=80`

`usewidths=true`

#### `stretch` Übersicht über Ansichten

Die `stretch` wird verwendet, um zu ermitteln, welche Spalten zusätzlichen Platz belegen, der für die Ansicht nicht benötigt wird. Die Breite der Benutzeroberfläche des Arbeitsbereichs für einen typischen Benutzer beträgt etwa 850 Pixel. Das bedeutet, dass Ihre Ansicht bei einer Ansicht mit vier Spalten (jeweils 150 Pixel) 600 von 850 Pixel umfasst. Die Benutzeroberfläche enthält 250 zusätzliche Pixel, die zu den Spalten hinzugefügt werden, für die ein gestreckter Prozentsatz bereitgestellt wird.

Der Abschnitt einer Spalte wird erzwungen, wenn Sie die zusätzliche Codezeile verwenden: `usewidths=true` für mindestens eine der Spalten in der Ansicht.

**Beispiel:** Verwenden Sie die folgenden Zeilen, um anzugeben, dass eine Spalte 70 % des leeren Bereichs in einer Ansicht verwenden kann:

`stretch=70`

`usewidths=true`

### Syntax für Filter und benutzerdefinierte Eingabeaufforderungen

Die Syntax zum Erstellen von Filtern ähnelt der zum Erstellen von benutzerdefinierten Aufforderungen.

>[!TIP]
>
>Sie können eine benutzerdefinierte Eingabeaufforderung erstellen, indem Sie zunächst einen Filter für die Anweisung erstellen, die Sie in die Eingabeaufforderung aufnehmen möchten. Verbinden Sie alle Codezeilen in einem Filter mit &quot;&amp;&quot;ohne Leerzeichen zwischen den Zeilen und der benutzerdefinierten Eingabeaufforderung.

Informationen zum Erstellen von Filtern und benutzerdefinierten Eingabeaufforderungen finden Sie unter:

* [Filterübersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

Informationen zum Erstellen von Filtern im Textmodus finden Sie unter [Filter im Textmodus bearbeiten](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

Sie können die folgenden Elemente verwenden, um Filter und benutzerdefinierte Eingabeaufforderungen im Textmodus zu erstellen:

* Eine Codezeile, die auf das Objekt der Filteranweisung verweist. Verwenden Sie die Binnenmajuskel-Schreibweise für das Filterobjekt.
* Eine Codezeile, die auf das Filterobjekt und den Modifikator für den Wert des Filterobjekts verweist. Verwenden Sie für das Filterobjekt in dieser Zeile die Binnenmajuskel-Schreibweise.

  >[!TIP]
  >
  >Beim Referenzieren von Bereichen sind dafür 2 Modifikatorlinien erforderlich.

* Ein Statement-Connector, der mehrere Filteranweisungen verbindet:

   * UND

     Dies ist der Standard-Connector zwischen Filteranweisungen.

   * ODER

     >[!TIP]
     >
     >Bei Anweisungs-Connectoren wird zwischen Groß- und Kleinschreibung unterschieden. &quot;AND&quot;kann im Textmodus weggelassen werden.

* Platzhalter, um Filter dynamischer zu gestalten und für die aktuelle Zeit oder den angemeldeten Benutzer anzupassen. Weitere Informationen zu Platzhaltern finden Sie unter [Übersicht über Wildcard-Filtervariablen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).
