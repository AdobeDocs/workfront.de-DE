---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Übersicht über die geplante Aufgabe - Startdatum
description: Das geplante Startdatum einer Aufgabe ist das Datum, an dem Sie als Ersteller der Aufgabe entscheiden, dass die Arbeit an der Aufgabe beginnen soll. Geplante Aufgabendaten beeinflussen die Daten und die Zeitleiste des Projekts. Weitere Informationen zum geplanten Projektstartdatum finden Sie unter Übersicht über das geplante Projektstartdatum.
author: Alina
feature: Work Management
exl-id: 2ac6327f-4a13-4fb8-ad8e-03d032221483
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 2%

---

# Übersicht über die geplante Aufgabe - Startdatum

Das geplante Startdatum einer Aufgabe ist das Datum, an dem Sie als Ersteller der Aufgabe entscheiden, dass die Arbeit an der Aufgabe beginnen soll. Geplante Aufgabendaten beeinflussen die Daten und die Zeitleiste des Projekts. Weitere Informationen zum geplanten Startdatum des Projekts finden Sie unter [Übersicht über das geplante Projektstartdatum](../../../manage-work/projects/planning-a-project/project-planned-start-date.md).

## Das geplante Startdatum einer Aufgabe

Sie können entweder das geplante Startdatum einer Aufgabe angeben oder es Adobe Workfront überlassen, sie nach bestimmten Kriterien zu berechnen. 

* [Manuelles Festlegen des geplanten Startdatums einer Aufgabe](#manually-set-the-planned-start-date-of-a-task)
* [Berechnung des geplanten Startdatums für eine Aufgabe](#how-the-planned-start-date-is-calculated-for-a-task)

### Manuelles Festlegen des geplanten Startdatums einer Aufgabe {#manually-set-the-planned-start-date-of-a-task}

Das Festlegen des geplanten Startdatums einer Aufgabe hängt vom Typ der Aufgabenbegrenzung ab, die Sie der Aufgabe zuweisen. 

Sie können das geplante Startdatum beim Erstellen einer Aufgabe manuell festlegen, wie im Artikel beschrieben [Erstellen von Aufgaben in einem Projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Sie können das geplante Startdatum manuell angeben, wenn Sie eine der folgenden Aufgabenbeschränkungen auswählen: 

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
   <td> <p>Muss beginnen am</p> <p>Nicht früher anfangen als</p> <p>Nicht später anfangen als</p> </td> 
   <td> <p><span class="s1">Das geplante Abschlussdatum wird angepasst, damit die Dauer unverändert bleibt.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Feste Daten</p> </td> 
   <td> <p>Die Dauer wird angepasst, damit das geplante Abschlussdatum unverändert bleibt.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Berechnung des geplanten Startdatums für eine Aufgabe {#how-the-planned-start-date-is-calculated-for-a-task}

Wenn sie automatisch vom System berechnet wird, kann Folgendes das geplante Startdatum einer Aufgabe beeinflussen:

* Die Voreinstellung für das Startdatum im Bereich &quot;Aufgaben und Probleme&quot;in der Einrichtung

   Ihr Workfront- oder Gruppenadministrator kann bestimmen, ob eine neue Aufgabe am selben Datum wie das geplante Startdatum des Projekts beginnt oder am Tag der Erstellung der Aufgabe.

   Weitere Informationen zu den Voreinstellungen für Aufgaben und Probleme finden Sie unter [Systemweite Aufgaben- und Problemeinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Aufgabenbeschränkung

   Weitere Informationen zu Aufgabenbegrenzungen finden Sie im Artikel [Übersicht über Aufgabenbegrenzungen](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)

* Aufgabenverlaufsbeziehung

   Weitere Informationen zu Aufgabenvorgängen finden Sie im Artikel [Übersicht über die Vorgänger von Aufgaben](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Projektstartdatum, an dem das Projekt ab dem Startdatum geplant ist.
* Die Zeitdauer des Primären Aufgabenempfängers.

   Wenn für den Primären Verantwortlichen während der Aufgabendauer eine Zeitüberschreitung geplant ist, werden die geplanten Zeitpunkte der Aufgabe entsprechend angepasst, sobald die **Benutzerzeitlimit in Aufgabendauern berücksichtigen** -Einstellung für **Zeitlimit für Benutzer** -Feld. Neue Projekte übernehmen diese Einstellung im Bereich &quot;Projekteinstellungen&quot;, Sie können die Einstellung jedoch auf Projektebene bearbeiten.

   Wenn beispielsweise eine Aufgabe mit der Beschränkung So bald wie möglich am 1. Juni beginnen und am 3. Juni abgeschlossen sein soll und der Primäre Verantwortliche den 1. Juni für die Zeitüberschreitung markiert hat, wird die Aufgabe &quot;Geplantes Startdatum&quot;zum 2. Juni.

   Informationen zum **Zeitlimit für Benutzer** -Voreinstellungen, siehe Artikel  [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) oder [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

Wenn das geplante Startdatum automatisch festgelegt wird, wird es anhand der folgenden Berechnung ermittelt: 

```
Planned Start Date = Planned Completion Date - Task Duration
```

Wenn Ihre Aufgabe beispielsweise das Abschlussdatum 16. September und die Dauer 10 Tage beträgt, ist das geplante Startdatum der 6. September.

>[!NOTE]
>
> Der Aktualisierungstyp für das Projekt muss ebenfalls auf &quot;Automatisch und bei Änderung&quot;oder &quot;Automatisch&quot;gesetzt werden, damit die geplanten Stunden und die geplante Dauer automatisch angepasst werden.\
Weitere Informationen zum Aktualisierungstyp finden Sie im Artikel [Wählen Sie den Projektaktualisierungstyp aus](../../../manage-work/projects/manage-projects/select-project-update-type.md).
