---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Übersicht über die Aufgabenbeschränkung: Letzte verfügbare Zeit'
description: Latest Available Time (LAT) ist eine Art von Aufgabenbeschränkung in Adobe Workfront.
author: Alina
feature: Work Management
exl-id: acf55004-9424-4e24-9ff5-90f6fd7f72a6
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---

# Übersicht über die Aufgabenbeschränkung: Letzte verfügbare Zeit

Latest Available Time (LAT) ist eine Art von Aufgabenbeschränkung in Adobe Workfront.

## Letzte verfügbare Zeitaufgabenbeschränkung verwenden

Sie können die letzte Einschränkung verwenden, wenn Sie einen Vorgang so planen möchten, dass er zum spätestens verfügbaren Zeitpunkt beginnt, nachdem Sie Vorgänger-Nachfolger-Beziehungen im Projekt berücksichtigt haben.

Diese Einschränkung unterscheidet sich von So bald wie möglich insofern, als sie keine Neuplanung von Vorgängern oder Nachfolgern erzwingt. Stattdessen wirkt sich dies nur auf den Zeitplan der Aufgabe aus, mit der es verknüpft ist, und setzt sie auf die neueste verfügbare Zeit, basierend auf ihrer Beziehung zu anderen Aufgaben.

Informationen zum Aktualisieren der Aufgabenbeschränkung für eine Aufgabe finden Sie unter [Aktualisieren der Aufgabenbeschränkung einer Aufgabe](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

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

## Die Differenz zwischen der neuesten verfügbaren Zeit und so spät wie möglich

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "As Late As Possible"] - inserted snippet in both (Alina)) </p>
-->

Die Zeitbeschränkung „Zuletzt verfügbar“ unterscheidet sich von der Beschränkung „So spät wie möglich“, wenn die folgenden Kriterien vorliegen:

* Das Projekt ist ab dem Startdatum geplant
* Aufgaben im Projekt haben eine Vorgängerbeziehung
* Die Nachfolgeaufgabe weist eine flexible Aufgabenbeschränkung auf

In dieser Situation:

* **Letzte verfügbare Zeit**: Bei Verwendung der Zeitbeschränkung „Letzte verfügbare Zeit“ für die Vorgängeraufgabe hat die flexible Beschränkung des Nachfolgers Priorität.

  **Beispiel:** Zum Beispiel ist Aufgabe A ein Vorgänger von Aufgabe B. Aufgabe A hat die neueste verfügbare Zeitbeschränkung und Aufgabe B hat die so bald wie möglich-Beschränkung. In diesem Fall wird Aufgabe A so nahe wie möglich am Beginn des Projekts geplant.

  ![Letzte verfügbare Zeitaufgabenbeschränkung in der Aufgabenliste](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **So spät wie möglich:** In diesem Szenario wird bei Verwendung der Einschränkung So spät wie möglich für die Vorgängeraufgabe die Priorität der Vorgängeraufgabe zugewiesen.

  **Beispiel:** Zum Beispiel ist Aufgabe A ein Vorgänger von Aufgabe B. Aufgabe A hat die Einschränkung So spät wie möglich und Aufgabe B hat die Einschränkung So bald wie möglich. In diesem Fall wird Aufgabe A so nah wie möglich am Ende des Projekts geplant.

  ![So spät wie möglich Aufgabenbeschränkung in Aufgabenliste](assets/as-late-as-possible-task-constraint-in-task-list-350x104.png)

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
