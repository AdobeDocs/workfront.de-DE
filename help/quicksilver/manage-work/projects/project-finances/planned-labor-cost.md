---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Geplante Lohnkosten berechnen
description: Wenn Sie die Arbeit an Ihren Projekten planen, berechnet Adobe Workfront die geplanten Lohnkosten für die Funktionen und Benutzer, die dieser Arbeit zugewiesen sind, auf der Grundlage ihrer Werte für „Kosten pro Stunde“.
author: Lisa
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# Geplante Lohnkosten berechnen

Wenn Sie die Arbeit an Ihren Projekten planen, berechnet Adobe Workfront die geplanten Lohnkosten für die Funktionen und Benutzer, die dieser Arbeit zugewiesen sind, auf der Grundlage ihrer Werte für „Kosten pro Stunde“.

Die geplanten Lohnkosten eines Projekts sind eine Berechnung zwischen den Kosten, die mit den Aufgabengebieten oder den Benutzern verbunden sind, die für die Fertigstellung der Arbeit am Projekt zugewiesen wurden, und der Anzahl der geplanten Stunden (geplante Stunden), die jede Funktion oder jeder Benutzer benötigen könnte, um diese Arbeit abzuschließen.

## Übersicht über die geplanten Lohnkosten

Die **geplanten Lohnkosten** eines Projekts werden durch Addition aller geplanten Lohnkosten aller Aufgaben im Projekt berechnet.

>[!TIP]
>
>Es gibt keine geplanten Lohnkosten, die mit Problemen oder dem Projekt selbst verbunden sind.

Workfront berechnet die geplanten Lohnkosten eines Projekts anhand der folgenden Formel:

```
Project Planned Labor Cost= SUM(Tasks Planned Labor Cost)
```

Die geplanten Lohnkosten für die Aufgabe werden wie folgt berechnet:

* Die Anzahl der Ressourcen für die Aufgabe und ihre individuelle Zuordnung zur Aufgabe
* Der Kostentyp der Aufgabe.

Die geplanten Lohnkosten für die Aufgabe werden anhand der folgenden Formel berechnet:

```
Task Planned Cost = Planned Hours x User or Job Role Cost Per Hour
```

Weitere Informationen dazu, wie Workfront die geplanten Lohnkosten für Aufgaben abhängig von Aufgabenzuweisungen und Kostentyp berechnet, finden Sie im Abschnitt „Ändern der Kostentypen für einzelne Aufgaben“ im Artikel [Kosten nachverfolgen](../../../manage-work/projects/project-finances/track-costs.md).

## Geplante Lohnkosten suchen

Sie können die geplanten Lohnkosten eines Projekts in den folgenden Bereichen von Workfront ermitteln:

* Ein Projektbericht
* Eine Liste von Projekten
* Ein Baseline-Bericht, in dem Sie ihn im Zeitverlauf verfolgen können
* Über die API

Informationen zum Erstellen von Berichten und zum Verwenden der Workfront-API finden Sie in den folgenden Artikeln:

* [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
* [API-Grundlagen](../../../wf-api/general/api-basics.md)
