---
content-type: reference
product-area: projects
navigation-topic: task-information
title: Unterschied zwischen geplanter Dauer und Dauer für Aufgaben
description: Die Dauer ist die Zeit zwischen dem geplanten Start- und dem geplanten Abschlussdatum eines Arbeitselements. Aufgaben haben je nach Aufgabendauer eine Dauer und eine geplante Dauer in Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 183a3334-b4af-4f45-8e72-9e82ff3862a0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Unterschied zwischen geplanter Dauer und Dauer für Aufgaben

Die Dauer ist die Zeit zwischen dem geplanten Start- und dem geplanten Abschlussdatum eines Arbeitselements. Aufgaben haben je nach Aufgabendauer eine Dauer und eine geplante Dauer in Adobe Workfront.

Probleme und Projekte können nicht mit einem Dauer-Typ verknüpft werden und haben nur eine Dauer.

## Aufgabendauer

Für Aufgaben zeigen die Dauer und die geplante Dauer in der Regel denselben Wert an: die Zeitspanne zwischen dem geplanten Startdatum und dem geplanten Abschlussdatum einer Aufgabe.

Wenn der Aufgabentyp &quot;Aufwandsgesteuert&quot;lautet, wird die geplante Dauer beim Hinzufügen von Ressourcen zur Aufgabe reduziert.

**Beispiel:** Wenn eine Aufgabe mit dem Typ Dauer des Aufwands Driven eine Dauer von 3 Tagen hat und Sie der Aufgabe eine Ressource mit einem vollen Zeitplan zuweisen, beträgt die geplante Dauer ebenfalls 3 Tage.

Wenn Sie derselben Aufgabe drei Ressourcen mit einem vollständigen Zeitplan zuweisen, bleibt die Dauer 3 Tage, die geplante Dauer jedoch 1 Tag. Die geplante Dauer ändert außerdem das geplante Start- und das geplante Abschlussdatum der Aufgabe, um die neue geplante Dauer widerzuspiegeln. Daher ist auch die Timeline des Projekts betroffen.
Sie können den Typ Ermüdungsgesteuerte Dauer verwenden, wenn Sie eine Aufgabe mehreren Ressourcen zuweisen. Auf diese Weise wird der Zeitaufwand für die Bearbeitung der Aufgabe reduziert.

Weitere Informationen zum Typ der anfechtbaren Dauer finden Sie unter [Übersicht über den Durationstyp: Aufwandsorientiert](../../../manage-work/tasks/taskdurtn/effort-driven.md).

## Problem und Projektdauer

Probleme und Projekte haben nur einen Wert für die Dauer, was der Unterschied zwischen dem geplanten Startdatum und dem geplanten Abschlussdatum des Problems bzw. des Projekts ist.
