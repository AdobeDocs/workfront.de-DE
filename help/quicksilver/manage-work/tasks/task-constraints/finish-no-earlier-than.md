---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Aufgabenbeschränkung - Übersicht: Beenden nicht früher als'
description: „Nicht früher als“ (FNET) ist eine Aufgabenbeschränkung, die den Abschluss einer Aufgabe nach dem von Ihnen angegebenen Datum plant.
author: Alina
feature: Work Management
exl-id: b1dbf5c9-34b6-4c25-b582-ce9454501e03
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Aufgabenbeschränkung - Übersicht: Beenden nicht früher als

„Nicht früher als“ (FNET) ist eine Aufgabenbeschränkung, die den Abschluss einer Aufgabe nach dem von Ihnen angegebenen Datum plant.

## Übersicht der Endbearbeitung Nicht früher als Bedingung

Beachten Sie Folgendes, wenn Sie die Bedingung „Beenden nicht früher als (FNET)“ für eine Aufgabe verwenden:

* Sie sollten diese Einschränkung verwenden, wenn das Projekt ab Abschlussdatum geplant ist. In diesem Fall können Sie eine weiche Begrenzung für die Aufgabe festlegen, bevor Sie andere abhängige Aufgaben zwingen, „Gefährdet“ anzuzeigen.
* Wenn Sie FNET für ein Projekt verwenden, **vom Startdatum**, wird die Aufgabe durch die Begrenzung so geplant, wie sie geplant wäre, wenn die Begrenzung so bald wie möglich festgelegt würde.
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
<h2>Use the Finish No Earlier Than constraint</h2>
<p>(NOTE: replaced with new article linked above)&nbsp;</p>
<p>To update the Task Constraint to Finish No Earlier Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>Finish No Earlier Than</strong>.</p> <p> <img src="assets/fnet-350x267.png" alt="FNET.png" style="width: 350;height: 267;"> </p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete no earlier than this date. </p> </li>
<li value="6">Click <strong>Save Changes.</strong> </li>
</ol>
</div>
-->
