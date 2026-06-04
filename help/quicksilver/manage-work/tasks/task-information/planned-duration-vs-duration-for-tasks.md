---
content-type: reference
product-area: projects
navigation-topic: task-information
title: Unterschied zwischen geplanter Dauer und Dauer für Aufgaben
description: Die Dauer ist der Zeitraum zwischen dem geplanten Start- und dem geplanten Abschlussdatum eines Arbeitselements. Die Aufgaben haben in Adobe Workfront je nach Art der Dauer eine Dauer und eine geplante Dauer.
author: Alina
feature: Work Management
exl-id: 183a3334-b4af-4f45-8e72-9e82ff3862a0
TQID: https://experienceleague.adobe.com/tVh55DKoBvOUZdq9lZ6y72rxZQ1WOoAYL-Pz8nlU588
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
source-wordcount: 272
ht-degree: 2%

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
