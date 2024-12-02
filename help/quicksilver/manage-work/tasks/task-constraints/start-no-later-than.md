---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Übersicht über Aufgabenbegrenzungen: Start nicht später als'
description: Start nicht später als (SNLT) ist eine Aufgabenbegrenzung, die den Beginn einer Aufgabe vor dem von Ihnen angegebenen Datum plant.
author: Alina
feature: Work Management
exl-id: 86139ce6-c6b1-4ac4-a5cb-fd4aa899a025
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# Übersicht über Aufgabenbegrenzungen: Start nicht später als

Start nicht später als (SNLT) ist eine Aufgabenbegrenzung, die den Beginn einer Aufgabe vor dem von Ihnen angegebenen Datum plant.

Beachten Sie beim Arbeiten mit der SNLT-Beschränkung Folgendes:

* Sie sollten die Beschränkung &quot;Start nicht später als&quot;verwenden, wenn das Projekt ab dem vollständigen Datum geplant ist. In diesem Fall können Sie eine weiche Einschränkung für eine Aufgabe festlegen, bevor andere abhängige Aufgaben als &quot;Risiko&quot;angezeigt werden.
* &quot;Start nicht später als&quot;ist die Standardeinschränkung, wenn ein Projekt den Planungsmodus &quot;Zeitplan ab Abschlussdatum&quot;verwendet und der standardmäßige System- oder Gruppenstandard für das Startdatum einer Aufgabe &quot;Heute&quot;lautet. Informationen darüber, wo die Standardbegrenzung für eine neue Aufgabe festgelegt werden soll, finden Sie unter [Systemweite Aufgaben konfigurieren und Ausgabeeinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* Wenn Sie die SNLT-Beschränkung mit einem Projekt &quot;Schedule From Start Date&quot;verwenden, plant Adobe Workfront die Aufgabe so, wie es eine Aufgabe so bald wie möglich wäre.
* Wenn Sie eine Aufgabe mit einer SNLT-Einschränkung in ein anderes Projekt verschieben oder kopieren, können sich die Beschränkung der Aufgabe oder die Daten des Projekts je nach den Einschränkungsdaten und den Start- und Abschlussdaten des Projekts ändern. Die folgenden Szenarien existieren:

   * Wenn das Zielprojekt von Anfang an geplant ist:

      * Wenn das Beschränkungsdatum der Aufgabe vor dem geplanten Startdatum des Projekts liegt, ändert sich die Aufgabenbegrenzung in So bald wie möglich.
      * Wenn das Beschränkungsdatum der Aufgabe nach dem geplanten Abschlussdatum des Projekts liegt, ändert sich das geplante Abschlussdatum des Projekts entsprechend dem Abschlussdatum der Aufgabe.

      * Wenn das Zielprojekt nach Abschluss geplant wird:

         * Wenn das Beschränkungsdatum der Aufgabe nach dem Abschlussdatum des Projekts liegt, ändert sich die Aufgabenbegrenzung in &quot;So spät wie möglich&quot;.
         * Wenn das Beschränkungsdatum der Aufgabe vor dem geplanten Startdatum des Projekts liegt, ändert sich das geplante Startdatum des Projekts entsprechend dem Startbegrenzungsdatum der Aufgabe.

      * Wenn das Beschränkungsdatum der Aufgabe innerhalb des Start- und Abschlussdatums des Projekts liegt, gibt es unabhängig vom Zeitplan des Projekts keine Änderungen an der Aufgabenbegrenzung oder den Projektzeitpunkten.

  Informationen zum Verschieben von Aufgaben finden Sie unter [Verschieben von Aufgaben](../../../manage-work/tasks/manage-tasks/move-tasks.md).

  Informationen zum Kopieren von Aufgaben finden Sie unter [Kopieren und Duplizieren von Aufgaben](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Informationen zum Aktualisieren der Aufgabenbegrenzung für eine Aufgabe finden Sie unter [Aktualisieren der Aufgabenbegrenzung einer Aufgabe](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

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
