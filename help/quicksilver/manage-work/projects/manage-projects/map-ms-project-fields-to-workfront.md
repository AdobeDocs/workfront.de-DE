---
product-area: projects
navigation-topic: manage-projects
title: Zuordnen von Microsoft-Projektfeldern zu Adobe Workfront-Projekten
description: Projekte im Adobe Workfront- und Microsoft-Projekt sind größtenteils kompatibel. In diesem Artikel wird beschrieben, wie die am häufigsten verwendeten Projektfelder von den beiden Anwendungen einander zugeordnet werden.
author: Alina
feature: Work Management
exl-id: 381eb6ad-8084-406b-90f9-44460b58a04c
source-git-commit: c566eb094e96abca6073554433434822c567bc34
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 3%

---

# Zuordnen von Microsoft-Projektfeldern zu Adobe Workfront-Projekten

Projekte im Adobe Workfront- und Microsoft-Projekt sind größtenteils kompatibel. Mithilfe der beiden Anwendungen haben Sie folgende Möglichkeiten:

* Exportieren von Projekten aus Microsoft Project und Importieren in Workfront
* Exportieren Sie Projekte aus Workfront und importieren Sie sie in Microsoft Project. 

Weitere Informationen zum Importieren von Projekten aus Microsoft Project in Workfront finden Sie unter [Importieren eines Projekts aus einem Microsoft-Projekt](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

Weitere Informationen zum Exportieren eines Projekts aus Workfront zum Importieren in Microsoft Project finden Sie unter [Projekt in ein Microsoft-Projekt exportieren](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md).

Bei der Durchführung solcher Datenimporte ist es wichtig zu verstehen, wie Informationen von einer Anwendung zur anderen übersetzt werden. In den meisten Fällen müssen Sie nach Abschluss des Imports einige manuelle Änderungen am Projekt vornehmen. 

## Übersicht über die Feldzuordnung

>[!NOTE]
>
>Die geplanten Daten entsprechen nicht immer zwischen beiden Systemen. Diskrepanzen können über einen Zeitplan und Unterschiede bei den Systemvoreinstellungen zwischen Workfront und Microsoft Project berücksichtigt werden. Diese Diskrepanzen beim Datum können auch zu Unterschieden in Aufwand, Dauer und Prozentsatz der Fertigstellung führen.

| **Microsoft-Projektfeld** | **Workfront Field** |
|---|---|
| Projekttitel | Projektname |
| Start- und Enddatum | Geplante Start- und Enddaten |
| Aufgabenname | Aufgabenname |
| Aufgabendauer | Geplante Dauer der Aufgabe |
| Aufgabenarbeit | Geplante Stunden für Aufgaben |
| Aufgabe % abgeschlossen | Aufgabe % abgeschlossen (basierend auf der Dauer der Aufgabe) |
| Aufgabe der Arbeit % abgeschlossen | Aufgabe % abgeschlossen (basierend auf den geplanten Stunden der Aufgabe) |
| Geplanter Start und Abschluss | Geplante Start- und Enddaten |
| Tatsächlicher Beginn und Abschluss | Tatsächliche Start- und Abschlussdaten |
| Ressourcenname | Aufgabenzuweisung |
| Zuweisungseinheiten | Zuweisungszuordnungsprozentsatz |
| Aufgabenbeschreibung | Aufgabenbeschreibung |
| Vorgänger | Vorgänger |

## Übersicht über nicht enthaltene Daten

Es gibt eine Reihe von Projektfeldern, die nicht in Workfront importiert oder aus exportiert werden.

Diese Felder umfassen unter anderem Folgendes:

* Dokumentanlagen
* Benutzerdefinierte Felder (auf Projekt- oder Aufgabenebene)
* Workfront-Hinweise
* Probleme
* Negative Verzögerung bei Aufgaben mit einer Vorgängerbeziehung vom Typ Start/Ende (Aufgaben werden ohne Verzögerung importiert)
* Arbeitsaufträge
* Aufgabenbegrenzungen

   >[!NOTE]
   Da Einschränkungen nicht zwischen Microsoft Project und Workfront zugeordnet werden, stellen Sie sicher, dass Vorgängerbeziehungen zwischen den Aufgaben bestehen. Andernfalls stimmen die geplanten Start- und Abschlussdaten der Aufgaben im importierten Projekt möglicherweise nicht überein. 
