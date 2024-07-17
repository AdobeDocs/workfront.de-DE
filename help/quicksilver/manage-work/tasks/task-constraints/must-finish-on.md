---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: "Task Constraint Overview: Must Finish On"
description: Sie können die Task-Beschränkung Must Finish On (MFO) verwenden, um eine Aufgabe so zu planen, dass sie an einem bestimmten Datum endet.
author: Alina
feature: Work Management
exl-id: 9e546a0f-7f7a-4f1c-9d9d-aa3cea377fdf
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Übersicht über Aufgabenbegrenzungen: Muss fertig gestellt sein am

Sie können die Task-Beschränkung Must Finish On (MFO) verwenden, um eine Aufgabe so zu planen, dass sie an einem bestimmten Datum endet.

&quot;Must Finish On constraint&quot;plant, dass eine Aufgabe genau zu dem Zeitpunkt und zu dem Datum beendet wird, den Sie im Feld **Geplantes Abschlussdatum** angeben.

>[!TIP]
>
>Durch manuelles Aktualisieren des geplanten Abschlussdatums einer Aufgabe wird die Beschränkung der Aufgabe in &quot;Must Finish On&quot;geändert.

## Übersicht über die &quot;Must Finish on Task Constraint&quot;-Beschränkung

Beachten Sie Folgendes bei der Planung einer Aufgabe mit der Einschränkung Must Finish On :

* Vorgängerbeziehungen erzwingen keine Neuplanung der Aufgabe. Adobe Workfront ignoriert im Wesentlichen die Vorgängerbeziehungen.
* Die Aufgabe wird als **Risiko** angezeigt, wenn die Vorgänger beginnen zu laufen oder sich verspäten.

* Wenn Sie eine Aufgabe mit einer MFO-Beschränkung verschieben oder in ein anderes Projekt kopieren, können sich die Beschränkung der Aufgabe oder die Daten des Projekts je nach den Einschränkungsdaten und den Start- und Abschlussdaten des Projekts ändern. Die folgenden Szenarien existieren:

   * Wenn das Zielprojekt von Anfang an geplant ist:

      * Wenn das Beschränkungsdatum der Aufgabe vor dem geplanten Startdatum des Projekts liegt, ändert sich die Aufgabenbegrenzung in So bald wie möglich.
      * Wenn das Beschränkungsdatum der Aufgabe nach dem geplanten Abschlussdatum des Projekts liegt, ändert sich das geplante Abschlussdatum des Projekts entsprechend dem Abschlussdatum der Aufgabe.

      * Wenn das Zielprojekt nach Abschluss geplant wird:

         * Wenn das Beschränkungsdatum der Aufgabe nach dem Abschlussdatum des Projekts liegt, ändert sich die Aufgabenbegrenzung in &quot;So spät wie möglich&quot;.
         * Wenn das Beschränkungsdatum der Aufgabe vor dem geplanten Startdatum des Projekts liegt, ändert sich das geplante Startdatum des Projekts entsprechend dem Startbegrenzungsdatum der Aufgabe.

      * Wenn das Beschränkungsdatum der Aufgabe innerhalb des Start- und Abschlussdatums des Projekts liegt, gibt es unabhängig vom Zeitplan des Projekts keine Änderungen an der Aufgabenbegrenzung oder den Projektzeitpunkten.

  Informationen zum Verschieben von Aufgaben finden Sie unter [Verschieben von Aufgaben](../../../manage-work/tasks/manage-tasks/move-tasks.md). Informationen zum Kopieren von Aufgaben finden Sie unter [Kopieren und Duplizieren von Aufgaben](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Informationen zum Aktualisieren der Aufgabenbegrenzung für eine Aufgabe finden Sie unter [Aktualisieren der Aufgabenbegrenzung einer Aufgabe](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Must Finish On Task Constraint</h2>
<p>To update the Task Constraint to Must Finish On:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Must Finish On</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete by this date, and no later than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
