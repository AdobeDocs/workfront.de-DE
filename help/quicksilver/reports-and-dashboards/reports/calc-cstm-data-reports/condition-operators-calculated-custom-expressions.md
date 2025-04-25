---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Bedingungsoperatoren in berechneten benutzerdefinierten Ausdrücken
description: Sie können im Textmodus beim Erstellen berechneter benutzerdefinierter Daten in Adobe Workfront Bedingungsoperatoren oder -modifikatoren verwenden.
author: Nolan
feature: Reports and Dashboards
exl-id: ce98ca39-cb86-4ef7-b75c-29ceb916e885
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '718'
ht-degree: 1%

---

# Bedingungsoperatoren in berechneten benutzerdefinierten Feldern

<!-- Audited: 2/2024 -->

Sie können im Textmodus beim Erstellen berechneter benutzerdefinierter Daten in Adobe Workfront Bedingungsoperatoren oder -modifikatoren verwenden. Informationen zur Verwendung des Textmodus in Workfront finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Bedingungsoperatoren oder -modifikatoren helfen beim Erstellen einer Bedingungsanweisung, indem sie vorhandene Workfront-Felder in -Anweisungen verbinden und ein neues Feld generieren. Bedingungsoperatoren werden meist verwendet, um die Bedingung einer „IF“-Anweisung zu erstellen.

Sie können „IF“-Anweisungen in Workfront verwenden, um Datenfelder sowohl für Reporting- als auch für benutzerdefinierte Datenzwecke zu vergleichen, zu formatieren und miteinander zu verknüpfen.

Sie können „IF“-Anweisungen für die folgenden Workfront-Elemente erstellen:

* Ansichten
* Gruppierungen
* Berechnete benutzerdefinierte Felder

Weitere Informationen zum Erstellen von „IF“-Anweisungen finden Sie unter [ „IF“-Anweisungen - Übersicht](../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md).

Die Beispiele in diesem Handbuch veranschaulichen die Verwendung von Bedingungsoperatoren in berechneten benutzerdefinierten Feldern. Sie können sie auch in berechneten benutzerdefinierten Spalten oder Gruppierungen verwenden, wenn Sie die korrekte Syntax für berechnete benutzerdefinierte Felder in Berichten befolgen.

