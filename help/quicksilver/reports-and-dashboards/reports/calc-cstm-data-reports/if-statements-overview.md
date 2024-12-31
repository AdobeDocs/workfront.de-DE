---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: IF-Anweisungen - Übersicht
description: Sie können „IF“-Anweisungen in allgemeinen Programmiersprachen verwenden. In Adobe Workfront können Sie mit „IF“-Anweisungen Datenfelder sowohl für Reporting- als auch für benutzerdefinierte Datenzwecke vergleichen, formatieren und zeichenfolgen. Mathematisch über „IF“-Aussagen nachzudenken führt außerdem zu einem besseren konzeptionellen Verständnis, da häufig Variablen für Ausdrücke verwendet werden.
author: Nolan
feature: Reports and Dashboards
exl-id: 090a85fd-fdbe-4507-8bad-ce8c29bf8fc9
source-git-commit: 23b5ba9564b514e11c1ca9d5cca276238ef11066
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# „IF“-Anweisungen - Übersicht

<!-- Audited: 1/2024 -->

Sie können „IF“-Anweisungen in allgemeinen Programmiersprachen verwenden. In Adobe Workfront können Sie mit „IF“-Anweisungen Datenfelder sowohl für Reporting- als auch für benutzerdefinierte Datenzwecke vergleichen, formatieren und zeichenfolgen. Mathematisch über „IF“-Aussagen nachzudenken führt außerdem zu einem besseren konzeptionellen Verständnis, da häufig Variablen für Ausdrücke verwendet werden.

## Recommendations für „IF“-Anweisungen

Beachten Sie Folgendes, bevor Sie eine „IF“-Anweisung erstellen:

* Wir empfehlen ein grundlegendes Verständnis einer allgemeinen Programmiersprache, aber wir benötigen es nicht, für dieses Handbuch.
* Wir benötigen ein fortgeschrittenes Verständnis der Workfront-Textmodussyntax. Dies hilft beim Verständnis der Terminologie der Workfront-API und beim Verständnis der Syntax von benutzerdefinierten Daten in diesen spezifischen Formaten.

  Weitere Informationen zur Workfront-API finden Sie unter [API-Grundlagen](../../../wf-api/general/api-basics.md).

  Weitere Informationen zur Verwendung des Textmodus finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

* Sie können „IF“-Anweisungen für die folgenden Workfront-Elemente erstellen:

   * Ansichten
   * Gruppierungen
   * Berechnete benutzerdefinierte Felder

* Für Filter können keine „IF“-Anweisungen erstellt werden. Dies führt zu einem Hoppla-Fehler in Workfront.
* Das Support-Team hilft nicht beim Erstellen benutzerdefinierter Daten. Sie können sich an das Support-Team wenden, nachdem Sie die benutzerdefinierten Felder oder Spalten erstellt haben und die gewünschten Ergebnisse nicht angezeigt werden. Wenn Sie Hilfe bei der Erstellung eines Ausdrucks benötigen, wenden Sie sich an Ihren Kundenbetreuer, um sich über unsere Beratungsoptionen zu informieren.
* Es wird empfohlen, diese Ausdrücke zunächst in einem Texteditor zu schreiben, z. B. in Sublime oder Visual Studio Code, da so die Daten klarer angezeigt werden können, als dies in Workfront der Fall wäre.

## Komponenten einer „IF“-Anweisung

Sie können „IF“-Anweisungen in Workfront in folgendem Format erstellen:
<pre>IF(Bedingung,True-Ausdruck,False-Ausdruck)</pre>Eine „IF“-Anweisung umfasst folgende Komponenten:

