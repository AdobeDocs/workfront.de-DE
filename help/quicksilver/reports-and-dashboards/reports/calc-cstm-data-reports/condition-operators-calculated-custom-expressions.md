---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Bedingungsoperatoren in berechneten benutzerdefinierten Ausdrücken
description: Sie können Bedingungsoperatoren oder Modifikatoren beim Erstellen berechneter benutzerdefinierter Daten in Adobe Workfront im Textmodus verwenden.
author: Nolan
feature: Reports and Dashboards
exl-id: ce98ca39-cb86-4ef7-b75c-29ceb916e885
source-git-commit: 3e1e651662f9ff695d475ffcbdc77f0802d108f1
workflow-type: tm+mt
source-wordcount: '718'
ht-degree: 1%

---

# Bedingungsoperatoren in berechneten benutzerdefinierten Feldern

Sie können Bedingungsoperatoren oder Modifikatoren beim Erstellen berechneter benutzerdefinierter Daten in Adobe Workfront im Textmodus verwenden.

Informationen zur Verwendung des Textmodus in Workfront finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Bedingungsoperatoren oder -modifikatoren helfen beim Erstellen einer Bedingungsanweisung, indem sie bestehende Workfront-Felder in -Anweisungen verbinden und ein neues Feld generieren. Die häufigste Verwendung von Bedingungsoperatoren besteht darin, die Bedingung einer &quot;IF&quot;-Anweisung zu erstellen.

Sie können &quot;IF&quot;-Anweisungen in Workfront verwenden, um Datenfelder für Berichterstellungs- und benutzerdefinierte Datenzwecke zu vergleichen, zu formatieren und zu zeichenfolgen.

Sie können &quot;IF&quot;-Anweisungen für die folgenden Workfront-Elemente erstellen:

* Ansichten
* Gruppierungen
* Berechnete benutzerdefinierte Felder

Weitere Informationen zum Erstellen von &quot;IF&quot;-Anweisungen finden Sie unter [Übersicht über &quot;IF&quot;-Anweisungen](../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md).

Die Beispiele in diesem Handbuch veranschaulichen die Verwendung von Bedingungsoperatoren in berechneten benutzerdefinierten Feldern. Sie können sie auch in berechneten benutzerdefinierten Spalten oder Gruppierungen verwenden, wenn Sie die richtige Syntax für berechnete benutzerdefinierte Felder in Berichten befolgen.

