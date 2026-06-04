---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Aufgabenbeschränkung - Übersicht: spätestens beginnen am'
description: Start Later Than (SNLT) ist eine Aufgabenbeschränkung, die eine Aufgabe so plant, dass sie vor dem angegebenen Datum beginnt.
author: Alina
feature: Work Management
exl-id: 86139ce6-c6b1-4ac4-a5cb-fd4aa899a025
TQID: https://experienceleague.adobe.com/eX2KAzQkOb0AmYcR5Zc6SPeySBTDKjM74QYi7ox4A0w
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 436
ht-degree: 1%

---

# Überblick über Aufgabenbeschränkungen: Nicht später anfangen als

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
