---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Duration Type overview: Simple'
description: Der Typ Einfache Dauer ist eine Dauer, die Sie für eine Aufgabe in Adobe Workfront festlegen können. Allgemeine Informationen zu den Durationstypen in Workfront finden Sie unter Übersicht über die Aufgabendauer und -dauer.
author: Alina
feature: Work Management
exl-id: 9bb472db-1448-467e-93ca-611453e1c00a
source-git-commit: 1efd7c0270fe1396345cfa6e5499e8f998297d61
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# Übersicht über den Dauer-Typ: Einfach

Der Typ Einfache Dauer ist eine Dauer, die Sie für eine Aufgabe in Adobe Workfront festlegen können. Allgemeine Informationen zu den Durationstypen in Workfront finden Sie unter [Übersicht über Aufgabendauer und -dauer](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Übersicht über den Typ der einfachen Dauer

Ihr Workfront- oder Gruppenadministrator kann den Standardtyp für die Dauer Ihres Systems oder Ihrer Gruppe auf &quot;Einfach&quot;festlegen. In diesem Fall werden alle neuen Aufgaben mit diesem Typ Dauer erstellt. Informationen zum Ändern der Aufgaben- und Problemvoreinstellungen im Rahmen Ihrer Projekteigenschaften auf System- oder Gruppenebene finden Sie unter [Systemweite Aufgaben- und Problemeinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Folgendes tritt auf, wenn eine Aufgabe den Typ Einfache Dauer aufweist:

* Projektmanager können die Dauer und die geplanten Stunden einer Aufgabe ändern, wenn sie ändern, wie diese Stunden auf die Bevollmächtigten verteilt werden sollen.

  Weitere Informationen finden Sie unter [Aktualisieren der geplanten Stunden und Dauer einer Aufgabe mit dem einfachen Typ Dauer](../../../manage-work/tasks/taskdurtn/update-planned-hours-duration-for-simple-duration-task.md).

  >[!IMPORTANT]
  >
  >Wenn Sie eine Aufgabe zum ersten Mal erstellen und ihr den Typ Einfache Dauer zuweisen und keine Dauer angeben, berechnet Workfront die Dauer der Aufgabe basierend auf der Anzahl der geplanten Stunden, die Sie für die Aufgabe angeben. Wenn Sie die Dauer einer Aufgabe mit einfacher Dauer manuell ändern, stoppt Workfront die Zuordnung der geplanten Stunden zur Dauer, da davon ausgegangen wird, dass Sie sie manuell selbst definieren möchten.
  >
  >Workfront berechnet die Dauer von Aufgaben, deren Dauer nicht manuell geändert wurde, nach folgender Formel:
  >
  > `Task Duration = Task Planned Hours / Typical hours per work day`
  >
  >Ihr Workfront-Administrator definiert `Typical hours per work day` im Bereich Projektvoreinstellungen im Setup Ihrer Instanz.

* Der Zuordnungsprozentsatz ist ausgeblendet und die Zuordnungszeiten können stattdessen bearbeitet werden.
* Bei allen neuen Kunden ist der Dauer-Typ auf Systemebene auf &quot;Einfach&quot;eingestellt.

## Ändern Sie den Aufgabentyp in Einfach .

Informationen zum Ändern der Dauer einer Aufgabe finden Sie unter [Aktualisierung des Zeitdauer-Typs einer Aufgabe](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Simple</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong><strong>.</strong></li>
</ol>
-->
