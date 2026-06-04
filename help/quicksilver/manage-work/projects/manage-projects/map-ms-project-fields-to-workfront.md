---
product-area: projects
navigation-topic: manage-projects
title: Zuordnen von Microsoft-Projektfeldern zu Adobe Workfront-Projekten
description: Projekte in Adobe Workfront und Microsoft Project sind größtenteils kompatibel. In diesem Artikel wird beschrieben, wie sich die häufigsten Projektfelder der beiden Anwendungen gegenseitig zuordnen.
author: Alina
feature: Work Management
exl-id: 381eb6ad-8084-406b-90f9-44460b58a04c
TQID: https://experienceleague.adobe.com/WdFf5O8kKyY43PsHLEINDaLzsEa0idHZPNz83O12bTI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 396
ht-degree: 6%

---

# Zuordnen von Microsoft Project-Feldern zu Adobe Workfront-Projekten

Projekte in Adobe Workfront und Microsoft Project sind größtenteils kompatibel. Mithilfe der beiden Anwendungen können Sie Folgendes tun:

* Exportieren von Projekten aus dem Microsoft-Projekt und Importieren in Workfront
* Exportieren Sie Projekte aus Workfront und importieren Sie sie in Microsoft Project.

Weitere Informationen zum Importieren von Projekten aus Microsoft Project in Workfront finden Sie unter [Importieren eines Projekts aus Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

Weitere Informationen zum Exportieren eines Projekts aus Workfront zum Importieren in Microsoft Project finden Sie unter [Exportieren eines Projekts in Microsoft Project](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md).

Bei solchen Datenimporten müssen Sie wissen, wie die Informationen von einer Anwendung in die andere übertragen werden. In den meisten Fällen müssen Sie nach Abschluss des Imports einige manuelle Änderungen am Projekt vornehmen.

## Übersicht über die Feldzuordnung

>[!NOTE]
>
>Die geplanten Termine stimmen nicht immer zwischen beiden Systemen überein. Abweichungen können durch den Zeitplan und Unterschiede in den Systemvoreinstellungen zwischen Workfront und Microsoft Project berücksichtigt werden. Diese Datumsdiskrepanzen können auch zu Unterschieden bei Aufwand, Dauer und Prozentsatz der Fertigstellung führen.

| **Microsoft-Projektfeld** | **Workfront-Feld** |
|---|---|
| Projekttitel | Projektname |
| Start- und Enddaten | Geplante Start- und Abschlussdaten |
| Aufgabenname | Aufgabenname |
| Aufgabendauer | Geplante Aufgabendauer |
| Aufgabenarbeit | Geplante Stunden der Aufgabe |
| Aufgabe % abgeschlossen | Aufgabe % abgeschlossen (basierend auf der Dauer der Aufgabe) |
| Aufgabenarbeit % abgeschlossen | Aufgabe % abgeschlossen (basierend auf den geplanten Stunden der Aufgabe) |
| Geplanter Anfang und Ende | Geplante Start- und Abschlussdaten |
| Tatsächlicher Start und tatsächliches Ende | Tatsächliche Start- und Abschlussdaten |
| Ressourcenname | Aufgabenzuweisung |
| Zuordnungseinheiten | Zuweisungsprozentsatz |
| Aufgabennotiz | Aufgabenbeschreibung |
| Vorgänger | Vorgänger |

## Übersicht über nicht enthaltene Daten

Es gibt eine Reihe von Projektfeldern, die nicht in Workfront importiert oder aus exportiert werden.

Zu diesen Feldern gehören unter anderem:

* Dokumentanhänge
* Benutzerdefinierte Felder (auf Projekt- oder Aufgabenebene)
* Workfront-Hinweise
* Probleme
* Negative Verzögerung bei Aufgaben mit einer Vorgängerbeziehung Start/Ende (Aufgaben werden ohne Verzögerung importiert)
* Arbeitsaufträge
* Aufgabenbeschränkungen

  >[!NOTE]
  >
  >Da Einschränkungen nicht zwischen Microsoft Project und Workfront zugeordnet sind, stellen Sie sicher, dass Vorgängerbeziehungen zwischen den Aufgaben vorhanden sind. Andernfalls sind das geplante Start- und Abschlussdatum der Aufgaben im importierten Projekt möglicherweise nicht korrekt.
