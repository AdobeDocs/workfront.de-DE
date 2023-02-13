---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Projekt-Prozent Vollständige Übersicht
description: Der Wert "Prozent abgeschlossen"eines Projekts wird basierend auf der geplanten Dauer oder den geplanten Stunden von Aufgaben im Projekt berechnet. Ihr Adobe Workfront-Administrator oder ein Gruppenadministrator definiert, welcher Wert bei der Berechnung des Prozentsatzes berücksichtigt wird, der in Ihrem System abgeschlossen ist, wenn er Informationen im Bereich Projekteinstellungen konfiguriert. Informationen zum Konfigurieren von Projektvoreinstellungen finden Sie unter Systemweite Projekteigenschaften konfigurieren .
author: Alina
feature: Work Management
exl-id: d2395569-9fe5-42e7-a392-cff49eb519d9
source-git-commit: 31533bd7ee1890a8343d32770d623d5d9a6007d2
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 0%

---

# Projekt-Prozent Vollständige Übersicht

Der Wert &quot;Prozent abgeschlossen&quot;eines Projekts wird basierend auf der Dauer oder den geplanten Stunden von Aufgaben im Projekt berechnet. Ihr Adobe Workfront-Administrator oder ein Gruppenadministrator definiert, welcher Wert bei der Berechnung des Prozentsatzes berücksichtigt wird, der in Ihrem System abgeschlossen ist, wenn er Informationen im Bereich Projekteinstellungen konfiguriert.

Informationen zum Konfigurieren von Projektvoreinstellungen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Der Prozentsatz der Abschlüsse einer übergeordneten Aufgabe basiert auf der Dauer oder den geplanten Stunden jeder ihrer Unteraufgaben.

Gleichermaßen basiert der Prozentsatz des Abschlusses eines Projekts auf den Dauer oder geplanten Stunden jeder Hauptaufgabe im Projekt.

Die Hauptaufgaben sind die übergeordneten Aufgaben und die eigenständigen Aufgaben, die keine untergeordneten Elemente haben.

>[!TIP]
>
>Hauptaufgaben sind in einem Projektplan nicht eingerückt.

## Berechnung der vollständigen Prozent durch Workfront

