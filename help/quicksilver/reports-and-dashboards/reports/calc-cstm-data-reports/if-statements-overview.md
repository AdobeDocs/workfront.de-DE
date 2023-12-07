---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Übersicht über IF-Anweisungen
description: Sie können "IF"-Anweisungen in allgemeinen Programmiersprachen verwenden. In Adobe Workfront ermöglichen Ihnen "IF"-Anweisungen den Vergleich, die Formatierung und die Zeichenfolge von Datenfeldern für Berichterstellungs- und benutzerdefinierte Datenzwecke. Außerdem führt das mathematische Denken über "IF"-Anweisungen zu einem besseren konzeptionellen Verständnis, da Variablen für Ausdrücke häufig verwendet werden.
author: Nolan
feature: Reports and Dashboards
exl-id: 090a85fd-fdbe-4507-8bad-ce8c29bf8fc9
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# Übersicht über &quot;IF&quot;-Anweisungen

Sie können &quot;IF&quot;-Anweisungen in allgemeinen Programmiersprachen verwenden. In Adobe Workfront ermöglichen Ihnen &quot;IF&quot;-Anweisungen den Vergleich, die Formatierung und die Zeichenfolge von Datenfeldern für Berichterstellungs- und benutzerdefinierte Datenzwecke. Außerdem führt das mathematische Denken über &quot;IF&quot;-Anweisungen zu einem besseren konzeptionellen Verständnis, da Variablen für Ausdrücke häufig verwendet werden.

## Recommendations für &quot;IF&quot;-Anweisungen

Beachten Sie Folgendes, bevor Sie eine &quot;IF&quot;-Anweisung erstellen:

* Wir empfehlen ein grundlegendes Verständnis jeder allgemeinen Programmiersprache, aber wir benötigen sie nicht für diesen Leitfaden.
* Wir benötigen ein erweitertes Verständnis der Syntax des Workfront-Textmodus. Dies hilft beim Verständnis der Terminologie der Workfront-API und beim Verständnis der Syntax benutzerdefinierter Daten in diesen spezifischen Formaten.

  Informationen zur Workfront-API finden Sie unter [API-Grundlagen](../../../wf-api/general/api-basics.md).

  Informationen zur Verwendung des Textmodus finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

* Sie können &quot;IF&quot;-Anweisungen für die folgenden Workfront-Elemente erstellen:

   * Ansichten
   * Gruppierungen
   * Berechnete benutzerdefinierte Felder

* Sie können keine &quot;IF&quot;-Anweisungen für Filter erstellen. Dies führt zu einem &quot;UUPS&quot;-Fehler in Workfront.
* Das Supportteam hilft nicht beim Erstellen benutzerdefinierter Daten. Sie können sich nach dem Erstellen der benutzerdefinierten Felder oder Spalten an das Supportteam wenden, ohne dass die gewünschten Ergebnisse angezeigt werden. Wenden Sie sich für die Erstellung eines Ausdrucks an Ihren Kundenbetreuer, um sich über unsere Beratungsoptionen zu informieren.
* Es wird empfohlen, diese Ausdrücke zuerst in einen Texteditor wie Sublime oder Visual Studio Code zu schreiben, da dies Ihnen dabei hilft, Daten deutlicher anzuzeigen, als es in Workfront der Fall wäre.

## Komponenten einer &quot;IF&quot;-Anweisung

Sie können &quot;IF&quot;-Anweisungen in Workfront im folgenden Format erstellen:
<pre>IF(Bedingung, True Expression, False Expression)</pre>Die Komponenten einer "IF"-Anweisung sind:

