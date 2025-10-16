---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Übersicht über das geplante Abschlussdatum der Aufgabe
description: Das geplante Abschlussdatum einer Aufgabe ist das Datum, bis zu dem die Aufgabe abgeschlossen sein soll.
author: Alina
feature: Work Management
exl-id: b0522db5-9c68-4b1a-82c8-5a9e613eb2ff
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 1%

---

# Übersicht über das geplante Abschlussdatum der Aufgabe

Das geplante Abschlussdatum einer Aufgabe ist das Datum, bis zu dem die Aufgabe abgeschlossen sein soll.

Sie können entweder das geplante Abschlussdatum einer Aufgabe angeben oder es Adobe Workfront überlassen, es nach bestimmten Kriterien zu berechnen.

Die geplanten Abschlussdaten von Aufgaben für ein Projekt bestimmen das geplante Abschlussdatum eines Projekts, wenn das Projekt ab dem Startdatum geplant wird. Weitere Informationen zum geplanten Abschlussdatum des Projekts finden Sie unter [Festlegen des geplanten Abschlussdatums ](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>Das geplante Abschlussdatum einer Aufgabe unterscheidet sich wie folgt vom Commit-Datum der Aufgabe oder dem voraussichtlichen Abschlussdatum der Aufgabe:
>
>* Das Commit-Datum ist das Datum, bis zu dem die der Aufgabe zugewiesene Person manuell schätzt, dass sie die Aufgabe abgeschlossen haben wird. Weitere Informationen finden Sie in den folgenden Artikeln:
>
>   * [Übersicht über das Commit-Datum](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
>   * [Interaktionen zwischen dem Commit-Datum und dem geplanten Abschlussdatum](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
>
>* Das voraussichtliche Abschlussdatum ist ein von Workfront berechnetes Datum und berücksichtigt Aufgabenverzögerungen, Zeitpläne der Aufgabe oder ihrer Vorgänger sowie andere Faktoren, um ein Echtzeit-Datum für den Zeitpunkt zu bestimmen, zu dem die Aufgabe realistisch abgeschlossen werden kann. Weitere Informationen finden Sie unter [Übersicht über das voraussichtliche Abschlussdatum für Projekte, Aufgaben und Probleme](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>

## Manuelles Festlegen des geplanten Abschlussdatums einer Aufgabe

Sie müssen Bearbeitungszugriff auf Aufgaben haben und Berechtigungen zum Verwalten für die Aufgabe besitzen, um das geplante Abschlussdatum der Aufgabe aktualisieren zu können.

Das Festlegen des geplanten Abschlussdatums einer Aufgabe hängt von der Art der Aufgabenbeschränkung ab, die Sie der Aufgabe zuweisen.

Sie können das geplante Abschlussdatum in den folgenden Bereichen von Workfront manuell festlegen:

* Im Feld Aufgabe bearbeiten beim Erstellen oder Bearbeiten einer Aufgabe. Weitere Informationen finden Sie unter [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* Im Bereich Aufgabendetails . Weitere Informationen finden Sie unter [Verwalten von Aufgabeninformationen im Bereich Aufgabendetails - Übersicht](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md).
* Im Bereich Startseite , wenn beim Anzeigen einer Aufgabe im Bedienfeld Zusammenfassung das geplante Abschlussdatum angezeigt wird. Weitere Informationen finden Sie [Aktualisieren oder Bearbeiten eines Arbeitselements im Bereich „Startseite“](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* In der Aufgabenkopfzeile. Weitere Informationen finden Sie unter [Neue Objekt-Kopfzeilen](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* In einer Aufgabenliste oder einem Bericht, wenn das Feld Geplantes Abschlussdatum in der Ansicht angezeigt wird.

  Weitere Informationen finden Sie unter [Bearbeiten von Aufgaben in einer Liste](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

Sie können das geplante Abschlussdatum manuell angeben, wenn Sie eine der folgenden Aufgabeneinschränkungen auswählen:

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
   <td> <p>Muss beendet werden am</p> <p>Nicht später beenden als (NSBA)</p> <p>Nicht früher beenden als (NFBA)</p> </td> 
   <td> <p><span class="s1">Das geplante Startdatum wird angepasst, um die Dauer beizubehalten.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Feste Daten</p> </td> 
   <td> <p>Die Dauer wird angepasst, um das geplante Startdatum unverändert zu lassen.</p> </td> 
  </tr> 
 </tbody> 
</table>

## So berechnet Workfront automatisch das geplante Abschlussdatum für eine Aufgabe

Wenn er automatisch vom System berechnet wird, kann Folgendes das geplante Abschlussdatum einer Aufgabe beeinflussen:

* Aufgabenbeschränkung

  Weitere Informationen zu Aufgabenbeschränkungen finden Sie im Artikel [Übersicht über Aufgabenbeschränkungen](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Vorgängerbeziehung für Aufgabe

  Weitere Informationen zu Aufgabenvorgängern finden Sie im Artikel [Übersicht über Aufgabenvorgänger](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Projekt-Abschlussdatum, wenn das Projekt ab Abschlussdatum geplant ist.
* Die Ausfallzeit des Primären Verantwortlichen für die Aufgabe.

  Wenn für den Primären Verantwortlichen Ausfallzeiten während der Aufgabendauer geplant sind, werden die geplanten Termine der Aufgabe entsprechend angepasst, wenn die Einstellung **Benutzer-Ausfallzeit in Aufgabendauer berücksichtigen** für das Feld **Benutzer-Ausfallzeit** ausgewählt ist. Neue Projekte übernehmen diese Einstellung aus dem Bereich Projektvoreinstellungen, Sie können die Einstellung jedoch auf Projektebene bearbeiten.

  Wenn beispielsweise eine Aufgabe mit der Einschränkung So bald wie möglich am 1. Juni beginnen und am 3. Juni abgeschlossen werden soll und der Primäre Verantwortliche den 2. Juni als Urlaub markiert hat, wird das geplante Abschlussdatum der Aufgabe zum 4. Juni.

  Informationen zur Einstellung **Benutzer-Ausfallzeit** finden Sie in den Artikeln [Konfigurieren von systemweiten Projektvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) oder [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

* Die Zeit, die den Genehmigungseinstellungen zugeordnet ist, wenn die Aufgabe mit einer Genehmigung verknüpft ist. Weitere Informationen finden Sie unter [Konfigurieren globaler Genehmigungseinstellungen](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

Bei automatischer Festlegung wird das geplante Abschlussdatum anhand der folgenden Berechnung ermittelt:

```
Planned Completion Date = Planned Start Date + Duration
```

Wenn Ihre Aufgabe beispielsweise ein Startdatum vom 16. September und eine Dauer von 10 Tagen hat, ist das geplante Abschlussdatum der 26. September.

>[!NOTE]
>
> Der Aktualisierungstyp für das Projekt muss auf „Automatisch“ und „Bei Änderung“ oder „Automatisch“ gesetzt werden, damit die geplanten Stunden und die Dauer automatisch angepasst werden.\
>Weitere Informationen zum Aktualisierungstyp finden Sie im Artikel [Auswahl des Projektaktualisierungstyps](../../../manage-work/projects/manage-projects/select-project-update-type.md).