* [Aktualisierung des Prozentsatzes für den Abschluss einer Aufgabe](#update-the-percent-complete-on-a-task)
* [Berechnung des Prozentsatzes der Abschlüsse einer übergeordneten Aufgabe durch Workfront](#how-workfront-calculates-percent-complete-on-a-parent-task)
* [Berechnung des Prozentsatzes der Abschlüsse eines Projekts durch Workfront](#how-workfront-calculates-percent-complete-on-a-project)

### Aktualisierung des Prozentsatzes für den Abschluss einer Aufgabe {#update-the-percent-complete-on-a-task}

Sie können den prozentualen Abschluss einer Aufgabe manuell ändern. Dies ist keine Berechnung.

Workfront verwendet den prozentualen Abschluss einer einzelnen Aufgabe, um den prozentualen Abschluss der übergeordneten Aufgabe oder den prozentualen Abschluss des Projekts zu berechnen.

Informationen zum Aktualisieren des Prozentsatzes der Fertigstellung einer Aufgabe finden Sie unter [Prozentsatz für Abgeschlossene Aufgaben anzeigen und aktualisieren](../../../manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md).

### Berechnung des Prozentsatzes der Abschlüsse einer übergeordneten Aufgabe durch Workfront {#how-workfront-calculates-percent-complete-on-a-parent-task}

Je nachdem, was Ihr Workfront- oder Gruppenadministrator in den Projekteigenschaften auf System- oder Gruppenebene ausgewählt hat, wird der Prozentsatz, der für eine übergeordnete Aufgabe abgeschlossen ist, entweder anhand der Dauer oder der geplanten Dauer berechnet.

Betrachten Sie die folgenden Szenarien:

* Wenn das System den Prozentsatz der Vollständigkeit anhand der geplanten Stunden berechnet, wird der Prozentsatz der Fertigstellung der übergeordneten Aufgabe anhand der folgenden Formel berechnet:

   `Parent Task Percent Complete = (((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of Parent)*100`

   Die Gesamtanzahl der geplanten Stunden der Eltern entspricht der Summe aller geplanten Stunden der einzelnen Kinder.

   ![](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

* Wenn das System den Prozentsatz der Fertigstellung anhand der Dauer berechnet, wird der Prozentsatz der Fertigstellung der übergeordneten Aufgabe anhand der folgenden Formel berechnet:

   `Parent Task Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/ Total Duration of Parent)*100`

   ![](assets/project-with-tasks-percent-complete-duration-calculation.png)

   >[!IMPORTANT]
   >
   >Die Gesamtdauer der übergeordneten Aufgabe entspricht der Gesamtdauer aller untergeordneten Aufgaben. Beispielsweise hat eine übergeordnete Aufgabe mit zwei untergeordneten Elementen mit einer Dauer von 1 Tag und 2 Tagen eine Gesamtdauer von 3 Tagen, selbst wenn die beiden untergeordneten Elemente am selben Tag beginnen können.


### Berechnung des Prozentsatzes der Abschlüsse eines Projekts durch Workfront {#how-workfront-calculates-percent-complete-on-a-project}

Je nachdem, was Ihr Workfront- oder Gruppenadministrator in den Projekteinstellungen auf System- oder Gruppenebene ausgewählt hat, wird der Prozentsatz, der für ein Projekt abgeschlossen ist, entweder anhand der Dauer oder der geplanten Stunden der Hauptaufgaben des Projekts berechnet.

* Wenn das System den Prozentsatz der Fertigstellung anhand geplanter Stunden berechnet, wird der Prozentsatz der Fertigstellung des Projekts anhand der folgenden Formel berechnet:

   `Project Percent Complete =(((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of the Project)*100`

   Die Gesamtdauer der geplanten Projektstunden ist die Summe der geplanten Stunden aller Hauptaufgaben des Projekts.

   ![](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

   >[!NOTE]
   >
   >Aufgabe 1 oder Aufgabe 2 kann nur übergeordnete Aufgaben oder eigenständige Aufgaben sein. Die Aufgaben Geplante Stunden und Prozent Abgeschlossen der untergeordneten Elemente werden in dieser Berechnung nicht verwendet.

* Wenn das System den Prozentsatz der Fertigstellung anhand der Dauer berechnet, wird der Prozentsatz der Fertigstellung des Projekts anhand der folgenden Formel berechnet:

   `Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

   >[!IMPORTANT]
   >
   >Die Dauer des Projekts entspricht der Gesamtdauer aller Hauptaufgaben, für die ein Prozentsatz der Fertigstellung angezeigt wird. Beispielsweise wird für ein Projekt mit einer eigenständigen Aufgabe mit einer Dauer von 2 Tagen und einer übergeordneten Aufgabe mit einer Dauer von 5 Tagen, an denen die Arbeit abgeschlossen wurde, eine Gesamtdauer von 7 Tagen festgelegt, selbst wenn die beiden Aufgaben am selben Tag beginnen können.

   ![](assets/project-with-tasks-percent-complete-duration-calculation.png)

   >[!NOTE]
   >
   >Aufgabe 1 oder Aufgabe 2 kann nur übergeordnete Aufgaben oder eigenständige Aufgaben sein. Die Aufgaben &quot;Dauer&quot;und &quot;Prozent abgeschlossen&quot;werden in dieser Berechnung nicht verwendet.

## Beispiel für den Abschluss eines Projekts mit einer Projektdauer

Wenn Sie die Dauer der Aufgaben zur Berechnung des Prozentsatzes des Projektabschlusses verwenden, beachten Sie das folgende Beispiel:

![](assets/project-with-tasks-percent-complete-duration-calculation.png)

Die folgenden Informationen werden verwendet, um den Prozentsatz des Abschlusses des Projekts zu berechnen

* Der prozentuale Abschluss der eigenständigen Aufgabe (Aufgabe 1 - 20%)
* Der prozentuale Abschluss der übergeordneten Aufgabe (Aufgabe 2 - 25%)
* Die Dauer von Aufgabe 1 (5 Tage)
* Die Dauer von Aufgabe 2 (2 Tage)
* Dauer des Projekts (7 Tage)


So berechnen Sie den Prozentsatz der Projektabwicklung anhand der Dauer:

`Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

Oder

`(((5*0.2)+(2*0.25))/7)*100= 21.43%`


<!--drafted, this was the old example:

When using the Planned Duration of the tasks to calculate the percent complete of a project, consider the following example:

percent_complete_on_project_example.png

Only the parent task (Task 1) and the standalone task (Task 8) are used to calculate the percent complete of the project.

The secondary parents of Task 1 are used to calculate the percent complete of the main parent (Task 1).

To calculate the percent complete of the main parent (Task 1), first calculate the percent complete of its secondary parents:

Task 5 Percent Complete = ((14 * 0.75 + 12 * 0.25)/(12 + 14))*100 = 51.92%

Task 2 Percent Complete = ((5 * 0.7 + 2 * 0.5)/(5 + 2))*100 = 64.29 %

Then, to calculate the percent complete of the main parent (Task 1), use the following formula:

Task 1 Percent Complete =((56 * 0.5192 + 7 * 0.6429)/63)*100 = 53.29%

To calculate the percent complete of the project, you will need to have the following numbers ready:

Task 1 Duration (63 hours) and Percent Complete (53.29%)
Task 8 Duration (100 hours) and Percent Complete (4%)
Now, to calculate the percent complete of the project, use the following formula:

Project Percent Complete =((100 * 0.04 + 63 * 0.5329))/163)*100 = 23.05%
-->