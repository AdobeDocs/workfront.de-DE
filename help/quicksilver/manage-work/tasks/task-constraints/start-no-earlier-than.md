---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Aufgabenbeschränkung - Übersicht: Nicht früher beginnen als'
description: Verwenden Sie die Aufgabenbeschränkung Nicht früher als (SNET) starten , um den Start einer Aufgabe nach dem von Ihnen angegebenen Datum zu planen.
author: Alina
feature: Work Management
exl-id: 857859fb-87ee-4397-b292-239ed9dc8281
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Aufgabenbeschränkung - Übersicht: Nicht früher beginnen als

Verwenden Sie die Aufgabenbeschränkung Nicht früher als (SNET) starten , um den Start einer Aufgabe nach dem von Ihnen angegebenen Datum zu planen.

## Übersicht über den Start bei Einschränkung „Nicht früher als Aufgabe“

Beachten Sie Folgendes, wenn Sie die Einschränkung Keine frühere als Aufgabe verwenden:

* Sie sollten die Einschränkung Start No Earlier Than verwenden, wenn das Projekt ab Startdatum geplant ist. In diesem Fall können Sie eine weiche Begrenzung für eine Aufgabe bereitstellen, bevor andere abhängige Aufgaben als gefährdet angezeigt werden.
* Beginn Nicht früher als ist die Standardeinschränkung, wenn ein Projekt ab Startdatum geplant ist und wenn das standardmäßige Startdatum des Systems oder der Gruppe für eine neue Aufgabe auf Heute festgelegt ist. Informationen zur Konfiguration der Standardeinstellungen für Aufgaben finden Sie [Konfigurieren von systemweiten Aufgaben- und Problemeinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Wenn Sie das Projekt vom Startdatum aus planen und das standardmäßige Startdatum für eine neue Aufgabe auf Basierend auf dem geplanten Datum des Projekts festgelegt ist, lautet die standardmäßige Einschränkung für eine neue Aufgabe So bald wie möglich .
* Wenn Sie für das Projekt das standardmäßige Startdatum ab Fertigstellungsdatum festlegen und das System für eine neue Aufgabe das Standardstartdatum auf Heute festlegt, wird die Aufgabe durch die Einschränkung Start Nicht früher als geplant, da dies eine Aufgabe mit dem Status „So spät wie möglich“ wäre.
* Wenn Sie eine Aufgabe mit einer SNET-Einschränkung in ein anderes Projekt verschieben oder kopieren, kann sich die Einschränkung für die Aufgabe oder das Datum des Projekts ändern, je nachdem, welche Einschränkungstermine gelten und welches Start- und Abschlussdatum das Projekt hat. Die folgenden Szenarien sind vorhanden:

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
