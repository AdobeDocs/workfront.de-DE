---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Übersicht über die geplante Aufgabe - Abschlussdatum
description: Das geplante Abschlussdatum einer Aufgabe ist das Datum, bis zu dem die Aufgabe abgeschlossen sein soll.
author: Alina
feature: Work Management
exl-id: b0522db5-9c68-4b1a-82c8-5a9e613eb2ff
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 1%

---

# Übersicht über die geplante Aufgabe - Abschlussdatum

Das geplante Abschlussdatum einer Aufgabe ist das Datum, bis zu dem die Aufgabe abgeschlossen sein soll.

Sie können entweder das geplante Abschlussdatum einer Aufgabe angeben oder es Adobe Workfront überlassen, sie nach bestimmten Kriterien zu berechnen. 

Das geplante Abschlussdatum der Aufgaben für ein Projekt bestimmt das geplante Abschlussdatum eines Projekts, an dem das Projekt ab dem Startdatum geplant ist. Weitere Informationen zum geplanten Abschlussdatum des Projekts finden Sie unter [Festlegen des geplanten Abschlussdatums des Projekts](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>Das geplante Abschlussdatum einer Aufgabe unterscheidet sich wie folgt vom Veröffentlichungsdatum der Aufgabe oder vom geplanten Abschlussdatum der Aufgabe:
>
>* Das Datum der Veröffentlichung ist das Datum, ab dem die der Aufgabe zugewiesene Person die Aufgabe nach Schätzungen manuell abgeschlossen hat. Weitere Informationen finden Sie in den folgenden Artikeln:
>
>   * [Übersicht über das Datum des Versands ](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
>   * [Interaktionen zwischen dem Veröffentlichungsdatum und dem geplanten Abschlussdatum](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
>
>* Das geplante Abschlussdatum ist ein von Workfront berechnetes Datum und berücksichtigt Aufgabenverzögerungen, Zeitpläne der Aufgabe oder ihrer Vorgänger sowie andere Faktoren, um ein Echtzeit-Datum für den Zeitpunkt zu bestimmen, zu dem die Aufgabe realistisch abgeschlossen werden kann. Weitere Informationen finden Sie unter [Überblick über das geplante Abschlussdatum für Projekte, Aufgaben und Probleme](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>

## Manuelles Festlegen des geplanten Abschlussdatums einer Aufgabe

Sie müssen Zugriff auf Aufgaben bearbeiten und Berechtigungen verwalten für die Aufgabe haben, um das geplante Abschlussdatum der Aufgabe aktualisieren zu können.

Das Festlegen des geplanten Abschlussdatums einer Aufgabe hängt vom Typ der Aufgabenbegrenzung ab, die Sie der Aufgabe zuweisen. 

Sie können das geplante Abschlussdatum in den folgenden Bereichen von Workfront manuell festlegen:

* Im Feld &quot;Aufgabe bearbeiten&quot;beim Erstellen oder Bearbeiten einer Aufgabe. Weitere Informationen finden Sie unter [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* Im Bereich &quot;Aufgabendetails&quot;. Weitere Informationen finden Sie unter [Verwalten von Aufgabeninformationen im Übersichtsbereich &quot;Aufgabendetails&quot;](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md).
* Im Startbereich , wenn das geplante Abschlussdatum bei Ansicht einer Aufgabe angezeigt wird. Weitere Informationen finden Sie unter [Aktualisieren oder Bearbeiten eines Arbeitselements im Startbereich](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* In der Aufgabenüberschrift. Weitere Informationen finden Sie unter [Neue Objektüberschriften](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* In einer Aufgabenliste oder in einem Bericht, wenn das Feld Geplantes Abschlussdatum in der Ansicht angezeigt wird.

  Weitere Informationen finden Sie unter [Aufgaben in einer Liste bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

Sie können das geplante Abschlussdatum manuell angeben, wenn Sie eine der folgenden Aufgabenbegrenzungen auswählen: 

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Task Constraint Type</strong> </p> </th> 
   <th> <p><strong>Auswirkung einer manuellen Änderung des geplanten Abschlussdatums</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Muss beendet werden am</p> <p>Nicht später beenden als (NSBA)</p> <p>Nicht früher beenden als (NFBA)</p> </td> 
   <td> <p><span class="s1">Das geplante Startdatum wird angepasst, damit die Dauer unverändert bleibt.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Feste Daten</p> </td> 
   <td> <p>Die Dauer wird angepasst, damit das geplante Startdatum unverändert bleibt.</p> </td> 
  </tr> 
 </tbody> 
</table>

## So berechnet Workfront automatisch das geplante Abschlussdatum für eine Aufgabe

Wenn sie automatisch vom System berechnet wird, kann Folgendes das geplante Abschlussdatum einer Aufgabe beeinflussen:

* Aufgabenbeschränkung

  Weitere Informationen zu Aufgabenbegrenzungen finden Sie im Artikel [Übersicht über Aufgabenbegrenzungen](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Aufgabenverlaufsbeziehung

  Weitere Informationen zu Aufgabenvorgängen finden Sie im Artikel [Übersicht über Aufgabenvorstufen](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Abschlussdatum des Projekts, an dem das Projekt nach dem Abschlussdatum geplant ist.
* Die Zeitdauer des Primären Aufgabenempfängers.

  Wenn für den Primären Verantwortlichen für die Dauer der Aufgabe eine Zeitüberschreitung geplant ist, werden die geplanten Zeitpunkte der Aufgabe entsprechend angepasst, wenn für das Feld **Zeitlimit für Benutzer außer Kraft setzen** die Einstellung **Für die Dauer der Aufgabe festlegen** ausgewählt ist. Neue Projekte übernehmen diese Einstellung im Bereich &quot;Projekteinstellungen&quot;, Sie können die Einstellung jedoch auf Projektebene bearbeiten.

  Wenn beispielsweise eine Aufgabe mit der Begrenzung So bald wie möglich am 1. Juni beginnen und am 3. Juni abgeschlossen sein soll und der Primäre Verantwortliche den 2. Juni für die Zeitüberschreitung markiert hat, wird das geplante Abschlussdatum zum 4. Juni.

  Weitere Informationen zur Voreinstellung **Benutzerzeit von** finden Sie in den Artikeln [Konfigurieren von systemweiten Projektvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) oder [Bearbeiten von Projekten](../../../manage-work/projects/manage-projects/edit-projects.md).

* Die Zeitdauer, die mit Genehmigungseinstellungen verknüpft ist, wenn die Aufgabe mit einer Genehmigung verknüpft ist. Weitere Informationen finden Sie unter [Konfigurieren der globalen Genehmigungseinstellungen](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

Wenn das geplante Abschlussdatum automatisch eingestellt wird, wird es anhand der folgenden Berechnung ermittelt: 

```
Planned Completion Date = Planned Start Date + Duration
```

Wenn Ihre Aufgabe beispielsweise das Startdatum 16. September und die Dauer 10 Tage beträgt, ist der geplante Abschluss der 26. September.

>[!NOTE]
>
> Der Aktualisierungstyp für das Projekt muss auf Automatisch und Bei Änderung oder Automatisch eingestellt sein, damit die geplanten Stunden und die geplante Dauer automatisch angepasst werden.\
>Weitere Informationen zum Aktualisierungstyp finden Sie im Artikel [Auswählen des Aktualisierungstyps für das Projekt](../../../manage-work/projects/manage-projects/select-project-update-type.md).
