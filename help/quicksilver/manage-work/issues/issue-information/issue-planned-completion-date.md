---
product-area: projects
navigation-topic: issue-information
title: Übersicht über das geplante Abschlussdatum der Anfrage
description: Das geplante Abschlussdatum einer Anfrage ist das Datum, bis zu dem die Anfrage voraussichtlich abgeschlossen wird.
author: Alina
feature: Work Management
exl-id: bdb206dc-18f8-4f8a-862b-e881408a8408
TQID: https://experienceleague.adobe.com/WodCHwmu7JYCZKdoqoJ6W88AP0xzlZ-Jglj5zxD8-6g
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: ce22a157-dd2c-405f-b740-c2f204bb4c1aid: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 595
ht-degree: 1%

---

# Überblick über das geplante Abschlussdatum des Problems

<!--Audited: 08/2025-->

Das geplante Abschlussdatum einer Anfrage ist das Datum, bis zu dem die Anfrage voraussichtlich abgeschlossen wird.

Sie können entweder das geplante Abschlussdatum eines Problems angeben oder es je nach bestimmten Kriterien Adobe Workfront überlassen, es zu berechnen.

Die geplanten Abschlussdaten von Problemen wirken sich nicht auf das geplante Abschlussdatum des Projekts aus. Nur die geplanten Abschlussdaten von Vorgängen wirken sich auf das geplante Abschlussdatum des Projekts aus. Weitere Informationen zum geplanten Abschlussdatum des Projekts finden Sie unter [Festlegen des geplanten Abschlussdatums ](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>Das geplante Abschlussdatum einer Anfrage unterscheidet sich wie folgt vom Commit-Datum der Anfrage oder dem voraussichtlichen Abschlussdatum der Anfrage:
>
>* Das Commit-Datum ist das Datum, bis zu dem die dem Problem zugewiesene Person manuell schätzt, dass sie das Problem abgeschlossen haben wird. Weitere Informationen finden Sie in den folgenden Artikeln:
>
>   * [Übersicht über das Commit-Datum](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
>   * [Interaktionen zwischen dem Commit-Datum und dem geplanten Abschlussdatum](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
>
>* Das voraussichtliche Abschlussdatum ist ein von Workfront berechnetes Datum, bei dem externe Faktoren berücksichtigt werden, um ein reales Datum für den Fall zu bestimmen, dass das Problem realistisch abgeschlossen werden kann. Weitere Informationen finden Sie unter [Übersicht über das voraussichtliche Abschlussdatum für Projekte, Aufgaben und Probleme](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>

## Manuelles Festlegen des geplanten Abschlussdatums einer Anfrage

Sie müssen Bearbeitungszugriff auf Probleme haben und Berechtigungen zum Verwalten des Problems besitzen, um das geplante Abschlussdatum des Problems aktualisieren zu können.

Sie können das geplante Abschlussdatum eines Problems in den folgenden Bereichen von Workfront manuell festlegen:

* Im Feld „Problem bearbeiten“ oder im Bereich „Problemdetails“ beim Erstellen oder Bearbeiten eines Problems. Weitere Informationen finden Sie unter [Probleme bearbeiten](../../../manage-work/issues/manage-issues/edit-issues.md).
* Im Bereich Startseite , wenn das geplante Abschlussdatum im Bedienfeld Zusammenfassung eines Problems angezeigt wird. Weitere Informationen finden Sie [Aktualisieren oder Bearbeiten eines Arbeitselements im Bereich „Startseite“](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* Im Problem-Header. Weitere Informationen finden Sie unter [Neue Objekt-Kopfzeilen](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* In einer Problemliste oder einem Bericht, wenn das Feld Geplantes Abschlussdatum in der Ansicht angezeigt wird.

  Weitere Informationen finden Sie unter [Probleme in einer Liste bearbeiten](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## So berechnet Workfront automatisch das geplante Abschlussdatum für ein Problem

Wenn Workfront das geplante Abschlussdatum eines Problems automatisch berechnet, kann sich Folgendes auf das Datum auswirken:

* Geplantes Startdatum

  Das Eingabedatum und das geplante Startdatum sollten beim ersten Erstellen des Problems mit dem ursprünglichen Datum übereinstimmen.

* Die Standarddauer wird im Abschnitt Warteschlangendetails des Projekts konfiguriert. Weitere Informationen finden Sie unter [Erstellen einer Anfrage-Warteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

  Wenn die Standarddauer 0 Tage ist, stimmt das geplante Abschlussdatum mit dem geplanten Startdatum des Problems überein.

* Projektzeitplan

Bei automatischer Festlegung wird das geplante Abschlussdatum anhand der folgenden Berechnung ermittelt:

```
Planned Completion Date = Planned Start Date (or Entry Date + Default Duration
```

**Beispiel:** Wenn Ihre Aufgabe beispielsweise ein Startdatum für Freitag, den 14. Januar, hat und die Standarddauer 5 Tage ist, ist das geplante Abschlussdatum Freitag, den 21. Januar, wenn der Projektzeitplan von Montag bis Freitag für 8 Stunden pro Tag ist.

Die folgenden Situationen bestehen:

* Wenn das Projekt keinen Zeitplan hat, wird der Standardzeitplan Ihres Workfront-Systems berücksichtigt. Weitere Informationen finden Sie unter [Zeitpläne - Übersicht](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).
* Wenn der Zeitplan von Montag bis Freitag 9:00 bis 13:00 Uhr (4 Stunden pro Tag) lautet und die typischen Arbeitszeiten Ihres Workfront-Systems 8 Stunden betragen, ist das geplante Abschlussdatum der 27. Januar.

>[!TIP]
>
>Workfront berücksichtigt bei der Berechnung der geplanten Abschlussdaten Zeitplanausnahmen wie Feiertage und Wochenenden.


