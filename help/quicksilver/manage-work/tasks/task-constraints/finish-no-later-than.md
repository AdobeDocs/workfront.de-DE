---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '"Task Constraint - Übersicht: Beenden nicht später als'''
description: '"Finish No Later Than (FNLT)"ist eine Aufgabenbegrenzung, die den Abschluss einer Aufgabe vor dem angegebenen Datum plant.'
author: Alina
feature: Work Management
exl-id: ea0e74fb-45a0-4466-b57d-294a9babb340
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# Übersicht über Aufgabenbeschränkungen: Finish No Later Than

&quot;Finish No Later Than (FNLT)&quot;ist eine Aufgabenbegrenzung, die den Abschluss einer Aufgabe vor dem angegebenen Datum plant.

## Übersicht über die Beschränkung &quot;Nicht später als&quot;beenden

Beachten Sie Folgendes bei Verwendung der Beschränkung &quot;Finish No Later Than (FNLT)&quot;für eine Aufgabe:

* Sie sollten diese Einschränkung verwenden, wenn das Projekt ab Startdatum geplant ist. In diesem Fall können Sie eine weiche Einschränkung für eine Aufgabe festlegen, bevor andere abhängige Aufgaben als &quot;Risiko&quot;angezeigt werden.
* Wenn Sie die FNLT-Einschränkung mit einem Projekt &quot;Zeitplan ab Abschlussdatum&quot;verwenden, plant diese Einschränkung die Aufgabe so wie eine Aufgabe, die so spät wie möglich ist.
* Wenn Sie eine Aufgabe mit einer FNET-Einschränkung in ein anderes Projekt verschieben oder kopieren, können sich die Beschränkung der Aufgabe oder die Daten des Projekts je nach dem, was die Beschränkungsdaten sind und was die Start- und Abschlussdaten des Projekts sind, ändern. Die folgenden Szenarien existieren:

   * Wenn das Zielprojekt von Anfang an geplant ist:

      * Wenn das Beschränkungsdatum der Aufgabe vor dem geplanten Startdatum des Projekts liegt, ändert sich die Aufgabenbegrenzung in So bald wie möglich.
      * Wenn das Beschränkungsdatum der Aufgabe nach dem geplanten Abschlussdatum des Projekts liegt, ändert sich das geplante Abschlussdatum des Projekts entsprechend dem Abschlussdatum der Aufgabe.

      * Wenn das Zielprojekt nach Abschluss geplant wird:

         * Wenn das Beschränkungsdatum der Aufgabe nach dem Abschlussdatum des Projekts liegt, ändert sich die Aufgabenbegrenzung in &quot;So spät wie möglich&quot;.
         * Wenn das Beschränkungsdatum der Aufgabe vor dem geplanten Startdatum des Projekts liegt, ändert sich das geplante Startdatum des Projekts entsprechend dem Startbegrenzungsdatum der Aufgabe.
      * Wenn das Beschränkungsdatum der Aufgabe innerhalb des Start- und Abschlussdatums des Projekts liegt, gibt es unabhängig vom Zeitplan des Projekts keine Änderungen an der Aufgabenbegrenzung oder den Projektzeitpunkten.

   Informationen zum Verschieben von Aufgaben finden Sie unter [Aufgaben verschieben](../../../manage-work/tasks/manage-tasks/move-tasks.md). Informationen zum Kopieren von Aufgaben finden Sie unter [Aufgaben kopieren und duplizieren](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Informationen zum Aktualisieren der Aufgabenbegrenzung für eine Aufgabe finden Sie unter [Aktualisieren der Aufgabenbegrenzung einer Aufgabe](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Finish No Later Than constraint</h2>
<p>To update the Task Constraint to Finish No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Finish No Later Than</strong>.</p> <p> <img src="assets/fnlt-350x266.png" alt="FNLT.png" style="width: 350;height: 266;"> </p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>You must complete the task on and not later than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
