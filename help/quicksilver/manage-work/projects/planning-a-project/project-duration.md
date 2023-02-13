---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Übersicht über die Projektdauer
description: Adobe Workfront berechnet die Projektdauer unter Berücksichtigung des Anfangsdatums der frühesten Aufgabe und des Abschlussdatums der letzten Aufgabe und zählt die Anzahl der Tage zwischen den beiden Daten.
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 2%

---

# Übersicht über die Projektdauer

Adobe Workfront berechnet die Projektdauer unter Berücksichtigung des Anfangsdatums der frühesten Aufgabe und des Abschlussdatums der letzten Aufgabe und zählt die Anzahl der Tage zwischen den beiden Daten.

## Projektdauer

Die Projektdauer wird nach folgender Formel berechnet:

```
Project Duration = Completion Date of the latest task - Start Date of the earliest task
```

>[!NOTE]
>
>Die Dauer des Projekts hat keine Auswirkungen auf die Dauer des Projekts.

Die Dauer des Projekts zählt die Anzahl der Tage zwischen den beiden Aufgabendaten basierend auf dem mit dem Projekt verknüpften Zeitplan oder den den Aufgaben zugewiesenen Benutzern. Informationen darüber, welchen Zeitplan Workfront zur Berechnung der Dauer verwendet, finden Sie unter [Zeitpläne - Übersicht](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).

## Typen der Projektdauer

Es gibt zwei Arten von Projektdauer und die Formeln, anhand derer Workfront sie berechnet:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Check these formulas? Should they be divided by the hours per day?!) </p>
-->

* **Geplante Dauer**: 

   ```
   Project Planned Duration = Planned Completion Date of the latest task - Planned Start Date of the earliest task / Typical hour per day
   ```

* **Tatsächliche Dauer**: 

   ```
   Project Actual Duration = Actual Completion Date of the latest task - Actual Start Date of the earliest task / Typical hour per day
   ```

## Projektdauer ermitteln

Sie können die geplanten und tatsächlichen Dauer des Projekts in den folgenden Bereichen von Workfront ermitteln:

* . Im Bereich Projektdetails im Abschnitt Übersicht .

   Weitere Informationen zur Unterregisterkarte &quot;Überblick&quot;eines Projekts finden Sie im Artikel [Informationen im Bereich &quot;Projektübersicht&quot;verwalten](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* in einem Projektbericht, indem die Felder Dauer oder tatsächliche Dauer in den Bericht aufgenommen werden.

   Weitere Informationen zum Erstellen von Berichten finden Sie im Artikel [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
