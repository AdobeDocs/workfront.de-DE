---
product-area: reporting
navigation-topic: reporting-elements
title: Filter- und Bedingungs-Modifikatoren
description: Mit Filter- und Bedingungsmodifikatoren können Sie Filter erstellen und Bedingungen zur Formatierung Ihrer Berichtsergebnisse festlegen.
author: Nolan
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '1566'
ht-degree: 0%

---

# Filter- und Bedingungs-Modifikatoren

<!-- Audited: 11/2024 -->

<!--(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit)-->

Mit Filter- und Bedingungsmodifikatoren können Sie Filter erstellen und Bedingungen zur Formatierung Ihrer Berichtsergebnisse festlegen.

Weitere Informationen zum Erstellen von Filtern finden Sie im Artikel [Filterübersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Weitere Informationen zur Verwendung der bedingten Formatierung in Ansichten finden Sie im Artikel [Bedingte Formatierung in Ansichten verwenden](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Filter- und Bedingungs-Modifikatoren

Einige Modifikatoren sind integriert und Sie können sie aus einem Dropdown-Menü innerhalb Ihrer Filter- oder bedingten Formatierungsanweisung auswählen. Andere Modifikatoren können nur in Textmodusfiltern verwendet werden.

Weitere Informationen zum Verständnis des Textmodus finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Eine Liste der integrierten Zeitrahmen-Modifikatoren finden Sie im Artikel [Berichte nach Zeitrahmen filtern](../../../reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

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
   <td> <p><strong>ist leer</strong> </p> </td> 
   <td> <p><strong>blank</strong> </p> </td> 
   <td> <p>Das Feld existiert für das Objekt, aber das Feld hat derzeit keinen Wert.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>ist nicht leer</strong> </p> </td> 
   <td> <p><strong>nicht leer</strong> </p> </td> 
   <td> <p>Das Feld, nach dem Sie filtern, ist vorhanden und hat einen Wert.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>null</strong> </p> </td> 
   <td> <p>Das Feld ist entweder leer oder existiert nicht. Sie möchten beispielsweise nach Elementen ohne übergeordnete Aufgaben-ID suchen. Das bedeutet, dass Sie nur eigenständige Aufgaben sehen möchten. Der Qualifizierer für die "übergeordnete Aufgaben-ID"wäre <strong>null</strong>, da eine Aufgabe ohne ID (in diesem Fall die übergeordnete Aufgabe) nicht vorhanden ist. </p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters mit dem Textmodus</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>Das Feld, nach dem Sie filtern, ist vorhanden und enthält einen anderen Wert als null.</p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters mit dem Textmodus</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Enthält</strong> </p> </td> 
   <td> <p><strong>cicontains</strong> </p> </td> 
   <td> <p>Dies ist die Version <i>nicht von Schreibweise abhängig </i> von <strong>enthält </strong>. Beispiel: <code>cicontains inf</code> erfasst jeden Wert, der entweder <code>Inf</code> oder <code>inf</code> enthält.</p> <p> <p>Hinweis: Adobe Workfront sucht nach dem genauen Wort oder der Wortgruppe, das bzw. die Sie für jede Filteranweisung angeben. Wenn Sie beispielsweise nach einem Projekt suchen, das die Wortgruppe <code>new project</code> im Namen enthält, zeigt Workfront keine Projekte an, die nur <code>new</code> oder nur <code>project</code> oder <code>new main project</code> im Namen enthalten. Der Filter findet nur Projekte mit dem genauen Wortlaut <code>new project</code> im Namen.</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>enthält nicht</strong> </p> </td> 
   <td> <p><strong>cinotcontains</strong> </p> </td> 
   <td> <p>Dies ist die Version <i>nicht von Schreibweise abhängig </i> von <strong>enthält nicht </strong>.</p><p>Dieser Modifikator filtert nach Elementen, denen der angegebene Wert fehlt.</p> <p>Beispiel: <code>does not contain inf</code> erfasst alles ohne <code>Inf</code> oder <code>inf</code> im Namen.</p> <p>Hinweis: <span>Wenn das Feld, nach dem Sie filtern, mehrere Optionen aufweist, werden die Ergebnisse herausgefiltert, die sowohl die von Ihnen festgelegte Auswahl als auch die von Ihnen angegebene Auswahl und alle weiteren Optionen enthalten.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>contains</strong> </p> </td> 
   <td> <p> Sucht während der gesamten Textzeichenfolge nach dem angegebenen Text <i>zwischen Groß- und Kleinschreibung unterscheiden</i>.</p> <p>Beispielsweise erfasst die Verwendung von <code>contains Inf</code> alles mit <code>Inf</code> darin, z. B. das Wort <code>Infinity.</code></p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Filter im Textmodus bearbeiten</a>.</p> </td> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>Er filtert nach Elementen, bei denen der angegebene Wert <i>zwischen Groß- und Kleinschreibung unterschieden</i> fehlt.</p> <p>Beispiel: <code>notcontains inf</code> erfasst alles ohne <code>inf</code>, zeigt jedoch Werte an, die <code>Inf</code> enthalten.</p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters mit dem Textmodus</a>.</p> </td> 
  </tr> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>Dies ist die Option <i>nicht von Schreibweise abhängig </i> von <strong>eq</strong>. Es wird nur eine exakte Übereinstimmung mit dem gesuchten Wert zurückgegeben.</p> <p>Wenn beispielsweise nach einer Aufgabe mit einem bestimmten Namen gesucht wird, sucht <code>task name cieq test</code> nach Aufgaben mit dem Namen <code>Test</code>, <code>TEST</code> oder <code>Test</code>, findet jedoch keine Aufgabe mit dem Namen <code>test 123.</code></p> <p>Bei der Suche nach einem Status wird der Modifikator <strong>cieq</strong> nicht unterstützt. Verwenden Sie den Modifikator "Groß-/Kleinschreibung beachten", <strong>eq</strong>, um nach einem Status zu suchen.</p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters mit dem Textmodus</a>.</p> </td>
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>cine</strong> </td> 
   <td> <p>Dies ist die Option <i>nicht von Schreibweise abhängig </i> von <strong>ne</strong> und das Gegenteil des Modifikators <b>cieq</b>. Es werden nur Ergebnisse zurückgegeben, die keine exakte Übereinstimmung mit dem gesuchten Wert sind, nicht jedoch die Groß-/Kleinschreibung des Werts.</p> <p>Beispiel: <b>cine</b> gibt Werte zurück, die weder "aktuell"noch "Aktuell"entsprechen. </p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters mit dem Textmodus</a>.</p> </td> 
  </tr>   <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>Dieser Modifikator gibt nur eine exakte Übereinstimmung von <i>zwischen Groß- und Kleinschreibung unterscheiden</i> mit dem gesuchten Wert zurück.</p> <p>Wenn Sie beispielsweise nach vollständigen Projekten suchen, gibt <code>eq CPL</code> alle Projekte mit dem Status "Complete"zurück. <code>eq CPL, CUR</code> gibt kein Ergebnis zurück, da ein Projekt nicht vollständig und aktuell sein kann.</p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters mit dem Textmodus</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>Dies ist die <i>Unterscheidung zwischen Groß- und Kleinschreibung </i> gegenüber <strong>eq</strong>. Es werden nur Ergebnisse zurückgegeben, die nicht exakt mit dem gesuchten Wert übereinstimmen, und es wird auch die Groß-/Kleinschreibung des Werts berücksichtigt.</p> <p>Beispiel: <b>ne</b> gibt Werte zurück, die nicht "Aktuell"sind, gibt jedoch keine Werte zurück, die nicht mit "Aktuell"übereinstimmen. </p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters mit dem Textmodus</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>ciin</strong> </p> </td> 
   <td> <p> Dies ist die Version <i>nicht von Schreibweise abhängig </i> von <strong>in</strong>.</p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters mit dem Textmodus</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cinotin</strong> </p> </td> 
   <td> <p>Dies ist die Version <i>nicht von Schreibweise abhängig </i> von <strong>notin</strong>.</p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters mit dem Textmodus</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>Equal</strong> </p> </td> 
   <td> <p><strong>in</strong> </p> </td> 
   <td> <p>Mit diesem Modifikator können Sie eine kommagetrennte Liste von <i>zwischen Groß- und Kleinschreibung unterschieden</i> Variablen erstellen, um sie mit einem einzelnen Attribut zu vergleichen, das in einem Filter ausgewertet wird. Die gesamte Liste wird als OR-Anweisung behandelt und gibt Ergebnisse zurück, die die Kriterien einer oder mehrerer Variablen erfüllen.</p> <p>Wenn Sie beispielsweise nach Projekten suchen, gibt die Verwendung von <code>in CUR, PLN, CPL</code> alle Projekte zurück, die sich im Status "Aktuell", "ODER Planung"oder "Abgeschlossen"befinden.</p> <p>Der integrierte Modifikator <strong>Equal</strong> entspricht dem Textmodus-Modifikator von <strong>in</strong>. Das bedeutet, dass Sie für das Feld "Gleich mit mehreren Werten"auswählen können.</p> <p>Beispielsweise können Sie in einem Projektbericht "Status gleich Aktuell, Planung, Tod"auswählen und Projekte in einem dieser Status anzeigen.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Nicht gleich</strong> </p> </td> 
   <td> <p><strong>notin</strong> </p> </td> 
   <td> <p>Dies ist die <i>Unterscheidung zwischen Groß- und Kleinschreibung </i> gegenüber <strong>in</strong>. Es werden nur Ergebnisse zurückgegeben, die nicht in der angegebenen Liste enthalten sind.</p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters mit dem Textmodus</a>.</p> <p>Hinweis: <span>Wenn das Feld, nach dem Sie filtern, mehrere Optionen aufweist, werden die Ergebnisse herausgefiltert, die sowohl die von Ihnen festgelegte Auswahl als auch die von Ihnen angegebene Auswahl und alle weiteren Optionen enthalten.</span> </p> </td> 
  </tr>
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>like</strong> </p> </td> 
   <td> <p>Dieser Modifikator sucht in ähnlicher Weise wie <strong>contains</strong> nach Teilen einer Textzeichenfolge, bei der <i>zwischen Groß- und Kleinschreibung unterschieden wird</i>. <strong>like</strong> bietet jedoch die Möglichkeit, Platzhalterzeichen einzufügen, um den Text aufzuschlüsseln.</p> <p>Wenn Sie beispielsweise nach Notizen suchen, gibt die Verwendung von <code>like %Current% %Dead%</code> einen Hinweis zurück, der die Wortgruppe "Aktuell bis tot"enthält. Es enthält keine Hinweise, die "Dead to Current"(Taubheit bis aktuell) enthalten. Jeder Wert wird in der angegebenen Reihenfolge durchsucht. Der % stellt eine Platzhalterkarte dar, um Zeichen oder Textsegmente zu ersetzen. Ein Unterstrich kann auch für ein einzelnes Platzhalterzeichen verwendet werden, wie in <code>like Project_</code> , das sowohl "Projekt"als auch "Projekte"zurückgibt. Wenn Sie beim Filtern einen Modifikator <strong>like</strong> oder <strong>clike</strong> verwenden möchten, empfehlen wir, %- oder _-Zeichen in benutzerdefinierten Datenfeldnamen, Parameteroptionenwerten oder anderen Objektnamen zu vermeiden.</p><p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters mit dem Textmodus</a>.</p> </td> 
  </tr>  
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cilike</strong> </p> </td> 
   <td> <p>Dies ist die Version <i>nicht von Schreibweise abhängig </i> von <strong>like</strong>. Beispiel: <code>cilike %Current% %Dead%</code> gibt alle Notizen zurück, die <code>Current to Dead</code> oder <code>current to dead</code> enthalten.</p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters mit dem Textmodus</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>Existiert nicht </strong> </td> 
   <td><strong>NOTEXISTS</strong> </td> 
   <td> <p>Dieser Modifikator wird nur mit komplexen Filtern in einer EXISTS-Anweisung verwendet. Diese Filter beziehen sich nur auf die folgenden Objekte: </p> 
    <ul> 
     <li>Objekte, die sich über mehrere Ebenen in der Objekthierarchie erstrecken </li> 
     <li>Fehlende Objekte </li> 
    </ul> <p>Informationen zum Erstellen komplexer Filter mithilfe von EXISTS-Anweisungen finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">Erstellen komplexer Textmodusfilter mit EXISTS-Anweisungen</a>. Dies ist der einzige Modifikator, der in EXISTS-Anweisungen verwendet wird.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Größer als</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>Hierbei wird nach allen Ergebnissen gesucht, deren Wert größer als der eingegebene Wert ist, wobei der eingegebene Wert nicht berücksichtigt wird.</p> </td> 
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
   <td> <p><strong>Kleiner als gleich</strong> </p> </td> 
   <td> <p><strong>lte</strong> </p> </td> 
   <td> <p>Hierbei werden alle Ergebnisse gesucht, deren Wert kleiner oder gleich dem eingegebenen Wert ist.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Between</strong> </p> </td> 
   <td> <p><strong>zwischen</strong> </p> </td> 
   <td> <p>Bietet zwei erforderliche Feldwerte und sucht nach allen Ergebnissen innerhalb des Bereichs beider Felder, einschließlich der eingegebenen Werte.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>nicht zwischen</strong> </p> </td> 
   <td> <p>Dies ist das Gegenteil von <strong>zwischen </strong>. Es stellt zwei erforderliche Wertefelder bereit und sucht nach allen Ergebnissen außerhalb des Bereichs beider Felder einschließlich der eingegebenen Werte.</p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters mit dem Textmodus</a>.</p> </td> 
  </tr>

</tbody> 
</table>
