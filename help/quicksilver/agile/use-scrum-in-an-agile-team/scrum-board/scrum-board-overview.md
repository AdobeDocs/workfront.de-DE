---
content-type: overview
product-area: agile-and-teams
navigation-topic: scrum-board
title: Übersicht über die Pinnwand
description: Die Landkarte Scrum-Geschichte wird zusammen mit dem Abschlussstatus und der Burndown-Grafik angezeigt.
author: Lisa
feature: Agile
exl-id: 584288bb-2d98-4b69-8deb-d3b8e54d328c
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# Überblick über die [!UICONTROL Scrum]-Pinnwand

Das agile Storyboard [!UICONTROL Scrum] wird zusammen mit dem Abschlussstatus und dem Burndown-Diagramm angezeigt. Diese agilen Komponenten sind in den folgenden Situationen in [!UICONTROL Adobe Workfront] verfügbar:

* Bei agilen Iterationen. Weitere Informationen zur Verwendung des agilen Story Pards, des Burndown-Diagramms und des Abschlussstatus in einer reinen agilen Umgebung (mit Rückständen und einer Iteration) finden Sie unter [Arbeiten in einer agilen Umgebung](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).
* Beim Anzeigen eines Projekts in einer agilen Ansicht. Informationen dazu, wie Sie das agile Storyboard, das Burndown-Diagramm und den Abschlussstatus innerhalb eines vorhandenen Projekts nutzen können, finden Sie unter [Projekt in der Agile-Ansicht verwalten](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

![Agile iteration](assets/agile-iteration-with-callouts.png)

## Layout und Funktionen von Meldungsfenstern

![Agile-Story-Pinnwand](assets/agile-storyboard-callouts.png)

Das Storyboard besteht aus folgenden Elementen:

* **[!UICONTROL Übergeordnete Meldung] Spalte:** Im Gegensatz zu den anderen Spalten auf der Storyboard-Pinnwand ist die Spalte [!UICONTROL Übergeordnete Meldung] kein Aufgabenstatus, sondern besteht darin, Meldungen zu unterteilen, die Unteraufgaben in der Iteration oder dem Projekt enthalten. In dieser Spalte können sich nur übergeordnete Meldungen befinden, die mindestens eine Unteraufgabe auf dem Storyboard haben. Die übergeordneten Geschichten selbst wechseln nicht von Status zu Status über die gesamte Geschichte hinweg.

  In einer Iteration erscheint diese Spalte nur dann auf der Storyboard-Pinnwand, wenn ein oder mehrere Storys auf der Storyboard mindestens eine Unteraufgabe enthält, die die folgenden Anforderungen erfüllt:

   * Dieselbe agile Team wie die übergeordnete Aufgabe zugewiesen
   * gehört zur Iteration

     In einem Projekt erscheint diese Spalte jedes Mal, wenn eine Aufgabe mindestens eine Unteraufgabe hat.

     ![Übergeordnete Story-Spalte](assets/agile-parentstory-swimlane.png)

* **Aufgabenstatus:** Geben Sie an, wie sich eine Geschichte durch die Iteration oder das Projekt entwickelt, basierend darauf, in welcher Statusspalte sich die Geschichte befindet.

  Aufgabenstatus können für das Projekt angepasst werden, indem die agile Ansicht geändert wird, wie unter Erstellen oder Anpassen einer Agile-Ansicht ](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in der Übersicht über Ansichten in [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md) beschrieben.[[

* **Swim Lane:** Wenn eine übergeordnete Meldung und ihre Unteraufgaben auf der Storyboard erscheinen, wird eine Swim-Spur speziell für die Geschichte und ihre Unteraufgaben erstellt. Dies bietet eine visuelle Unterscheidung, um besser zu sehen, wie die Unteraufgaben einer Geschichte über die gesamte Geschichte hinweg weitergehen.

  In einer Iteration erscheinen Swim-Spuren nur dann auf dem Storyboard, wenn eine Geschichte auf dem Storyboard mindestens eine Unteraufgabe enthält, die die folgenden Anforderungen erfüllt:

   * Dieselbe agile Team wie die übergeordnete Aufgabe zugewiesen
   * gehört zur Iteration

  In einem Projekt werden Schwimmspuren immer dann angezeigt, wenn eine Aufgabe mindestens eine Unteraufgabe oder eine übergeordnete Aufgabe hat.

* **Individuelle Geschichten:** Einzelne Geschichten und Probleme werden unter allen Swim-Spuren auf dem Storyboard angezeigt. Dies unterscheidet visuell von den Geschichten, die Teil einer Swim-Spur sind.

## Beziehung zwischen Unteraufgaben und Meldungen

Wenn eine Geschichte Unteraufgaben enthält, können Sie keine Informationen über die übergeordnete Meldung selbst aktualisieren (z. B. Punkte/Stunden oder Prozentsatz der Vollständigkeit). Außerdem können Sie die Geschichte nicht über die gesamte Seite verschieben, um ihren Status zu aktualisieren. Stattdessen spiegeln sich alle Änderungen, die Sie an den Unteraufgaben der Geschichte vornehmen, in der Geschichte wider. Die kombinierten Story-Punkte oder -Stunden für alle Unteraufgaben bestimmen die Punkte oder Stunden der übergeordneten Story.

Wenn zum Beispiel eine Geschichte nur eine Unteraufgabe an 4 Punkten bewertet hat, hat die Geschichte selbst auch 4 Punkte. Wenn Sie den Wert des Unteraufgabepunkts auf 3 ändern, wird der Punktwert der übergeordneten Meldung auf 3 geändert. Wenn Sie eine weitere Unteraufgabe für denselben Artikel erstellen und den Punktwert für diese Unteraufgabe auf 4 setzen, wird der Punktwert für den Artikel auf 7 geändert, um den kombinierten Punktwert für beide Unteraufgaben widerzuspiegeln.

Dasselbe gilt für Unteraufgaben der zweiten Ebene (Unteraufgaben von Unteraufgaben). Wenn eine Unteraufgabe eine oder mehrere Unteraufgaben der zweiten Ebene enthält, wird die Unteraufgabe anhand der Unteraufgaben der zweiten Ebene berechnet.

## Beziehung zwischen dem Meldungsbrett und dem Rückholprotokoll

>[!NOTE]
>
>Die Informationen in diesem Abschnitt gelten nur für agile Ansichten bei einer Iteration; agile Ansichten in einem Projekt verwenden keinen Rückstand. (Weitere Informationen zu den Unterschieden zwischen agilen Ansichten bei einer Iteration und einem Projekt finden Sie unter &quot;Unterschiede bei der Verwendung der [!UICONTROL Agile]-Ansicht auf einer Projektansicht auf eine Iteration&quot;in [Projekt in der Agile-Ansicht verwalten](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).)

Der Iterations-Backlog zeigt nur Meldungen oder Unteraufgaben an, in denen Sie eine Schätzung festlegen können. Wenn eine übergeordnete Meldung Unteraufgaben enthält, die auf der Story-Pinnwand angezeigt werden (weil sie demselben agilen Team zugewiesen sind und zur Iteration gehören), wird die übergeordnete Aufgabe nicht im Rückstand angezeigt. In diesem Fall werden nur die Unteraufgaben im Rückstand angezeigt, während die Unteraufgaben und der übergeordnete Verlauf auf dem Storyboard angezeigt werden.

Angenommen, Geschichte A enthält Unteraufgabe 1 und Unteraufgabe 2 (und beide Unteraufgaben werden demselben agilen Team zugewiesen). In diesem Fall wird Story A auf dem Storyboard in einer Swim-Spur mit Unteraufgabe 1 und Unteraufgabe 2 angezeigt. Allerdings werden nur die Unteraufgabe 1 und die Unteraufgabe 2 im Backlog angezeigt.

Dasselbe gilt für Unteraufgaben der zweiten Ebene (Unteraufgaben von Unteraufgaben). Wenn einer Unteraufgabe eine oder mehrere Unteraufgaben der zweiten Ebene demselben agilen Team zugewiesen sind und zur Iteration gehören, wird nur die Unteraufgabe der zweiten Ebene im Backlog angezeigt.

Weitere Informationen zum Rückstand finden Sie unter [Verwalten des agilen Rückstands-Logs](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).
