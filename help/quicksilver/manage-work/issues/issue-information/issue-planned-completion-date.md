---
product-area: projects
navigation-topic: issue-information
title: Überblick über das geplante Abschlussdatum
description: Das geplante Abschlussdatum eines Problems ist das Datum, bis zu dem das Problem voraussichtlich abgeschlossen sein wird.
author: Alina
feature: Work Management
exl-id: bdb206dc-18f8-4f8a-862b-e881408a8408
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# Überblick über das geplante Abschlussdatum

Das geplante Abschlussdatum eines Problems ist das Datum, bis zu dem das Problem voraussichtlich abgeschlossen sein wird.

Sie können entweder das geplante Abschlussdatum eines Problems angeben oder es an Adobe Workfront überlassen, es nach bestimmten Kriterien zu berechnen. 

Das geplante Abschlussdatum der Probleme hat keine Auswirkungen auf das geplante Abschlussdatum des Projekts. Nur die geplanten Abschlussdaten von Aufgaben wirken sich auf das geplante Abschlussdatum des Projekts aus. Weitere Informationen zum geplanten Abschlussdatum des Projekts finden Sie unter [Festlegen des geplanten Abschlussdatums des Projekts](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>Das geplante Abschlussdatum eines Problems unterscheidet sich wie folgt vom Veröffentlichungsdatum des Problems oder vom geplanten Abschlussdatum des Problems:
>
>* Das Datum der Veröffentlichung ist das Datum, bis zu dem die Person, die dem Problem zugewiesen ist, schätzt, dass sie das Problem abgeschlossen haben wird. Weitere Informationen finden Sie in den folgenden Artikeln:
   * [Datum bestätigen - Übersicht](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
   * [Wechselwirkungen zwischen dem Veröffentlichungsdatum und dem geplanten Abschlussdatum](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
* Das prognostizierte Abschlussdatum ist ein von Workfront berechnetes Datum, das externe Faktoren berücksichtigt, um ein Echtzeit-Datum zu bestimmen, ab dem das Problem realistisch abgeschlossen werden kann. Weitere Informationen finden Sie unter [Übersicht über das geplante Abschlussdatum für Projekte, Aufgaben und Probleme](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>


## Manuelles Festlegen des geplanten Abschlussdatums eines Problems

Sie müssen Zugriff auf Probleme bearbeiten und Berechtigungen zum Verwalten des Problems haben, um das geplante Abschlussdatum des Problems aktualisieren zu können.

Sie können das geplante Abschlussdatum eines Problems in den folgenden Bereichen von Workfront manuell festlegen:

* Im Feld Problem bearbeiten oder im Bereich Problemdetails beim Erstellen oder Bearbeiten eines Problems. Weitere Informationen finden Sie unter [Probleme bearbeiten](../../../manage-work/issues/manage-issues/edit-issues.md).
* Im Bereich Startseite , wenn das geplante Abschlussdatum bei der Anzeige eines Problems angezeigt wird. Weitere Informationen finden Sie unter [Aktualisieren oder Bearbeiten eines Arbeitselements im Startbereich](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* In der Ausgabe-Kopfzeile. Weitere Informationen finden Sie unter [Neue Objektüberschriften](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* In einer Problemliste oder einem Bericht, wenn das Feld Geplantes Abschlussdatum in der Ansicht angezeigt wird.

   Weitere Informationen finden Sie unter [Probleme in einer Liste bearbeiten](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## Wie Workfront das geplante Abschlussdatum für ein Problem automatisch berechnet

Wenn Workfront das geplante Abschlussdatum eines Problems automatisch berechnet, kann Folgendes das Datum beeinflussen:

* Geplantes Startdatum

   Das Einstiegsdatum und das geplante Startdatum sollten bei einem Problem übereinstimmen, wenn Sie das Problem zum ersten Mal erstellen.

* Die Standarddauer, wie im Abschnitt &quot;Queue Details&quot;des Projekts konfiguriert. Weitere Informationen finden Sie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Wenn die Standarddauer 0 Tage beträgt, stimmt das geplante Abschlussdatum mit dem geplanten Startdatum des Problems überein.

* Projektzeitplan

Wenn das geplante Abschlussdatum automatisch eingestellt wird, wird es anhand der folgenden Berechnung ermittelt: 

```
Planned Completion Date = Planned Start Date (or Entry Date + Default Duration
```

**Beispiel:** Wenn Ihre Aufgabe beispielsweise das Startdatum Freitag, 14. Januar hat und die Standarddauer 5 Tage beträgt, ist das geplante Abschlussdatum Freitag, der 21. Januar, wenn der Projektzeitplan Montag bis Freitag für 8 Stunden am Tag ist.

Die folgenden Situationen sind vorhanden:

* Wenn das Projekt keinen Zeitplan aufweist, wird der Standardzeitplan Ihres Workfront-Systems berücksichtigt. Weitere Informationen finden Sie unter [Zeitpläne - Übersicht](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).
* Wenn der Zeitplan Montag bis Freitag von 9:00 bis 13:00 Uhr (4 Stunden am Tag) ist und die typischen Arbeitszeiten Ihres Workfront-Systems pro Arbeitstag 8 Stunden betragen, ist das geplante Abschlussdatum der 27. Januar.

>[!TIP]
Workfront berücksichtigt bei der Berechnung der geplanten Abschlussdaten Ausnahmen wie Feiertage und Wochenenden.

 
