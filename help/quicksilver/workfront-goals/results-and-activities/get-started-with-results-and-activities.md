---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Erste Schritte mit Ergebnissen und Aktivitäten in Adobe Workfront-Zielen
description: Sie müssen einem Ziel Ergebnisse, Aktivitäten oder aufeinander abgestimmte Ziele hinzufügen, um es aktivieren zu können. Dadurch wird der Zielstatus von "Entwurf"zu "Aktiv"aktualisiert und der Fortschritt beim Ziel wird aufgezeichnet.
author: Alina
feature: Workfront Goals
exl-id: 64fa0aef-cb92-465a-9b74-d863fc232fd1
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '859'
ht-degree: 0%

---

# Erste Schritte mit Ergebnissen und Aktivitäten in Adobe Workfront-Zielen

Ihr Unternehmen muss über Folgendes verfügen, um die in diesem Artikel beschriebene Funktion verwenden zu können:

* Für den neuen Plan und die Lizenzstruktur:

   * Ein ultimativer Plan

     Oder

     Eine zusätzliche Lizenz für Adobe Workfront Goals für die Prime- oder Select Adobe Workfront-Pläne. Weitere Informationen finden Sie unter [Adobe Workfront-Abo](https://www.workfront.com/plans).

* Für den aktuellen Plan und die Lizenzstruktur:

   * A Pro oder höher
   * Eine Adobe Workfront Goals-Lizenz zusätzlich zu einer Workfront-Lizenz.

Wenden Sie sich an Ihren Workfront-Kundenbetreuer, um mehr über eine Workfront Goals-Lizenz zu erfahren.

Wenn Sie ein Ziel erstellen, hat das Ziel den Status Entwurf . Informationen zum Erstellen von Zielen finden Sie unter [Ziele in Adobe Workfront erstellen](../../workfront-goals/goal-management/create-goals.md).

Um den Fortschritt eines Ziels aufzuzeichnen, müssen Sie es aktivieren. Um Ihr Ziel zu aktivieren und seinen Status auf Aktiv zu ändern, müssen Sie ihm zunächst Folgendes hinzufügen:

* Ergebnis
* Eine Aktivität
* Ein Projekt
* Ein ausgerichtetes Ziel

Nachdem mindestens eines dieser Elemente hinzugefügt wurde, können Sie das Ziel aktivieren. Sie müssen die Ergebnisse und Aktivitäten der Ziele aktualisieren, um Fortschritte beim Ziel anzuzeigen.


>[!IMPORTANT]
>
> Ein Ziel darf nicht mehr als 1000 Aktivitäten, Ergebnisse, Projekte oder aufeinander abgestimmte Ziele haben.</span>

Dieser Artikel gibt einen Überblick über Aktivitäten und Ergebnisse. Informationen zum Ausrichten von Zielen finden Sie unter [Zielausrichtung bei Adobe Workfront-Zielen](../../workfront-goals/goal-alignment/goal-alignment.md). Informationen zum Verbinden von Projekten mit Zielen finden Sie unter [Hinzufügen von Projekten zu Zielen in Adobe Workfront-Zielen](../results-and-activities/connect-projects-to-goals-overview.md).

## Ergebnisübersicht

<!--
<p> This will have additional types in the future - add another section for types?)</p>
-->

Die Ergebnisse messen den Fortschritt Ihres Ziels oder dessen Nähe zum Erreichen. Als Zieleigentümer können Sie auch Eigentümer des Ergebnisses sein. Ein Ergebnis für Ihr Ziel kann auch einem anderen Benutzer zugewiesen werden.

Informationen zum Hinzufügen von Ergebnissen zu Zielen finden Sie unter [Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/add-results-to-goals.md).

Sie können Ihren eigenen Zielen oder Zielen Ergebnisse hinzufügen, die zu anderen Entitäten in Ihrer Organisation gehören.

Beachten Sie beim Arbeiten mit Ergebnissen Folgendes:

* Sie beantworten die Frage: &quot;Woher weiß ich, wann mein Ziel abgeschlossen ist?&quot;
* Sie sind Metrikindikatoren. Sie können aus den folgenden Optionen auswählen, um einen Fortschritt für Ihr Ergebnis anzugeben:

  <!--
  this might change (jira, Salesforce, etc))
  -->

   * Währung
   * Zahl
   * Prozentsatz

