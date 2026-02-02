---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Übersicht über Aufgabenvorgänger
description: Ein Vorgänger ist die Aufgabe, von der eine andere Aufgabe (eine so genannte Nachfolger- oder abhängige Aufgabe) abhängt. Adobe Workfront unterstützt fünf Arten von Vorgängerabhängigkeiten.
author: Alina
feature: Work Management
exl-id: b2020a50-0921-4ed2-8a34-1a0411992b99
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '1184'
ht-degree: 0%

---

# Übersicht über Aufgabenvorgänger

<!--Audited: 12/2023-->

<!-- 

CONTEXT SENSITIVE HELP article. DO NOT CHANGE THE NAME OF THE ARTICLE/ DO NOT MOVE OR DELETE! -->

Ein Vorgänger ist die Aufgabe, von der eine andere Aufgabe (eine so genannte Nachfolger- oder abhängige Aufgabe) abhängt. Adobe Workfront unterstützt fünf Arten von Vorgängerabhängigkeiten. Informationen zu Vorgängerabhängigkeiten finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Übersicht über Vorgänger

Zum Verständnis der Timelines in Ihren Projekten ist es wichtig, die Vorgängerfunktionen zu verstehen.

Aufgabenvorgängerbeziehungen bestehen sowohl zwischen Aufgaben innerhalb eines einzelnen Projekts als auch zwischen Aufgaben aus verschiedenen Projekten.

Bei einer Abhängigkeit mehrerer Projekte können Sie projektübergreifende Vorgänger zwischen Aufgaben aus zwei verschiedenen Projekten festlegen.

Unabhängig davon, ob die Vorgänger- und Nachfolgeaufgaben zu demselben Projekt oder zu zwei verschiedenen Projekten gehören, werden die Abhängigkeiten und die Timelines der einzelnen Projekte auf dieselbe Weise berechnet.

Bei Vorgängern wirkt sich Folgendes auf die Zeitleiste des Projekts aus:

