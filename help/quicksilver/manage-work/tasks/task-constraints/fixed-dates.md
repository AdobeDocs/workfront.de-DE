---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Übersicht über die Aufgabenbeschränkung: Feste Termine'
description: Sie können die Aufgabenbeschränkung Feste Termine verwenden, wenn Sie das genaue Start- und Enddatum Ihrer Aufgaben genau angeben möchten. Weitere Informationen zu Aufgabenbeschränkungen finden Sie unter Übersicht über Aufgabenbeschränkungen.
author: Alina
feature: Work Management
exl-id: 084f54a6-e757-405c-b388-5d5f61608e71
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Aufgabenbeschränkung - Übersicht: Feste Termine

Sie können die Aufgabenbeschränkung Feste Termine verwenden, wenn Sie das genaue Start- und Enddatum Ihrer Aufgaben genau angeben möchten. Weitere Informationen zu Aufgabenbeschränkungen finden Sie unter [Übersicht über Aufgabenbeschränkungen](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

## Übersicht über die Beschränkung Feste Daten

Beachten Sie bei Verwendung der Beschränkung Feste Daten Folgendes:

* Wenn Sie die Aufgabenbeschränkung Feste Termine (FIXT) auswählen, müssen Sie das geplante Startdatum und das geplante Abschlussdatum der Aufgabe angeben. In diesem Fall wird die Vorgängerbeziehung der Aufgabe ignoriert.
* Das Feld Dauer der Aufgabe kann bei Verwendung der FIXT-Beschränkung nicht bearbeitet werden. Die Dauer wird als Differenz zwischen dem geplanten Start- und dem geplanten Abschlussdatum der Aufgabe berechnet.
* Wenn der Dauertyp der Aufgabe vom Aufwand gesteuert wird, wirkt sich die Anzahl der Beauftragten für die Aufgabe auch auf die Dauer der Aufgabe aus.
* Wenn Sie eine Aufgabe mit einer FIXT-Beschränkung in ein anderes Projekt verschieben oder kopieren, kann sich die Begrenzung der Aufgabe oder die Termine des Projekts ändern, je nachdem, welche Einschränkungstermine gelten und welches Start- und Abschlussdatum das Projekt hat. Die folgenden Szenarien sind vorhanden:

   * Wenn das Zielprojekt von Anfang an geplant ist:

      * Wenn ein Einschränkungsdatum der Aufgabe vor dem Projektstartdatum liegt, wird die Aufgabenbeschränkung auf „So bald wie möglich“ geändert.
      * Wenn ein oder beide Einschränkungstermine der Aufgabe nach dem geplanten Abschlussdatum des Projekts liegen, ändert sich das geplante Abschlussdatum des Projekts, sodass es dem Fertigstellungseinschränkungsdatum der Aufgabe entspricht.

   * Wenn das Zielprojekt für den Abschluss geplant ist:

      * Wenn ein Einschränkungstermin der Aufgabe nach dem Projektabschlussdatum liegt, wird die Aufgabenbeschränkung auf So spät wie möglich geändert.
      * Wenn ein oder beide Einschränkungstermine des Vorgangs vor dem geplanten Startdatum des Projekts liegen, ändert sich das geplante Startdatum des Projekts, sodass es dem Starteinschränkungsdatum des Vorgangs entspricht.

   * Wenn die Einschränkungstermine der Aufgabe innerhalb des Start- und Abschlussdatums des Projekts liegen, gibt es unabhängig vom Projektplan keine Änderungen an der Aufgabenbeschränkung oder den Projektterminen.

  Informationen zum Verschieben von Aufgaben finden Sie unter [Aufgaben verschieben](../../../manage-work/tasks/manage-tasks/move-tasks.md). Informationen zum Kopieren von Aufgaben finden Sie unter [Aufgaben kopieren und duplizieren](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Informationen zum Aktualisieren der Aufgabenbeschränkung für eine Aufgabe finden Sie unter [Aktualisieren der Aufgabenbeschränkung einer Aufgabe](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Fixed Dates Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
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
