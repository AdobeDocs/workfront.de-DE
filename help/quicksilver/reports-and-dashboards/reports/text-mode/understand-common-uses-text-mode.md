---
product-area: reporting
navigation-topic: text-mode-reporting
title: Übersicht über häufige Verwendungszwecke für den Textmodus
description: Übersicht über häufige Verwendungszwecke für den Textmodus
author: Nolan
feature: Reports and Dashboards
exl-id: 81512837-1ec4-4dbc-ace4-bdf08fe667ce
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 0%

---

# Übersicht über häufige Verwendungszwecke für den Textmodus

<!-- Audited: 1/2025 -->

<!--(NOTE: Alina: ***This is linked to Understanding Text Mode (article), and the TOC article for examples of various reporting elements)</p>-->

Sie können Ihre Berichtsfunktionen durch die Verwendung des Textmodus in Berichten und Berichtselementen erweitern. Sie können auch eine Version des Textmodus verwenden, um komplexere berechnete benutzerdefinierte Felder zu erstellen. Weitere Informationen zum Textmodus finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

In diesem Artikel werden nur einige Beispiele beschrieben, in denen Sie am ehesten den Textmodus verwenden müssten, um die Funktionen für Berichte oder berechnete benutzerdefinierte Felder in Adobe Workfront zu erweitern. Eine ausführlichere Liste der Beispiele finden Sie unter:

