---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Aufgabenbeschränkung - Übersicht: So spät wie möglich'
description: So spät wie möglich (ALAP) ist eine Adobe Workfront-Aufgabenbeschränkung, die die Abschlusszeit der Aufgabe so nah wie möglich am Ende des Projekts platziert.
author: Alina
feature: Work Management
exl-id: 475427d0-020b-4851-a614-c9931659e07d
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# Aufgabenbeschränkung - Übersicht: So spät wie möglich

So spät wie möglich (ALAP) ist eine Adobe Workfront-Aufgabenbeschränkung, die die Abschlusszeit der Aufgabe so nah wie möglich am Ende des Projekts platziert.

Die Verwendung dieser Einschränkung kann dazu führen, dass Vorgänger oder abhängige Aufgaben neu geplant werden.

Weitere Informationen zu Vorgängerbeziehungen finden Sie unter [Verwenden von Aufgabenvorgängern: Artikelindex](../../../manage-work/tasks/use-prdcssrs/use-task-predecessors.md).

So spät wie möglich ist die Standardbedingung, wenn für ein Projekt der Planungsmodus „Abschlussdatum“ verwendet wird und der System- oder Gruppenstandard für das Startdatum einer Aufgabe auf dem geplanten Projektdatum basiert.

Informationen dazu, wo die Standardeinschränkung für eine neue Aufgabe festgelegt werden soll, finden Sie [Konfigurieren von systemweiten Aufgaben- und Problemeinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Informationen zum Aktualisieren der Aufgabenbeschränkung für eine Aufgabe finden Sie unter [Aktualisieren der Aufgabenbeschränkung einer Aufgabe](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the As Late As Possible Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Late As Possible: </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>As Late As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Die Differenz zwischen der neuesten verfügbaren Zeit und so spät wie möglich

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Latest Available Time"] - inserted a snippet for both articles (Alina)) </p>
-->

Die Zeitbeschränkung „Zuletzt verfügbar“ unterscheidet sich von der Beschränkung „So spät wie möglich“, wenn die folgenden Kriterien vorliegen:

* Das Projekt ist ab dem Startdatum geplant
* Aufgaben im Projekt haben eine Vorgängerbeziehung
* Die Nachfolgeaufgabe weist eine flexible Aufgabenbeschränkung auf

In dieser Situation:

* **Letzte verfügbare Zeit**: Bei Verwendung der Zeitbeschränkung „Letzte verfügbare Zeit“ für die Vorgängeraufgabe hat die flexible Beschränkung des Nachfolgers Priorität.

  **Beispiel:** Zum Beispiel ist Aufgabe A ein Vorgänger von Aufgabe B. Aufgabe A hat die neueste verfügbare Zeitbeschränkung und Aufgabe B hat die so bald wie möglich-Beschränkung. In diesem Fall wird Aufgabe A so nahe wie möglich am Beginn des Projekts geplant.

  ![Letzte verfügbare Zeitaufgabenbeschränkung](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **So spät wie möglich:** In diesem Szenario wird bei Verwendung der Einschränkung So spät wie möglich für die Vorgängeraufgabe die Priorität der Vorgängeraufgabe zugewiesen.

  **Beispiel:** Zum Beispiel ist Aufgabe A ein Vorgänger von Aufgabe B. Aufgabe A hat die Einschränkung So spät wie möglich und Aufgabe B hat die Einschränkung So bald wie möglich. In diesem Fall wird Aufgabe A so nah wie möglich am Ende des Projekts geplant.

  ![So spät wie möglich Aufgabenbeschränkung in einer Aufgabenliste](assets/as-late-as-possible-task-constraint-in-task-list-350x104.png)



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
<li> <p><strong>Latest Available Time:</strong> Using the Latest Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest Available Time constraint and Task A has the As Soon As Possible constraint. In this situation, the task is scheduled as close to the start of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late As Possible constraint and Task A has the As Soon As Possible constraint. In this situation, the task is scheduled as close to the end of the project as possible.</p> </li>
</ul>
</div>
-->
