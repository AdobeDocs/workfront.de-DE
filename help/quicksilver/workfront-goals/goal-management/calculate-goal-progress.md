---
product-previous: workfront-goals
navigation-topic: goal-management
title: Übersicht über den Zielfortschritt und die Bedingung in Adobe Workfront Goals
description: Der Zielfortschritt wird von Fortschrittsindikatoren wie Aktivitäten, Ergebnissen oder untergeordneten Zielen gesteuert. Die Zielbedingung wird durch den Fortschritt des Ziels zum aktuellen Zeitpunkt bestimmt.
author: Alina
feature: Workfront Goals
exl-id: 3050f7ff-a579-4fb8-82fd-bef850f27c20
source-git-commit: 7c1bd52c6d1878b556bc92849b5d65fd0e89f51b
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 1%

---

# Übersicht über den Zielfortschritt und die Bedingung in Adobe Workfront Goals

Ihr Unternehmen muss über Folgendes verfügen, um die in diesem Artikel beschriebenen Funktionen nutzen zu können:

* Für die neue Plan- und Lizenzstruktur:

   * Ein Ultimate-Plan

     Oder

     Eine zusätzliche Lizenz für Adobe Workfront-Ziele für Prime- oder Select Adobe Workfront-Pläne.

* Für die aktuelle Plan- und Lizenzstruktur:

   * Ein Profi oder höher
   * Eine Adobe Workfront-Ziellizenz zusätzlich zu einer Workfront-Lizenz.

Wenden Sie sich an Ihren Workfront Account Manager, um mehr über eine Workfront Goals-Lizenz zu erfahren.

