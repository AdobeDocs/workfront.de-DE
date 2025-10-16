---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Aufgabenbeschränkung - Übersicht: so bald wie möglich'
description: So bald wie möglich ist eine Aufgabenbeschränkung, die die Startzeit der Aufgabe so nah wie möglich am Anfang des Projekts platziert.
author: Alina
feature: Work Management
exl-id: 9cb232fe-bc74-4433-afac-88be69514c88
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Aufgabenbeschränkung - Übersicht: So bald wie möglich

So bald wie möglich ist eine Aufgabenbeschränkung, die die Startzeit der Aufgabe so nah wie möglich am Anfang des Projekts platziert.

## Überlegungen zur Verwendung der Einschränkung So bald wie möglich

* So bald wie möglich ist die Standardeinschränkung, wenn ein Projekt den Planungsmodus vom Startdatum aus verwendet und wenn das standardmäßige Startdatum des Systems für eine neue Aufgabe auf Basierend auf dem geplanten Datum des Projekts festgelegt ist.

* Wenn ein Projekt den Zeitplanmodus vom Startdatum aus verwendet und das standardmäßige Startdatum des Systems oder der Gruppe für eine neue Aufgabe auf Heute festgelegt ist, lautet die standardmäßige Vorgangseinschränkung „Start erst nach“.

  Informationen dazu, wo die Standardeinschränkung für eine neue Aufgabe festgelegt werden soll, finden Sie [Konfigurieren von systemweiten Aufgaben- und Problemeinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Informationen zum Aktualisieren der Aufgabenbeschränkung für eine Aufgabe finden Sie unter [Aktualisieren der Aufgabenbeschränkung einer Aufgabe](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Soon As Possible: </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>As Soon As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Die Differenz zwischen der frühesten verfügbaren Zeit und so bald wie möglich

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])&nbsp;</p>
-->

Die frühestmögliche verfügbare Zeitbeschränkung unterscheidet sich von der so bald wie möglich -Beschränkung, wenn alle folgenden Kriterien vorhanden sind:

* Das Projekt ist für den Abschluss geplant.
* Aufgaben im Projekt haben eine Vorgängerbeziehung.
* Die Vorgängeraufgabe weist eine flexible Aufgabenbeschränkung auf.

In dieser Situation:

* **Früheste verfügbare Zeit** Bei Verwendung der Zeitbeschränkung „Früheste verfügbare Zeit“ für die Nachfolgeaufgabe wird der flexiblen Zeitbeschränkung des Vorgängers Priorität eingeräumt.

  Angenommen, Aufgabe A ist ein Vorgänger von Aufgabe B. Aufgabe B hat die frühestmögliche verfügbare Zeitbeschränkung und Aufgabe A hat die so spät wie möglich-Beschränkung. In diesem Fall wird die Aufgabe so nah wie möglich am Abschluss des Projekts geplant.

* **So bald wie möglich** In diesem Szenario wird bei Verwendung der Einschränkung So bald wie möglich für die Nachfolgeaufgabe die Priorität der Nachfolgeaufgabe zugewiesen.

  Angenommen, Aufgabe A ist ein Vorgänger von Aufgabe B. Aufgabe B hat die Einschränkung So bald wie möglich und Aufgabe A hat die Einschränkung So spät wie möglich. In diesem Fall wird die Aufgabe so nah wie möglich am Beginn des Projekts geplant.
