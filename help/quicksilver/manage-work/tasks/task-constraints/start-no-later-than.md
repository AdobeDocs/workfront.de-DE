---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Aufgabenbeschränkung - Übersicht: spätestens beginnen am'
description: Start Later Than (SNLT) ist eine Aufgabenbeschränkung, die eine Aufgabe so plant, dass sie vor dem angegebenen Datum beginnt.
author: Alina
feature: Work Management
exl-id: 86139ce6-c6b1-4ac4-a5cb-fd4aa899a025
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# Aufgabenbeschränkung - Übersicht: spätestens beginnen am

Start Later Than (SNLT) ist eine Aufgabenbeschränkung, die eine Aufgabe so plant, dass sie vor dem angegebenen Datum beginnt.

Beachten Sie beim Arbeiten mit der SNT-Einschränkung Folgendes:

* Sie sollten die Einschränkung Start Später als verwenden, wenn das Projekt ab Abschlussdatum geplant ist. In diesem Fall können Sie eine weiche Begrenzung für eine Aufgabe bereitstellen, bevor andere abhängige Aufgaben als gefährdet angezeigt werden.
* Start Später als ist die Standardbedingung, wenn ein Projekt den Planungsmodus „Zeitplan“ ab Abschlussdatum verwendet und der System- oder Gruppenstandard für das Startdatum einer Aufgabe „Heute“ ist. Informationen dazu, wo die Standardeinschränkung für eine neue Aufgabe festgelegt werden soll, finden Sie [Konfigurieren von systemweiten Aufgaben- und Problemeinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* Wenn Sie die SNLT-Einschränkung mit einem Projekt vom Startdatum an verwenden, plant Adobe Workfront die Aufgabe so, wie es sich für eine Aufgabe vom Typ „So bald wie möglich“ gehört.
* Wenn Sie eine Aufgabe mit einer SNLT-Beschränkung in ein anderes Projekt verschieben oder kopieren, kann sich die Begrenzung der Aufgabe oder die Termine des Projekts ändern, je nachdem, welche Einschränkungstermine gelten und welches die Start- und Abschlussdaten des Projekts sind. Die folgenden Szenarien sind vorhanden:

   * Wenn das Zielprojekt von Anfang an geplant ist:

      * Wenn das Einschränkungsdatum der Aufgabe vor dem geplanten Startdatum des Projekts liegt, ändert sich die Aufgabenbeschränkung in So bald wie möglich.
      * Wenn das Einschränkungsdatum der Aufgabe nach dem geplanten Abschlussdatum des Projekts liegt, ändert sich das geplante Abschlussdatum des Projekts entsprechend dem Einschränkungsdatum der Aufgabe.

      * Wenn das Zielprojekt für den Abschluss geplant ist:

         * Wenn das Einschränkungsdatum der Aufgabe nach dem Abschlussdatum des Projekts liegt, ändert sich die Aufgabenbeschränkung in So spät wie möglich.
         * Wenn das Einschränkungsdatum der Aufgabe vor dem geplanten Startdatum des Projekts liegt, ändert sich das geplante Startdatum des Projekts, sodass es dem Starteinschränkungsdatum der Aufgabe entspricht.

      * Wenn das Einschränkungsdatum der Aufgabe innerhalb des Start- und Abschlussdatums des Projekts liegt, gibt es unabhängig vom Projektplan keine Änderungen an der Aufgabenbeschränkung oder den Projektdaten.

  Informationen zum Verschieben von Aufgaben finden Sie unter [Aufgaben verschieben](../../../manage-work/tasks/manage-tasks/move-tasks.md).

  Informationen zum Kopieren von Aufgaben finden Sie unter [Aufgaben kopieren und duplizieren](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Informationen zum Aktualisieren der Aufgabenbeschränkung für eine Aufgabe finden Sie unter [Aktualisieren der Aufgabenbeschränkung einer Aufgabe](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Start No Later Than Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Start No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Start No Later Than</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>This is the date by which the task must start, and not later than this date.</p> </li>
<li value="6">Click <strong>Save Changes</strong>.<br></li>
</ol>
</div>
-->
