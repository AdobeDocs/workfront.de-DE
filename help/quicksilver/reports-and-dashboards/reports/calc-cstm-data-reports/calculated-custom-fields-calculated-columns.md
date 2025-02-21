---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Berechnete benutzerdefinierte Felder im Vergleich zu berechneten Spalten
description: Um mehrere Felder in Adobe Workfront zu aggregieren und diesen Aggregatwert in einem neuen Feld anzuzeigen, können Sie ein berechnetes benutzerdefiniertes Feld in einem benutzerdefinierten Formular oder eine berechnete Spalte in einer Ansicht erstellen.
author: Nolan
feature: Reports and Dashboards
exl-id: 17ac554d-0c90-4592-946e-a89f1784571d
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Berechnete benutzerdefinierte Felder im Vergleich zu berechneten Spalten

Um mehrere Felder in Adobe Workfront zu aggregieren und diesen Aggregatwert in einem neuen Feld anzuzeigen, können Sie Folgendes erstellen:

* Ein berechnetes benutzerdefiniertes Feld in einem benutzerdefinierten Formular\
  Weitere Informationen zum Hinzufügen eines berechneten benutzerdefinierten Felds zu einem benutzerdefinierten Formular finden Sie unter [Hinzufügen berechneter Felder zu einem Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

* Eine berechnete Spalte in einer Ansicht\
  Weitere Informationen zur Verwendung von Berechnungen in einer Ansicht finden Sie im Abschnitt [Verwenden des Textmodus in Ansichten](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#use-text-mode-in-views) im Artikel [Übersicht über häufig verwendete Anwendungen für den Textmodus](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

Obwohl Sie den Textmodus verwenden, um sowohl berechnete Felder als auch berechnete Spalten zu erstellen, unterscheidet sich die Syntax für ihre Erstellung. In den oben aufgeführten Artikeln erfahren Sie, wie Sie berechnete Felder und berechnete Spalten erstellen. Informationen über die verschiedene Syntax, die in berechneten Datenausdrücken wie berechneten benutzerdefinierten Feldern und Spalten verwendet wird, finden Sie im Abschnitt [Syntax von berechneten benutzerdefinierten Feldern im Vergleich zu berechneten benutzerdefinierten Spalten](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) in diesem Artikel.

Sie können dieselben Berechnungen sowohl in berechneten Feldern als auch in einer berechneten Spalte verwenden. Je nachdem, welchen Zweck diese Berechnungen haben, sollten Sie jedoch erwägen, eine gegen die andere zu erstellen.

## Syntax von berechneten benutzerdefinierten Feldern im Vergleich zu berechneten benutzerdefinierten Spalten

Obwohl die von Ihnen verwendeten Funktionen identisch sind, kann sich die Syntax zum Erstellen eines Ausdrucks in einem berechneten benutzerdefinierten Feld von der Syntax zum Erstellen einer berechneten benutzerdefinierten Spalte unterscheiden.

Beispiel:

* In einem benutzerdefinierten Feld in einem benutzerdefinierten Formular für Aufgaben würden Sie Folgendes verwenden, um den Namen des übergeordneten Projekts der Aufgabe zu generieren, an das das benutzerdefinierte Formular angehängt ist:

  `{project}.{name}`

* In einer benutzerdefinierten Spalte in einem Bericht würden Sie Folgendes verwenden, um eine benutzerdefinierte Spalte „Projektname“ zu einem Aufgabenbericht hinzuzufügen:

  `valuefield=project:name`

  Oder

  `valueexpression={project}.{name}`

  >[!TIP]
  >
  >Dieselbe Syntax gilt für alle Berichtselemente im Textmodus, in denen berechnete Ausdrücke verwendet werden: Ansichten, Filter, Gruppierungen und Eingabeaufforderungen.

Die Unterschiede zwischen den beiden Syntaxen sind:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Berechnetes benutzerdefiniertes Feld</strong></td>
   <td><strong>Berechnetes benutzerdefiniertes Berichterstellungselement</strong></td> 
  </tr> 
  <tr> 
   <td> <p>Verwenden Sie die Namen der Felder, wie sie in der Benutzeroberfläche von Workfront angezeigt werden.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Beispiel für einen Feldnamen in einem berechneten benutzerdefinierten Feld: <code>Planned Completion Date</code>.</p> </td> 
   <td> <p>Verwenden Sie den Namen der Objekte oder Felder so, wie sie in der Workfront-Datenbank angezeigt werden. Die Namen von Objekten und Feldern werden in Kleinbuchstaben oder Binnenmajuskeln geschrieben, wenn es sich um zusammengesetzte Namen handelt. </p> <p>Eine Aufstellung aller Workfront-Objekte und -Felder, wie sie in der Datenbank angezeigt werden, finden Sie unter <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Beispiel eines Feldnamens, der in einem berechneten benutzerdefinierten Berichterstellungselement verwendet wird: <code>plannedCompletionDate</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Umschließen von Feldnamen in Klammern oder geschweiften Klammern</td> 
   <td> <p>Schließen Sie Feldnamen nicht in Klammern oder Klammern ein, wenn Sie sie in einer <code>valuefield </code> verwenden.</p> <p>Schließen Sie Feldnamen in geschweifte Klammern ein, wenn Sie sie in einer <code>valueexpression</code> verwenden.</p> </td> 
  </tr> 
  <tr> 
   <td>Felder durch Punkte trennen</td> 
   <td> <p>Trennen Sie die Felder durch Doppelpunkte, wenn Sie sie in einer <code>valuefield</code> verwenden.</p> <p>Trennen Sie die Felder durch Punkte, wenn Sie sie in einer <code>valueexpression</code> verwenden.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zur Syntax, die Sie in einer berechneten benutzerdefinierten Spalte verwenden müssen, finden Sie unter [Übersicht über den Textmodus](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Verwendung berechneter benutzerdefinierter Felder

* Wenn Sie die aggregierten Ergebnisse in einem Bericht gruppieren oder diese Informationen in einem Diagramm anzeigen möchten
* Beim Aggregieren der Daten über die im Feld berechnete Aggregation hinaus
* Wenn Sie nicht an der Aktualität der Daten interessiert sind, da die Daten nicht aktualisiert werden und sich diese im Laufe der Zeit ändern können

## Aktionen, durch die die Aktualisierung eines berechneten benutzerdefinierten Felds Trigger wird

* Klicken Sie auf der Hauptseite eines Objekts auf das Symbol Mehr ![Symbol Mehr](assets/more-icon.png) und klicken Sie dann auf **Ausdrücke neu berechnen**

* Massenbearbeitung mehrerer Objekte, wenn **Benutzerdefinierte Ausdrücke neu**) aktiviert ist
* Das Bearbeiten eines benutzerdefinierten Formulars, wenn **Aktualisieren vorheriger Berechnungen** für das berechnete benutzerdefinierte Feld aktiviert ist

## Verwendung berechneter Spalten in einer Ansicht

* Wenn Echtzeitdaten in einem Bericht verfügbar sein sollen.

  Berechnete Ansichten sind immer neu, da die Berechnung erfolgt, wenn der Bericht ausgeführt oder die Ansicht angewendet wird.

* Wenn Sie keine Pläne haben, nach aggregierten Ergebnissen zu gruppieren oder diese Informationen in einem Diagramm zu verwenden.
* Wenn Sie keine Aggregation der Daten über die in der Spalte berechnete Aggregation hinaus planen (Daten können nur einmal aggregiert werden).
* Wenn bei der Berechnung ein Verweis auf das aktuelle Datum mithilfe der Platzhalter $$TODAY oder $$NOW enthalten sein soll.

  >[!TIP]
  >
  >Verwenden Sie diese Referenz nicht in berechneten benutzerdefinierten Feldern, da sie nur neu berechnet werden, wenn das angehängte Objekt bearbeitet wird. Diese Berechnungsarten sind überholt.

## Beispiele für berechnete benutzerdefinierte Felder und Spalten

Beispiele für berechnete benutzerdefinierte Felder finden Sie unter [Berechnete benutzerdefinierte Daten in Berichten](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

Beispiele für berechnete benutzerdefinierte Spalten in Ansichten finden Sie in den folgenden Artikeln:

* [Übersicht über häufige Verwendungen für den Textmodus](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)
* [Beispiele für benutzerdefinierte Ansichten, Filter und Gruppierungen: Artikelindex](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
