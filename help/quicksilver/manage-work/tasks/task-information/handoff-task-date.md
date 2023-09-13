---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Übersicht über das Datum der Aufgabenübergabe
description: Das Übergabedatum ist das Datum, an dem eine Aufgabe zur Arbeit verfügbar wird. Dies bedeutet in der Regel, dass die Vorgänger die Aufgabe gelöst haben und der Verantwortliche der Aufgabe damit beginnen kann, daran zu arbeiten.
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
source-git-commit: b774a74863bb35e3477a69ff11189c40a6d66437
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 2%

---

# Übersicht über das Datum der Aufgabenübergabe

Das Übergabedatum ist das Datum, an dem eine Aufgabe zur Arbeit verfügbar wird. Dies bedeutet in der Regel, dass die Vorgänger die Aufgabe gelöst haben und der Verantwortliche der Aufgabe damit beginnen kann, daran zu arbeiten.

>[!TIP]
>
>Für Probleme und Projekte gibt es keine Übergabedaten.

## Berechnung des Übergabedatums durch Adobe Workfront

>[!NOTE]
>
>Das Übergabedatum wird nur berechnet, wenn der Projektstatus den folgenden Status aufweist:
>
>* Zurückgestellt
>* Aktuell
>* Abgeschlossen
>* Eingestellt
>

Workfront verwendet die folgenden Regeln zur Berechnung des Übergabedatums einer Aufgabe:

