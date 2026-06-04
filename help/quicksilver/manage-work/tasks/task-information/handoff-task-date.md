---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Übersicht über das Datum der Aufgabenübergabe
description: Das Übergabedatum ist das Datum, an dem eine Aufgabe für die Arbeit verfügbar wird. Dies bedeutet in der Regel, dass die Vorgänger aufgelöst wurden und der Verantwortliche der Aufgabe mit der Bearbeitung beginnen kann.
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/56lnSl470ICfCvl-m0ZfyTNoj71NMShHD4xJcjsdWNg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 730
ht-degree: 3%

---

# Überblick über das Übergabedatum der Aufgabe

Das Übergabedatum ist das Datum, an dem eine Aufgabe für die Arbeit verfügbar wird. Dies bedeutet in der Regel, dass die Vorgänger aufgelöst wurden und der Verantwortliche der Aufgabe mit der Bearbeitung beginnen kann.

>[!TIP]
>
>Für Probleme und Projekte sind keine Übergabedaten vorhanden.

## So berechnet Adobe Workfront das Übergabedatum

>[!NOTE]
>
>Das Übergabedatum wird nur berechnet, wenn der Projektstatus folgenden Status entspricht:
>
>* Zurückgestellt
>* Aktuell
>* Abgeschlossen
>* Eingestellt
>

Workfront berechnet das Übergabedatum einer Aufgabe anhand der folgenden Regeln:

* **Wenn die Aufgabe einen unvollständigen Vorgänger hat**: Das Übergabedatum für die Aufgabe ist null.
* **Wenn die Aufgabe einen vollständigen Vorgänger hat**: Das Übergabedatum entspricht dem tatsächlichen Abschlussdatum der Vorgängeraufgabe. Wenn der Vorgänger eine Verzögerung aufweist, berechnet Workfront das Übergabedatum der Nachfolgeaufgabe mithilfe der folgenden Formel:

  `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

  Informationen zu Verzögerungszeiten finden Sie unter [Übersicht über Verzögerungsarten](../use-prdcssrs/lag-types.md).

  Wenn die Nachfolgeaufgabe mehr als einen Vorgänger hat, wird das Übergabedatum auf der Grundlage des letzten tatsächlichen Abschlussdatums der Vorgänger berechnet. Wenn beispielsweise die tatsächlichen Abschlussdaten der beiden Vorgänger der 8. November 2022 und der 20. November 2022 sind, ist das Übergabedatum des Nachfolgers der 20. November 2022.

  >[!NOTE]
  >
  >   Die Berechnung des Übergabedatums einer Nachfolgeaufgabe auf der Grundlage des tatsächlichen Abschlussdatums oder einer Vorgängeraufgabe ist unabhängig davon, ob der Vorgänger erzwungen wird oder nicht, identisch. Weitere Informationen zu erzwungenen Vorgängern finden Sie unter [Erzwungene Vorgänger](../use-prdcssrs/enforced-predecessors.md).


* **Wenn die Aufgabe keinen Vorgänger hat und**:

   * **Das geplante Startdatum liegt in der Vergangenheit**: Das Übergabedatum entspricht dem geplanten Startdatum des Projekts, wenn für die Aufgabe keine erzwungene Begrenzung festgelegt ist. Die Fälle, in denen Aufgaben erzwungene Einschränkungen aufweisen, finden Sie unten im Abschnitt „Wenn die Aufgabe für die geplanten Termine eine erzwungene Einschränkung aufweist“.
   * **Das geplante Startdatum liegt in der Zukunft (beliebiges Datum nach dem aktuellen Datum)**: Das Übergabedatum entspricht dem geplanten Startdatum der Aufgabe, wenn für die Aufgabe keine erzwungene Einschränkung festgelegt ist. Die Fälle, in denen Aufgaben erzwungene Einschränkungen aufweisen, finden Sie unten im Abschnitt „Wenn die Aufgabe für die geplanten Termine eine erzwungene Einschränkung aufweist“.

>[!NOTE]
>
>Wenn die Aufgabe einen projektübergreifenden Vorgänger hat, wird das Übergabedatum des Nachfolgers nur neu berechnet, wenn einer der folgenden Fälle eintritt:
>
>* Sie berechnen die Timeline des Nachfolgeprojekts manuell neu. Sie müssen über Verwaltungsberechtigungen für das Projekt verfügen, um die Zeitleiste neu zu berechnen.
>* Die Zeitleiste des Nachfolgeprojekts wird nachts automatisch neu berechnet.
>
>Informationen zur Neuberechnung der Zeitleiste des Projekts finden Sie unter [Neuberechnen von Projektzeitleisten](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* **Wenn die Aufgabe eine erzwungene Einschränkung für die geplanten Termine aufweist**: Das Übergabedatum variiert je nach Art der Einschränkung und abhängig davon, ob die Aufgabe ein tatsächliches Startdatum hat oder nicht.\
  Im Folgenden werden erzwungene Einschränkungen für Aufgaben beschrieben:

   * Muss beginnen am
   * Muss beendet werden am
   * Nicht früher anfangen als
   * Nicht später anfangen als
   * Festes Datum

  Die folgenden Szenarien sind vorhanden:

   * **Wenn die Aufgabe eine Einschränkung aufweist, die auf „Start am“ oder „Start nicht früher als“**: Wenn die Vorgangseinschränkung in der Vergangenheit liegt und es kein tatsächliches Startdatum für die Aufgabe gibt (die Aufgabe wurde noch nicht gestartet), ist das Übergabedatum das nächstmögliche Datum, an dem die Aufgabe gestartet werden kann. Wenn die Aufgabe gestartet wurde, ist das Übergabedatum gleich dem Startdatum des Projekts.
   * **Wenn für den Vorgang der Wert „Ende am“ oder „Beginn nicht später als“ festgelegt ist**: Wenn der Einschränkungstermin für den Vorgang in der Zukunft liegt und es kein tatsächliches Startdatum für den Vorgang gibt (der Vorgang wurde noch nicht gestartet), ist das Übergabedatum das geplante Startdatum des Vorgangs. Wenn für die Aufgabe ein tatsächliches Startdatum vorhanden ist, ist das Übergabedatum das Startdatum des Projekts.
   * **Wenn die Aufgabe eine Einschränkung fester Datumswerte aufweist**: Das Übergabedatum ist das geplante Startdatum der Aufgabe, unabhängig davon, ob sie einen Vorgänger hat oder nicht und ob der Vorgänger abgeschlossen ist oder nicht.

<!--
these are old descriptions, edited by Anna As. on August 25, 2023 in this issue - https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/64c0032500018fabd4fc484167eb10dc/updates
   * When the task has a constraint of Must Start On or Start No Earlier Than, the Handoff Date is the Constraint date, unless there is an Actual Start Date on the task. If there is an Actual Start Date on the task, the Handoff Date is the Actual Completion Date of the predecessor.
   * When the task has a constraint of Must Finish On or Start No Later Than, the Handoff Date is always the Actual Completion Date of the predecessor, regardless of whether there is an Actual Start Date on the task or not. 
   * When the task has a constraint of Fixed Dates, the Handoff Date is the Planned Start Date of the task, regardless of whether it has a predecessor or not and regardless of whether the predecessor is completed or not.

-->

## Suchen des Übergabedatums

Sie können das Übergabedatum einer Aufgabe in einem Aufgabenbericht oder in der Ansicht einer Aufgabenliste anzeigen.\
Weitere Informationen zum Erstellen eines Berichts finden Sie unter [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
