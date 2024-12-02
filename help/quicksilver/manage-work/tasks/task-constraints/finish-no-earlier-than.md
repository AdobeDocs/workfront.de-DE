---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Aufgabenbegrenzung - Übersicht: Beenden nicht früher als'
description: '"Finish No Previlier Than (FNET)"ist eine Aufgabenbegrenzung, die den Abschluss einer Aufgabe nach dem von Ihnen angegebenen Datum plant.'
author: Alina
feature: Work Management
exl-id: b1dbf5c9-34b6-4c25-b582-ce9454501e03
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Aufgabenbegrenzung - Übersicht: Beenden nicht früher als

&quot;Finish No Previlier Than (FNET)&quot;ist eine Aufgabenbegrenzung, die den Abschluss einer Aufgabe nach dem von Ihnen angegebenen Datum plant.

## Übersicht über die Beschränkung &quot;Keine frühere Beschränkung als&quot;

Beachten Sie Folgendes bei der Verwendung der Beschränkung &quot;Fertigstellen nicht früher als (FNET)&quot;für eine Aufgabe:

* Sie sollten diese Einschränkung verwenden, wenn das Projekt ab dem Abschlussdatum geplant ist. In diesem Fall können Sie eine weiche Einschränkung für die Aufgabe festlegen, bevor Sie andere abhängige Aufgaben zwingen, &quot;Risiko&quot;anzuzeigen.
* Wenn Sie FNET für ein Projekt verwenden, das geplant ist **Vom Startdatum**, dann plant die Beschränkung die Aufgabe so, wie sie es planen würde, wenn die Beschränkung so bald wie möglich wäre.
* Wenn Sie eine Aufgabe mit einer FNET-Einschränkung in ein anderes Projekt verschieben oder kopieren, können sich die Beschränkung der Aufgabe oder die Daten des Projekts je nach dem, was die Beschränkungsdaten sind und was die Start- und Abschlussdaten des Projekts sind, ändern. Die folgenden Szenarien existieren:

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