* **Wenn die Aufgabe einen unvollständigen Vorgänger hat**: Das Übergabedatum für die Aufgabe ist null.
* **Wenn die Aufgabe einen vollständigen Vorgänger hat**: Das Übergabedatum entspricht dem tatsächlichen Abschlussdatum der vorherigen Aufgabe. Wenn der Vorgänger über eine Verzögerung verfügt, berechnet Workfront das Übergabedatum der Nachfolgeaufgabe anhand der folgenden Formel:

  `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

  Weitere Informationen zur Zeitverzögerung finden Sie unter [Übersicht über die Lag-Typen](../use-prdcssrs/lag-types.md).

  Wenn die Nachfolgeaufgabe mehr als einen Vorgänger aufweist, wird das Übermittlungsdatum auf der Grundlage des letzten tatsächlichen Abschlussdatums der Vorgänger berechnet. Wenn die tatsächlichen Abschlussdaten der beiden Vorgänger beispielsweise der 8. November 2022 und der 20. November 2022 sind, ist das Übergabedatum des Nachfolgers der 20. November 2022.

  >[!NOTE]
  >
  >   Das Übermittlungsdatum einer Nachfolgeaufgabe basierend auf dem tatsächlichen Abschlussdatum oder einer Vorläuferaufgabe wird unabhängig davon, ob der Vorgänger erzwungen wird oder nicht, auf die gleiche Weise berechnet. Weitere Informationen zu erzwungenen Vorgängern finden Sie unter [Durchsetzen von Vorgängern](../use-prdcssrs/enforced-predecessors.md).


* **Wenn die Aufgabe keinen Vorgänger hat und**:

   * **Das geplante Startdatum liegt in der Vergangenheit.**: Das Übergabedatum entspricht dem geplanten Startdatum des Projekts, wenn für die Aufgabe keine erzwungene Beschränkung festgelegt ist. Informationen zu den Fällen, in denen Aufgaben Zwänge erzwungen haben, finden Sie im Abschnitt &quot;Wenn die Aufgabe eine erzwungene Beschränkung für die geplanten Datumswerte hat&quot;unten.
   * **Das geplante Startdatum ist in der Zukunft (ein beliebiges Datum nach dem aktuellen Datum)**: Das Übergabedatum entspricht dem geplanten Startdatum der Aufgabe, wenn für die Aufgabe keine erzwungene Beschränkung festgelegt ist. Informationen zu den Fällen, in denen Aufgaben Zwänge erzwungen haben, finden Sie im Abschnitt &quot;Wenn die Aufgabe eine erzwungene Beschränkung für die geplanten Datumswerte hat&quot;unten.

>[!NOTE]
>
>Wenn die Aufgabe einen projektübergreifenden Vorgänger hat, wird das Übermittlungsdatum des Nachfolgers nur dann neu berechnet, wenn eine der folgenden Ereignisse eintritt:
>
>* Sie berechnen die Timeline des Nachfolger-Projekts manuell neu. Sie müssen über Verwaltungsberechtigungen für das Projekt verfügen, um die Timeline neu zu berechnen.
>* Die Zeitleiste des Nachfolgeprojekts wird nachts automatisch neu berechnet.
>
>Weitere Informationen zur Neuberechnung der Projektzeitleiste finden Sie unter [Projektzeitpläne neu berechnen](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* **Wenn die Aufgabe eine erzwungene Beschränkung für die geplanten Datumswerte hat**: Das Übergabedatum variiert je nach Art der Einschränkung und abhängig davon, ob die Aufgabe über ein tatsächliches Startdatum verfügt oder nicht.\
  Die folgenden erzwungenen Einschränkungen gelten für Aufgaben:

   * Muss beginnen am
   * Muss beendet werden am
   * Nicht früher anfangen als
   * Nicht später anfangen als
   * Festes Datum

  Die folgenden Szenarien existieren:

   * **Wenn die Aufgabe die Beschränkung Muss beginnen am oder Start nicht früher als hat**: Wenn das Datum der Aufgabenbegrenzung in der Vergangenheit liegt und es für die Aufgabe kein aktuelles Startdatum gibt (die Aufgabe wurde noch nicht gestartet), ist das Übermittlungsdatum das nächstmögliche Datum, an dem die Aufgabe gestartet werden kann, um bearbeitet zu werden. Wenn die Aufgabe gestartet wurde, entspricht das Übergabedatum dem Startdatum des Projekts.
   * **Wenn die Aufgabe die Beschränkung Must Finish On oder Start No Later Than hat**: Wenn das Datum der Aufgabenbegrenzung in der Zukunft liegt und es für die Aufgabe kein tatsächliches Startdatum gibt (die Aufgabe wurde noch nicht gestartet), ist das Übergabedatum das geplante Startdatum der Aufgabe. Wenn für die Aufgabe das tatsächliche Startdatum angegeben ist, ist das Übergabedatum das Anfangsdatum des Projekts.
   * **Wenn die Aufgabe eine Beschränkung von &quot;Feste Datumswerte&quot;hat**: Das Übergabedatum ist das geplante Startdatum der Aufgabe, unabhängig davon, ob sie über einen Vorgänger verfügt oder nicht und unabhängig davon, ob der Vorgänger abgeschlossen ist oder nicht.

<!--these are old descriptions, edited by Anna As. on August 25, 2023 in this issue - https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/64c0032500018fabd4fc484167eb10dc/updates
   * When the task has a constraint of Must Start On or Start No Earlier Than, the Handoff Date is the Constraint date, unless there is an Actual Start Date on the task. If there is an Actual Start Date on the task, the Handoff Date is the Actual Completion Date of the predecessor.
   * When the task has a constraint of Must Finish On or Start No Later Than, the Handoff Date is always the Actual Completion Date of the predecessor, regardless of whether there is an Actual Start Date on the task or not. 
   * When the task has a constraint of Fixed Dates, the Handoff Date is the Planned Start Date of the task, regardless of whether it has a predecessor or not and regardless of whether the predecessor is completed or not.

-->

## Suchen Sie das Übermittlungsdatum.

Sie können das Übergabedatum einer Aufgabe in einem Aufgabenbericht oder die Ansicht einer Aufgabenliste anzeigen.\
Weitere Informationen zum Erstellen eines Berichts finden Sie unter [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