* **IF**= Dies ist der berechnete Workfront-Datenausdruck für &quot;function&quot;. Ähnlich wie die SUM- und PROD-Ausdrücke weist dieses zuerst das System an, die Funktion als &quot;IF&quot;-Anweisung zu verstehen. Verwenden Sie für &quot;IF&quot;immer Großbuchstaben in dieser Anweisung.\
  Eine Liste aller berechneten Datenausdrücke finden Sie unter [Übersicht über berechnete Datenausdrücke](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

* **Bedingung**= Dies ist die Bedingung, die die Workfront-Variable erfüllen muss, und die Grundlage für diese Gleichung. Alles, was später in der Gleichung angegeben werden kann, hängt von der Bedingung ab. Sie können eine Reihe von Verweisen, Vergleichen oder mathematischen Ausdrücken verwenden, um eine Gleichung zu beginnen. Beispiele für Bedingungen:

   * Ein Datum ist größer als ein anderes Datum für ein bestimmtes Objekt.
   * Der Status entspricht einem der verfügbaren Status für ein bestimmtes Objekt.
   * Der prozentuale Abschluss einer Aufgabe ist kleiner oder größer als ein bestimmter Prozentsatz.

* **Bedingungsoperator** = dies ist der Operator, der Ihnen beim Erstellen der Bedingung Ihrer &quot;IF&quot;-Anweisung hilft. Beispielsweise sind Bedingungsoperatoren &quot;ist gleich&quot;oder &quot;ist größer als&quot;. Eine Liste der Bedingungsoperatoren, die Sie in -Anweisungen verwenden können, finden Sie unter [Bedingungsoperatoren in berechneten benutzerdefinierten Ausdrücken](../../../reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

* **True***Ausdruck**= Dies ist die Variable &quot;True&quot;, die die Gleichung angibt, welcher Indikator angezeigt werden soll, sobald die Kriterien der Bedingung erfüllt sind (wahre Indikatoren).

* **Falscher Ausdruck**= Dies ist die Variable &quot;False&quot;, die der Gleichung mitteilt, welcher Indikator angezeigt werden soll, wenn die Kriterien der Bedingung nicht erfüllt sind (falsche Indikatoren).

Im folgenden Beispiel wird das ursprüngliche Anweisungsformat verwendet, um einen einfachen Datenausdruck für eine &quot;IF&quot;-Anweisung zu schreiben. Der Ausdruck vergleicht zwei verschiedene Datumsfelder in Workfront , gefolgt von einem True-/False-Ergebnis als Datenzeichenfolge:

```
IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

In Alltagsreden würde diese Aussage bedeuten: Wenn das voraussichtliche Abschlussdatum meines Objekts &quot;größer als&quot;ist, das geplante Abschlussdatum meines gleichen Objekts, dann zeigen Sie in diesem Feld die Wörter &quot;Off Track&quot;an. Wenn nicht, zeigen Sie die Wörter &quot;Auf Track&quot;an.

## Erstellen Sie berechnete Felder in benutzerdefinierten Formularen oder benutzerdefinierten Spalten mithilfe von &quot;IF&quot;-Anweisungen.

Sie können &quot;IF&quot;-Anweisungen in einem berechneten Feld entweder in einem benutzerdefinierten Formular oder in einer benutzerdefinierten Spalte erstellen.

Es gibt einen Unterschied in der Syntax, die Sie in einem berechneten benutzerdefinierten Formular verwenden, im Vergleich zu einer berechneten benutzerdefinierten Spalte. Siehe folgende Beispiele:

* [Einzelne &quot;IF&quot;-Anweisungen](#single-if-statements)
* [Mehrere &quot;IF&quot;-Anweisungen](#multiple-if-statements)

### Einzelne &quot;IF&quot;-Anweisungen {#single-if-statements}

Im Folgenden finden Sie Beispiele für ein berechnetes benutzerdefiniertes Feld und dessen entsprechende Spalte mit der Anweisung &quot;IF&quot;:

* Berechnetes benutzerdefiniertes Feld:

Verwenden Sie beim Erstellen eines benutzerdefinierten Felds die folgende Syntax für eine &quot;IF&quot;-Anweisung:

```
IF({Projected Completion Date}>{Planned Completion Date},"Off Track","On Track")
```

* Berechnete benutzerdefinierte Spalte:

Beim Erstellen einer benutzerdefinierten Spalte sollten Sie die folgende Syntax für die &quot;IF&quot;-Anweisung in der Wertausdruckszeile verwenden:

```
valueexpression=IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

### Mehrere &quot;IF&quot;-Anweisungen {#multiple-if-statements}

Sie können mehrere &quot;IF&quot;-Anweisungen mit der folgenden Anweisung zusammenstellen, um einen komplexeren und dynamischeren Ausdruck zu erstellen:

<pre>IF(Condition1, True Expression, IF(Condition2, True Expression, False Expression))</pre>Beachten Sie, dass es jetzt keine falsche Aussage für das erste "IF"gibt. Stattdessen haben wir ihn durch den Beginn einer zweiten "IF" ersetzt.

Im Folgenden finden Sie Beispiele für ein berechnetes benutzerdefiniertes Feld und die zugehörige benutzerdefinierte Spalte mit mehreren &quot;IF&quot;-Anweisungen:

* Berechnetes benutzerdefiniertes Feld:

  ```
  IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
  ```

* Berechnete benutzerdefinierte Spalte:

```
valueexpression=IF({"projectedCompletionDate"}>{"plannedCompletionDate"},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
```

In diesem Beispiel wurde dasselbe erreicht, indem zwei verschiedene Kriterienvariablen zusammengefügt wurden.\
Sie können diese Optionen weiter untersuchen, indem Sie diese Beispiele in Ihrer eigenen Umgebung neu erstellen.

Die beste Möglichkeit, dies zu erfahren, besteht darin, mit verschiedenen Feldern und Szenarien zu experimentieren. Machen Sie sich auch mit dem API Explorer vertraut, der die zu verwendenden Feldnamen anzeigt. Informationen zum API Explorer finden Sie unter [API-Explorer](../../../wf-api/general/api-explorer.md).

Weitere Informationen zur Workfront-Syntax berechneter Datenausdrücke finden Sie unter [Übersicht über berechnete Datenausdrücke](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
