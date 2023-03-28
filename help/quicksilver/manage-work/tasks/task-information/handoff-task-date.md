---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Übersicht über das Datum der Aufgabenübergabe
description: Das Übergabedatum ist das Datum, an dem eine Aufgabe zur Arbeit verfügbar wird. Dies bedeutet in der Regel, dass die Vorgänger die Aufgabe gelöst haben und der Verantwortliche der Aufgabe damit beginnen kann, daran zu arbeiten.
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
source-git-commit: 161084a3b459d4a9598fa780132d420bf0890c71
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 3%

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

   Informationen zur Zeitverzögerung finden Sie unter [Übersicht über die Lag-Typen](../use-prdcssrs/lag-types.md).

   Wenn die Nachfolgeaufgabe mehr als einen Vorgänger aufweist, wird das Übermittlungsdatum auf der Grundlage des letzten tatsächlichen Abschlussdatums der Vorgänger berechnet. Wenn die tatsächlichen Abschlussdaten der beiden Vorgänger beispielsweise der 8. November 2022 und der 20. November 2022 sind, ist das Übergabedatum des Nachfolgers der 20. November 2022.

   >[!NOTE]
   >
   >   Das Übermittlungsdatum einer Nachfolgeaufgabe basierend auf dem tatsächlichen Abschlussdatum oder einer Vorläuferaufgabe wird unabhängig davon, ob der Vorgänger erzwungen wird oder nicht, auf die gleiche Weise berechnet. Weitere Informationen zu erzwungenen Vorgängern finden Sie unter [Durchsetzen von Vorgängern](../use-prdcssrs/enforced-predecessors.md).


* **Wenn die Aufgabe keinen Vorgänger hat und**:

   * **Das geplante Startdatum liegt in der Vergangenheit.**: Das Übergabedatum entspricht dem geplanten Startdatum des Projekts.
   * **Das geplante Startdatum ist in der Zukunft (ein beliebiges Datum nach dem aktuellen Datum)**: Das Übergabedatum entspricht dem geplanten Startdatum des Projekts.

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

   * Wenn die Aufgabe die Beschränkung Muss beginnen am oder Anfang nicht früher als aufweist, ist das Übergabedatum das Beschränkungsdatum, es sei denn, es gibt ein aktuelles Startdatum für die Aufgabe. Wenn für die Aufgabe ein tatsächliches Anfangsdatum vorliegt, ist das Übergabedatum das tatsächliche Abschlussdatum des Vorgängers.
   * Wenn die Aufgabe die Beschränkung &quot;Must Finish On&quot;oder &quot;Start No Later Than&quot;hat, ist das Übergabedatum immer das tatsächliche Abschlussdatum des Vorgängers, unabhängig davon, ob für die Aufgabe ein tatsächliches Startdatum vorliegt oder nicht.
   * Wenn die Aufgabe eine Beschränkung von &quot;Feste Datumswerte&quot;hat, ist das Übergabedatum das geplante Startdatum der Aufgabe, unabhängig davon, ob es einen Vorgänger hat oder nicht und ob der Vorgänger abgeschlossen ist oder nicht.


## Suchen Sie das Übermittlungsdatum.

Sie können das Übergabedatum einer Aufgabe in einem Aufgabenbericht oder die Ansicht einer Aufgabenliste anzeigen.\
Weitere Informationen zum Erstellen eines Berichts finden Sie unter [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