* [Beispiele für benutzerdefinierte Ansichten, Filter und Gruppierungen: Artikelindex](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
* [Berechnete benutzerdefinierte Daten in Berichten](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md)

Weitere Informationen zum Erstellen von Berichten im Textmodus, einschließlich Klassen, Videos und Tutorials, finden Sie im Abschnitt Lernen auf der Adobe Experience League-Site.

## Instanzen, bei denen Sie den Textmodus in Listen und Berichten verwenden könnten

Es wird empfohlen, zum Erstellen Ihrer Ansichten, Filter und Gruppierungen Report Builder zu verwenden. Es gibt jedoch einige Fälle, in denen Sie den Textmodus verwenden können, um Ihre Berichte und Listen zu verbessern.

Sie können den Textmodus verwenden, wenn Sie in Workfront Folgendes erreichen möchten:

* Erstellen benutzerdefinierter berechneter Felder in einem benutzerdefinierten Formular.\
  Weitere Informationen zu berechneten benutzerdefinierten Feldern finden Sie im Abschnitt [Verwenden des Textmodus in berechneten benutzerdefinierten Feldern](#use-text-mode-in-calculated-custom-fields) in diesem Artikel.
* Filter, Ansichten und Gruppierungen über die Möglichkeiten in Report Builder hinaus verbessern. Informationen zur Verwendung des Textmodus für Filter, Ansichten und Gruppierungen finden Sie in den folgenden Abschnitten in diesem Artikel:

   * [Verwenden des Textmodus in Ansichten](#use-text-mode-in-views)
   * [Verwenden des Textmodus in Filtern](#use-text-mode-in-filters)
   * [Verwenden des Textmodus in Gruppierungen](#use-text-mode-in-groupings)

* Erstellen Sie benutzerdefinierte Eingabeaufforderungen. Sie können benutzerdefinierte Eingabeaufforderungen nur im Textmodus erstellen.

  Informationen zum Erstellen benutzerdefinierter Eingabeaufforderungen finden Sie unter [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

## Verwenden des Textmodus in berechneten benutzerdefinierten Feldern {#use-text-mode-in-calculated-custom-fields}

Sie können den Textmodus verwenden, um einem benutzerdefinierten Formular ein berechnetes benutzerdefiniertes Feld hinzuzufügen.

Weitere Informationen zum Hinzufügen eines berechneten benutzerdefinierten Felds zu einem benutzerdefinierten Formular finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Weitere Informationen zum Erstellen eines berechneten benutzerdefinierten Felds im Textmodus finden Sie unter [Hinzufügen berechneter Felder zu einem Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Sie können beispielsweise ein berechnetes benutzerdefiniertes Feld hinzufügen, das einen Zeit- und Datumsstempel des Zeitpunkts anzeigt, zu dem ein Element als In Bearbeitung markiert wurde. Sie können diese Berechnung für andere Status verwenden.

Weitere Informationen finden Sie unter [Beispiel für berechnete benutzerdefinierte Felder: Anzeigen eines Status-Zeitstempels in einem benutzerdefinierten Formular](../../../reports-and-dashboards/reports/calc-cstm-data-reports/example-status-timestamp-in-calculated-field.md).

## Verwenden des Textmodus in Ansichten {#use-text-mode-in-views}

Sie können den Textmodus in Ansichten verwenden, um die Felder und Objekte zu erweitern, die Sie in der Ansicht anzeigen können.

Beispiele für die häufigsten Gründe für die Verwendung des Textmodus in einer Ansicht finden Sie in den folgenden Artikeln:

* [Anzeigen: Zeigt Objekte an, die nicht in der Standardschnittstelle enthalten sind](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-objects-not-in-standard-interface.md)
* [Anzeigen: zeigt das Ergebnis einer Berechnung zwischen zwei Feldern in einer Spalte an](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-calculation-between-two-fields.md)
* [Anzeigen: Die Breite einer Spalte dauerhaft bearbeiten](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md)
* [Anzeigen: Zusammenführungsinformationen aus mehreren Spalten in einer gemeinsamen Spalte](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md)
* [Anzeigen: Entfernen eines Links zu einem Objekt in einer Spalte](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-remove-link-to-object.md)
* [Referenzieren von Sammlungen in einem Bericht](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)
* [Anzeigen: Blendet den Inhalt einer Spalte aus](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-hide-column-content.md)
* [Anzeigen: Ein Bild anstelle einer Zeichenfolge in einer Spalte anzeigen](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-image-in-view.md)
* [Anzeigen: Aufgabeneinzüge in einer Aufgabenliste anzeigen](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-task-identations.md)
* [Ansicht: Uhrzeit- und Datumsunterschiede berechnen](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-calculate-time-and-date-differences.md)

## Verwenden des Textmodus in Filtern {#use-text-mode-in-filters}

Sie können den Textmodus beim Erstellen von Filtern verwenden, um die Felder und Objekte zu erweitern, nach denen Sie filtern können.

Beispiele für die häufigsten Gründe für die Verwendung des Textmodus in einem Filter finden Sie in den folgenden Artikeln:

* [Filter: Erstellen Sie mehrere Filterregeln, die auf dasselbe Feld verweisen (AND-Anweisungen)](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-refrence-the-same-field-multiple-times.md)
* [Filter: Zeigt nur Elemente mit einem Genehmigungsstatus an](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-for-items-in-approval-status.md)
* [Filtern: Zeigt Elemente mit demselben Namensstatus an, wenn die Status mit verschiedenen Gruppen verknüpft sind](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-same-name-statuses-from-different-groups.md)
* [Filtern: Eliminieren Sie Elemente in einer Liste, indem Sie zwei Felder vergleichen](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-items-by-comparing-two-fields.md)
* Der Abschnitt [Beispiele für Textmodusfilter, die sich über mehrere Ebenen in der Objekthierarchie erstrecken](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md#examples) im Artikel [Erstellen komplexer Textmodusfilter mit EXISTS-Anweisungen](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md)
* Der Abschnitt [Erstellen komplexer Textmodusfilter für fehlende Objekte](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md#missing-object-filters) im Artikel [Erstellen komplexer Textmodusfilter mit EXISTS-Anweisungen](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md)

## Verwenden des Textmodus in Gruppierungen {#use-text-mode-in-groupings}

Sie können den Textmodus beim Erstellen von Gruppierungen verwenden, um die Felder und Objekte zu erweitern, nach denen Sie in Listen und Berichten gruppieren können.

Beispiele für die häufigsten Gründe für die Verwendung des Textmodus in einer Gruppierung finden Sie in den folgenden Artikeln:

* [Gruppierung: Organisieren Sie die Listenergebnisse nach einem berechneten Wert, der für alle Objekte in der Gruppierung gleich ist](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-by-calculated-common-values.md)
* [Gruppierung: Eine vierte Gruppierung zu einer Liste hinzufügen](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-add-fourth-grouping.md)
* [Gruppierung: Anzeigenamen in einer Gruppierung bearbeiten](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-rename-grouping.md)
* [Gruppierung: Gibt an, ob die Ergebnisse einer Gruppierung im Textmodus reduziert oder erweitert werden sollen](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-collapsed-or-expanded-results.md)
