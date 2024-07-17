---
product-previous: workfront-goals
navigation-topic: goal-management
title: Übersicht über den Zielfortschritt und die Bedingungen in den Adobe Workfront-Zielen
description: Der Zielfortschritt wird von Fortschrittsindikatoren wie Aktivitäten, Ergebnissen oder Kinderzielen bestimmt. Die Zielbedingung wird durch den Fortschritt des Ziels zum aktuellen Zeitpunkt bestimmt.
author: Alina
feature: Workfront Goals
exl-id: 3050f7ff-a579-4fb8-82fd-bef850f27c20
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 1%

---

# Übersicht über den Zielfortschritt und die Bedingungen in den Adobe Workfront-Zielen

Ihr Unternehmen muss über Folgendes verfügen, um die in diesem Artikel beschriebene Funktion verwenden zu können:

* Für den neuen Plan und die Lizenzstruktur:

   * Ein ultimativer Plan

     Oder

     Eine zusätzliche Lizenz für Adobe Workfront Goals für die Prime- oder Select Adobe Workfront-Pläne. Weitere Informationen finden Sie unter [Adobe Workfront-Plan](https://www.workfront.com/plans).

* Für den aktuellen Plan und die Lizenzstruktur:

   * A Pro oder höher
   * Eine Adobe Workfront Goals-Lizenz zusätzlich zu einer Workfront-Lizenz.

Wenden Sie sich an Ihren Workfront-Kundenbetreuer, um mehr über eine Workfront Goals-Lizenz zu erfahren.

Weitere Informationen zum Zugriff auf Workfront-Ziele finden Sie unter [Voraussetzungen für die Verwendung von Workfront-Zielen](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

Adobe Workfront berechnet den Zielfortschritt anhand der Fortschrittsanzeigen automatisch.

## Voraussetzungen

Sie müssen über Folgendes verfügen, bevor Sie beginnen können:

* Eine Layout-Vorlage, die den Bereich Ziele im Hauptmenü enthält.

## Übersicht über den Zielfortschritt und die Schwelle

Nachdem Sie ein Ziel aktiviert haben, beginnt Workfront Goals mit der Berechnung des Fortschritts und der Bedingung und zeigt die folgenden Indikatoren an, wenn Sie den Mauszeiger über das Feld Fortschritt bewegen:

| Indikator | Indikatorbeschreibung |
|---|---|
| Tatsächliche prozentuale Fertigstellung | Wie viel von dem Ziel tatsächlich bis jetzt erreicht wurde. Workfront Goals berechnet diesen Wert, indem es im Durchschnitt den vollständigen Prozentsatz aller mit dem Ziel verbundenen Fortschrittsindikatoren berechnet. |
| Erwartetes Prozent abgeschlossen | Wie viel des Ziels sollte bis jetzt erreicht sein, damit das Ziel rechtzeitig erreicht werden kann. Workfront Goals berechnet diesen Wert anhand der Zieldauer und des aktuellen Zeitpunkts. Das Ziel sollte diesen Wert zum aktuellen Zeitpunkt anzeigen, wenn er rechtzeitig abgeschlossen werden sollte. |
| Fortschritt | Eine Beschriftung, die anzeigt, ob das Ziel auf Zielgruppe gesetzt ist, um rechtzeitig abgeschlossen zu werden, oder ob das Ziel gefährdet ist oder nicht abgeschlossen werden kann. |

![](assets/in-trouble-goal-progress-expanded.png)

<!--drafted for the redesign: replace the screen shot above with the redesigned one which is white, not black-->

* [Tatsächliche prozentuale Fertigstellung](#actual-percent-complete)
* [Erwarteter prozentualer Abschluss](#expected-percent-complete)
* [Fortschritt und Bedingung](#progress)

### Tatsächliche prozentuale Fertigstellung {#actual-percent-complete}

Workfront-Ziele berechnen automatisch den tatsächlichen prozentualen Abschluss eines Ziels basierend auf dem vollständigen Prozentwert der Zielfortschrittsindikatoren.

Die folgenden Punkte werden als Fortschrittsindikatoren für Ziele betrachtet:

* Ergebnisse

  Informationen zum Hinzufügen von Ergebnissen zu Zielen finden Sie unter [Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/add-results-to-goals.md).

* Aktivitäten

  Informationen zum Hinzufügen von Aktivitäten, einschließlich Projekten, zu Zielen finden Sie unter [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

* Angepasste Kinderziele

  Weitere Informationen zu übergeordneten und untergeordneten Zielen finden Sie unter [Ziele durch Verbinden in Adobe Workfront-Zielen ausrichten](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

  Workfront Goals berechnet den tatsächlichen prozentualen Abschluss anhand der folgenden Formel:

  ```
  Actual percent complete of goal = SUM(Percent complete of goal progress indicators)* 100 / Number of progress indicators
  ```

  Wenn beispielsweise ein Ziel ein &quot;Ergebnis, das 20 % abgeschlossen ist&quot;, eine manuelle Fortschrittsleiste, die zu 30 % abgeschlossen ist, ein Projekt, das zu 10 % abgeschlossen ist, und ein untergeordnetes Ziel, das zu 40 % abgeschlossen ist, beträgt der Zielprozentsatz &quot;complete&quot;25 %.

### Erwartetes Prozent abgeschlossen {#expected-percent-complete}

Workfront Goals berechnet automatisch den erwarteten Prozentsatz der Vollendung eines Ziels basierend auf der Gesamtanzahl der Tage während der Zieldauer sowie der Anzahl der Tage, die seit dem Zielstartdatum vergangen sind.

Workfront Goals berechnet den erwarteten Prozentsatz der Fertigstellung anhand der folgenden Formel:

```
Expected percent complete of goal = Number of days since the goal start date * 100/ Number of days in the goal duration
```

Wenn ein Ziel beispielsweise in 90 Tagen abgeschlossen sein soll und heute der 45. Tag dieser Dauer ist, beträgt der erwartete Prozentsatz der Vollendung 50 %.

### Fortschritt und Bedingung {#progress}

Workfront Goals berechnet einen Prozentsatz an Fortschritten und weist Zielen einen Fortschrittstitel zu, basierend darauf, welcher Prozentsatz des erwarteten Abschlusses zum aktuellen Zeitpunkt erreicht wurde. Die Farbe der Vollbildleiste des Ziels in Prozent ändert sich, um den Fortschritt des Ziels anzuzeigen.

Die Bedingung des Ziels wird ebenfalls entsprechend aktualisiert, um anzugeben, ob das Ziel rechtzeitig erreicht werden soll oder nicht.

Workfront Goals berechnet den Prozentsatz des Fortschritts eines Ziels anhand der folgenden Formel:

```
Goal progress percentage = Actual percent complete * 100 / Expected percent complete
```

Wenn beispielsweise der erwartete prozentuale Abschluss zur aktuellen Zeit 53 % beträgt und der tatsächliche Prozentsatz der Fertigstellung 30 % beträgt, beträgt der Prozentsatz des Zielfortschritts 56 %. Workfront will dieses Ziel mit der Bedingung &quot;In Schwierigkeiten&quot;kennzeichnen.

Die folgende Tabelle zeigt die Beziehung zwischen den Bedingungsbeschriftungen und dem Fortschrittsprozentsatz:

![](assets/progress-status-labels-charted-after-match-with-project-condition-350x147.png)

In der folgenden Tabelle sind die Zielbedingungsbeschriftungen und die mit den einzelnen Bezeichnungen verknüpften Zielfortschrittsprozentsätze aufgeführt.

>[!TIP]
>
>Die Beschriftungen für Zielbedingungen stimmen mit dem Namen und der Farbe der Workfront-Projektbedingung überein.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Name des Zielfortschritts</b></td> 
   <td><b>Definition des Zielfortschritts</b></td> 
   <td><b>Prozentsatz des Zielfortschritts</b></td> 
   <td><b>Farbe des vollständigen Balkens in Prozent</b></td> 
   <td><b>Symbol für Bedingungsanzeige</b></td> 
  </tr> 
  <tr> 
   <td>Neu</td> 
   <td> <p>Das Ziel wurde neu erstellt und zeichnet noch keinen Fortschritt auf. Ein Zielfortschritt wird als Neu angezeigt, bis ein Benutzer seinen Fortschritt zum ersten Mal aktualisiert. </p> <p>Informationen zum Aktualisieren des Zielfortschritts finden Sie unter <a href="../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md" class="MCXref xref">Aktualisieren des Zielfortschritts in Adobe Workfront-Zielen</a>.</p> </td> 
   <td>Kein Prozentsatz</td> 
   <td>Keine Leiste</td> 
   <td><img src="assets/new-goal-icon-condition.png" alt="new_target_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>Auf Ziel</span> </p> </td> 
   <td>Das Ziel erreicht die Erwartungen und es besteht eine große Wahrscheinlichkeit, dass es rechtzeitig abgeschlossen wird. </td> 
   <td>90-100 %</td> 
   <td>Grün</td> 
    <td><img src="assets/on-target-icon-condition.png" alt="on_target_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>Risiko</span> </p> </td> 
   <td>Das Ziel hinkt hinterher, aber es kann noch möglich sein, es rechtzeitig abzuschließen. </td> 
   <td>70-89,99%</td> 
   <td>Gelb</td>
   <td><img src="assets/at-risk-icon-condition.png" alt="at_risk_icon_condition.png"></td> 
  </tr> 
  <tr> 
   <td> <p><span>In Trouble</span> </p> </td> 
   <td> <p>Es ist sehr wahrscheinlich, dass das Ziel nicht rechtzeitig abgeschlossen wird. </p> </td> 
   <td>0-69,99%</td> 
   <td>Rot</td> 
   <td><img src="assets/in-trouble-icon-condition.png" alt="in_issues_icon_condition.png"></td> 
  </tr> 
 </tbody> 
</table>