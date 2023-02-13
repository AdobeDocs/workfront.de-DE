---
content-type: overview
product-area: projects
navigation-topic: task-information
title: '"Can Start" - Übersicht über Aufgaben'
description: Wenn eine Aufgabe startbereit ist, fügt Adobe Workfront der Aufgabe einen "Kann starten"-Indikator hinzu, um leicht erkennen zu können, ob es für Sie sicher ist, mit der Arbeit zu beginnen. Sie können diesen Indikator in der Ansicht einer Aufgabenliste oder eines Berichts anzeigen.
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# &quot;Can Start&quot;-Übersicht für Aufgaben

Wenn eine Aufgabe startbereit ist, fügt Adobe Workfront der Aufgabe einen &quot;Kann starten&quot;-Indikator hinzu, um leicht erkennen zu können, ob es für Sie sicher ist, mit der Arbeit zu beginnen. Sie können diesen Indikator in der Ansicht einer Aufgabenliste oder eines Berichts anzeigen.

Wenn die Aufgabe bereit für die Bearbeitung ist, ist das Feld Kann starten für die Aufgabe auf True eingestellt.

## So kennzeichnet Workfront eine Aufgabe als &quot;Kann starten&quot;

Workfront sucht nach den folgenden Elementen, bevor eine Aufgabe für das Feld Kann starten als True markiert wird:

* Wenn die Aufgabe über eine übergeordnete Aufgabe verfügt, wird überprüft, ob der Wert Kann starten für die übergeordnete Aufgabe True hat. Wenn der Wert für das übergeordnete Element False ist, haben alle Unteraufgaben auch den Wert &quot;Can Start&quot;auf &quot;False&quot; gesetzt. 
* Es prüft auch, ob die Vorgänger der Aufgabe sowie die Vorgänger ihrer Eltern vollständig sind. Wenn sie abgeschlossen sind, wird der Kann-Start-Wert für die Aufgabe auf True gesetzt. Wenn einer der Aufgabenverfasser oder der Vorgänger der übergeordneten Elemente nicht abgeschlossen ist oder den Status &quot;Genehmigung abgeschlossen/ausstehend&quot;aufweist, wird der Wert Kann starten für die Aufgabe auf &quot;False&quot;gesetzt. 

   Weitere Informationen zu Aufgabenvorgängen finden Sie unter [Übersicht über die Vorgänger von Aufgaben](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Überlegungen zur Identifizierung von Aufgaben, die startbereit sind

* Wenn der Abhängigkeitstyp zwischen einer Aufgabe und ihren Vorgängern Start-Start ist, muss der Vorgänger beginnen, bevor die Vorgängerbeziehung als aufgelöst betrachtet wird und die Nachfolgeaufgaben beginnen können. Weitere Informationen zu Abhängigkeitstypen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).
* Wenn eine Aufgabe über einen projektübergreifenden Vorgänger verfügt, wird nach Abschluss des Vorgängers die Kann-Start-Anzeige nicht Trigger, sodass sie automatisch auf den Nachfolger angewendet wird. Sie müssen die Timeline des Nachfolgeprojekts manuell neu berechnen oder Workfront muss es automatisch neu berechnen, bevor die Nachfolgeaufgabe als Kann-Start-Aufgabe angezeigt wird. Weitere Informationen zur Neuberechnung von Projektzeitplänen finden Sie unter [Projektzeitpläne neu berechnen](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

   Weitere Informationen zu projektübergreifenden Vorgängern finden Sie unter [Erstellen projektübergreifender Vorgänger](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
