---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Übersicht über die Projektdauer
description: Adobe Workfront berechnet die Dauer eines Projekts anhand des Startdatums der ersten Aufgabe und des Abschlussdatums der letzten Aufgabe und zählt die Anzahl der Tage zwischen den beiden Terminen.
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Übersicht über die Projektdauer

Adobe Workfront berechnet die Dauer eines Projekts anhand des Startdatums der ersten Aufgabe und des Abschlussdatums der letzten Aufgabe und zählt die Anzahl der Tage zwischen den beiden Terminen.

## Projektdauer

Die Dauer des Projekts wird nach folgender Formel berechnet:

```
Project Duration = Completion Date of the latest task - Start Date of the earliest task
```

>[!NOTE]
>
>Die Dauer von Problemen im Projekt wirkt sich nicht auf die Dauer des Projekts aus.

Die Dauer des Projekts zählt die Anzahl der Tage zwischen den beiden Aufgabendaten auf der Grundlage des mit dem Projekt verknüpften Zeitplans oder der den Aufgaben zugewiesenen Benutzer. Informationen dazu, welchen Zeitplan Workfront für die Berechnung der Dauer verwendet, finden Sie unter [Zeitpläne - Übersicht](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).

## Typen der Projektdauer

Es gibt zwei Arten der Projektdauer und die Formeln, nach denen sie von Workfront berechnet werden:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Check these formulas? Should they be divided by the hours per day?!) </p>
-->

* **Geplante**:

  ```
  Project Planned Duration = Planned Completion Date of the latest task - Planned Start Date of the earliest task / Typical hour per day
  ```

* **Tatsächliche**:

  ```
  Project Actual Duration = Actual Completion Date of the latest task - Actual Start Date of the earliest task / Typical hour per day
  ```

## Suchen der Projektdauer

Die geplante Projektdauer und die tatsächliche Projektdauer finden Sie in den folgenden Bereichen von Workfront:

* . Im Bereich Projektdetails im Abschnitt Übersicht .

  Weitere Informationen zur Unterregisterkarte Überblick eines Projekts finden Sie im Artikel [Verwalten von Informationen im Bereich Projektübersicht](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* In einem Projektbericht, indem Sie die Felder Dauer oder Tatsächliche Dauer in den Bericht aufnehmen.

  Weitere Informationen zum Erstellen von Berichten finden Sie im Artikel [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
