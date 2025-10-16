---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Aufgabenbeschränkung - Übersicht: Muss beginnen am'
description: Verwenden Sie die Aufgabenbeschränkung Muss beginnen am (MSO) , um den Start einer Aufgabe genau an einem bestimmten Datum zu planen.
author: Alina
feature: Work Management
exl-id: 09062d46-2b80-4758-946e-d6dec0f7a7c0
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Aufgabenbeschränkung - Übersicht: Muss beginnen am

Verwenden Sie die Aufgabenbeschränkung Muss beginnen am (MSO) , um den Start einer Aufgabe genau an einem bestimmten Datum zu planen.

Mit der Einschränkung Muss beginnen am wird ein Vorgang so geplant, dass er genau zu der Uhrzeit und zu dem Datum beginnt, die Sie im Feld **Geplantes Startdatum** angeben.

>[!TIP]
>
>Durch die manuelle Aktualisierung des geplanten Startdatums einer Aufgabe wird die Begrenzung der Aufgabe in „Muss beginnen am“ geändert.

## Übersicht über „Muss bei Aufgabenbeschränkung beginnen“

Beachten Sie beim Planen einer Aufgabe mit der Einschränkung Muss beginnen bei Folgendes:

* Vorgängerbeziehungen erzwingen nicht, dass diese Aufgabe neu geplant wird. Workfront ignoriert mit dieser Einschränkung im Wesentlichen alle Vorgängerbeziehungen der Aufgabe.
* Die Aufgabe zeigt &quot;**Risiko** an, wenn Vorgänger zurückliegen oder sich verspäten.

* Wenn Sie eine Aufgabe mit einer MSO-Einschränkung in ein anderes Projekt verschieben oder kopieren, kann sich die Einschränkung für die Aufgabe oder das Datum des Projekts ändern, je nachdem, welche Einschränkungstermine es gibt und welches Start- und Abschlussdatum das Projekt hat. Die folgenden Szenarien sind vorhanden:

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
<h2>Use the Must Start On Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Must Start On:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Must Start On</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>The task must start by this date, and no later than this date.</p> </li>
<li value="6">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
