---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Berechnete benutzerdefinierte Felder vs. berechnete Spalten
description: Um mehrere Felder in Adobe Workfront zu aggregieren und diesen aggregierten Wert in einem neuen Feld anzuzeigen, können Sie ein berechnetes benutzerdefiniertes Feld in einem benutzerdefinierten Formular oder eine berechnete Spalte in einer Ansicht erstellen.
author: Nolan
feature: Reports and Dashboards
exl-id: 17ac554d-0c90-4592-946e-a89f1784571d
source-git-commit: c49b545938a78716084296ef1b4e7c0fc075ef95
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 0%

---

# Berechnete benutzerdefinierte Felder vs. berechnete Spalten

Um mehrere Felder in Adobe Workfront zu aggregieren und diesen aggregierten Wert in einem neuen Feld anzuzeigen, können Sie Folgendes erstellen:

* Ein berechnetes benutzerdefiniertes Feld in einem benutzerdefinierten Formular\
  Weitere Informationen zum Hinzufügen eines berechneten benutzerdefinierten Felds zu einem benutzerdefinierten Formular finden Sie im Abschnitt . [Berechnetes Feld zu einem benutzerdefinierten Formular hinzufügen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#add-a-calculated-field-to-a-custom-form) im Artikel [Hinzufügen errechneter Daten zu einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* Eine berechnete Spalte in einer Ansicht\
  Weitere Informationen zur Verwendung von Berechnungen in einer Ansicht finden Sie im Abschnitt . [Textmodus in Ansichten verwenden](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#use-text-mode-in-views) im Artikel [Übersicht über die häufigsten Verwendungen für den Textmodus](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

Obwohl Sie den Textmodus verwenden, um sowohl berechnete Felder als auch berechnete Spalten zu erstellen, unterscheidet sich die Syntax für ihre Erstellung. In den oben aufgeführten Artikeln erfahren Sie, wie Sie berechnete Felder und Spalten erstellen. Informationen zur unterschiedlichen Syntax, die in berechneten Datenausdrücken wie berechneten benutzerdefinierten Feldern und Spalten verwendet wird, finden Sie im Abschnitt . [Syntax von berechneten benutzerdefinierten Feldern im Vergleich zu berechneten benutzerdefinierten Spalten](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) in diesem Artikel.

Sie können dieselben Berechnungen in beiden berechneten Feldern sowie in einer berechneten Spalte verwenden. Je nachdem, welchen Zweck Sie für diese Berechnungen haben, sollten Sie jedoch in Erwägung ziehen, die eine oder die andere zu erstellen.

## Syntax von berechneten benutzerdefinierten Feldern im Vergleich zu berechneten benutzerdefinierten Spalten

Die von Ihnen verwendeten Funktionen sind zwar identisch, die Syntax für die Erstellung eines Ausdrucks in einem berechneten benutzerdefinierten Feld kann sich jedoch von der für die Erstellung einer berechneten benutzerdefinierten Spalte unterscheiden.

Beispiel:

* In einem benutzerdefinierten Feld würden Sie in einem benutzerdefinierten Formular für Aufgaben den Namen des übergeordneten Projekts der Aufgabe generieren, an das das benutzerdefinierte Formular angehängt ist:

  `{project}.{name}`

* In einer benutzerdefinierten Spalte in einem Bericht können Sie wie folgt eine benutzerdefinierte Spalte für den Projektnamen zu einem Aufgabenbericht hinzufügen:

  `valuefield=project:name`

  Oder

  `valueexpression={project}.{name}`

  >[!TIP]
  >
  >Dieselbe Syntax gilt für alle Berichterstellungselemente im Textmodus, in denen berechnete Ausdrücke verwendet werden: Ansichten, Filter, Gruppierungen und Eingabeaufforderungen.

Die Unterschiede zwischen den beiden Syntaxen sind:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Berechnetes benutzerdefiniertes Feld</strong></td>
   <td><strong>Berechnetes benutzerdefiniertes Berichtselement</strong></td> 
  </tr> 
  <tr> 
   <td> <p>Verwenden Sie den Feldnamen so, wie er in der Benutzeroberfläche von Workfront angezeigt wird.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Beispiel für einen Feldnamen, der in einem berechneten benutzerdefinierten Feld verwendet wird: <code>Planned Completion Date</code>.</p> </td> 
   <td> <p>Verwenden Sie den Namen der Objekte oder Felder, wie er in der Workfront-Datenbank angezeigt wird. Die Namen von Objekten und Feldern werden in Kleinbuchstaben oder Binnenmajuskel geschrieben, wenn es sich um zusammengesetzte Namen handelt. </p> <p>Eine Bestandsaufnahme aller Workfront-Objekte und -Felder, wie sie in der Datenbank angezeigt werden, finden Sie unter <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API-Explorer</a>. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Beispiel für einen Feldnamen, der in einem berechneten benutzerdefinierten Berichterstellungselement verwendet wird: <code>plannedCompletionDate</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Feldnamen in Klammern oder geschweifte Klammern einschließen</td> 
   <td> <p>Schließen Sie Feldnamen nicht in Klammern oder Klammern ein, wenn Sie sie in einer <code>valuefield </code>Linie.</p> <p>Fügen Sie Feldnamen in geschweifte Klammern bei der Verwendung in einer <code>valueexpression</code> Linie.</p> </td> 
  </tr> 
  <tr> 
   <td>Trennen Sie die Felder durch Punkte.</td> 
   <td> <p>Trennen Sie die Felder bei Verwendung in einer <code>valuefield</code>Linie.</p> <p>Trennen Sie die Felder bei der Verwendung in einer <code>valueexpression</code>Linie.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zur Syntax, die Sie in einer berechneten benutzerdefinierten Spalte verwenden müssen, finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Verwendung berechneter benutzerdefinierter Felder

* Wenn Sie die aggregierten Ergebnisse in einem Bericht gruppieren möchten oder diese Informationen in einer Grafik anzeigen möchten
* Wenn Sie die Daten über die im Feld berechnete Aggregation hinaus aggregieren möchten
* Wenn Sie sich nicht um die Aktualität der Daten sorgen, da die Daten nicht aktualisiert werden und sich diese im Laufe der Zeit ändern können

## Aktionen, die die Aktualisierung eines berechneten benutzerdefinierten Felds Trigger haben

* Klicken Sie auf der Hauptseite eines Objekts auf das Symbol Mehr . ![](assets/more-icon.png), klicken Sie auf **Ausdrücke neu berechnen**

* Massenbearbeitung mehrerer Objekte bei **Benutzerdefinierte Ausdrücke neu berechnen** ist aktiviert
* Bearbeiten eines benutzerdefinierten Formulars beim **Vorherige Berechnungen aktualisieren** für das berechnete benutzerdefinierte Feld aktiviert ist

## Verwendung berechneter Spalten in einer Ansicht

* Wenn Echtzeitdaten für einen Bericht verfügbar sein sollen.

  Berechnete Ansichten sind immer neu, da die Berechnung bei Ausführung des Berichts oder Anwendung der Ansicht erfolgt.

* Wenn Sie nicht planen, diese Informationen nach aggregierten Ergebnissen zu gruppieren, oder diese Informationen in einer Grafik verwenden möchten.
* Wenn Sie nicht planen, die Daten über die in der Spalte berechnete Aggregation hinaus zu aggregieren (Daten können nur einmal aggregiert werden).
* Wenn Sie möchten, dass die Berechnung einen Verweis auf das aktuelle Datum mit den Platzhaltern $$TODAY oder $$NOW enthält.

  >[!TIP]
  >
  >Verwenden Sie diese Referenz nicht in berechneten benutzerdefinierten Feldern, da diese nur neu berechnet werden, wenn das angehängte Objekt bearbeitet wird. Diese Art von Berechnungen sind überholt.

## Beispiele für berechnete benutzerdefinierte Felder und Spalten

Beispiele für berechnete benutzerdefinierte Felder finden Sie unter [Berechnete benutzerdefinierte Daten in Berichten](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

Beispiele für berechnete benutzerdefinierte Spalten in Ansichten finden Sie in den folgenden Artikeln:

* [Übersicht über die häufigsten Verwendungen für den Textmodus](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)
* [Beispiele für benutzerdefinierte Ansicht, Filter und Gruppierung: Artikelindex](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