* Vorgängerabhängigkeit
* Verzögerungswert und -typ\
  Weitere Informationen zu Abhängigkeiten und Verzögerungen finden Sie unter [Beispiele für Vorgängerwerte in einer Aufgabenliste](#examples-of-predecessor-values-in-a-task-list).

  Wenn beispielsweise Aufgabe A ein Vorgänger von Aufgabe B in einer Ende-Anfang-Beziehung ist und Aufgabe B die Aufgabenbeschränkung „So bald wie möglich“ aufweist, weist Workfront Aufgabe B ein geplantes Startdatum unmittelbar nach dem geplanten Abschlussdatum von Aufgabe A zu, unabhängig davon, ob der Vorgänger erzwungen wird oder nicht.

Um Vorgängerbeziehungen zu verstehen, müssen Sie Folgendes verstehen:

* **Abhängigkeitstypen:** Vorgänger sind durch verschiedene Abhängigkeitstypen verknüpft. Weitere Informationen zu Abhängigkeitstypen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

* **Erzwingen eines Vorgängers:** Beim Erzwingen eines Vorgängers kann die Nachfolgeaufgabe absolut erst gestartet werden, wenn der Vorgänger abgeschlossen ist. Die Nachfolgeaufgabe wird als unmittelbar nach Abschluss des Vorgängers beginnend angezeigt.

  Wenn der Vorgänger nicht abgeschlossen (oder gestartet) ist und er nicht erzwungen wird, kann die Nachfolgeaufgabe beginnen, aber die Projektzeitleiste ist weiterhin von den Daten des Vorgängers und der Nachfolgeaufgaben betroffen.

  Bei einem erzwungenen Vorgänger lässt Workfront es nicht zu, dass die Nachfolgeaufgabe als In Bearbeitung oder Abgeschlossen markiert wird, bis der Vorgänger abgeschlossen ist.

  Workfront lässt jedoch zu, dass zu dieser Aufgabe Stundenberichte erstellt werden.\
  Weitere Informationen zum Erzwingen von Vorgängern finden Sie unter [Erzwingen von Vorgängern](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

* **Verzögerungen** Sie können Verzögerungen in Ihren Abhängigkeiten erstellen, die eine Verzögerung verursachen, die nach Abschluss einer Vorgängeraufgabe und vor dem Beginn der Nachfolgeaufgabe auftreten muss. Verzögerungen wirken sich auf die Zeitleiste des Projekts aus.

  Informationen zu Verzögerungsarten finden Sie unter [Übersicht zu Verzögerungsarten](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

## Erstellen von Vorgängerbeziehungen

Informationen zum Erstellen von Vorgängern finden Sie in den folgenden Artikeln:

* Informationen zum Erstellen von Vorgängern mithilfe der Registerkarte „Vorgänger“ der Aufgabe finden [ unter „Erstellen einer Vorgängerbeziehung mithilfe des Bereichs „Vorgänger“](../../../manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).
* Informationen zum Einrichten von Vorgängern in einer Aufgabenliste finden Sie unter [Erstellen einer Vorgängerbeziehung in der Aufgabenliste](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).
* Informationen zum Erstellen von Vorgängerbeziehungen durch Verketten von Aufgaben finden Sie unter [Erstellen von Vorgängerbeziehungen durch Verketten von Aufgaben](../../../manage-work/tasks/use-prdcssrs/create-predecessors-by-chaining-tasks.md).
* Informationen zum Einrichten von projektübergreifenden Vorgängern finden Sie unter [Erstellen von projektübergreifenden Vorgängern](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

## Suchen der Vorgänger einer Aufgabe {#locate-the-predecessors-of-a-task}

Führen Sie einen der folgenden Schritte aus, um die Vorgänger einer Aufgabe zu finden:

* Gehen Sie zu dem Projekt, an dem Sie arbeiten, und führen Sie folgende Schritte aus:

   1. Suchen Sie die Aufgabe, für die Sie die Vorgänger suchen möchten, und klicken Sie auf die Aufgabe.
   1. Klicken Sie **linken Bedienfeld auf** Vorgänger“.
   1. Der Name des Projekts, das den Vorgänger enthält, wird in der Spalte **Projekt** angezeigt.

      Die Zahl in der Spalte **#** zeigt die Nummer der Vorgängeraufgabe an. Beispiel: „6“ bedeutet die sechste Aufgabe im Projekt.

      ![Abschnitt Vorgänger der Aufgabe](assets/predecessors-area-with-task-header.png)

* Gehen Sie zu dem Projekt, an dem Sie arbeiten, und führen Sie folgende Schritte aus:

   1. Klicken Sie auf **Registerkarte** Aufgaben“.
   1. Wählen Sie oben **der Aufgabenliste** Standardansicht“ aus.
   1. Die Spalte **Vorgänger** zeigt die Vorgängeraufgaben-Nummern an.

      Bei einem projektübergreifenden Vorgänger zeigt die Spalte Vorgänger die Referenznummer des Projekts, zu dem der Vorgänger gehört, und die Nummer der Aufgabe, getrennt durch einen Doppelpunkt.

      Das Symbol Vorgänger wird grün, wenn die Vorgängeraufgabe als abgeschlossen markiert ist. Dies signalisiert, dass die abhängige Aufgabe arbeitsbereit ist.

      Bewegen Sie den Mauszeiger über diesen Wert, um weitere Informationen über den Vorgänger, das Projekt und die Daten zu erhalten.

      ![Vorgängerdetails](assets/predecessor-details-in-task-list.png)

## Beispiele für Vorgängerwerte in einer Aufgabenliste {#examples-of-predecessor-values-in-a-task-list}

Wenn Sie Vorgänger in einer Liste von Aufgaben anzeigen, sehen Sie möglicherweise einen der folgenden Typen von Vorgängern mit ihren jeweiligen Abhängigkeitstypen und Verzögerungsbeträgen:

* **1fs -** Die Vorgänger-Aufgabennummer ist 1. Der Abhängigkeitstyp ist Beenden-Start. In der Projektzeitleiste wird diese Aufgabe sofort nach Abschluss von Aufgabe 1 gestartet. Trotzdem kann es als In Bearbeitung oder Abgeschlossen gekennzeichnet werden.
* **1 -** Die Vorgänger-Aufgabennummer ist 1. Dies ist dasselbe wie **1fs**, da **fs** die standardmäßige Vorgängerbeziehung in Workfront ist.

* **1fse -** Die Vorgänger-Aufgabennummer ist 1. Der Abhängigkeitstyp ist Beenden-Start-Erzwungen. In der Projekt-Zeitleiste wird diese Aufgabe als unmittelbar nach Abschluss von Aufgabe 1 beginnend angezeigt. Workfront lässt die Kennzeichnung als In Bearbeitung oder Abgeschlossen erst zu, wenn Aufgabe 1 abgeschlossen ist. Workfront lässt jedoch zu, dass zu dieser Aufgabe Stundenberichte erstellt werden.
* **1fs+3d -** Die Vorgänger-Aufgabennummer ist 1. Der Abhängigkeitstyp ist Beenden-Start mit einer Verzögerungszeit von 3 Tagen. In der Projekt-Zeitleiste wird diese Aufgabe 3 Arbeitstage nach Abschluss von Aufgabe 1 als gestartet angezeigt.
* **1fs-3d -** Die Vorgänger-Aufgabennummer ist 1. Der Abhängigkeitstyp ist Beenden-Start mit einer Verzögerungszeit von 3 Tagen. In der Projekt-Zeitleiste wird diese Aufgabe als 3 Werktage vor Abschluss der Vorgängeraufgabe angezeigt.
* **1fs+3de** - Die Vorgänger-Aufgabennummer ist 1. Der Abhängigkeitstyp ist Beenden-Start-Erzwungen mit einer Verzögerungszeit von 3 Tagen. In der Projekt-Zeitleiste wird diese Aufgabe 3 Arbeitstage nach Abschluss von Aufgabe 1 als gestartet angezeigt. Workfront lässt die Kennzeichnung als In Bearbeitung oder Abgeschlossen erst zu, wenn Aufgabe 1 abgeschlossen ist. Workfront lässt jedoch zu, dass zu dieser Aufgabe Stundenberichte erstellt werden.

  >[!NOTE]
  >
  >Sie müssen den erzwungenen Wert (**e**) zur Verzögerung und nicht zum Vorgänger hinzufügen.

* **4515:2** Die Vorgänger-Aufgabennummer ist 2. - Dies ist eine nicht erzwungene „Finish to Start“-Abhängigkeit mit dem Vorgänger im Projekt mit der Referenznummer **4515**.

## Anzeigen von Vorgängerinformationen

Sie können Vorgängerinformationen in den folgenden Bereichen von Workfront anzeigen. Dazu gehören Informationen zu projektübergreifenden Vorgängern:

* Auf Aufgabenebene, im Abschnitt Vorgänger .

  Informationen zum Anzeigen von Vorgängerinformationen im Abschnitt Vorgänger finden Sie im Abschnitt [Suchen der Vorgänger einer Aufgabe](#locate-the-predecessors-of-a-task) in diesem Artikel.

* Im Gantt-Diagramm.

  Weitere Informationen zur Anzeige von Vorgängern im Gantt-Diagramm finden Sie unter [Konfigurieren der Anzeige von Informationen im Gantt-Diagramm](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

* In einer Aufgabenliste.

  Um Informationen zu den Vorgängern Ihrer Aufgaben in einer Aufgabenliste anzuzeigen, haben Sie folgende Möglichkeiten:

   * Wenden Sie die integrierte Standardansicht in einer Aufgabenliste an.

     Informationen zum Anzeigen von Vorgängerinformationen in der Standardansicht finden Sie im Abschnitt [Suchen der Vorgänger einer Aufgabe](#locate-the-predecessors-of-a-task) in diesem Artikel.

   * Erstellen Sie eine Aufgabenansicht oder einen Bericht und fügen Sie dieser Ansicht die Spalte Vorgänger hinzu.

     Weitere Informationen zum Erstellen einer benutzerdefinierten Ansicht für Aufgaben mit Vorgängerinformationen finden Sie unter [Anzeigen: Vorgängerdetails](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-predecessor-details.md).

* In der Aufgabenkopfzeile beim Zugriff auf die Aufgabe.

  ![Vorgängerinformationen in der Aufgabenkopfzeile](assets/qs-predecessor-info-in-task-header-350x141.png)
