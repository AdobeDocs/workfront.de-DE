---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: "Task Constraint Overview: Neueste verfügbare Zeit"
description: Die neueste verfügbare Zeit (LAT) ist eine Art von Aufgabenbegrenzung in Adobe Workfront.
author: Alina
feature: Work Management
exl-id: acf55004-9424-4e24-9ff5-90f6fd7f72a6
source-git-commit: c3abb5dce14c0b19ab2e5b82f159cd29f80f79e4
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Übersicht über Aufgabenbeschränkungen: Aktuelle verfügbare Zeit

Die neueste verfügbare Zeit (LAT) ist eine Art von Aufgabenbegrenzung in Adobe Workfront.

## Verwenden der aktuellen Zeitaufgabenbegrenzung

Sie können die LAT-Beschränkung verwenden, wenn Sie planen möchten, dass eine Aufgabe zum neuesten verfügbaren Zeitpunkt beginnt, nachdem Sie Beziehungen zwischen Vorgänger und Nachfolger im Projekt in Betracht gezogen haben.

Diese Einschränkung unterscheidet sich von So bald wie möglich insofern, als sie keine Neuplanung von Vorgängern oder Nachfolgern erzwingt. Stattdessen wirkt sich dies nur auf den Zeitplan der Aufgabe aus, der sie zugeordnet ist, und setzt sie basierend auf ihrer Beziehung zu anderen Aufgaben auf die neueste verfügbare Zeit.

Informationen zum Aktualisieren der Aufgabenbegrenzung für eine Aufgabe finden Sie unter [Aktualisieren der Aufgabenbegrenzung einer Aufgabe](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To update the Task Constraint to Latest Available Time:</p>
<p>(NOTE: replaced with new article linked above) </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Latest Available Time</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## Differenz zwischen der neuesten verfügbaren Zeit und so spät wie möglich

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "As Late As Possible"] - inserted snippet in both (Alina)) </p>
-->

Die aktuelle Zeitbeschränkung unterscheidet sich von der so spät wie möglich Beschränkung, wenn die folgenden Kriterien vorhanden sind:

* Das Projekt ist ab dem Startdatum geplant.
* Aufgaben im Projekt haben eine Vorgängerbeziehung
* Die Nachfolgeaufgabe hat eine flexible Aufgabenbegrenzung

In diesem Fall:

* **Neueste verfügbare Zeit:** Durch die Verwendung der Zeitbegrenzung &quot;Neueste verfügbare Zeit&quot;für die Vorgängeraufgabe erhält die flexible Beschränkung des Nachfolgers Priorität.

  **Beispiel:** Beispielsweise ist Aufgabe A ein Vorgänger von Aufgabe B. Aufgabe A hat die neueste verfügbare Zeitbegrenzung und Aufgabe B die so bald wie möglich einschränkende Funktion. In diesem Fall wird Aufgabe A so nah wie möglich am Projektstart geplant.

  ![](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **So spät wie möglich:** In diesem Szenario räumt die Verwendung der Beschränkung So spät wie möglich für die Vorgängeraufgabe der Vorgängeraufgabe die Priorität der Vorgängeraufgabe ein.

  **Beispiel:** Beispielsweise ist Aufgabe A ein Vorgänger von Aufgabe B. Aufgabe A hat die so spät wie möglich Beschränkung und Aufgabe B hat die so bald wie möglich Einschränkung. In diesem Fall wird Aufgabe A so nah wie möglich am Ende des Projekts geplant.

  ![](assets/as-late-as-possible-task-constraint-in-task-list-350x104.png)

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: this content was here before but it was wrong - according to this issue in Hub, per Dev, the correct functionality is in the snippet above: https://hub.workfront.com/task/6193c6910004bce9de07cda7757f3ce8/updates?email-source=subscribedCommunication) </p>
<p>The Latest Available Time constraint differs from the As Late As Possible constraint when the following criteria exist:</p>
<ul>
<li> The project is scheduled From Completion </li>
<li> Tasks in the project have a predecessor relationship </li>
<li> The predecessor task has a flexible task constraint </li>
</ul>
<p> In this situation: </p>
<ul>
<li> <p><strong>Latest Available Time:</strong> Using the Latest Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest Available Time constraint and Task A has the As Soon As Possible constraint. In this situation, Task B is scheduled as close to the start of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late As Possible constraint and Task A has the As Soon As Possible constraint. In this situation, Task B is scheduled as close to the end of the project as possible.</p> </li>
</ul>
</div>
-->
