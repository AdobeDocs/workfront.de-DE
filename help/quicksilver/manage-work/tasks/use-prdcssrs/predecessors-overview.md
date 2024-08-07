---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Übersicht über die Vorgänger von Aufgaben
description: Ein Vorgänger ist die Aufgabe, von der eine andere Aufgabe (als Nachfolger oder abhängige Aufgabe bezeichnet) abhängt. Adobe Workfront unterstützt fünf Typen von Vorgängerabhängigkeiten.
author: Alina
feature: Work Management
exl-id: b2020a50-0921-4ed2-8a34-1a0411992b99
source-git-commit: d5f4e83badd4d011816551f06b056ffe886d3b17
workflow-type: tm+mt
source-wordcount: '1189'
ht-degree: 0%

---

# Übersicht über die Vorgänger von Aufgaben

<!--Audited: 12/2023-->

<!-- 

CONTEXT SENSITIVE HELP article. DO NOT CHANGE THE NAME OF THE ARTICLE/ DO NOT MOVE OR DELETE! -->

Ein Vorgänger ist die Aufgabe, von der eine andere Aufgabe (als Nachfolger oder abhängige Aufgabe bezeichnet) abhängt. Adobe Workfront unterstützt fünf Typen von Vorgängerabhängigkeiten. Informationen zu Vorgängerabhängigkeiten finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Übersicht über Vorgänger

Das Verständnis der Vorgängerfunktionalität ist wichtig, um die Zeitpläne in Ihren Projekten zu verstehen.

Aufgabenvorherigen Beziehungen bestehen sowohl zwischen Aufgaben innerhalb eines Projekts als auch zwischen Aufgaben aus verschiedenen Projekten.

Bei einer Abhängigkeit von mehreren Projekten können Sie projektübergreifende Vorläufer zwischen Aufgaben aus zwei verschiedenen Projekten erstellen.

Ob die Vorgänger- und Nachfolgeaufgaben zum selben Projekt oder zu zwei verschiedenen Projekten gehören, die Abhängigkeiten und die Zeitpläne der einzelnen Projekte werden auf die gleiche Weise berechnet.

Bei Vorgängern hat die Timeline des Projekts folgende Auswirkungen:

