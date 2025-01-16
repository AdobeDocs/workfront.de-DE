---
product-area: reporting
navigation-topic: text-mode-reporting
title: Übersicht über die Textmodussyntax
description: Sie können die Benutzeroberfläche des Textmodus verwenden, um komplexere Ansichten, Filter, Gruppierungen und benutzerdefinierte Eingabeaufforderungen in Listen und Berichten zu erstellen. Durch die Verwendung des Textmodus können Sie auf Felder und ihre Attribute zugreifen, die nicht in der Standardmodus-Benutzeroberfläche verfügbar sind.
author: Nolan
feature: Reports and Dashboards
role: User
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '1862'
ht-degree: 0%

---

# Übersicht über die Textmodussyntax

<!--Audited: 1/2025-->

Sie können die Benutzeroberfläche des Textmodus verwenden, um komplexere Ansichten, Filter, Gruppierungen und benutzerdefinierte Eingabeaufforderungen in Listen und Berichten zu erstellen. Durch die Verwendung des Textmodus können Sie auf Felder und ihre Attribute zugreifen, die nicht in der Standardmodus-Benutzeroberfläche verfügbar sind.

Informationen und Überlegungen zum Textmodus vor dem Start finden Sie unter [Übersicht über den Textmodus](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Eine vollständige Liste aller unserer berichtspflichtigen Felder und ihrer Attribute finden Sie im [API-Explorer](../../../wf-api/general/api-explorer.md).

Weitere Informationen zum Erstellen von Berichten im Textmodus, einschließlich Klassen, Videos und Tutorials, finden Sie im Abschnitt Lernen auf der Adobe Experience League-Site.

## Überlegungen zur Textmodussyntax

* Sie müssen die Adobe Workfront-Syntax verstehen, bevor Sie mit dem Erstellen von Berichterstellungselementen im Textmodus beginnen können. Die Workfront-Syntax für den Textmodus ist in dieser Anwendung eindeutig und weist eindeutige Merkmale auf, mit denen Sie vertraut sein müssen.
* Bevor Sie mit der Verwendung des Textmodus in Ihren Berichten beginnen, empfehlen wir Ihnen dringend, unsere Kurse über erweiterte Berichte zu absolvieren, um ein tieferes Verständnis unserer Textmodussprache zu erhalten.
* Sie können Ansichten, Filter und Gruppierungen über die Standardmodus-Benutzeroberfläche anpassen. Sie können jedoch benutzerdefinierte Eingabeaufforderungen nur im Textmodus erstellen.

## Allgemeine Richtlinien zum Erstellen von Berichterstellungselementen im Textmodus

Im Folgenden finden Sie allgemeine Richtlinien zum Erstellen von Reporting- oder Listenelementen im Textmodus:

* Verwenden Sie immer Groß-/Kleinschreibung beim Referenzieren von Objekten oder Attributen in der Workfront-Datenbank.
* Beachten Sie die Objekthierarchie in Workfront. Die folgenden Unterschiede bestehen zwischen Ansichten, Filtern und Gruppierungen:

   * Sie können ein -Objekt anzeigen, das drei Objekte vom Bericht entfernt ist, oder ein Listenobjekt in einer Ansicht.
   * Sie können in einer Gruppierungs-, Filter- oder benutzerdefinierten Eingabeaufforderung nicht auf Objekte verweisen, die mehr als zwei Objekte vom Hauptobjekt entfernt sind.

  **Beispiel** Sie können den Namen oder die GUID des Portfolio-Inhabers in einer Aufgabenansicht anzeigen:

  `valuefield=project:portfolio:ownerID`

  Sie können den Verantwortlichen für das Portfolio nicht in einer Aufgabenansicht gruppieren, filtern oder dazu auffordern:

  `project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa`

  In diesen Beispielen ist die Portfolio-Eigentümer-ID drei Objekte vom Objekt der Liste entfernt.

  Informationen zur Objekthierarchie in Workfront finden Sie unter:

   * [Verstehen von Objekten in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
   * [API Explorer](../../../wf-api/general/api-explorer.md)

* Verwenden Sie nach Möglichkeit Platzhalter, um Ihre Berichte und Listen dynamischer zu gestalten und um zu vermeiden, dass sie für verschiedene Benutzer und ähnliche Timelines dupliziert werden.

## Fallübersicht

Beim Referenzieren von Workfront-Feldern oder deren Attributen im Textmodus verlangt Workfront, dass Sie deren Namen in Binnenmajuskel-Schreibweise eingeben. In diesem Fall werden die Felder mit dem einzelnen Namen in Kleinbuchstaben geschrieben. Zusammengesetzte Felder werden nach dem folgenden Muster geschrieben:

`camelCaseSyntax`

>[!IMPORTANT]
>
>Alle Berichtselemente folgen diesem Groß-/Kleinschreibung.

Die Merkmale des Camel Case sind:

* Das erste Wort beginnt immer mit einem Kleinbuchstaben.
* Die folgenden Wörter beginnen immer mit einem Großbuchstaben.
* Zwischen den Wörtern gibt es keine Leerzeichen.

**Beispiel** Um auf das tatsächliche Abschlussdatum eines Projekts zu verweisen, würde der Name des Felds, den Sie beim Erstellen von Berichtselementen im Textmodus verwenden würden, lauten

`actualCompletionDate`

## Textmodus-Syntax für verschiedene Berichterstellungselemente

Die Syntax der unten aufgeführten Sätze von Reporting-Elementen weist beim Erstellen im Textmodus die folgenden Ähnlichkeiten auf:

* Die Code- und Syntaxzeilen für Ansichten und Gruppierungen sind ähnlich.

  Informationen zu den Schlüsselzeilen von Codes für Ansichten und Gruppierungen beim Erstellen im Textmodus finden Sie unter:

   * [Bearbeiten einer Ansicht im Textmodus](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
   * [Bearbeiten einer Gruppierung im Textmodus](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* Die Code- und Syntaxzeilen für Filter und benutzerdefinierte Eingabeaufforderungen sind ähnlich.

  Weitere Informationen finden Sie unter:

   * [Bearbeiten eines Filters im Textmodus](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
   * [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### Syntax für Ansichten und Gruppierungen

Die Codezeilen beim Erstellen von Ansichten und Gruppierungen sind ähnlich.

Informationen zum Erstellen von Ansichten und Gruppierungen finden Sie in den folgenden Artikeln:

* [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Übersicht über Gruppierungen in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

Die wichtigste Codezeile für eine Ansicht oder eine Gruppierung ist die Zeile, die das Objekt identifiziert, auf das in der Spalte der Ansicht oder in der Gruppierung verwiesen wird. Diese Codezeile kann mit `valuefield` oder `valueexpression` beginnen, je nachdem, ob dieses Feld ein direkter Verweis auf ein Workfront-Datenbankfeld oder eine Berechnung zwischen mehreren Feldern ist.

In der folgenden Tabelle sind die häufigsten Codezeilen in einer Ansicht oder Gruppierung aufgeführt:

| Codezeile | Beschreibung |
|-----------------|------------------------------------------------------------------------------------------------------------------------------|
| `valuefield` | Identifiziert das Objekt, auf das in der Spalte der Ansicht oder in der Gruppierung verwiesen wird. Dies ist ein direkter Verweis auf das referenzierte Objekt. |
| `valueexpression` | Identifiziert das Objekt, auf das in der Spalte der Ansicht oder in der Gruppierung verwiesen wird. Dies ist eine Berechnung zwischen mehreren Feldern. |
| `valueformat` | Gibt das Format an, in dem Workfront den in den Zeilen valueField oder valueExpression angegebenen Wert zurückgibt. |
| `width` | Gibt die Breite einer Spalte in Pixel an. |
| `stretch` | Gibt an, welche Spalten zusätzlichen Platz belegen, der für die Ansicht nicht benötigt wird. |

>[!TIP]
>
>* Obwohl die Codezeilen in den folgenden Beispielen zwischen Ansichten und Gruppierungen ähnlich sind, sollten Sie immer daran denken, dass jede Codezeile für eine Gruppierung mit der Gruppierungsnummer beginnt.
>
>  Um in einer Projektliste oder einem Bericht nach Projektnamen zu gruppieren, verwenden Sie die folgende Zeile für die Gruppierung der ersten Ebene:
>
>  `group.0.valuefield=name`
>  
>* Wenn Sie mehrere Spalten in einer Ansicht in derselben Spalte bearbeiten (wie dies bei gemeinsam genutzten Spalten der Fall ist), denken Sie daran, dass jede Codezeile für jede Spalte mit der Spaltennummer beginnt.
>
>  Verwenden Sie das folgende Format, um die erste Spalte einer Ansicht anzugeben:
>
>  `column.0.valuefield=name`
>  
>  Informationen zur gemeinsamen Nutzung von Spalten finden Sie unter [Anzeigen: Zusammenführen von Informationen aus mehreren Spalten in einer gemeinsamen Spalte](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).
>

#### Übersicht über die `Valuefield` für Ansichten und Gruppierungen

`Valuefield=` ist eine Schlüsselzeile von Code in Ansichten und Gruppierungen, die das Objekt identifiziert, auf das Sie direkt verweisen.

Die Syntax für den direkten Verweis auf Felder ist für Gruppierungen und Ansichten identisch.

Die folgenden Regeln gelten für den Verweis auf Workfront-Objekte mithilfe einer `valuefield`:

* Verwenden Sie Groß-/Kleinschreibung, um direkt auf Felder zu verweisen.

  **Beispiel** Verwenden Sie die folgende Zeile, um in einer Aufgabenansicht auf das tatsächliche Abschlussdatum der Aufgabe zu verweisen:

  `valuefield=actualCompletionDate`

* Verwenden Sie Binnenmajuskeln und Doppelpunkte, um Felder für dasselbe Objekt zu trennen, die miteinander verknüpft sind.

  **Beispiel** Verwenden Sie die folgende Zeile, um in einer Aufgabenansicht auf das geplante Abschlussdatum des Projekts zu verweisen:

  `valuefield=project:plannedCompletionDate`

  Weitere Informationen dazu, wie Objekte in der Workfront-Datenbank aufeinander verweisen, finden Sie unter [API-Explorer](../../../wf-api/general/api-explorer.md).

* Verwenden Sie beim Referenzieren eines benutzerdefinierten Felds den Namen des Felds genau so, wie er in der Benutzeroberfläche angezeigt wird.

  **Beispiel** Verwenden Sie die folgende Zeile, um in einer Aufgabenansicht auf ein benutzerdefiniertes Feld des Projekts mit der Bezeichnung „Zusätzliche Details“ zu verweisen:

  `valuefield=project:Additional Details`

#### Übersicht über die `Valueexpression` für Ansichten und Gruppierungen

Sie können die `valuefield=` Codezeile beim Erstellen von Ansichten und Gruppierungen im Textmodus durch `valueexpression=` ersetzen, wenn Sie auf eine Berechnung zwischen zwei oder mehr Feldern verweisen möchten.

>[!TIP]
>
>Sie können zwar berechnete Felder erstellen, die Sie in Berichten anzeigen können, berechnete Ansichten und Gruppierungen sind jedoch dynamischer. Berechnete Ansichten und Gruppierungen werden bei jeder Ausführung des Berichts oder der Anzeige einer Liste mit neuen Informationen aktualisiert.
>
>Informationen zum Erstellen berechneter Spalten in einer Ansicht finden Sie unter [Berechnete benutzerdefinierte Felder im Vergleich zu berechneten Spalten](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Das Erstellen einer berechneten Gruppierung ähnelt dem Erstellen einer berechneten Spalte in einer Ansicht.

Die folgenden Regeln gelten für den Verweis auf Workfront-Objekte mithilfe einer `valueexpression`:

* Verwenden Sie Groß-/Kleinschreibung, um Felder direkt zu referenzieren und jedes Feld in geschweifte Klammern einzuschließen.

  **Beispiel:** Um das Feld „Aufgabenname“ in einer Aufgabenspalte mithilfe von &quot;`valueexpression`&quot; anzuzeigen, verwenden Sie die folgende Zeile:

  `valueexpression={name}`


* Verwenden Sie Binnenmajuskeln und Punkte, um miteinander verknüpfte Felder voneinander zu trennen.

  **Beispiel** Um den Namen eines Projekts in Verbindung mit dem Namen der Aufgabe in einem Aufgabenbericht anzuzeigen, verwenden Sie die folgenden Zeilen:

   * In einer Ansicht:

     `valueexpression=CONCAT({project}.{name},' - ',{name})`

   * In einer Gruppierung:

     `group.0.valueexpression=CONCAT({project}.{name},' - ',{name})`

  Weitere Informationen dazu, wie Objekte in der Workfront-Datenbank aufeinander verweisen, finden Sie unter [API-Explorer](../../../wf-api/general/api-explorer.md).

* Verwenden Sie beim Referenzieren eines benutzerdefinierten Felds die folgenden Regeln:

   * Verwenden Sie den Namen des Felds genau so, wie er in der Benutzeroberfläche angezeigt wird.
   * Stellen Sie dem Namen des Felds „DE:“ voran.
   * Schließen Sie das Feld in geschweiften Klammern ein.
   * Trennen Sie die mit dem Objekt verbundenen Felder durch Punkte.

  **Beispiel:** Um das benutzerdefinierte Feld „Projekt Zusätzliche Details“ in einer Aufgabenansicht in einer Ausdruckszeile für Werte anzuzeigen, verwenden Sie die folgende Zeile:

  `valueexpression={project}.{DE:Additional Details}`

* Sie können einen Platzhalter in einem `valueexpression`, aber nicht in einer `valuefield` verwenden.

  Informationen zu Platzhaltern finden Sie unter [Übersicht über Platzhalterfiltervariablen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).


#### `Valueformat` für Ansichten und Gruppierungen

Die zweitwichtigste Codezeile in einer Ansicht oder Gruppierung ist die `valueformat=`. Dadurch wird Workfront mitgeteilt, in welchem Format der Wert zurückgegeben werden soll, den Sie in den `valuefield` oder `valueexpression` Zeilen angeben. Obwohl Sie verschiedene Formate für die `valueformat` verwenden können, empfehlen wir, bei der Verwendung von `valueexpression` immer den folgenden Wert zu verwenden:

`valueformat=HTML`

Weitere `valueformat` finden Sie in den folgenden Artikeln:

* [Formatieren von Datumsangaben in Berichten im Textmodus](../../reports/text-mode/format-dates-in-text-mode-reports.md)
* [Formatieren von Zahlen, Währungs- und Prozentwerten in Textmodusberichten](../../reports/text-mode/format-numbers-in-text-mode-reports.md)

#### `width` für Ansichten

`width=` ist die Codezeile, in der Sie die Breite jeder Spalte in Pixel angeben können. Workfront bietet eine empfohlene Breite für jedes Feld. Je nach Feldtyp und Format können Sie jedoch Anpassungen vornehmen.

Sie müssen die zusätzliche `usewidths=true` Codezeile verwenden, um die für die Spalte angegebene Breite zu erzwingen.

**Beispiel:** Um eine Spalte mit einer Breite von 80 Pixel anzuzeigen, verwenden Sie die folgenden Zeilen:

`width=80`

`usewidths=true`

#### `stretch` für Ansichten

Mit dem `stretch` wird ermittelt, welche Spalten zusätzlichen Platz belegen, der für die Ansicht nicht benötigt wird. Die Breite der Benutzeroberfläche des Arbeitsbereichs beträgt für einen typischen Benutzer etwa 850 Pixel. Das bedeutet, dass bei einer Ansicht mit vier Spalten (je 150 Pixel) die Ansicht 600 von 850 Pixel ausfüllt. Die Benutzeroberfläche von enthält 250 zusätzliche Pixel, die den Spalten hinzugefügt werden, für die ein Dehnungsprozentsatz angegeben ist.

Die Ausdehnung einer Spalte wird erzwungen, wenn Sie die zusätzliche Codezeile verwenden: `usewidths=true` für mindestens eine der Spalten in der Ansicht.

**Beispiel:** Verwenden Sie die folgenden Zeilen, um anzugeben, dass eine Spalte 70 % des leeren Bereichs in einer Ansicht verwenden könnte:

`stretch=70`

`usewidths=true`

### Syntax für Filter und benutzerdefinierte Eingabeaufforderungen

Die Syntax zum Erstellen von Filtern ähnelt der Syntax zum Erstellen benutzerdefinierter Eingabeaufforderungen.

>[!TIP]
>
>Sie können eine benutzerdefinierte Eingabeaufforderung erstellen, indem Sie zunächst einen Filter für die Anweisung erstellen, die Sie in die Eingabeaufforderung aufnehmen möchten. Verbinden Sie alle Codezeilen in einem Filter mit &quot;&amp;&quot;, ohne dass Leerzeichen zwischen den Zeilen vorhanden sind. Daraus wird dann Ihre benutzerdefinierte Eingabeaufforderung.

Informationen zum Erstellen von Filtern und benutzerdefinierten Eingabeaufforderungen finden Sie unter:

* [Filter - Übersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

Weitere Informationen zum Erstellen von Filtern im Textmodus finden Sie unter [Bearbeiten eines Filters im Textmodus](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

Sie können die folgenden Elemente verwenden, um Filter und benutzerdefinierte Eingabeaufforderungen im Textmodus zu erstellen:

* Eine Codezeile, die auf das Objekt der Filteranweisung verweist. Verwenden Sie Binnenmajuskeln für das Filterobjekt.
* Eine Codezeile, die auf das Filterobjekt und den Modifikator für den Wert des Filterobjekts verweist. Verwenden Sie Binnenmajuskeln für das Filterobjekt in dieser Zeile.

  >[!TIP]
  >
  >Beim Referenzieren von Bereichen sind hierfür zwei Modifikatorzeilen erforderlich.

* Ein Anweisungs-Connector, der mehrere Filteranweisungen verbindet:

   * UND

     Dies ist der Standard-Connector zwischen Filteranweisungen.

   * ODER

     >[!TIP]
     >
     >Bei Anweisungs-Connectoren wird zwischen Groß- und Kleinschreibung unterschieden. „AND“ kann im Textmodus weggelassen werden.

* Platzhalter, um Filter dynamischer zu gestalten und sie für die aktuelle Zeit oder den angemeldeten Benutzer anzupassen. Informationen zu Platzhaltern finden Sie unter [Übersicht über Platzhalterfiltervariablen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).
