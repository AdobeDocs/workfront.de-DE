---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: "Task Constraint - Übersicht: Frühzeitige verfügbare Zeit"
description: Die früheste verfügbare Zeit ist eine Aufgabenbegrenzung, mit der eine Aufgabe so geplant wird, dass sie zum frühestmöglichen Zeitpunkt nach Berücksichtigung von Vorgängerbeziehungen beginnt.
author: Alina
feature: Work Management
exl-id: 9c01e4bd-c6ca-4540-a0f1-ecdd44df84e0
source-git-commit: 18f26f976a47af003817f2f82f8550bdfbc0ab90
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# Übersicht über Aufgabenbeschränkungen: Frühzeitige Verfügbarkeitszeit

Die früheste verfügbare Zeit ist eine Aufgabenbegrenzung, mit der eine Aufgabe so geplant wird, dass sie zum frühestmöglichen Zeitpunkt nach Berücksichtigung von Vorgängerbeziehungen beginnt.

Informationen zum Aktualisieren der Aufgabenbegrenzung für eine Aufgabe finden Sie unter [Aktualisieren der Aufgabenbegrenzung einer Aufgabe](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above) </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To update the Task Constraint to Earliest Available Time:</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Go to a task whose constraint you want to modify. </li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Edit Task</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Select <strong>Earliest Available Time</strong>.</p>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save Changes</strong>.</li>
   -->

## Differenz zwischen der frühesten verfügbaren Zeit und so bald wie möglich

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])</p>
-->

Die früheste Zeitbeschränkung unterscheidet sich von der so bald wie möglich geltenden Beschränkung, wenn alle folgenden Kriterien vorhanden sind:

* Das Projekt wird nach Abschluss geplant
* Aufgaben im Projekt haben eine Vorgängerbeziehung
* Die Vorgängeraufgabe hat eine flexible Aufgabenbegrenzung

In diesem Fall:

* **Früheste verfügbare Zeit:** Die Verwendung der frühesten Zeitbeschränkung für die Nachfolgeaufgabe gibt der flexiblen Beschränkung des Vorgängers Priorität.

   **BEISPIEL**

   Aufgabe A ist ein Vorgänger von Aufgabe B. Aufgabe B hat die früheste verfügbare Zeitbeschränkung und Aufgabe A hat die so spät wie möglich Beschränkung. In diesem Fall wird die Aufgabe B so kurz wie möglich am Ende des Projekts geplant.

   ![Die früheste Zeitbeschränkung für &quot;Verfügbare Zeit&quot;, wenn die Aufgabe die Daten nahe dem Abschlussdatum des Projekts hat](assets/earliest-available-constraint-dates-closer-to-project-completion-350x137.png)

* **So bald wie möglich:** In diesem Szenario räumt die Verwendung der Beschränkung So bald wie möglich für die Nachfolgeaufgabe der Nachfolgeaufgabe die Priorität ein.

   **BEISPIEL**

   Aufgabe A ist ein Vorgänger von Aufgabe B. Aufgabe B hat so bald wie möglich die Beschränkung und Aufgabe A hat die so spät wie möglich Beschränkung. In diesem Fall wird Aufgabe B so nahe wie möglich am Projektstart geplant.

   ![Sofort wie möglich Beschränkung, wenn die Aufgabe die Daten nahe dem Startdatum des Projekts hat](assets/as-soon-as-possible-dates-closer-to-project-start-350x126.png)
