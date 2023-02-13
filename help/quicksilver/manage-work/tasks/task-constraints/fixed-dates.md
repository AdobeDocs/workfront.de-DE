---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '"Task Constraint - Übersicht: Feste Datumswerte'
description: Sie können die Aufgabenbegrenzung Feste Datumswerte verwenden, wenn Sie für das genaue Start- und Enddatum Ihrer Aufgaben spezifisch sein möchten. Weitere Informationen zu Aufgabenbegrenzungen finden Sie unter Übersicht über Aufgabenbegrenzungen .
author: Alina
feature: Work Management
exl-id: 084f54a6-e757-405c-b388-5d5f61608e71
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Übersicht über Aufgabenbeschränkungen: Feste Datumswerte

Sie können die Aufgabenbegrenzung Feste Datumswerte verwenden, wenn Sie für das genaue Start- und Enddatum Ihrer Aufgaben spezifisch sein möchten. Weitere Informationen zu Aufgabenbegrenzungen finden Sie unter [Übersicht über Aufgabenbegrenzungen](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

## Übersicht über die Beschränkung &quot;Feste Datumswerte&quot;

Beachten Sie Folgendes bei Verwendung der Beschränkung &quot;Feste Datumswerte&quot;:

* Wenn Sie die Aufgabenbegrenzung Feste Datumswerte (FIXT) auswählen, müssen Sie das geplante Startdatum und das geplante Abschlussdatum der Aufgabe angeben. In diesem Fall wird die Vorgängerbeziehung der Aufgabe ignoriert.
* Das Feld Dauer der Aufgabe kann bei Verwendung der FIXT-Beschränkung nicht bearbeitet werden. Die Dauer wird als Differenz zwischen dem geplanten Start- und dem geplanten Abschlussdatum der Aufgabe berechnet.
* Wenn der Aufgabentyp Effort gesteuert ist, wirkt sich die Anzahl der Zuweisung der Aufgabe auch auf die Dauer der Aufgabe aus.
* Wenn Sie eine Aufgabe mit einer FIXT-Einschränkung in ein anderes Projekt verschieben oder kopieren, können sich die Beschränkung der Aufgabe oder die Daten des Projekts je nach den Einschränkungsdaten und den Start- und Abschlussdaten des Projekts ändern. Die folgenden Szenarien existieren:

   * Wenn das Zielprojekt von Anfang an geplant ist:

      * Wenn ein Beschränkungsdatum der Aufgabe vor dem Projektstartdatum liegt, ändert sich die Aufgabenbegrenzung in So bald wie möglich.
      * Wenn ein oder beide Beschränkungsdaten der Aufgabe nach dem geplanten Abschlussdatum des Projekts liegen, ändert sich das geplante Abschlussdatum des Projekts entsprechend dem Abschlussdatum der Aufgabe.
   * Wenn das Zielprojekt nach Abschluss geplant wird:

      * Wenn ein Beschränkungsdatum der Aufgabe nach dem Projektabschlussdatum liegt, ändert sich die Aufgabenbegrenzung in &quot;So spät wie möglich&quot;.
      * Wenn ein oder beide Beschränkungsdaten der Aufgabe vor dem geplanten Startdatum des Projekts liegen, wird das geplante Startdatum des Projekts an das Startdatum der Aufgabe angepasst.
   * Unabhängig vom Zeitplan des Projekts gibt es keine Änderungen an der Aufgabenbegrenzung oder den Projektzeitpunkten, wenn die Beschränkungsdaten der Aufgabe innerhalb des Start- und Abschlussdatums des Projekts liegen.

   Informationen zum Verschieben von Aufgaben finden Sie unter [Aufgaben verschieben](../../../manage-work/tasks/manage-tasks/move-tasks.md). Informationen zum Kopieren von Aufgaben finden Sie unter [Aufgaben kopieren und duplizieren](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Informationen zum Aktualisieren der Aufgabenbegrenzung für eine Aufgabe finden Sie unter [Aktualisieren der Aufgabenbegrenzung einer Aufgabe](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Fixed Dates Task Constraint</h2>
<p>(NOTE:&nbsp;replaced with new article linked above) </p>
<p>To update the Task Constraint to Finish No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Fixed Dates</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>The task must start on this date. </p> </li>
<li value="6"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete on this date. </p> </li>
<li value="7">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