* **IF** = Dies ist der von Workfront berechnete Datenausdruck für „function“. Ähnlich wie bei den SUM- und PROD-Ausdrücken wird dem System zunächst mitgeteilt, dass es die Funktion als „IF“-Anweisung verstehen soll. Verwenden Sie in dieser Anweisung immer Großbuchstaben für „IF“.\
  Eine Liste aller berechneten Datenausdrücke finden Sie unter [Übersicht über berechnete Datenausdrücke](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

* **Bedingung** = Dies ist die Bedingung, die die Workfront-Variable erfüllen muss, und sie ist die Grundlage für diese Gleichung. Alles, was später in der Gleichung angegeben werden kann, hängt von der Bedingung ab. Sie können mehrere Verweise, Vergleiche oder mathematische Ausdrücke verwenden, um eine Gleichung zu starten. Beispiele für Bedingungen:

   * Ein Datum ist größer als ein anderes Datum für ein angegebenes Objekt.
   * Ein Status entspricht einem der verfügbaren Status für ein angegebenes Objekt.
   * Prozent abgeschlossen einer Aufgabe ist kleiner oder größer als ein bestimmter Prozentsatz.

* **Bedingungsoperator** = Dies ist der Operator, der Ihnen beim Erstellen der Bedingung Ihrer „IF“-Anweisung hilft. Beispielsweise sind „ist gleich“ oder „ist größer als“ Bedingungsoperatoren. Eine Liste der Bedingungsoperatoren, die Sie in Anweisungen verwenden können, finden Sie unter [Bedingungsoperatoren in berechneten benutzerdefinierten Ausdrücken](../../../reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

* **True****Expression** = Dies ist die Variable „True“, die der Gleichung mitteilt, welcher Indikator angezeigt werden soll, wenn die Kriterien der Bedingung erfüllt sind (wahre Indikatoren).

* **Falscher Ausdruck** = Dies ist die Variable „Falsch“, die der Gleichung mitteilt, welcher Indikator angezeigt werden soll, wenn die Kriterien der Bedingung nicht erfüllt sind (falsche Indikatoren).

Im folgenden Beispiel wird das ursprüngliche Anweisungsformat verwendet, um einen einfachen Datenausdruck für eine „IF“-Anweisung zu schreiben. Der Ausdruck vergleicht zwei verschiedene Datumsfelder in Workfront, gefolgt von einem Ergebnis „true/false“ als Datenzeichenfolge:

```
IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

Im Alltag würde diese Aussage bedeuten: Wenn das voraussichtliche Abschlussdatum meines Objekts „größer als“ das geplante Abschlussdatum meines gleichen Objekts ist, dann sollten Sie in diesem Feld die Wörter „Aus dem Weg“ anzeigen. Ist dies nicht der Fall, werden die Wörter „On Track“ angezeigt.

## Erstellen von berechneten Feldern in benutzerdefinierten Formularen oder benutzerdefinierten Spalten mithilfe von „IF“-Anweisungen

Sie können „IF“-Anweisungen in einem berechneten Feld entweder in einem benutzerdefinierten Formular oder in einer benutzerdefinierten Spalte erstellen.

Die Syntax, die Sie in einem berechneten benutzerdefinierten Formular verwenden, unterscheidet sich von der berechneten benutzerdefinierten Spalte. Siehe die folgenden Beispiele:

* [Einzelne „IF“-Anweisungen](#single-if-statements)
* [Mehrere „IF“-Anweisungen](#multiple-if-statements)

### Einzelne „IF“-Anweisungen {#single-if-statements}

Im Folgenden finden Sie Beispiele für ein berechnetes benutzerdefiniertes Feld und die entsprechende Spalte mit einer „IF“-Anweisung:

* Berechnetes benutzerdefiniertes Feld:

Verwenden Sie beim Erstellen eines benutzerdefinierten Felds die folgende Syntax für eine „IF“-Anweisung:

```
IF({Projected Completion Date}>{Planned Completion Date},"Off Track","On Track")
```

* Berechnete benutzerdefinierte Spalte:

Beim Erstellen einer benutzerdefinierten Spalte sollten Sie die folgende Syntax für die „IF“-Anweisung in der Ausdruckszeile für den Wert verwenden:

```
valueexpression=IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

### Mehrere „IF“-Anweisungen {#multiple-if-statements}

Sie können mehrere „IF“-Anweisungen mit der folgenden Anweisung zusammenstellen, um einen komplexeren und dynamischeren Ausdruck zu erstellen:

<pre>IF(Bedingung1,Ausdruck wahr,IF(Bedingung2,Ausdruck wahr,Ausdruck falsch))</pre>Beachten Sie, dass es jetzt keine Falschaussage für das erste „IF“ gibt. Stattdessen haben wir es durch den Beginn eines zweiten „IF“ ersetzt.

Im Folgenden finden Sie Beispiele für ein berechnetes benutzerdefiniertes Feld und die entsprechende benutzerdefinierte Spalte mit mehreren „IF“-Anweisungen:

* Berechnetes benutzerdefiniertes Feld:

  ```
  IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
  ```

* Berechnete benutzerdefinierte Spalte:

```
valueexpression=IF({"projectedCompletionDate"}>{"plannedCompletionDate"},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
```

In diesem Beispiel wurde dasselbe erreicht, indem zwei verschiedene Kriterienvariablen zusammengestellt wurden.\
Sie können diese Optionen weiter untersuchen, indem Sie diese Beispiele in Ihrer eigenen Umgebung neu erstellen.

Am einfachsten erfahren Sie dies, indem Sie mit verschiedenen Feldern und Szenarien experimentieren. Machen Sie sich auch mit dem API Explorer vertraut, der die Feldnamen anzeigt, die verwendet werden können. Informationen zum API-Explorer finden Sie unter [API-Explorer](../../../wf-api/general/api-explorer.md).

Weitere Informationen zur Workfront-Syntax für berechnete Datenausdrücke finden Sie unter [Übersicht über berechnete Datenausdrücke](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
