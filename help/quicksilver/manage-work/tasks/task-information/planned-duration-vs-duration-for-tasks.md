---
content-type: reference
product-area: projects
navigation-topic: task-information
title: Unterschied zwischen geplanter Dauer und Dauer für Aufgaben
description: Die Dauer ist der Zeitraum zwischen dem geplanten Start- und dem geplanten Abschlussdatum eines Arbeitselements. Die Aufgaben haben in Adobe Workfront je nach Art der Dauer eine Dauer und eine geplante Dauer.
author: Alina
feature: Work Management
exl-id: 183a3334-b4af-4f45-8e72-9e82ff3862a0
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Unterschied zwischen geplanter Dauer und Dauer für Aufgaben

Die Dauer ist der Zeitraum zwischen dem geplanten Start- und dem geplanten Abschlussdatum eines Arbeitselements. Die Aufgaben haben in Adobe Workfront je nach Art der Dauer eine Dauer und eine geplante Dauer.

Probleme und Projekte können nicht mit einem Dauertyp verknüpft werden und haben nur eine Dauer.

## Aufgabendauer

Für Aufgaben weisen die Dauer und die geplante Dauer normalerweise denselben Wert auf: die Zeitdauer zwischen dem geplanten Startdatum und dem geplanten Abschlussdatum einer Aufgabe.

Wenn der Dauertyp der Aufgabe leistungsgesteuert ist, verringert sich die geplante Dauer, wenn Sie Ressourcen zur Aufgabe hinzufügen.

**Beispiel** Wenn ein Vorgang mit dem Dauertyp „Arbeitsaufwand gesteuert“ eine Dauer von 3 Tagen hat und Sie dem Vorgang eine Ressource mit einem Vollzeitplan zuweisen, beträgt die geplante Dauer ebenfalls 3 Tage.

Wenn Sie derselben Aufgabe drei Ressourcen mit einem Vollzeitplan zuweisen, bleibt die Dauer 3 Tage, aber die geplante Dauer wird zu 1 Tag. Die geplante Dauer ändert auch die geplanten Start- und Abschlussdaten der Aufgabe, um die neue geplante Dauer widerzuspiegeln. Daher ist auch die Zeitleiste des Projekts betroffen.
Sie können den leistungsgesteuerten Dauertyp verwenden, wenn Sie eine Aufgabe mehreren Ressourcen zuweisen. Dadurch wird der Zeitaufwand für den Abschluss der Arbeit an der Aufgabe reduziert.

Weitere Informationen über den Typ der leistungsgesteuerten Dauer finden Sie unter [Übersicht über den Dauertyp: Leistungsgesteuert](../../../manage-work/tasks/taskdurtn/effort-driven.md).

## Anfrage- und Projektdauer

Anfragen und Projekte haben nur einen einzigen Wert für die Dauer, nämlich die Differenz zwischen dem geplanten Startdatum und dem geplanten Abschlussdatum der Anfrage bzw. des Projekts.
