---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Aufgabenbeschränkung - Übersicht: spätestens beenden'
description: „Spätestes Ende“ (FNLT) ist eine Aufgabenbeschränkung, die einen Vorgang so terminiert, dass er vor dem angegebenen Datum abgeschlossen wird.
author: Alina
feature: Work Management
exl-id: ea0e74fb-45a0-4466-b57d-294a9babb340
TQID: https://experienceleague.adobe.com/lNcQlOWhkCOl0keoOBLgyKVo3VmlOnEPXRmVGhHFHF8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 388
ht-degree: 1%

---

# Überblick über Aufgabenbeschränkungen: Nicht später beenden als (NSBA)

„Spätestes Ende“ (FNLT) ist eine Aufgabenbeschränkung, die einen Vorgang so terminiert, dass er vor dem angegebenen Datum abgeschlossen wird.

## Übersicht über die Bedingung „Spätestens am“

Beachten Sie Folgendes, wenn Sie die Einschränkung Beenden nicht später als (FNLT) für eine Aufgabe verwenden:

* Sie sollten diese Einschränkung verwenden, wenn das Projekt ab Startdatum geplant wird. In diesem Fall können Sie eine weiche Begrenzung für eine Aufgabe bereitstellen, bevor andere abhängige Aufgaben als gefährdet angezeigt werden.
* Wenn Sie die FNLT-Beschränkung mit einem Projekt „Zeitplan ab Abschlussdatum“ verwenden, plant diese Beschränkung die Aufgabe so, wie es bei einer Aufgabe mit möglichst spätem Datum der Fall wäre.
* Wenn Sie einen Vorgang mit einer FNET-Einschränkung in ein anderes Projekt verschieben oder kopieren, kann sich die Einschränkung für den Vorgang oder die Termine des Projekts ändern, je nachdem, welche Einschränkungstermine es gibt und welches Start- und Abschlussdatum das Projekt hat. Die folgenden Szenarien sind vorhanden:

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