Weitere Informationen zum Zugriff auf Workfront-Ziele finden Sie unter [Voraussetzungen für die Verwendung von Workfront-Zielen](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

Adobe Workfront berechnet den Zielfortschritt automatisch auf der Grundlage der Fortschrittsanzeigen.

## Übersicht über den Zielfortschritt und Schwellenwert

Nachdem Sie ein Ziel aktiviert haben, beginnt Workfront Goals mit der Berechnung des Fortschritts und der Bedingung und zeigt die folgenden Indikatoren an, wenn Sie den Mauszeiger über das Feld Fortschritt bewegen:

| Indikator | Indikatorbeschreibung |
|---|---|
| Tatsächlicher Prozentsatz abgeschlossen | Wie viel von dem Ziel tatsächlich bis jetzt erreicht wurde. Workfront Goals berechnet diesen Wert durch Mittelung des Prozentsatzes der Fertigstellung aller Fortschrittsindikatoren, die mit dem Ziel verknüpft sind. |
| Erwarteter Prozentsatz der Fertigstellung | Welcher Anteil des Ziels sollte bis jetzt abgeschlossen sein, damit das Ziel termingerecht abgeschlossen werden kann. Workfront Goals berechnet diesen Wert anhand der Zieldauer und des aktuellen Zeitpunkts. Das Ziel sollte diesen Wert zur aktuellen Zeit anzeigen, wenn er termingerecht abgeschlossen werden soll. |
| Fortschritt | Eine Kennzeichnung, die angibt, ob das Ziel pünktlich erreicht werden soll oder ob das Risiko besteht oder die Aufgabe nicht abgeschlossen werden kann. |

![](assets/in-trouble-goal-progress-expanded.png)

<!--drafted for the redesign: replace the screen shot above with the redesigned one which is white, not black-->

* [Tatsächlicher Prozentsatz abgeschlossen](#actual-percent-complete)
* [Erwarteter Prozentsatz abgeschlossen](#expected-percent-complete)
* [Fortschritt und Zustand](#progress)

### Tatsächlicher Prozentsatz abgeschlossen {#actual-percent-complete}

Workfront-Ziele berechnet automatisch den tatsächlichen Prozentsatz der Fertigstellung eines Ziels auf der Grundlage des Prozentsatzes der Fertigstellung der Zielfortschrittsindikatoren.

Die folgenden Punkte gelten als Fortschrittsindikatoren für Ziele:

* Ergebnisse

  Informationen zum Hinzufügen von Ergebnissen zu Zielen finden Sie unter [Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).

* Aktivitäten

  Informationen zum Hinzufügen von Aktivitäten, einschließlich Projekten, zu Zielen finden Sie unter [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

* Abgestimmte untergeordnete Ziele

  Informationen zu übergeordneten und untergeordneten Zielen finden Sie unter [Ausrichten von Zielen durch Verbinden in Adobe Workfront-Zielen](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

  Workfront Goals berechnet den tatsächlichen Prozentsatz der Fertigstellung anhand der folgenden Formel:

  ```
  Actual percent complete of goal = SUM(Percent complete of goal progress indicators)* 100 / Number of progress indicators
  ```

  Wenn beispielsweise ein Ziel ein Ergebnis hat, das zu 20 % abgeschlossen ist, eine manuelle Fortschrittsleiste, die zu 30 % abgeschlossen ist, ein Projekt, das zu 10 % abgeschlossen ist, und ein untergeordnetes Ziel, das zu 40 % abgeschlossen ist, lautet das Ziel zu 25 % abgeschlossen.

### Erwarteter Prozentsatz der Fertigstellung {#expected-percent-complete}

Workfront Goals berechnet automatisch den erwarteten Prozentsatz der Fertigstellung eines Ziels auf der Grundlage der Gesamtzahl der Tage während der Zieldauer sowie der Anzahl der Tage, die seit dem Startdatum des Ziels vergangen sind.

Workfront Goals berechnet den erwarteten Prozentsatz der Fertigstellung anhand der folgenden Formel:

```
Expected percent complete of goal = Number of days since the goal start date * 100/ Number of days in the goal duration
```

Wenn beispielsweise ein Ziel in 90 Tagen abgeschlossen werden soll und heute der 45. Tag dieser Dauer ist, beträgt der erwartete Prozentsatz der Fertigstellung 50 %.

### Fortschritt und Zustand {#progress}

Workfront-Ziele : Berechnet einen Fortschrittsprozentsatz und weist den Zielen eine Fortschrittsbezeichnung zu, basierend darauf, welcher Prozentsatz des erwarteten Prozentsatzes der Fertigstellung zum aktuellen Zeitpunkt erreicht wurde. Die Farbe des Balkens Ziel Prozent abgeschlossen ändert sich, um den Fortschritt des Ziels anzuzeigen.

Die Zielbedingung wird entsprechend aktualisiert, um anzugeben, ob das Ziel im Zeitplan und fristgerecht abgeschlossen ist oder ob es im Rückstand ist.

Workfront-Ziele : Berechnet den Fortschrittsprozentsatz eines Ziels anhand der folgenden Formel:

```
Goal progress percentage = Actual percent complete * 100 / Expected percent complete
```

Beispiel: Wenn der erwartete Prozentsatz der Fertigstellung zum aktuellen Zeitpunkt 53 % und der tatsächliche Prozentsatz der Fertigstellung 30 % beträgt, beträgt der Zielfortschritt in Prozent der Fertigstellung 56 %. Workfront Goals kennzeichnet dieses Ziel mit der Bedingung „In Schwierigkeiten“.

Die folgende Grafik zeigt die Beziehung zwischen den Bedingungsbeschriftungen und dem Fortschrittsprozentsatz:

![](assets/progress-status-labels-charted-after-match-with-project-condition-350x147.png)

In der folgenden Tabelle sind die Beschriftungen der Zielbedingungen und die mit den einzelnen Beschriftungen verknüpften Prozentsätze des Zielfortschritts aufgeführt.

>[!TIP]
>
>Die Beschriftungen der Zielbedingung entsprechen dem Namen und der Farbe der Workfront-Projektbedingung.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Name des Zielstatus</b></td> 
   <td><b>Definition des Zielfortschritts</b></td> 
   <td><b>Zielfortschritt in Prozent</b></td> 
   <td><b>Farbe des Balkens für prozentuale Vollständigkeit</b></td> 
   <td><b>Symbol für Bedingungsindikator</b></td> 
  </tr> 
  <tr> 
   <td>Neu</td> 
   <td> <p>Das Ziel wurde neu erstellt und erfasst noch keinen Fortschritt. Ein Zielfortschritt wird als Neu angezeigt, bis jemand seinen Fortschritt zum ersten Mal aktualisiert. </p> <p>Informationen zum Aktualisieren des Zielfortschritts finden Sie unter <a href="../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md" class="MCXref xref">Aktualisieren des Zielfortschritts in Adobe Workfront Goals</a>.</p> </td> 
   <td>Kein Prozentsatz</td> 
   <td>Keine Leiste</td> 
   <td><img src="assets/new-goal-icon-condition.png" alt="new_goal_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>Im Zielbereich</span> </p> </td> 
   <td>Das Ziel funktioniert wie erwartet und die Wahrscheinlichkeit ist hoch, dass es pünktlich abgeschlossen wird. </td> 
   <td>90-100 %</td> 
   <td>Grün</td> 
    <td><img src="assets/on-target-icon-condition.png" alt="on_target_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>Gefährdet</span> </p> </td> 
   <td>Das Ziel hinkt hinterher, aber es könnte noch möglich sein, es rechtzeitig abzuschließen. </td> 
   <td>70-89,99 %</td> 
   <td>Gelb</td>
   <td><img src="assets/at-risk-icon-condition.png" alt="at_risk_icon_condition.png"></td> 
  </tr> 
  <tr> 
   <td> <p><span>In Schwierigkeiten</span> </p> </td> 
   <td> <p>Es ist sehr wahrscheinlich, dass das Ziel nicht rechtzeitig erreicht wird. </p> </td> 
   <td>0-69,99 %</td> 
   <td>Rot</td> 
   <td><img src="assets/in-trouble-icon-condition.png" alt="in_Trouble_icon_condition.png"></td> 
  </tr> 
 </tbody> 
</table>