Informationen zur Syntaxdifferenz zwischen berechneten benutzerdefinierten Feldern und berechneten benutzerdefinierten Daten in Berichten finden Sie unter [Berechnete benutzerdefinierte Felder vs. berechnete Spalten](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Im API Explorer finden Sie die Felder, die Sie in Ihren berechneten benutzerdefinierten Ausdrücken referenzieren möchten. Informationen zum API Explorer finden Sie unter [API-Explorer](../../../wf-api/general/api-explorer.md).

Sie können die folgenden Bedingungsmodifikatoren in Workfront verwenden:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Bedingungsoperator</th> 
   <th>Syntax des Bedingungsbedieners</th> 
   <th>Definition des Bedingungsbedieners</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Gleich (ignoriert Groß- und Kleinschreibung)</td> 
   <td>= </td> 
   <td> <p>Verwenden Sie diesen Operator, um anzugeben, dass die Bedingung erfüllt ist, wenn das erste Feld Ihrer Anweisung dem zweiten Feld entspricht.</p> <p>Verwenden Sie beispielsweise die folgende Anweisung in einem berechneten benutzerdefinierten Feld, um eine "IF"-Anweisung zu erstellen, die das geplante Abschlussdatum mit dem geplanten Abschlussdatum einer Aufgabe vergleicht: </p><p><code>IF({projectedCompletionDate}={plannedCompletionDate},"On Track","Off Track")</code></p> </td> 
  </tr> 
  <tr> 
   <td>Größer als </td> 
   <td>&gt; </td> 
   <td>Verwenden Sie diesen Operator, um anzugeben, dass die Bedingung erfüllt ist, wenn das erste Feld Ihrer Anweisung größer als das zweite Feld ist. <p>Verwenden Sie beispielsweise die folgende Anweisung in einem berechneten benutzerdefinierten Feld, um eine "IF"-Anweisung zu erstellen, die das geplante Abschlussdatum mit dem geplanten Abschlussdatum einer Aufgabe vergleicht: </p><p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Late","")</code></p></td> 
  </tr> 
  <tr> 
   <td>Größer oder gleich </td> 
   <td>&gt;= </td> 
   <td>Verwenden Sie diesen Operator, um anzugeben, dass die Bedingung erfüllt ist, wenn das erste Feld Ihrer Anweisung größer oder gleich dem zweiten Feld ist. <p>Verwenden Sie beispielsweise die folgende Anweisung in einem berechneten benutzerdefinierten Feld, um eine "IF"-Anweisung zu erstellen, die das geplante Abschlussdatum mit dem geplanten Abschlussdatum einer Aufgabe vergleicht: </p><p><code>IF({projectedCompletionDate}&gt;={plannedCompletionDate},"Late","Early")</code></p></td> 
  </tr> 
  <tr> 
   <td>Kleiner als </td> 
   <td>&lt; </td> 
   <td>Verwenden Sie diesen Operator, um anzugeben, dass die Bedingung erfüllt ist, wenn das erste Feld Ihrer Anweisung kleiner als das zweite Feld ist. <p>Verwenden Sie beispielsweise die folgende Anweisung in einem berechneten benutzerdefinierten Feld, um eine "IF"-Anweisung zu erstellen, die das geplante Abschlussdatum mit dem geplanten Abschlussdatum einer Aufgabe vergleicht: </p><p><code>IF({projectedCompletionDate}&lt;{plannedCompletionDate},"Early","")</code></p></td> 
  </tr> 
  <tr> 
   <td>Kleiner oder gleich </td> 
   <td>&lt;= </td> 
   <td>Verwenden Sie diesen Operator, um anzugeben, dass die Bedingung erfüllt ist, wenn das erste Feld Ihrer Anweisung kleiner oder gleich dem zweiten Feld ist. <p>Verwenden Sie beispielsweise die folgende Anweisung in einem berechneten benutzerdefinierten Feld, um eine "IF"-Anweisung zu erstellen, die das geplante Abschlussdatum mit dem geplanten Abschlussdatum einer Aufgabe vergleicht: </p><p><code>IF({projectedCompletionDate}&lt;={plannedCompletionDate},"Early","Late")</code></p></td> 
  </tr> 
  <tr> 
   <td>Ist nicht </td> 
   <td>! </td> 
   <td> <p>Fügen Sie diesen Operator vor einem der oben genannten Operatoren hinzu, um den Operator zu umkehren. </p> <p>Beispiel: </p> 
    <ul> 
     <li>Gleich: = </li> 
     <li>Ist nicht gleich: != </li> 
    </ul> <p>Durch Hinzufügen dieses Operators vor den folgenden Datenausdrücken wird Ausdrücken eine negative Anweisung hinzugefügt: </p> 
    <ul> 
     <li>CONTAINS </li> 
     <li>IN </li> 
     <li>IFIN </li> 
     <li>ISBLANK </li> 
    </ul> <p>Informationen zu diesen Datenausdrücken sowie eine vollständige Liste finden Sie unter <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md" class="MCXref xref">Übersicht über berechnete Datenausdrücke</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>Oder </td> 
   <td>|| </td> 
   <td> <p>Verwenden Sie diesen Operator, um anzugeben, dass die Bedingung erfüllt ist, wenn der Ausdruck den ersten oder zweiten Wert Ihrer Anweisung findet. </p> <p>Verwenden Sie beispielsweise die folgende Anweisung in einem berechneten benutzerdefinierten Feld, um eine "IF"-Anweisung zu erstellen, die Projekte im Status "Aktuell"oder "Planung"als "Aktiv"markiert: </p><p><code>IF({status}="PLN"||{status}="CUR","Active","Not Active")</code></p> </td> 
  </tr> 
  <tr> 
   <td> und </td> 
   <td>&amp;&amp; </td> 
   <td> <p>Verwenden Sie diesen Operator, um anzugeben, dass die Bedingung erfüllt ist, wenn der Ausdruck ein Element findet, das zwei Bedingungen gleichzeitig erfüllt. </p> <p>Verwenden Sie beispielsweise die folgende Anweisung in einem berechneten benutzerdefinierten Feld, um eine "IF"-Anweisung zu erstellen, die Projekte sucht, die sich im aktuellen Status befinden und die Bedingung "Risiko"aufweisen, und sie als "Erforderliche Mediation"kennzeichnet. </p><p><code>IF({status}="CUR"&&{condition}="AR","Mediation Needed","")</code></p> </td> 
  </tr> 
 </tbody> 
</table>
