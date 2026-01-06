---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Übersicht über das geplante Startdatum der Aufgabe
description: Das geplante Startdatum einer Aufgabe ist das Datum, an dem Sie als Ersteller der Aufgabe entscheiden, dass die Arbeit an der Aufgabe beginnen soll. Die geplanten Aufgabentermine beeinflussen die Termine und die Timeline im Projekt. Informationen zum geplanten Startdatum des Projekts finden Sie in der Übersicht über das geplante Startdatum des Projekts.
author: Alina
feature: Work Management
exl-id: 2ac6327f-4a13-4fb8-ad8e-03d032221483
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 2%

---

# Übersicht über das geplante Startdatum der Aufgabe

<!-- Audited: 6/2025 -->

Das geplante Startdatum einer Aufgabe ist das Datum, an dem Sie als Ersteller der Aufgabe entscheiden, dass die Arbeit an der Aufgabe beginnen soll. Die geplanten Aufgabentermine beeinflussen die Termine und die Timeline im Projekt. Informationen zum geplanten Startdatum des Projekts finden Sie unter [Übersicht über das geplante Startdatum des Projekts](../../../manage-work/projects/planning-a-project/project-planned-start-date.md).

## Das geplante Startdatum einer Aufgabe

Sie können entweder das geplante Startdatum der Aufgabe angeben oder es Adobe Workfront überlassen, diese anhand bestimmter Kriterien zu berechnen.

* [Legen Sie das geplante Startdatum einer Aufgabe manuell fest](#manually-set-the-planned-start-date-of-a-task)
* [Berechnen des geplanten Startdatums einer Aufgabe](#how-the-planned-start-date-is-calculated-for-a-task)

### Manuelles Festlegen des geplanten Startdatums einer Aufgabe {#manually-set-the-planned-start-date-of-a-task}

Das Festlegen des geplanten Startdatums einer Aufgabe hängt von der Art der Aufgabenbeschränkung ab, die Sie der Aufgabe zuweisen.

Sie können das geplante Startdatum beim Erstellen einer Aufgabe manuell festlegen. Weitere Informationen finden Sie unter [Erstellen von Aufgaben in einem Projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Sie können das geplante Startdatum manuell angeben, wenn Sie eine der folgenden Aufgabeneinschränkungen auswählen:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Aufgabenbeschränkungstyp</strong> </p> </th> 
   <th> <p><strong>Auswirkung einer manuellen Änderung des geplanten Abschlussdatums</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Muss beginnen am</p> <p>Nicht früher anfangen als</p> <p>Nicht später anfangen als</p> </td> 
   <td> <p><span class="s1">Das geplante Abschlussdatum wird angepasst, um die Dauer beizubehalten.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Feste Daten</p> </td> 
   <td> <p>Die Dauer wird angepasst, um das geplante Abschlussdatum unverändert zu lassen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Berechnen des geplanten Startdatums einer Aufgabe {#how-the-planned-start-date-is-calculated-for-a-task}

Wenn es automatisch vom System berechnet wird, kann Folgendes das geplante Startdatum einer Aufgabe beeinflussen:

* Die Einstellung „Startdatum“ im Bereich „Aufgaben und Probleme“ im Setup

  Der Workfront- oder Gruppen-Administrator kann bestimmen, ob eine neue Aufgabe am gleichen Datum wie das geplante Startdatum des Projekts oder an dem Tag beginnt, an dem Sie die Aufgabe erstellen.

  Informationen zu den Voreinstellungen für Aufgaben und Probleme finden [ unter „Systemweite Voreinstellungen für Aufgaben und Probleme konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Aufgabenbeschränkung

  Weitere Informationen zu Aufgabenbeschränkungen finden Sie unter [Übersicht über Aufgabenbeschränkungen](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Vorgängerbeziehung für Aufgabe

  Weitere Informationen zu Aufgabenvorgängen finden Sie unter [Übersicht über Aufgabenvorgänge](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Projektstartdatum, wenn das Projekt ab dem Startdatum geplant wird.
* Die Ausfallzeit des Primären Zugewiesenen der Aufgabe.

  Wenn für den Primären Verantwortlichen Ausfallzeiten während der Aufgabendauer geplant sind, werden die geplanten Termine der Aufgabe entsprechend angepasst, wenn die Einstellung „Benutzer-Ausfallzeit berücksichtigen“ in der Aufgabendauer für das Feld „Benutzer-Ausfallzeit“ ausgewählt ist. Neue Projekte übernehmen diese Einstellung aus dem Bereich Projektvoreinstellungen, Sie können die Einstellung jedoch auf Projektebene bearbeiten.

  Wenn beispielsweise eine Aufgabe mit der Einschränkung So bald wie möglich am 1. Juni beginnen und am 3. Juni abgeschlossen werden soll und der Primäre Verantwortliche für die Ausfallzeit den 1. Juni markiert hat, wird das geplante Startdatum der Aufgabe zum 2. Juni.

  Weitere Informationen zu den Urlaubseinstellungen für Benutzer finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) oder [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

Wenn es automatisch festgelegt wird, wird das geplante Startdatum anhand der folgenden Berechnung bestimmt:

```
Planned Start Date = Planned Completion Date - Task Duration
```

Wenn Ihre Aufgabe beispielsweise ein Abschlussdatum vom 16. September und eine Dauer von 10 Tagen hat, ist das geplante Startdatum der 6. September.

>[!NOTE]
>
> Der Aktualisierungstyp für das Projekt muss ebenfalls auf „Automatisch“ und „Bei Änderung“ oder „Automatisch“ gesetzt werden, damit die geplanten Stunden und die Dauer automatisch angepasst werden.\
>Weitere Informationen zum Aktualisierungstyp finden Sie unter [Auswahl des Projektaktualisierungstyps](../../../manage-work/projects/manage-projects/select-project-update-type.md).
