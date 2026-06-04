---
content-type: overview
product-area: projects
navigation-topic: task-information
title: '&grave;Kann beginnen&grave;-Übersicht für Aufgaben'
description: Wenn eine Aufgabe startbereit ist, fügt Adobe Workfront der Aufgabe einen Indikator „Kann starten“ hinzu, um leicht festzustellen, ob Sie mit der Arbeit an der Aufgabe beginnen können. Sie können diesen Indikator in der Ansicht einer Aufgabenliste oder eines Berichts anzeigen.
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
TQID: https://experienceleague.adobe.com/jb8Vj9wMNCQj31cgjHMIm6M0RH3VusK5jBdNx233yjw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 440
ht-degree: 1%

---

# Überblick über „Kann beginnen“ für Aufgaben

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
* Wenn eine Aufgabe einen projektübergreifenden Vorgänger hat, führt der Abschluss des Vorgängers nicht dazu, dass der Indikator „Kann starten“ automatisch auf den Nachfolger angewendet wird. Sie müssen die Zeitleiste des Nachfolgeprojekts manuell neu berechnen. Andernfalls muss Workfront sie automatisch neu berechnen, bevor die Nachfolgeaufgabe als Kann-Start-Aufgabe angezeigt wird. Weitere Informationen zur Neuberechnung der Projektzeitleisten finden Sie unter [Neuberechnen von Projektzeitleisten](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

  Informationen zu projektübergreifenden Vorgängern finden Sie unter [Erstellen von projektübergreifenden Vorgängern](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
