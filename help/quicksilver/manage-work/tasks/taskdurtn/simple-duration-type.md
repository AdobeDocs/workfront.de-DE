---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Übersicht über den Dauertyp: Einfach'
description: Der einfache Dauertyp ist ein Dauertyp, den Sie für eine Aufgabe in Adobe Workfront festlegen können. Allgemeine Informationen zu den Dauertypen in Workfront finden Sie unter Übersicht über die Aufgabendauer und den Dauertyp.
author: Alina
feature: Work Management
exl-id: 9bb472db-1448-467e-93ca-611453e1c00a
source-git-commit: 1efd7c0270fe1396345cfa6e5499e8f998297d61
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# Übersicht über den Dauertyp: Einfach

Der einfache Dauertyp ist ein Dauertyp, den Sie für eine Aufgabe in Adobe Workfront festlegen können. Allgemeine Informationen zu den Dauertypen in Workfront finden Sie unter [Übersicht über die Aufgabendauer und den Dauertyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Übersicht über den einfachen Dauertyp

Ihr Workfront-Administrator oder ein Gruppenadministrator kann den Standarddauertyp Ihres Systems oder Ihrer Gruppe als „Einfach“ festlegen. In diesem Fall werden alle neuen Aufgaben mit diesem Dauertyp erstellt. Informationen zum Ändern der Voreinstellungen für Aufgaben und Probleme als Teil der Voreinstellungen für Projekte auf Systemebene oder Gruppenebene finden Sie unter [Konfigurieren von systemweiten Voreinstellungen für Aufgaben und Probleme](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Wenn eine Aufgabe den Dauertyp „Einfach“ hat, treten folgende Dinge auf:

* Projektmanager können die Dauer und die geplanten Stunden einer Aufgabe ändern, wenn sie festlegen, wie diese Stunden auf die Beauftragten verteilt werden sollen.

  Weitere Informationen finden Sie unter [Aktualisieren der geplanten Stunden und der Dauer einer Aufgabe mit einem einfachen Dauertyp](../../../manage-work/tasks/taskdurtn/update-planned-hours-duration-for-simple-duration-task.md).

  >[!IMPORTANT]
  >
  >Wenn Sie eine Aufgabe zum ersten Mal erstellen, ihr den Typ Einfache Dauer zuweisen und keine Dauer angeben, berechnet Workfront die Dauer der Aufgabe auf der Basis der für die Aufgabe angegebenen geplanten Stunden. Wenn Sie die Dauer einer Aufgabe vom Typ Einfache Dauer manuell ändern, gleicht Workfront die geplanten Stunden nicht mehr mit der Dauer ab, da davon ausgegangen wird, dass Sie sie manuell selbst definieren möchten.
  >
  >Workfront berechnet die Dauer von Aufgaben, deren Dauer nicht manuell mithilfe der folgenden Formel geändert wurde:
  >
  > `Task Duration = Task Planned Hours / Typical hours per work day`
  >
  >Ihr Workfront-Administrator definiert die `Typical hours per work day` im Bereich Projektvoreinstellungen der Instanzeinrichtung.

* Der Zuordnungsprozentsatz ist ausgeblendet und stattdessen können Zuordnungsstunden bearbeitet werden.
* Für alle neuen Kunden ist der Dauertyp auf Systemebene auf „Einfach“ festgelegt.

## Ändern des Dauertyps einer Aufgabe in „Einfach“

Informationen zum Ändern des Dauertyps einer Aufgabe finden Sie unter [Aktualisieren des Dauertyps einer Aufgabe](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

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
