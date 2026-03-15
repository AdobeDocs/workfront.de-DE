---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Bedingungsoperatoren in berechneten benutzerdefinierten Ausdrücken
description: Sie können Bedingungsoperatoren oder Modifikatoren verwenden, wenn Sie berechnete benutzerdefinierte Daten in Adobe Workfront erstellen, wenn Sie den Textmodus verwenden.
author: Courtney
feature: Reports and Dashboards
exl-id: ce98ca39-cb86-4ef7-b75c-29ceb916e885
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 5%

---

# Bedingungsoperatoren in berechneten benutzerdefinierten Feldern

<!-- Audited: 2/2024 -->

Sie können Bedingungsoperatoren oder Modifikatoren verwenden, wenn Sie berechnete benutzerdefinierte Daten in Adobe Workfront erstellen, wenn Sie den Textmodus verwenden. Informationen zur Verwendung des Textmodus in Workfront finden Sie unter [Übersicht über den Textmodus](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Bedingungsoperatoren oder Modifikatoren helfen beim Erstellen einer Bedingungsanweisung, indem sie bestehende Workfront-Felder in Anweisungen verbinden und ein neues Feld generieren. Die häufigste Verwendung von Bedingungsoperatoren ist das Erstellen der Bedingung einer &quot;IF&quot;-Anweisung.

Sie können &quot;IF&quot;-Anweisungen in Workfront verwenden, um Datenfelder sowohl für die Berichterstellung als auch für benutzerdefinierte Datenzwecke zu vergleichen, zu formatieren und zusammenzufügen.

Sie können &quot;IF&quot;-Anweisungen für die folgenden Workfront-Elemente erstellen:

* Ansichten 
* Gruppierungen
* Berechnete benutzerdefinierte Felder
* Geschäftsregeln

Weitere Informationen zum Erstellen von „IF“-Anweisungen finden Sie unter [Überblick über „IF“-Anweisungen](../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md).

Die Beispiele in dieser Anleitung veranschaulichen die Verwendung von Bedingungsoperatoren in berechneten benutzerdefinierten Feldern. Sie können sie auch in berechneten benutzerdefinierten Spalten oder Gruppierungen verwenden, wenn Sie der richtigen Syntax für berechnete benutzerdefinierte Felder in Berichten folgen.

Informationen zum Syntaxunterschied zwischen den berechneten benutzerdefinierten Feldern und den berechneten benutzerdefinierten Daten in Berichten finden Sie unter [Berechnete benutzerdefinierte Felder und berechnete Spalten](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Weitere Informationen zu Geschäftsregeln finden Sie unter [Geschäftsregeln erstellen und bearbeiten](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md).

Im API-Explorer finden Sie die Felder, die Sie in den berechneten benutzerdefinierten Ausdrücken referenzieren möchten. Weitere Informationen zum API-Explorer finden Sie unter [API-Explorer](../../../wf-api/general/api-explorer.md).

Sie können die folgenden Bedingungsmodifizierer in Workfront verwenden:

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
   <td> <p>Verwenden Sie diesen Operator, um anzugeben, dass die Bedingung erfüllt ist, wenn das erste Feld Ihrer Anweisung dem zweiten Feld entspricht.</p> <p>Verwenden Sie z. B. die folgende Anweisung in einem berechneten benutzerdefinierten Feld, um eine IF-Anweisung zu erstellen, die das geplante Abschlussdatum mit dem voraussichtlichen Abschlussdatum eines Vorgangs vergleicht: </p><p><code>IF({projectedCompletionDate}={plannedCompletionDate},"On Track","Off Track")</code></p> </td> 
  </tr> 
  <tr> 
   <td>Größer als </td> 
   <td>&gt; </td> 
   <td>Verwenden Sie diesen Operator, um anzugeben, dass die Bedingung erfüllt ist, wenn das erste Feld Ihrer Anweisung größer als das zweite Feld ist. <p>Verwenden Sie z. B. die folgende Anweisung in einem berechneten benutzerdefinierten Feld, um eine IF-Anweisung zu erstellen, die das geplante Abschlussdatum mit dem voraussichtlichen Abschlussdatum eines Vorgangs vergleicht: </p><p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Late","")</code></p></td> 
  </tr> 
  <tr> 
   <td>Größer oder gleich </td> 
   <td>&gt;= </td> 
   <td>Verwenden Sie diesen Operator, um anzugeben, dass die Bedingung erfüllt ist, wenn das erste Feld Ihrer Anweisung größer oder gleich dem zweiten Feld ist. <p>Verwenden Sie z. B. die folgende Anweisung in einem berechneten benutzerdefinierten Feld, um eine IF-Anweisung zu erstellen, die das geplante Abschlussdatum mit dem voraussichtlichen Abschlussdatum eines Vorgangs vergleicht: </p><p><code>IF({projectedCompletionDate}&gt;={plannedCompletionDate},"Late","Early")</code></p></td> 
  </tr> 
  <tr> 
   <td>Kleiner als </td> 
   <td>&lt; </td> 
   <td>Mit diesem Operator können Sie angeben, dass die Bedingung erfüllt ist, wenn  das erste Feld Ihrer Erklärung ist kleiner als das zweite Feld. <p>Verwenden Sie z. B. die folgende Anweisung in einem berechneten benutzerdefinierten Feld, um eine IF-Anweisung zu erstellen, die das geplante Abschlussdatum mit dem voraussichtlichen Abschlussdatum eines Vorgangs vergleicht: </p><p><code>IF({projectedCompletionDate}&lt;{plannedCompletionDate},"Early","")</code></p></td> 
  </tr> 
  <tr> 
   <td>Kleiner als oder gleich </td> 
   <td>&lt;= </td> 
   <td>Mit diesem Operator können Sie angeben, dass die Bedingung erfüllt ist, wenn  das erste Feld Ihrer Anweisung kleiner oder gleich dem zweiten Feld ist. <p>Verwenden Sie z. B. die folgende Anweisung in einem berechneten benutzerdefinierten Feld, um eine IF-Anweisung zu erstellen, die das geplante Abschlussdatum mit dem voraussichtlichen Abschlussdatum eines Vorgangs vergleicht: </p><p><code>IF({projectedCompletionDate}&lt;={plannedCompletionDate},"Early","Late")</code></p></td> 
  </tr> 
  <tr> 
   <td>Trifft nicht zu </td> 
   <td>! </td> 
   <td> <p>Fügen Sie diesen Operator vor einem der oben genannten Operatoren hinzu, um ihn zu negieren. </p> <p>Beispiel: </p> 
    <ul> 
     <li>Ist gleich: = </li> 
     <li>Ist nicht gleich: != </li> 
    </ul> <p>Wenn Sie diesen Operator vor den folgenden Datenausdrücken hinzufügen, wird den Ausdrücken eine negative Anweisung hinzugefügt: </p> 
    <ul> 
     <li>CONTAINS </li> 
     <li>IN </li> 
     <li>IFIN </li> 
     <li>ISBLANK </li> 
    </ul> <p>Informationen zu diesen Datenausdrücken sowie eine vollständige Liste finden Sie unter <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md" class="MCXref xref">Übersicht über berechnete Datenausdrücke</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>ODER </td> 
   <td>|| </td> 
   <td> <p>Verwenden Sie diesen Operator, um anzugeben, dass die Bedingung erfüllt ist, wenn der Ausdruck  findet entweder den ersten oder den zweiten Wert Ihrer Anweisung. </p> <p>Verwenden Sie z. B. die folgende Anweisung in einem berechneten benutzerdefinierten Feld, um eine IF-Anweisung zu erstellen, die Projekte mit dem Status "Aktuell" oder "Planung" als "Aktiv" markiert: </p><p><code>IF({status}="PLN"||{status}="CUR","Active","Not Active")</code></p> </td> 
  </tr> 
  <tr> 
   <td> und </td> 
   <td>&amp;&amp; </td> 
   <td> <p>Verwenden Sie diesen Operator, um anzugeben, dass die Bedingung erfüllt ist, wenn der Ausdruck  findet ein Element, das zwei Bedingungen gleichzeitig erfüllt. </p> <p>Verwenden Sie z. B. die folgende Anweisung in einem berechneten benutzerdefinierten Feld, um eine "IF"-Anweisung zu erstellen, die Projekte mit dem Status Aktuell und der Bedingung Risiko findet und sie als "Vermittlung erforderlich" markiert. </p><p><code>IF({status}="CUR"&&{condition}="AR","Mediation Needed","")</code></p> </td> 
  </tr> 
 </tbody> 
</table>
