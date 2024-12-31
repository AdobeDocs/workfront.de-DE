---
product-area: projects
navigation-topic: update-work-in-a-project
title: Interaktionen zwischen dem Commit-Datum und dem geplanten Abschlussdatum
description: Sowohl das geplante Abschlussdatum als auch das Commit-Datum geben an, wann die Aufgabe abgeschlossen werden soll. Aber sie unterscheiden sich aufgrund dessen, wer jedes Datum festlegt.
author: Alina
feature: Work Management
exl-id: 1709c60c-ac75-48eb-9226-ec2cf556ebf0
source-git-commit: 1eb1e919bede7e366956d8c0bd969329a641123f
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 1%

---

# Interaktionen zwischen dem Commit-Datum und dem geplanten Abschlussdatum

<!--
this article has mostly information that is repeated from the articles linked from here. I left it in here for searchability's sake.
-->

Sowohl das geplante Abschlussdatum als auch das Commit-Datum geben an, wann die Aufgabe abgeschlossen werden soll. Aber sie unterscheiden sich aufgrund dessen, wer jedes Datum festlegt.

## Übersicht über das Commit-Datum und das geplante Abschlussdatum

Geplante Fertigstellungs- und Commit-Termine gibt es sowohl für Aufgaben als auch für Probleme.

Die folgende Tabelle enthält Informationen zum Unterschied zwischen dem Commit- und dem geplanten Abschlussdatum:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Verpflichtungsdatum</td> 
   <td> <p>Das Commit-Datum ist das Datum, bis zu dem die Person, die einer Aufgabe oder einem Problem zugewiesen ist, manuell schätzt, dass sie die Aufgabe oder das Problem abgeschlossen haben wird.</p> <p>Informationen zu Commit-Terminen finden Sie <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Übersicht Commit-Datum</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Geplantes Abschlussdatum</td> 
   <td> <p>Das geplante Abschlussdatum gibt an, wann der Projektinhaber erwartet, dass die Aufgabe oder das Problem abgeschlossen ist. Sie kann entweder vom Projektbesitzer oder von jedem mit Verwaltungsberechtigungen für die Aufgabe oder das Problem manuell festgelegt oder automatisch von Adobe Workfront berechnet werden.</p> <p>Weitere Informationen zu geplanten Abschlussdaten finden Sie unter <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Übersicht über das geplante Abschlussdatum der Aufgabe</a></p> </td> 
  </tr> 
 </tbody> 
</table>

## Interaktionen zwischen dem Commit-Datum und dem geplanten Abschlussdatum

Wenn der Projektbesitzer eine Aufgabe oder ein Problem erstellt und zuweist, hat die Aufgabe oder das Problem Folgendes:

* Ein geplantes Abschlussdatum
* Kein Commit-Datum

Der Verantwortliche, der an der Aufgabe oder dem Problem arbeitet, kann das Commit-Datum manuell aktualisieren oder durch Akzeptieren der Bearbeitung automatisch aktualisieren. Dies ist eine visuelle Methode, um dem Projekteigentümer mitzuteilen, wann es für ihn realistisch wäre, die Aufgabe oder das Problem abzuschließen.

>[!TIP]
>
>Nur der Verantwortliche kann das Commit-Datum einer Aufgabe oder eines Problems aktualisieren.

Der Verantwortliche, der das Verpflichtungsdatum ändert, ändert nicht automatisch das geplante Abschlussdatum. Umgekehrt gilt auch: Durch die Änderung des geplanten Abschlussdatums wird das Commit-Datum nicht geändert.

Wenn sich das Commit-Datum ändert, wird der Projektbesitzer über eine In-App-Benachrichtigung von Workfront darüber benachrichtigt, dass diese Änderung vorgenommen wurde.

Wenn das vom Verantwortlichen angebotene Commit-Datum für den Projektbesitzer akzeptabel ist, muss er das geplante Abschlussdatum für die Aufgabe manuell aktualisieren, um die Auswirkungen zu veranschaulichen, die es auf die Timeline des Projekts haben kann. Änderungen am geplanten Abschlussdatum von Problemen wirken sich nicht auf die Projektzeitleiste aus.

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Übersicht über das Commit-Datum](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
* [Aktualisieren von Commit-Terminen für Aufgaben und Probleme](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md)
