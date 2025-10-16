---
content-type: overview
product-area: projects
navigation-topic: task-information
title: '&grave;Kann beginnen&grave;-Übersicht für Aufgaben'
description: Wenn eine Aufgabe startbereit ist, fügt Adobe Workfront der Aufgabe einen Indikator „Kann starten“ hinzu, um leicht festzustellen, ob Sie mit der Arbeit an der Aufgabe beginnen können. Sie können diesen Indikator in der Ansicht einer Aufgabenliste oder eines Berichts anzeigen.
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# Überblick „Kann starten“ für Aufgaben

Wenn eine Aufgabe startbereit ist, fügt Adobe Workfront der Aufgabe einen Indikator „Kann starten“ hinzu, um leicht festzustellen, ob Sie mit der Arbeit an der Aufgabe beginnen können. Sie können diesen Indikator in der Ansicht einer Aufgabenliste oder eines Berichts anzeigen.

Wenn die Aufgabe fertig zur Bearbeitung ist, wird das Feld Kann starten der Aufgabe auf True gesetzt.

## Wie Workfront eine Aufgabe als „Kann beginnen“ kennzeichnet

Workfront sucht nach den folgenden Elementen, bevor eine Aufgabe für das Feld „Kann starten“ als „true“ markiert wird:

* Ob der Wert von für das übergeordnete Element auf „True“ gesetzt werden kann, wenn die Aufgabe ein übergeordnetes Element hat. Wenn der Wert für das übergeordnete Element „false“ ist, kann für alle Teilaufgaben der Wert „can start“ ebenfalls auf „false“ festgelegt werden.
* Ob die Vorgänger der Aufgabe sowie die Vorgänger ihrer Eltern abgeschlossen sind. Wenn sie abgeschlossen sind, wird der Wert „Kann starten“ für die Aufgabe auf „True“ gesetzt. Wenn einer der Aufgabenvorgänger oder die Vorgänger seiner Eltern nicht abgeschlossen sind oder den Status „Genehmigung abgeschlossen - Ausstehende Genehmigung“ aufweisen, wird der Wert „Kann starten“ für die Aufgabe auf „False“ gesetzt.
* Gibt an, ob der Aufgabenabhängigkeitstyp entweder „Start-Start“ oder „Start-Ende“ ist. Wenn der Abhängigkeitstyp „Start-Start“ oder „Start-Ende“ ist, wird die Markierung „Kann starten“ für die abhängige Aufgabe auf „True“ gesetzt, nachdem die Vorgängeraufgabe in Bearbeitung ist (oder nachdem der Prozentsatz der Fertigstellung der Vorgängeraufgabe größer als 1 % ist).

  Informationen zu Aufgabenvorgängen finden Sie unter [Übersicht über Aufgabenvorgänge](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Überlegungen zur Identifizierung von Aufgaben, die startbereit sind

* Wenn der Abhängigkeitstyp zwischen einer Aufgabe und ihren Vorgängern „Start-Start“ ist, muss der Vorgänger beginnen, bevor die Vorgängerbeziehung als gelöst betrachtet wird und die Nachfolgeaufgaben beginnen können. Informationen zu Abhängigkeitstypen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).
* Trigger Wenn eine Aufgabe einen projektübergreifenden Vorgänger hat, führt der Abschluss des Vorgängers nicht dazu, dass der Indikator „Kann starten“ automatisch auf den Nachfolger angewendet wird. Sie müssen die Zeitleiste des Nachfolgeprojekts manuell neu berechnen. Andernfalls muss Workfront sie automatisch neu berechnen, bevor die Nachfolgeaufgabe als Kann-Start-Aufgabe angezeigt wird. Weitere Informationen zur Neuberechnung der Projektzeitleisten finden Sie unter [Neuberechnen von Projektzeitleisten](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

  Informationen zu projektübergreifenden Vorgängern finden Sie unter [Erstellen von projektübergreifenden Vorgängern](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
