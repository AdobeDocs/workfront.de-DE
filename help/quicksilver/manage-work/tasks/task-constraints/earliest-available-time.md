---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Übersicht über die Aufgabenbeschränkung: früheste verfügbare Zeit'
description: Die früheste verfügbare Zeit ist eine Aufgabenbeschränkung, die eine Aufgabe so plant, dass sie zum frühestmöglichen verfügbaren Zeitpunkt beginnt, nachdem alle Vorgängerbeziehungen berücksichtigt wurden.
author: Alina
feature: Work Management
exl-id: 9c01e4bd-c6ca-4540-a0f1-ecdd44df84e0
TQID: https://experienceleague.adobe.com/htQAqPWSYcdft3g3RDQuRu3VdmxmvVQt2EFrvFJsRU4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 299
ht-degree: 2%

---

# Überblick über Aufgabenbeschränkungen: Frühestmögliche Zeit

Die früheste verfügbare Zeit ist eine Aufgabenbeschränkung, die eine Aufgabe so plant, dass sie zum frühestmöglichen verfügbaren Zeitpunkt beginnt, nachdem alle Vorgängerbeziehungen berücksichtigt wurden.

Informationen zum Aktualisieren der Aufgabenbeschränkung für eine Aufgabe finden Sie unter [Aktualisieren der Aufgabenbeschränkung einer Aufgabe](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

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

## Die Differenz zwischen der frühesten verfügbaren Zeit und so bald wie möglich

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])</p>
-->

Die frühestmögliche verfügbare Zeitbeschränkung unterscheidet sich von der so bald wie möglich -Beschränkung, wenn alle folgenden Kriterien vorhanden sind:

* Das Projekt ist für den Abschluss geplant
* Aufgaben im Projekt haben eine Vorgängerbeziehung
* Die Vorgängeraufgabe weist eine flexible Aufgabenbeschränkung auf

In dieser Situation:

* **Früheste verfügbare Zeit** Bei Verwendung der Zeitbeschränkung „Früheste verfügbare Zeit“ für die Nachfolgeaufgabe wird der flexiblen Zeitbeschränkung des Vorgängers Priorität eingeräumt.

  **BEISPIEL**

  Aufgabe A ist ein Vorgänger von Aufgabe B. Aufgabe B hat die frühestmögliche verfügbare Zeitbeschränkung und Aufgabe A hat die so spät wie möglich-Beschränkung. In diesem Fall wird Aufgabe B so nah wie möglich am Abschluss des Projekts geplant.

  ![Früheste verfügbare Zeitbeschränkung, wenn die Termine der Aufgabe nahe am Abschlussdatum des Projekts liegen](assets/earliest-available-constraint-dates-closer-to-project-completion-350x137.png)

* **So bald wie möglich** In diesem Szenario wird bei Verwendung der Einschränkung So bald wie möglich für die Nachfolgeaufgabe die Priorität der Nachfolgeaufgabe zugewiesen.

  **BEISPIEL**

  Aufgabe A ist ein Vorgänger von Aufgabe B. Aufgabe B unterliegt der Beschränkung „So bald wie möglich“ und Aufgabe A der Beschränkung „So spät wie möglich“. In diesem Fall wird Aufgabe B so nahe wie möglich am Beginn des Projekts geplant.

  ![Sobald wie möglich Einschränkung, wenn die Termine der Aufgabe nahe am Startdatum des Projekts liegen](assets/as-soon-as-possible-dates-closer-to-project-start-350x126.png)
