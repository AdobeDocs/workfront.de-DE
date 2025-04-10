---
product-area: reporting
navigation-topic: reporting-elements
title: Filter- und Bedingungsmodifikatoren
description: Mit den Filter- und Bedingungsmodifikatoren können Sie Filter erstellen und Bedingungen zur Formatierung Ihrer Berichtsergebnisse festlegen.
author: Nolan
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: b2b17c34fe4887e291e69facf76f5071bca43b06
workflow-type: tm+mt
source-wordcount: '1565'
ht-degree: 0%

---

# Filter- und Bedingungsmodifikatoren

<!-- Audited: 11/2024 -->

<!--(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit)-->

Mit den Filter- und Bedingungsmodifikatoren können Sie Filter erstellen und Bedingungen zur Formatierung Ihrer Berichtsergebnisse festlegen.

Weitere Informationen zum Erstellen von Filtern finden Sie im Artikel [Filter - Übersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Weitere Informationen zur Verwendung der bedingten Formatierung in Ansichten finden Sie im Artikel [Verwenden der bedingten Formatierung in Ansichten](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Filter- und Bedingungsmodifikatoren

Einige Modifikatoren sind integriert und Sie können sie aus einem Dropdown-Menü in Ihrem Filter oder Ihrer bedingten Formatierungsanweisung auswählen. Andere Modifikatoren können nur in Textmodusfiltern verwendet werden.

Weitere Informationen zum Textmodus finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Eine Liste der integrierten Zeitrahmen-Modifikatoren finden Sie im Artikel [Filtern von Berichten nach Zeitrahmen](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

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
   <td> <p><strong>Ist leer</strong> </p> </td> 
   <td> <p><strong>blank</strong> </p> </td> 
   <td> <p>Das Feld existiert für das Objekt, aber das Feld hat derzeit keinen Wert.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Ist nicht leer</strong> </p> </td> 
   <td> <p><strong>nicht leer</strong> </p> </td> 
   <td> <p>Das Feld, nach dem gefiltert werden soll, ist vorhanden und wurde mit einem Wert versehen.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>null</strong> </p> </td> 
   <td> <p>Das Feld ist entweder leer oder nicht vorhanden. Sie möchten beispielsweise nach Elementen ohne ID der übergeordneten Aufgabe suchen. Das bedeutet, dass Sie nur eigenständige Aufgaben anzeigen möchten. Der Qualifizierer für die „ID der übergeordneten Aufgabe“ wäre <strong>null</strong> da eine Aufgabe ohne ID (in diesem Fall das übergeordnete Element) nicht vorhanden ist. </p> <p>Dieser Modifikator kann nur in Filtern im Textmodus verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters im Textmodus</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notNull</strong> </p> </td> 
   <td> <p>Das Feld, nach dem Sie filtern, ist vorhanden und enthält einen anderen Wert als null.</p> <p>Dieser Modifikator kann nur in Filtern im Textmodus verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters im Textmodus</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Enthält</strong> </p> </td> 
   <td> <p><strong>CiContains</strong> </p> </td> 
   <td> <p>Dies ist die (<i> Groß-/</i>) Version von <strong>contains</strong>. Beispiel: <code>cicontains inf</code> erfasst jeden Wert, der entweder <code>Inf</code> oder <code>inf</code> enthält.</p> <p> <p>Hinweis: Adobe Workfront sucht für jede Filteranweisung nach dem Wort oder der Phrase, das bzw. die Sie angeben. Wenn Sie beispielsweise nach einem Projekt suchen, das die im Namen <code>new project</code> Phrase enthält, zeigt Workfront keine Projekte an, die nur <code>new</code> oder nur <code>project</code> oder <code>new main project</code> im Namen enthalten. Der Filter findet nur Projekte mit der exakten Phrase <code>new project</code> im Namen.</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Enthält nicht</strong> </p> </td> 
   <td> <p><strong>cinotcontains</strong> </p> </td> 
   <td> <p>Dies ist die (<i> Groß-/</i>) Version von <strong>notContains</strong>.</p><p>Dieser Modifikator filtert nach Elementen, denen der angegebene Wert fehlt.</p> <p>Beispiel: <code>does not contain inf</code> erfasst alles, ohne <code>Inf</code> oder <code>inf</code> im Namen.</p> <p>Hinweis: <span>Wenn das Feld, nach dem gefiltert werden soll, mehrere Optionen hat, werden die Ergebnisse herausgefiltert, die sowohl die angegebene Auswahl als auch die angegebene Auswahl und alle zusätzlichen Auswahlmöglichkeiten enthalten.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>Enthält</strong> </p> </td> 
   <td> <p> Sucht den angegebenen <i> (unter Berücksichtigung </i> Groß-/Kleinschreibung) über die gesamte Textzeichenfolge.</p> <p>Die Verwendung von <code>contains Inf</code> erfasst beispielsweise alles, was <code>Inf</code> enthält, wie das Wort . <code>Infinity.</code></p> <p>Dieser Modifikator kann nur in Textmodusfiltern verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters im Textmodus</a>.</p> </td> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>NotContains</strong> </p> </td> 
   <td> <p>Er filtert nach Elementen, denen der angegebene Wert <i> Groß-/</i> fehlt.</p> <p>Beispielsweise erfasst <code>notcontains inf</code> alles ohne <code>inf</code>, zeigt jedoch Werte an, die <code>Inf</code> enthalten.</p> <p>Dieser Modifikator kann nur in Filtern im Textmodus verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters im Textmodus</a>.</p> </td> 
  </tr> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>Dies ist die <i>Groß-/</i>) Option von <strong>eq</strong>. Gibt nur eine exakte Übereinstimmung mit dem gesuchten Wert zurück.</p> <p>Wenn <code>task name cieq test</code> beispielsweise nach einer Aufgabe mit einem bestimmten Namen sucht, findet er Aufgaben, deren Name <code>Test</code>, <code>TEST</code> oder <code>Test</code> lautet, aber keine Aufgabe mit dem Namen <code>test 123.</code></p> <p>Bei der Suche nach einem Status <strong> der Modifikator </strong>cieq“ nicht unterstützt. Sie sollten den Modifikator zur Unterscheidung von Groß- <strong> Kleinschreibung (</strong>) verwenden, um nach einem Status zu suchen.</p> <p>Dieser Modifikator kann nur in Filtern im Textmodus verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters im Textmodus</a>.</p> </td>
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>Cine</strong> </td> 
   <td> <p>Dies ist die Option <i>ohne </i>) von <strong>ne</strong>, und sie ist das Gegenteil des <b>cieq</b>-Modifikators. Es werden nur Ergebnisse zurückgegeben, die nicht exakt mit dem gesuchten Wert übereinstimmen, wobei die Groß-/Kleinschreibung des Werts nicht berücksichtigt wird.</p> <p>Beispielsweise gibt <b>cine</b> alle Werte zurück, die weder „current“ noch „Current“ entsprechen. </p> <p>Dieser Modifikator kann nur in Filtern im Textmodus verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters im Textmodus</a>.</p> </td> 
  </tr>   <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>äq</strong> </p> </td> 
   <td> <p>Dieser Modifikator gibt nur eine exakte Übereinstimmung des gesuchten Werts <i> Berücksichtigung </i> Groß-/Kleinschreibung zurück.</p> <p>Wenn Sie beispielsweise nach abgeschlossenen Projekten suchen, gibt <code>eq CPL</code> alle Projekte mit dem Status Abgeschlossen zurück. <code>eq CPL, CUR</code> gibt kein Ergebnis zurück, da ein Projekt nicht gleichzeitig abgeschlossen und aktuell sein kann.</p> <p>Dieser Modifikator kann nur in Filtern im Textmodus verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters im Textmodus</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>Dies ist das <i>Groß-/Kleinschreibung</i> Gegenteil von <strong>eq</strong>. Es werden nur Ergebnisse zurückgegeben, die nicht genau mit dem gesuchten Wert übereinstimmen. Außerdem wird die Groß-/Kleinschreibung des Werts zurückgegeben.</p> <p>Beispielsweise gibt <b>ne</b> alle Werte zurück, die nicht gleich „current“ sind, aber es werden keine Werte zurückgegeben, die nicht gleich „current“ sind. </p> <p>Dieser Modifikator kann nur in Filtern im Textmodus verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters im Textmodus</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>Münze</strong> </p> </td> 
   <td> <p> Dies ist die (<i> Groß-/</i>) Version von <strong>in</strong>.</p> <p>Dieser Modifikator kann nur in Filtern im Textmodus verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters im Textmodus</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>Cinotin</strong> </p> </td> 
   <td> <p>Dies ist die (<i> Groß-/</i>) Version von <strong>notin</strong>.</p> <p>Dieser Modifikator kann nur in Filtern im Textmodus verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters im Textmodus</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>Gleich</strong> </p> </td> 
   <td> <p><strong>in</strong> </p> </td> 
   <td> <p>Mit diesem Modifikator können Sie eine kommagetrennte Liste von Variablen erstellen<i> bei denen zwischen Groß- </i> Kleinschreibung unterschieden wird, um sie mit einem einzelnen Attribut zu vergleichen, das in einem Filter ausgewertet wird. Die gesamte Liste wird als OR-Anweisung behandelt und gibt alle Ergebnisse zurück, die die Kriterien einer oder mehrerer der Variablen erfüllen.</p> <p>Wenn Sie beispielsweise nach Projekten suchen, werden bei Verwendung von <code>in CUR, PLN, CPL</code> alle Projekte zurückgegeben, die den Status „Aktuell“, „Planung“ oder „Abgeschlossen“ aufweisen.</p> <p>Der integrierte Modifikator <strong>Gleich</strong> entspricht dem Textmodus-Modifikator von <strong>in</strong>. Dies bedeutet, dass Sie Gleich mit mehreren Werten für das Feld auswählen können.</p> <p>Sie können beispielsweise in einem Projektbericht „Status ist gleich aktuell, Planung, Inaktiv“ auswählen und Projekte mit einem dieser Status anzeigen.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Ungleich</strong> </p> </td> 
   <td> <p><strong>notin</strong> </p> </td> 
   <td> <p>Dies ist das <i>Groß-/Kleinschreibung</i> Gegenteil von <strong>in</strong>. Es werden nur Ergebnisse zurückgegeben, die nicht in der angegebenen Liste enthalten sind.</p> <p>Dieser Modifikator kann nur in Filtern im Textmodus verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters im Textmodus</a>.</p> <p>Hinweis: <span>Wenn das Feld, nach dem gefiltert werden soll, mehrere Optionen hat, werden die Ergebnisse herausgefiltert, die sowohl die angegebene Auswahl als auch die angegebene Auswahl und alle zusätzlichen Auswahlmöglichkeiten enthalten.</span> </p> </td> 
  </tr>
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>Gefällt mir</strong> </p> </td> 
   <td> <p>Dieser Modifikator sucht nach Teilen einer Textzeichenfolge, bei der <i> Groß- </i> Kleinschreibung beachtet wird, ähnlich wie <strong>Enthält</strong>. <strong>like</strong> bietet jedoch die Möglichkeit, Platzhalterzeichen einzufügen, um den Text aufzuteilen.</p> <p>Wenn Sie beispielsweise nach Notizen suchen, gibt <code>like %Current% %Dead%</code> jede Notiz zurück, die den Satz „Aktuell bis tot“ enthält. Es enthält keine Notizen, die „Dead to Current“ enthalten. Jeder Wert wird in der Reihenfolge durchsucht, in der er aufgeführt ist. % stellt einen Platzhalter dar, der Zeichen oder Textsegmente ersetzt. Ein Unterstrich kann auch für ein einzelnes Platzhalterzeichen verwendet werden, wie in <code>like Project_</code>, das sowohl „Projekt“ als auch „Projekte“ zurückgibt. Wenn Sie bei Ihrer Filterung einen <strong>like</strong>- oder <strong>like</strong>-Modifikator verwenden möchten, empfehlen wir, %- oder _-Zeichen in benutzerdefinierten Datenfeldnamen, Parameteroptionenwerten oder anderen Objektnamen zu vermeiden.</p><p>Dieser Modifikator kann nur in Filtern im Textmodus verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters im Textmodus</a>.</p> </td> 
  </tr>  
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cilike</strong> </p> </td> 
   <td> <p>Dies ist die (<i> Groß-/</i>) Version <strong>like</strong>. Beispiel: <code>cilike %Current% %Dead%</code> gibt alle Notizen zurück, die <code>Current to Dead</code> oder <code>current to dead</code> enthalten.</p> <p>Dieser Modifikator kann nur in Filtern im Textmodus verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters im Textmodus</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>Ist nicht vorhanden</strong> </td> 
   <td><strong>NOTEXISTS</strong> </td> 
   <td> <p>Dieser Modifikator wird nur mit komplexen Filtern in einer EXISTS-Anweisung verwendet. Diese Filter beziehen sich nur auf die folgenden Objekte: </p> 
    <ul> 
     <li>Objekte, die sich über mehrere Ebenen in der Objekthierarchie erstrecken </li> 
     <li>Fehlende Objekte </li> 
    </ul> <p>Informationen zum Erstellen komplexer Filter mit EXISTS-Anweisungen finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">Erstellen komplexer Textmodusfilter mit EXISTS-Anweisungen</a>. Dies ist der einzige Modifikator, der in EXISTS-Anweisungen verwendet wird.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>größer als</strong> </p> </td> 
   <td> <p><strong>GT</strong> </p> </td> 
   <td> <p>Hierbei werden alle Ergebnisse mit einem Wert gesucht, der größer ist als der eingegebene Wert, ohne den eingegebenen Wert zu berücksichtigen.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>kleiner als</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>Hierbei werden alle Ergebnisse mit einem Wert gesucht, der kleiner als der eingegebene ist, ohne den eingegebenen Wert zu berücksichtigen.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>größer als gleich</strong> </p> </td> 
   <td> <p><strong>GTE</strong> </p> </td> 
   <td> <p>Hierbei werden alle Ergebnisse mit Werten gesucht, die größer oder gleich dem eingegebenen Wert sind.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Kleiner als gleich</strong> </p> </td> 
   <td> <p><strong>LTE</strong> </p> </td> 
   <td> <p>Hierbei werden alle Ergebnisse mit einem Wert gesucht, der kleiner oder gleich dem eingegebenen Wert ist.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Zwischen</strong> </p> </td> 
   <td> <p><strong>zwischen</strong> </p> </td> 
   <td> <p>Stellt zwei erforderliche Feldwerte bereit und sucht nach allen Ergebnissen innerhalb des Bereichs beider Felder, einschließlich der eingegebenen Werte.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notBetween</strong> </p> </td> 
   <td> <p>Das ist das Gegenteil von <strong>Zwischen</strong>. Es werden zwei erforderliche Wertefelder bereitgestellt und alle Ergebnisse außerhalb des Bereichs beider Felder, einschließlich der eingegebenen Werte, gesucht.</p> <p>Dieser Modifikator kann nur in Filtern im Textmodus verwendet werden. Weitere Informationen zum Textmodus in Filtern finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters im Textmodus</a>.</p> </td> 
  </tr>

</tbody> 
</table>