* Vorgängerabhängigkeit
* Launch-Wert und -Typ\
  Weitere Informationen zu Abhängigkeiten und Lagern finden Sie unter [Beispiele für Vorgängerwerte in einer Aufgabenliste](#examples-of-predecessor-values-in-a-task-list).

  Wenn beispielsweise Aufgabe A in einer Finish-Start-Beziehung eine Vorgängerin von Aufgabe B ist und Aufgabe B die Aufgabenbeschränkung so bald wie möglich hat, weist Workfront der Aufgabe B ein geplantes Startdatum unmittelbar nach dem geplanten Fertigstellungsdatum von Aufgabe A zu, unabhängig davon, ob der Vorgänger erzwungen wurde oder nicht.

Um die Vorgängerbeziehungen zu verstehen, müssen Sie Folgendes verstehen:

* **Abhängigkeitstypen:** Vorgänger sind durch verschiedene Abhängigkeitstypen verknüpft. Weitere Informationen zu Abhängigkeitstypen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

* **Erzwingen eines Vorgängers:** Bei der Erzwingung eines Vorgängers kann die Nachfolgeaufgabe unbedingt erst gestartet werden, nachdem der Vorgänger abgeschlossen ist. Die Nachfolgeaufgabe wird als unmittelbar nach Abschluss des Vorgängers gestartet.

  Wenn der Vorgänger nicht abgeschlossen (oder gestartet) ist und nicht durchgesetzt wird, kann die Nachfolgeaufgabe beginnen, aber die Projektzeitleiste wird weiterhin durch die Daten der Vorgänger- und der Nachfolgeaufgaben beeinflusst.

  Bei einem erzwungenen Vorgänger lässt Workfront die Kennzeichnung der Nachfolgeaufgabe als &quot;Wird ausgeführt&quot;oder &quot;Abgeschlossen&quot;zu, bis der Vorgänger abgeschlossen ist.

  Workfront lässt jedoch zu, dass Stunden für die Aufgabe gemeldet werden.\
  Weitere Informationen zum Erzwingen von Vorgängern finden Sie unter [Erzwingen von Vorgängern](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

* **Lages:** Sie können in Ihren Abhängigkeiten Pausen erstellen, die eine Verzögerung verursachen, die nach Abschluss einer Vorgängeraufgabe und bevor die Nachfolgeaufgabe beginnen kann, eintreten muss. Ebenen wirken sich auf die Zeitleiste des Projekts aus.

  Informationen zu den Latenztypen finden Sie unter [Übersicht über Lag-Typen](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

## Erstellen von Vorgängerbeziehungen

Informationen zum Erstellen von Vorgängern finden Sie in einem der folgenden Artikel:

* Informationen zum Einrichten von Vorgängern mithilfe der Registerkarte &quot;Vorgänger&quot;der Aufgabe finden Sie unter [Erstellen einer Vorgängerbeziehung im Bereich &quot;Vorgänger&quot;](../../../manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).
* Informationen zum Einrichten von Vorgängern in einer Aufgabenliste finden Sie unter [Erstellen einer Vorgängerbeziehung in der Aufgabenliste](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).
* Informationen zum Einrichten von Vorgängerbeziehungen durch Verketten von Aufgaben finden Sie unter [Erstellen von Vorgängerbeziehungen durch Verketten von Aufgaben](../../../manage-work/tasks/use-prdcssrs/create-predecessors-by-chaining-tasks.md).
* Informationen zum Einrichten projektübergreifender Vorgänger finden Sie unter [Erstellen projektübergreifender Vorgänger](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

## Suchen der Vorgänger einer Aufgabe {#locate-the-predecessors-of-a-task}

Führen Sie einen der folgenden Schritte aus, um die Vorgänger einer Aufgabe zu finden:

* Gehen Sie zum Projekt, an dem Sie arbeiten, und führen Sie die folgenden Schritte aus:

   1. Suchen Sie die Aufgabe, für die Sie die Vorgänger finden möchten, und klicken Sie auf die Aufgabe.
   1. Klicken Sie im linken Bereich auf **Vorgänger** . Möglicherweise müssen Sie auf **Mehr anzeigen** und dann auf **Vorgänger** klicken.
   1. Der Name des Projekts, auf dem sich der Vorgänger befindet, wird in der Spalte **Projekt** angezeigt.

      Die Zahl in der Spalte **#** gibt die vorherige Aufgabennummer an. Beispielsweise steht &quot;6&quot;für die sechste Aufgabe im Projekt.

      ![Abschnitt &quot;Vorgänger&quot;der Aufgabe](assets/predecessors-area-with-task-header.png)

* Gehen Sie zum Projekt, an dem Sie arbeiten, und führen Sie die folgenden Schritte aus:

   1. Klicken Sie auf die Registerkarte **Aufgaben**.
   1. Wählen Sie die **Standardansicht** oben in der Aufgabenliste aus.
   1. Die Spalte **Vorgänger** enthält die vorherigen Aufgabennummern.

      Bei einem projektübergreifenden Vorgänger zeigt die Spalte &quot;Vorgänger&quot;die Referenznummer des Projekts, zu dem der Vorgänger gehört, und die Nummer der Aufgabe, durch einen Doppelpunkt getrennt.

      Das Vorgängersymbol wird grün, wenn die Vorgängeraufgabe als abgeschlossen markiert ist. Dies signalisiert, dass die abhängige Aufgabe einsatzbereit ist.

      Bewegen Sie den Mauszeiger über diesen Wert, um weitere Informationen zum Vorgänger, zum Projekt und zu den Daten zu erhalten.

      ![Details des Vorgängers](assets/predecessor-details-in-task-list.png)

## Beispiele für Vorgängerwerte in einer Aufgabenliste {#examples-of-predecessor-values-in-a-task-list}

Wenn Sie Vorgänger in einer Liste von Aufgaben anzeigen, sehen Sie möglicherweise eine der folgenden Typen von Vorgängern mit den jeweiligen Abhängigkeitstypen und -schwellenwerten:

* **1fs -** Die Vorgänger-Aufgabennummer ist 1. Der Abhängigkeitstyp ist Finish-Start. In der Projekt-Timeline ist geplant, diese Aufgabe sofort nach Abschluss von Aufgabe 1 zu starten. Trotzdem kann es als &quot;Wird ausgeführt&quot;oder &quot;Fertig gestellt&quot;markiert werden.
* **1 -** Die Vorgänger-Aufgabennummer ist 1. Dies entspricht **1fs**, da **fs** die standardmäßige Vorgängerbeziehung in Workfront ist.

* **1fse -** Die Vorgänger-Aufgabennummer ist 1. Der Abhängigkeitstyp ist Finish-Start-Enforced. In der Projekt-Timeline wird diese Aufgabe als unmittelbar nach Abschluss von Aufgabe 1 gestartet. Workfront lässt die Kennzeichnung als In Bearbeitung oder Abgeschlossen erst zu, wenn Aufgabe 1 abgeschlossen ist. Workfront lässt jedoch zu, dass Stunden für die Aufgabe gemeldet werden.
* **1fs+3d -** Die vorherige Aufgabennummer ist 1. Der Abhängigkeitstyp ist Finish-Start mit einer Latenzzeit von 3 Tagen. In der Projekt-Timeline wird diese Aufgabe als drei Arbeitstage nach Abschluss von Aufgabe 1 angezeigt.
* **1fs-3d -** Die Vorgänger-Aufgabennummer ist 1. Der Abhängigkeitstyp ist Finish-Start mit einer Latenzzeit von 3 Tagen. In der Projekt-Timeline wird diese Aufgabe als drei Werktage vor Abschluss der Vorgängeraufgabe angezeigt.
* **1fs+3de** - Die vorherige Aufgabennummer ist 1. Der Abhängigkeitstyp ist &quot;Finish-Start-Enforced&quot;mit einer Latenzzeit von 3 Tagen. In der Projekt-Timeline wird diese Aufgabe als drei Arbeitstage nach Abschluss von Aufgabe 1 angezeigt. Workfront lässt es nicht zu, als &quot;Wird ausgeführt&quot;oder &quot;Abgeschlossen&quot;markiert zu werden, bis Aufgabe 1 abgeschlossen ist. Workfront lässt jedoch zu, dass Stunden für die Aufgabe gemeldet werden.

  >[!NOTE]
  >
  >Sie müssen den erzwungenen Wert (**e**) zum Lag und nicht zum Vorgänger hinzufügen.

* **4515:2** Die vorherige Aufgabennummer ist 2. - Dies ist eine nicht erzwungene Abhängigkeit vom Vorgänger im Projekt mit der Referenznummer **4515** vom Typ &quot;Finish to Start&quot;.

## Anzeigen von Vorgängerinformationen

Sie können die Vorgängerinformationen in den folgenden Bereichen von Workfront anzeigen. Dazu gehören Informationen zu projektübergreifenden Vorgängern:

* Auf Aufgabenebene im Abschnitt &quot;Vorgänger&quot;.

  Informationen zum Anzeigen von Vorgängerinformationen im Abschnitt &quot;Vorgänger&quot;finden Sie im Abschnitt [Vorgänger einer Aufgabe finden](#locate-the-predecessors-of-a-task) in diesem Artikel.

* In der Gantt-Grafik.

  Informationen zum Anzeigen von Vorgängern im Gantt-Diagramm finden Sie unter [Konfigurieren der Anzeige von Informationen im Gantt-Diagramm](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

* In einer Aufgabenliste.

  Um Informationen über die Vorgänger Ihrer Aufgaben in einer Aufgabenliste anzuzeigen, können Sie einen der folgenden Schritte ausführen:

   * Wenden Sie die integrierte Standardansicht in einer Liste von Aufgaben an.

     Informationen zum Anzeigen von Vorgängerinformationen in der Standardansicht finden Sie im Abschnitt [Vorgänger einer Aufgabe suchen](#locate-the-predecessors-of-a-task) in diesem Artikel.

   * Erstellen Sie eine Aufgabenansicht oder einen Bericht und fügen Sie dieser Ansicht die Spalte &quot;Vorgänger&quot;hinzu.

     Weitere Informationen zum Erstellen einer benutzerdefinierten Ansicht für Aufgaben mit Vorgängerinformationen finden Sie unter [Ansicht: Details des Vorgängers](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-predecessor-details.md).

* In der Aufgabenüberschrift beim Zugriff auf die Aufgabe.

  ![](assets/qs-predecessor-info-in-task-header-350x141.png)
