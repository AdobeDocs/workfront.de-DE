---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Übersicht über Aufgabenbegrenzungen: Start nicht früher als'
description: Verwenden Sie die Task-Beschränkung Start nicht früher als (SNET) , um eine Aufgabe so zu planen, dass sie nach dem von Ihnen angegebenen Datum beginnt.
author: Alina
feature: Work Management
exl-id: 857859fb-87ee-4397-b292-239ed9dc8281
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Übersicht über Aufgabenbegrenzungen: Start nicht früher als

Verwenden Sie die Task-Beschränkung Start nicht früher als (SNET) , um eine Aufgabe so zu planen, dass sie nach dem von Ihnen angegebenen Datum beginnt.

## Übersicht über die Startbeschränkung &quot;Keine frühere Aufgabe als Task&quot;

Beachten Sie Folgendes bei Verwendung der Beschränkung &quot;Start nicht früher als Aufgabe&quot;:

* Sie sollten die Beschränkung Start nicht früher als verwenden, wenn das Projekt ab Startdatum geplant ist. In diesem Fall können Sie eine weiche Einschränkung für eine Aufgabe festlegen, bevor andere abhängige Aufgaben als &quot;Risiko&quot;angezeigt werden.
* &quot;Anfang nicht früher&quot;ist die Standardeinschränkung, wenn ein Projekt vom Startdatum geplant ist und das standardmäßige Start-Datum des Systems oder der Gruppe für eine neue Aufgabe auf &quot;Heute&quot;festgelegt ist. Weitere Informationen zum Konfigurieren von Standardeinstellungen für Aufgaben finden Sie unter [Konfigurieren von systemweiten Aufgaben und Ausgabevoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Wenn Sie das Projekt vom Startdatum planen und das standardmäßige Startdatum des Systems für eine neue Aufgabe auf &quot;Basierend auf dem geplanten Projektdatum&quot;festgelegt ist, ist die Standardeinschränkung für eine neue Aufgabe so bald wie möglich.
* Wenn Sie das Projekt vom Abschlussdatum planen und das standardmäßige Startdatum des Systems für eine neue Aufgabe auf Heute festgelegt ist, wird die Aufgabe durch die Einstellung &quot;Anfang nicht früher als Begrenzung&quot;so geplant, wie es für eine möglichst späte Aufgabe wäre.
* Wenn Sie eine Aufgabe mit einer SNET-Einschränkung in ein anderes Projekt verschieben oder kopieren, können sich die Beschränkung der Aufgabe oder die Daten des Projekts je nach den Einschränkungsdaten und den Start- und Abschlussdaten des Projekts ändern. Die folgenden Szenarien existieren:

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
<h2>Use the Start No Earlier Than Task Constraint</h2>
<p>(NOTE:&nbsp;replaced with new article linked above)&nbsp;</p>
<p>To update the Task Constraint to Start No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Start No Earlier Than</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>This is the date by which the task must start, and not earlier than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
