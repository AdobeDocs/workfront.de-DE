---
product-area: reporting
navigation-topic: reporting-elements
title: Filter- und Bedingungs-Modifikatoren
description: Mit Filter- und Bedingungsmodifikatoren können Sie Filter erstellen und Bedingungen zur Formatierung Ihrer Berichtsergebnisse festlegen.
author: Nolan
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '1556'
ht-degree: 1%

---

# Filter- und Bedingungs-Modifikatoren

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit) </p>
-->

Mit Filter- und Bedingungsmodifikatoren können Sie Filter erstellen und Bedingungen zur Formatierung Ihrer Berichtsergebnisse festlegen.

Weitere Informationen zum Erstellen von Filtern finden Sie im Artikel [Filterübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Weitere Informationen zur Verwendung von bedingter Formatierung in Ansichten finden Sie im Artikel [Bedingte Formatierung in Ansichten verwenden](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Filter- und Bedingungs-Modifikatoren

Eine Liste der integrierten Zeitrahmen-Modifikatoren finden Sie im Artikel [Berichte nach Zeitrahmen filtern](../../../reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

Einige Modifikatoren sind integriert und Sie können sie aus einem Dropdown-Menü innerhalb Ihrer Filter- oder bedingten Formatierungsanweisung auswählen. Andere Modifikatoren können nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Verständnis des Textmodus finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Sie können die folgenden Bedingungsmodifikatoren in Filtern und Anweisungen zur bedingten Formatierung verwenden:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Integrierter Modifikator</strong> </p> </th> 
   <th> <p><strong>Textmodus-Modifikator</strong> </p> </th> 
   <th> <p><strong>Beschreibung</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td> <p><strong>Leer</strong> </p> </td> 
   <td> <p><strong>leer</strong> </p> </td> 
   <td> <p>Das Feld existiert für das Objekt, dem Feld wurde jedoch noch kein Wert zugewiesen.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Nicht leer</strong> </p> </td> 
   <td> <p><strong>notblank</strong> </p> </td> 
   <td> <p>Das Feld, nach dem Sie filtern, ist vorhanden und hat einen Wert.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>null</strong> </p> </td> 
   <td> <p>Das Feld ist entweder leer oder existiert nicht. Sie möchten beispielsweise nach Elementen ohne übergeordnete Aufgaben-ID suchen. Das bedeutet, dass Sie nur eigenständige Aufgaben sehen möchten. Der Qualifizierer für die "übergeordnete Aufgaben-ID"wäre <strong>null</strong>, da eine Aufgabe ohne ID (in diesem Fall das übergeordnete Element) nicht vorhanden ist. </p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Filter im Textmodus bearbeiten</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>Das Feld, nach dem Sie filtern, ist vorhanden und enthält einen anderen Wert als null.</p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Filter im Textmodus bearbeiten</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Enthält</strong> </p> </td> 
   <td> <p><strong>cicontains</strong> </p> </td> 
   <td> <p>(Groß-/Kleinschreibung nicht beachten) Diese Version von <strong>contains</strong>. Beispiel: "cicontains inf"erfasst alle Werte, die "Inf"oder "inf"enthalten.</p> <p> <p>Hinweis: Adobe Workfront sucht nach dem genauen Wort oder der Wortgruppe, das bzw. die Sie für jede Filteranweisung angeben. Wenn Sie beispielsweise nach einem Projekt suchen, das den Begriff "neues Projekt"im Namen enthält, zeigt Workfront keine Projekte an, die nur "neu"oder "Projekt"oder "neues Hauptprojekt"im Namen enthalten. Der Filter findet nur Projekte mit dem genauen Wortlaut "neues Projekt"im Namen.</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>(Groß-/Kleinschreibung nicht beachten) Diese Option unterscheidet nicht zwischen Groß- und Kleinschreibung. <strong>eq</strong>. Es wird nur eine exakte Übereinstimmung mit dem gesuchten Wert zurückgegeben.</p> <p>Wenn beispielsweise nach einer Aufgabe mit einem bestimmten Namen gesucht wird, findet "task name cieq test"Aufgaben, bei denen der Name "Test", "TEST"oder "Test" lautet, aber keine Aufgabe mit dem Namen "test 123".</p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Filter im Textmodus bearbeiten</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>ciin</strong> </p> </td> 
   <td> <p>(Groß-/Kleinschreibung nicht beachten) Diese Version von <strong>in</strong>.</p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Filter im Textmodus bearbeiten</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cilike</strong> </p> </td> 
   <td> <p>Dies ist die Version von, die nicht von Schreibweise abhängig ist <strong>like</strong>. Beispiel: "cilike %Current% %Dead%"gibt alle Notizen zurück, die "Current to Dead"(Aktuell bis tot) oder "Aktuell bis tot"enthalten.</p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Filter im Textmodus bearbeiten</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cinotin</strong> </p> </td> 
   <td> <p>(Groß-/Kleinschreibung nicht beachten) Diese Version von <strong>notin</strong>.</p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Erstellen von Filtern mithilfe des Textmodus finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Filter im Textmodus bearbeiten</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>enthält</strong> </p> </td> 
   <td> <p>(Groß-/Kleinschreibung beachten) Sucht den angegebenen Text in einer gesamten Textzeichenfolge.</p> <p>Beispielsweise erfasst die Verwendung von "enthält Inf"alles mit "Inf"darin, z. B. das Wort "Unendlichkeit".</p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Filter im Textmodus bearbeiten</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Beinhaltet nicht</strong> </p> </td> 
   <td> <p><strong>Cinotcontains</strong> </p> </td> 
   <td> <p>(Groß-/Kleinschreibung nicht beachten) Er filtert Elemente, bei denen der angegebene Wert fehlt.</p> <p>Beispielsweise erfasst "enthält nicht inf"alles ohne "Inf"oder "inf"im Namen.</p> <p>Hinweis: <span>Wenn das Feld, nach dem Sie filtern, mehrere Optionen aufweist, werden die Ergebnisse herausgefiltert, die sowohl die von Ihnen festgelegte Auswahl als auch die von Ihnen festgelegte Auswahl und zusätzliche Optionen enthalten.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>Nicht vorhanden</strong> </td> 
   <td><strong>NOTEXISTEN</strong> </td> 
   <td> <p>Dieser Modifikator wird nur mit komplexen Filtern in einer EXISTS-Anweisung verwendet. Diese Filter beziehen sich nur auf die folgenden Objekte: </p> 
    <ul> 
     <li>Objekte, die sich über mehrere Ebenen in der Objekthierarchie erstrecken </li> 
     <li>Fehlende Objekte </li> 
    </ul> <p>Informationen zum Erstellen komplexer Filter mithilfe von EXISTS-Anweisungen finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">Erstellen komplexer Textmodusfilter mit vorhandenen Anweisungen</a>. Dies ist der einzige Modifikator, der in EXISTS-Anweisungen verwendet wird.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>Gleich (ignoriert Groß- und Kleinschreibung)</strong> </p> </td> 
   <td> <p><strong>in</strong> </p> </td> 
   <td> <p>(Groß-/Kleinschreibung beachten) Mit diesem Modifikator können Sie eine kommagetrennte Liste von Variablen erstellen, die mit einem einzelnen Attribut verglichen werden, das in einem Filter ausgewertet wurde. Die gesamte Liste wird als OR-Anweisung behandelt und gibt Ergebnisse zurück, die die Kriterien einer oder mehrerer Variablen erfüllen.</p> <p>Wenn Sie beispielsweise nach Projekten suchen, gibt "in CUR, PLN, CPL"alle Projekte zurück, die sich im Status "Aktuell", "Planung"oder "Abgeschlossen"befinden.</p> <p>Der integrierte Modifikator <strong>Gleich</strong> entspricht dem Textmodus-Modifikator von <strong>in</strong>. Das bedeutet, dass Sie für das Feld "Gleich mit mehreren Werten"auswählen können.</p> <p>Beispielsweise können Sie in einem Projektbericht "Status gleich Aktuell, Planung, Tod"auswählen und Projekte in einem dieser Status anzeigen.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>(Groß-/Kleinschreibung beachten) Dies gibt nur eine exakte Übereinstimmung mit dem gesuchten Wert zurück.</p> <p>Wenn Sie beispielsweise nach vollständigen Projekten suchen, gibt "eq CPL"alle Projekte mit dem vollständigen Status zurück. "eq CPL, CUR"gibt kein Ergebnis zurück, da ein Projekt nicht vollständig und aktuell sein kann.</p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zur Verwendung des Textmodus zum Erstellen von Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Filter im Textmodus bearbeiten</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>größer als</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>Hierbei wird nach allen Ergebnissen gesucht, deren Wert größer als der eingegebene Wert ist, wobei der eingegebene Wert nicht berücksichtigt wird.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>like</strong> </p> </td> 
   <td> <p>(Groß-/Kleinschreibung beachten) Sucht nach Teilen einer Textzeichenfolge auf ähnliche Weise wie <strong>contains</strong>. Allerdings <strong>like</strong> bietet die Möglichkeit, Platzhalterzeichen einzufügen, um den Text aufzuteilen.</p> <p>Wenn Sie beispielsweise nach Notizen suchen, gibt "like %Current% %Dead%"jede Notiz zurück, die die Wortgruppe "Current to Dead"enthält. Es enthält keine Hinweise, die "Dead to Current"(Taubheit bis aktuell) enthalten. Jeder Wert wird in der angegebenen Reihenfolge durchsucht. Der % stellt eine Platzhalterkarte dar, um Zeichen oder Textsegmente zu ersetzen.</p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Filter im Textmodus bearbeiten</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Kleiner als</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>Hierbei wird nach allen Ergebnissen gesucht, deren Wert kleiner ist als der eingegebene Wert, wobei der eingegebene Wert nicht berücksichtigt wird.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Größer gleich</strong> </p> </td> 
   <td> <p><strong>get</strong> </p> </td> 
   <td> <p>Hierdurch werden alle Ergebnisse gesucht, deren Werte größer oder gleich dem eingegebenen Wert sind.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Kleiner gleich</strong> </p> </td> 
   <td> <p><strong>lte</strong> </p> </td> 
   <td> <p>Hierbei werden alle Ergebnisse gesucht, deren Wert kleiner oder gleich dem eingegebenen Wert ist.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Zwischen</strong> </p> </td> 
   <td> <p><strong>zwischen</strong> </p> </td> 
   <td> <p>Bietet zwei erforderliche Feldwerte und sucht nach allen Ergebnissen im Bereich beider Felder, einschließlich der eingegebenen Werte.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>(Groß-/Kleinschreibung beachten) Er filtert nach Elementen, denen der angegebene Wert fehlt.</p> <p>Beispielsweise erfasst "enthält nicht inf"alles mit ohne "inf", zeigt jedoch Werte an, die "Inf"enthalten.</p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Filter im Textmodus bearbeiten</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notbetween</strong> </p> </td> 
   <td> <p>Dies ist das Gegenteil von <strong>between</strong>. Es stellt zwei erforderliche Wertefelder bereit und sucht nach allen Ergebnissen außerhalb des Bereichs beider Felder einschließlich der eingegebenen Werte.</p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Filter im Textmodus bearbeiten</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Ungleich</strong> </p> </td> 
   <td> <p><strong>notin</strong> </p> </td> 
   <td> <p>(Groß-/Kleinschreibung beachten) Dies ist das Gegenteil von <strong>in</strong>. Es werden nur Ergebnisse zurückgegeben, die nicht in der angegebenen Liste enthalten sind.</p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Filter im Textmodus bearbeiten</a>.</p> <p>Hinweis: <span>Wenn das Feld, nach dem Sie filtern, mehrere Optionen aufweist, werden die Ergebnisse herausgefiltert, die sowohl die von Ihnen festgelegte Auswahl als auch die von Ihnen festgelegte Auswahl und zusätzliche Optionen enthalten.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>(Groß-/Kleinschreibung beachten) Dies ist das Gegenteil von <strong>eq</strong>. Es werden nur Ergebnisse zurückgegeben, die nicht exakt mit dem gesuchten Wert übereinstimmen, und es wird auch die Groß-/Kleinschreibung des Werts berücksichtigt.</p> <p>Beispiel: <b>ne</b> gibt Werte zurück, die nicht mit "Aktuell"übereinstimmen, jedoch keine Werte zurück, die nicht mit "Aktuell"übereinstimmen. </p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Filter im Textmodus bearbeiten</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>cine</strong> </td> 
   <td> <p>(Groß-/Kleinschreibung nicht beachten) Diese Option unterscheidet nicht zwischen Groß- und Kleinschreibung. <strong>ne</strong> und das Gegenteil der <b>cieq</b> -Modifikator. Es werden nur Ergebnisse zurückgegeben, die keine exakte Übereinstimmung mit dem gesuchten Wert sind, nicht jedoch die Groß-/Kleinschreibung des Werts.</p> <p>Beispiel: <b>cine</b> gibt Werte zurück, die weder "aktuell"noch "Aktuell"entsprechen. </p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Filter im Textmodus bearbeiten</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
