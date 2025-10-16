---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Aufgabenbeschränkung - Übersicht: Muss abgeschlossen sein am'
description: Sie können die Aufgabenbeschränkung Muss abgeschlossen sein (MFO) verwenden, um eine Aufgabe so zu planen, dass sie an einem bestimmten Datum endet.
author: Alina
feature: Work Management
exl-id: 9e546a0f-7f7a-4f1c-9d9d-aa3cea377fdf
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Aufgabenbeschränkung - Übersicht: Muss abgeschlossen sein am

Sie können die Aufgabenbeschränkung Muss abgeschlossen sein (MFO) verwenden, um eine Aufgabe so zu planen, dass sie an einem bestimmten Datum endet.

Mit der Bedingung „Muss abgeschlossen sein am“ wird ein Vorgang so geplant, dass er genau zu dem Zeitpunkt und zu dem Datum abgeschlossen wird, **Sie im Feld „Geplantes Abschlussdatum** angeben.

>[!TIP]
>
>Durch die manuelle Aktualisierung des geplanten Abschlussdatums einer Aufgabe wird die Begrenzung der Aufgabe in „Muss abgeschlossen sein am“ geändert.

## Übersicht über „Muss beendet werden bei Aufgabenbeschränkung“

Beachten Sie beim Planen einer Aufgabe mit einer „Muss abgeschlossen sein am“-Einschränkung Folgendes:

* Vorgängerbeziehungen erzwingen keine Neuplanung der Aufgabe. Adobe Workfront ignoriert im Wesentlichen die Vorgängerbeziehungen.
* Die Aufgabe wird als **Gefährdet** angezeigt, wenn die Vorgänger zurückliegen oder sich verspäten.

* Wenn Sie eine Aufgabe mit einer MFO-Einschränkung in ein anderes Projekt verschieben oder kopieren, kann sich die Einschränkung für die Aufgabe oder das Datum des Projekts ändern, je nachdem, welche Einschränkungstermine gelten und welches Start- und Abschlussdatum das Projekt hat. Die folgenden Szenarien sind vorhanden:

   * Wenn das Zielprojekt von Anfang an geplant ist:

      * Wenn das Einschränkungsdatum der Aufgabe vor dem geplanten Startdatum des Projekts liegt, ändert sich die Aufgabenbeschränkung in So bald wie möglich.
      * Wenn das Einschränkungsdatum der Aufgabe nach dem geplanten Abschlussdatum des Projekts liegt, ändert sich das geplante Abschlussdatum des Projekts entsprechend dem Einschränkungsdatum der Aufgabe.

      * Wenn das Zielprojekt für den Abschluss geplant ist:

         * Wenn das Einschränkungsdatum der Aufgabe nach dem Abschlussdatum des Projekts liegt, ändert sich die Aufgabenbeschränkung in So spät wie möglich.
         * Wenn das Einschränkungsdatum der Aufgabe vor dem geplanten Startdatum des Projekts liegt, ändert sich das geplante Startdatum des Projekts, sodass es dem Starteinschränkungsdatum der Aufgabe entspricht.

      * Wenn das Einschränkungsdatum der Aufgabe innerhalb des Start- und Abschlussdatums des Projekts liegt, gibt es unabhängig vom Projektplan keine Änderungen an der Aufgabenbeschränkung oder den Projektdaten.

  Informationen zum Verschieben von Aufgaben finden Sie unter [Aufgaben verschieben](../../../manage-work/tasks/manage-tasks/move-tasks.md). Informationen zum Kopieren von Aufgaben finden Sie unter [Aufgaben kopieren und duplizieren](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Informationen zum Aktualisieren der Aufgabenbeschränkung für eine Aufgabe finden Sie unter [Aktualisieren der Aufgabenbeschränkung einer Aufgabe](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

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