Weitere Informationen zu Ergebnissen finden Sie in der Liste der Ähnlichkeiten zwischen Ergebnissen und Aktivitäten im Abschnitt [Ähnlichkeiten zwischen Ergebnissen, Aktivitäten und Projekten](#similarities-between-results-activities-and-projects) in diesem Artikel.

## Übersicht über Aktivitäten

<!--
This will have additional types in the future - add another section for types?
-->

Aktivitäten sind wie Ergebnisse spezifisch und messbar und enthalten in der Regel einen Indikator für die Vollständigkeit in Prozent. Als Zieleigentümer können Sie auch Eigentümer der mit dem Ziel verknüpften Aktivitäten sein. Eine Aktivität für Ihr Ziel kann auch einem anderen Benutzer zugewiesen werden.

Informationen zum Hinzufügen von Aktivitäten zu Zielen finden Sie unter [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

Beachten Sie Folgendes, wenn Sie Aktivitäten mit Ihren Zielen verknüpfen:

* Sie beantworten die Frage: &quot;Was werde ich erreichen, wenn das Ziel abgeschlossen ist?&quot;
* Aktivitäten sind benutzerspezifische Einträge, die in Bezug auf Vollständigkeit oder Unvollständigkeit besser betrachtet werden können. Sie müssen manuell aktualisiert werden, um anzugeben, welcher Prozentsatz der Aktivitäten bisher abgeschlossen wurde.

<!--
* You can associate the following activities with goals:

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Manual progress bar </td> 
     <td> <p>Custom entries that can be thought of more in terms of complete or incomplete. They must be manually updated.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><p>Project</p></td> 
     <td> <p>Existing projects that you have at least permissions to View and are not in a status of Dead. They are updated automatically, based on the progress of their work items. </p> <p>The projects must exist before associating them with the goal. You can associate a project with multiple goals. For information about adding projects to goals, see <a href="../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md" class="MCXref xref">Add projects to goals in Adobe Workfront Goals</a>.</p>
     <p><span class="preview">In the Preview environment, projects are separate progress indicators, independent from activities. Adding projects to a goal in the Preview environment is different from adding activities. For more information, see <a href="../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md" class="MCXref xref">Add projects to goals in Adobe Workfront Goals</a>.</span></p>
      </td> 
    </tr> 
   </tbody> 
  </table>
-->
<!--drafted for goal redesign: For THE PRODUCTION RELEASE: remove the projects in this article altogether.-->

Weitere Informationen zu Ergebnissen und Aktivitäten finden Sie in der Liste der Ähnlichkeiten zwischen Ergebnissen und Aktivitäten im Abschnitt [Ähnlichkeiten zwischen Ergebnissen, Aktivitäten und Projekten](#similarities-between-results-activities-and-projects) in diesem Artikel.

## Ähnlichkeiten zwischen Ergebnissen, Aktivitäten und Projekten {#similarities-between-results-activities-and-projects}

Ergebnisse, Aktivitäten und Projekte sind Zielfortschrittsindikatoren.

Es gibt einige Unterschiede in der Art und Weise, wie Sie Projekte verwalten, und in der Art und Weise, wie Sie Ergebnisse und Aktivitäten verwalten. Weitere Informationen zum Hinzufügen von Projekten zu Zielen finden Sie unter [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/add-activities-to-goals.md). Informationen zu Projekten, die mit Zielen verbunden sind, finden Sie unter [Hinzufügen von Projekten zu Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

Neben Ergebnissen, Aktivitäten und Projekten können Sie auch untergeordnete Ziele mit einem Ziel verknüpfen. Kinderziele sind auch eine Art Fortschrittsanzeige für ein Ziel. Weitere Informationen finden Sie unter [Ziele durch Verbinden in Adobe Workfront-Zielen ausrichten](../goal-alignment/align-goals-by-connecting-them.md). Der Fortschritt der Fortschrittsindikatoren des untergeordneten Ziels treibt auch den Fortschritt des übergeordneten Ziels.

Die folgende Tabelle zeigt Ähnlichkeiten und Unterschiede zwischen Ergebnissen, Aktivitäten und Projekten als Zielindikatoren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b><p>Funktion</p></b></td> 
   <td><b><p>Ergebnisse</p></b></td> 
   <td><b><p>Aktivitäten</p></b></td> 
   <td> <p><strong>Projekte</strong> </p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td><span style="font-weight: normal;">Sie können den Objektnamen in der Workfront-Benutzeroberfläche anpassen</span> </td> 
   <td>ms</td> 
   <td>ms</td> 
   <td>ms</td> 
  </tr> 
  <tr> 
   <td>Sie können sie früheren Zielen hinzufügen.</td> 
   <td>ms</td> 
   <td>ms</td> 
   <td>ms</td> 
  </tr> 
  <tr> 
   <td>Sie können mehrere Ergebnisse, Aktivitäten oder Projekte mit demselben Ziel verknüpfen. </td> 
   <td>ms</td> 
   <td>ms</td> 
   <td>ms</td> 
  </tr> 
  <tr> 
   <td>Sie können einen von ihnen mit mehreren Zielen verknüpfen.</td> 
   <td> </td> 
   <td> </td> 
   <td>ms</td> 
  </tr> 
  <tr> 
   <td>Ihr Fortschritt wird bei der Berechnung des Zielfortschritts berücksichtigt. </td> 
   <td>ms</td> 
   <td>ms</td> 
   <td>ms</td> 
  </tr> 
  <tr> 
   <td>Sie müssen manuell in den Workfront-Zielen aktualisiert werden</td> 
   <td>ms</td> 
   <td>ms</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Sie müssen am Enddatum des Ziels abgeschlossen sein.</td> 
   <td>ms</td> 
   <td>ms</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Sie können nur einem Benutzer und nicht einem Team, einer Gruppe oder dem Unternehmen zugewiesen werden. </td> 
   <td>ms</td> 
   <td>ms</td> 
   <td>ms</td> 
  </tr> 
  <tr> 
   <td>Sie sind spezifisch und messbar und enthalten in der Regel festgelegte Zahlen, die ihren Fortschritt anzeigen. </td> 
   <td>ms</td> 
   <td>ms</td> 
   <td>ms</td> 
  </tr> 
  <tr> 
   <td>Sie bieten einen Wertebereich zwischen dem Start- und dem Endwert, der zeigt, wie nah Sie an der Erreichung dieser Werte sind. Die Nähe zum Endwert berechnet einen Fortschrittswert für Ihr Ziel. </td> 
   <td>ms</td> 
   <td>ms</td> 
   <td>ms</td> 
  </tr> 
 </tbody> 
</table>