Informationen über den Syntaxunterschied zwischen den berechneten benutzerdefinierten Feldern und den berechneten benutzerdefinierten Daten in Berichten finden Sie unter [Berechnete benutzerdefinierte Felder im Vergleich zu berechneten Spalten](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Im API Explorer finden Sie die Felder, auf die Sie in Ihren berechneten benutzerdefinierten Ausdrücken verweisen möchten. Weitere Informationen zum API-Explorer finden Sie unter [API-Explorer](../../../wf-api/general/api-explorer.md).

Sie können die folgenden Bedingungsmodifikatoren in Workfront verwenden:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Bedingungsoperator</th> 
   <th>Syntax des Bedingungsoperators</th> 
   <th>Definition des Bedingungsoperators</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Equal</td> 
   <td>= </td> 
   <td> <p>Verwenden Sie diesen Operator, um anzugeben, dass die Bedingung erfüllt ist, wenn das erste Feld Ihrer Anweisung dem zweiten Feld entspricht.</p> <p>Verwenden Sie beispielsweise die folgende Anweisung in einem berechneten benutzerdefinierten Feld, um eine „IF“-Anweisung zu erstellen, die das geplante Abschlussdatum mit dem voraussichtlichen Abschlussdatum einer Aufgabe vergleicht: </p><p><code>IF({projectedCompletionDate}={plannedCompletionDate},"On Track","Off Track")</code></p> </td> 
  </tr> 
  <tr> 
   <td>Größer als </td> 
   <td>&gt; </td> 
   <td>Verwenden Sie diesen Operator, um anzugeben, dass die Bedingung erfüllt ist, wenn das erste Feld Ihrer Anweisung größer als das zweite Feld ist. <p>Verwenden Sie beispielsweise die folgende Anweisung in einem berechneten benutzerdefinierten Feld, um eine „IF“-Anweisung zu erstellen, die das geplante Abschlussdatum mit dem voraussichtlichen Abschlussdatum einer Aufgabe vergleicht: </p><p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Late","")</code></p></td> 
  </tr> 
  <tr> 
   <td>Größer als oder gleich </td> 
   <td>&gt;= </td> 
   <td>Verwenden Sie diesen Operator, um anzugeben, dass die Bedingung erfüllt ist, wenn das erste Feld Ihrer Anweisung größer oder gleich dem zweiten Feld ist. <p>Verwenden Sie beispielsweise die folgende Anweisung in einem berechneten benutzerdefinierten Feld, um eine „IF“-Anweisung zu erstellen, die das geplante Abschlussdatum mit dem voraussichtlichen Abschlussdatum einer Aufgabe vergleicht: </p><p><code>IF({projectedCompletionDate}&gt;={plannedCompletionDate},"Late","Early")</code></p></td> 
  </tr> 
  <tr> 
   <td>Kleiner als </td> 
   <td>&lt; </td> 
   <td>Mit diesem Operator geben Sie an, dass die Bedingung erfüllt ist, wenn  Das erste Feld Ihrer Anweisung ist kleiner als das zweite Feld. <p>Verwenden Sie beispielsweise die folgende Anweisung in einem berechneten benutzerdefinierten Feld, um eine „IF“-Anweisung zu erstellen, die das geplante Abschlussdatum mit dem voraussichtlichen Abschlussdatum einer Aufgabe vergleicht: </p><p><code>IF({projectedCompletionDate}&lt;{plannedCompletionDate},"Early","")</code></p></td> 
  </tr> 
  <tr> 
   <td>Kleiner oder gleich </td> 
   <td>&lt;= </td> 
   <td>Mit diesem Operator geben Sie an, dass die Bedingung erfüllt ist, wenn  Das erste Feld Ihrer Anweisung ist kleiner oder gleich dem zweiten Feld. <p>Verwenden Sie beispielsweise die folgende Anweisung in einem berechneten benutzerdefinierten Feld, um eine „IF“-Anweisung zu erstellen, die das geplante Abschlussdatum mit dem voraussichtlichen Abschlussdatum einer Aufgabe vergleicht: </p><p><code>IF({projectedCompletionDate}&lt;={plannedCompletionDate},"Early","Late")</code></p></td> 
  </tr> 
  <tr> 
   <td>Ist nicht </td> 
   <td>! </td> 
   <td> <p>Fügen Sie diesen Operator vor einem der oben genannten Operatoren hinzu, um den Operator zu negieren. </p> <p>Beispiel: </p> 
    <ul> 
     <li>Gleich: = </li> 
     <li>Ist nicht gleich: != </li> 
    </ul> <p>Wenn Sie diesen Operator vor den folgenden Datenausdrücken hinzufügen, wird eine negative Anweisung zu Ausdrücken hinzugefügt: </p> 
    <ul> 
     <li>CONTAINS </li> 
     <li>IN </li> 
     <li>IFIN </li> 
     <li>ISBLANK </li> 
    </ul> <p>Weitere Informationen zu diesen Datenausdrücken und eine vollständige Liste finden Sie unter <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md" class="MCXref xref">Übersicht über berechnete Datenausdrücke</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>Oder </td> 
   <td>|| </td> 
   <td> <p>Verwenden Sie diesen Operator, um anzugeben, dass die Bedingung erfüllt ist, wenn der Ausdruck  Sucht entweder den ersten oder den zweiten Wert Ihrer Anweisung. </p> <p>Verwenden Sie beispielsweise die folgende Anweisung in einem berechneten benutzerdefinierten Feld, um eine „IF“-Anweisung zu erstellen, die Projekte im aktuellen Status oder im Planungsstatus als „Aktiv“ markiert: </p><p><code>IF({status}="PLN"||{status}="CUR","Active","Not Active")</code></p> </td> 
  </tr> 
  <tr> 
   <td> und </td> 
   <td>&amp;&amp; </td> 
   <td> <p>Verwenden Sie diesen Operator, um anzugeben, dass die Bedingung erfüllt ist, wenn der Ausdruck  Sucht ein Element, das zwei Bedingungen gleichzeitig erfüllt. </p> <p>Verwenden Sie beispielsweise die folgende Anweisung in einem berechneten benutzerdefinierten Feld, um eine „IF“-Anweisung zu erstellen, die Projekte im aktuellen Status mit der Bedingung „Gefährdet“ findet und als „Mediation erforderlich“ kennzeichnet. </p><p><code>IF({status}="CUR"&&{condition}="AR","Mediation Needed","")</code></p> </td> 
  </tr> 
 </tbody> 
</table>
