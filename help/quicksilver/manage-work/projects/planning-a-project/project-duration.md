---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Übersicht über die Projektdauer
description: Adobe Workfront berechnet die Dauer eines Projekts anhand des Startdatums der ersten Aufgabe und des Abschlussdatums der letzten Aufgabe und zählt die Anzahl der Tage zwischen den beiden Terminen.
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
TQID: https://experienceleague.adobe.com/1j0nj2W5f7FtgIk46G3ePFA-zwt7VAyV9fQWKm2kZJ4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 254
ht-degree: 2%

---

# Überblick über die Projektdauer

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
