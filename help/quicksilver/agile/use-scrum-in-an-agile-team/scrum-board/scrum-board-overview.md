---
content-type: overview
product-area: agile-and-teams
navigation-topic: scrum-board
title: Scrum Board - Übersicht
description: Das Agile-Story-Board von Scrum wird zusammen mit dem Abschlussstatus und dem Burndown-Diagramm angezeigt.
author: Jenny
feature: Agile
exl-id: 584288bb-2d98-4b69-8deb-d3b8e54d328c
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 0%

---

# Übersicht über [!UICONTROL Scrum]-Board

<!-- Audited: 5/2025 -->

Das [!UICONTROL Scrum] Agile-Story-Board wird zusammen mit dem Abschlussstatus und dem Burndown-Diagramm angezeigt. Diese Agile-Komponenten sind in den folgenden Situationen in [!UICONTROL Adobe Workfront verfügbar]:

* Bei agilen Iterationen. Weitere Informationen zur Verwendung des Agile-Story-Boards, des Burndown-Diagramms und des Abschlussstatus in einer rein agilen Umgebung (mit Rückständen und einer Iteration) finden Sie unter [Arbeiten in einer agilen Umgebung](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).
* Beim Anzeigen eines Projekts in einer Agile-Ansicht. Informationen dazu, wie Sie das Agile-Story-Board, das Burndown-Diagramm und den Abschlussstatus in einem vorhandenen Projekt nutzen können, finden Sie unter [Verwalten eines Projekts in der Agile-Ansicht](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

![Agile Iteration](assets/agile-iteration-with-callouts.png)

## Layout und Funktionen des Story Boards

![Agile-Story-Board](assets/agile-storyboard-callouts.png)

Das Story Board besteht aus folgenden Elementen:

* **Übergeordnete Story-Spalte**: Im Gegensatz zu den anderen Spalten auf dem Story Board ist die Spalte [!UICONTROL Übergeordnete Story] kein Aufgabenstatus, sondern dient zur Unterbringung von Storys, die Unteraufgaben in der Iteration oder im Projekt enthalten. Nur übergeordnete Storys, die mindestens eine Unteraufgabe auf dem Storyboard haben, können sich in dieser Spalte befinden. Die übergeordneten Storys selbst wechseln nicht über das Storyboard hinweg vom Status zum Status .

  In einer Iteration wird diese Spalte nur dann im Story Board angezeigt, wenn mindestens eine Story Board mindestens eine Teilaufgabe enthält, die die folgenden Anforderungen erfüllt:

   * Diesem Agile-Team wie die übergeordnete Aufgabe zugewiesen.
   * Gehört zur Iteration.

     In einem Projekt wird diese Spalte immer dann angezeigt, wenn eine Aufgabe mindestens eine Teilaufgabe hat.

     ![Übergeordnete Story-Spalte](assets/agile-parentstory-swimlane.png)

* **Aufgabenstatus**: Gibt an, wie eine Story durch die Iteration oder das Projekt verläuft, je nachdem, in welcher Statusspalte sich die Story befindet.

  Der Aufgabenstatus kann für das Projekt angepasst werden, indem die Agile-Ansicht geändert wird.

* **Schwimmspur**: Wenn eine übergeordnete Story und ihre Unteraufgaben auf dem Storyboard angezeigt werden, wird eine Schwimmspur speziell für die Story und ihre Unteraufgaben erstellt. Dies bietet eine visuelle Unterscheidung, um besser zu erkennen, wie die Unteraufgaben einer Story über die Story-Tafel hinweg voranschreiten.

  In einer Iteration werden Schwimmspuren nur dann auf dem Story Board angezeigt, wenn eine Story auf dem Story Board mindestens eine Teilaufgabe enthält, die die folgenden Anforderungen erfüllt:

   * Diesem Agile-Team wie die übergeordnete Aufgabe zugewiesen.
   * Gehört zur Iteration.

  In einem Projekt werden Schwimmspuren immer dann angezeigt, wenn eine Aufgabe mindestens eine Unteraufgabe oder eine übergeordnete Aufgabe hat.

* **Individuelle Geschichten**: Einzelne Geschichten und Probleme werden unter allen Schwimmspuren auf dem Storyboard angezeigt. Dies bietet eine visuelle Unterscheidung zu den Geschichten, die Teil einer Schwimmspur sind.

## Beziehung zwischen Teilaufgaben und Storys

Wenn eine Story Unteraufgaben enthält, können Sie keine Informationen zur übergeordneten Story selbst aktualisieren (z. B. Punkte/Stunden oder Prozent abgeschlossen). Außerdem können Sie die Story nicht über die Story verschieben, um ihren Status zu aktualisieren. Stattdessen werden alle Änderungen, die Sie an den Unteraufgaben der Story vornehmen, in der Story widergespiegelt. Die kombinierten Story-Punkte oder -Stunden für alle Teilaufgaben bestimmen die Punkte oder Stunden der übergeordneten Story.

Wenn beispielsweise eine Story nur eine Teilaufgabe mit 4 Punkten hat, hat die Story selbst auch 4 Punkte. Wenn Sie den Punktwert für die Teilaufgabe in 3 ändern, wird der Punktwert der übergeordneten Story in 3 geändert. Wenn Sie eine weitere Teilaufgabe für dieselbe Story erstellen und den Punktwert für diese Teilaufgabe auf 4 setzen, wird der Punktwert für die Story auf 7 geändert, um den kombinierten Punktwert für beide Teilaufgaben widerzuspiegeln.

Dieselbe Logik gilt für Teilaufgaben der zweiten Ebene (Teilaufgaben von Teilaufgaben). Wenn eine Unteraufgabe eine oder mehrere Unteraufgaben der zweiten Ebene aufweist, wird die Unteraufgabe basierend auf den Unteraufgaben der zweiten Ebene berechnet.

## Beziehung zwischen dem Story Board und dem Auftragsbestand

Der Iterationsrückstand zeigt nur Storys oder Unteraufgaben an, für die Sie einen Kostenvoranschlag festlegen können. Wenn eine übergeordnete Story Unteraufgaben aufweist, die auf dem Story Board angezeigt werden (da sie demselben Agile-Team zugewiesen sind und zur Iteration gehören), wird die übergeordnete Aufgabe nicht im Rückstand angezeigt. In diesem Fall werden nur die Unteraufgaben im Rückstand angezeigt, während die Unteraufgaben und die übergeordnete Story auf dem Story Board angezeigt werden.

Angenommen, Story A enthält Unteraufgabe 1 und Unteraufgabe 2 (und beide Unteraufgaben werden demselben Agile-Team zugewiesen). In diesem Fall wird Story A auf dem Storyboard in einer Schwimmspur mit Unteraufgabe 1 und Unteraufgabe 2 angezeigt. Im Rückstand werden jedoch nur Teilaufgabe 1 und Teilaufgabe 2 angezeigt.

Dieselbe Logik gilt für Teilaufgaben der zweiten Ebene (Teilaufgaben von Teilaufgaben). Wenn eine Unteraufgabe eine oder mehrere Unteraufgaben der zweiten Ebene demselben Agile-Team zugewiesen hat und zur Iteration gehören, wird nur die Unteraufgabe der zweiten Ebene im Rückstand angezeigt.

Weitere Informationen zum Auftragsbestand finden Sie unter [Verwalten des agilen Auftragsbestands](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).
