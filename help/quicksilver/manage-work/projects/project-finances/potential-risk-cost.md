---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Mögliche Risikokosten berechnen
description: Die potenziellen Risikokosten eines Projekts berücksichtigen die potenziellen Kosten der Projektrisiken und deren Eintrittswahrscheinlichkeit.
author: Lisa
feature: Work Management
exl-id: f4dc1950-efd8-4936-83fd-1280ee465923
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Mögliche Risikokosten berechnen

Die potenziellen Risikokosten eines Projekts berücksichtigen die potenziellen Kosten der Projektrisiken und deren Eintrittswahrscheinlichkeit.

## Überblick über die potenziellen Risikokosten eines Projekts

Adobe Workfront berechnet die potenziellen Risikokosten eines Projekts anhand der folgenden Formel:

```
Potential Risk Cost =SUM(Potential Risk Costs * Risk Probability)
```

Berücksichtigen Sie bei der Prüfung der potenziellen Risikokosten eines Projekts Folgendes:

* Die geplanten Risikokosten eines Projekts sind mit den potenziellen Risikokosten identisch.
* Die potenziellen Risikokosten sind nicht in den geplanten Kosten eines Projekts enthalten. Stattdessen wird er zur Ermittlung seines Nettowerts verwendet.

## Identifizieren der potenziellen Risikokosten eines Projekts

Die Risiken für ein Projekt und deren potenzielle Kosten finden Sie in den folgenden Bereichen in Workfront:

* Auf der Registerkarte Risiken des Projekts.
* In der Zusammenfassung eines Business-Case.\
  Weitere Informationen zum Business Case eines Projekts finden Sie im Artikel [Erstellen eines Business Case für ein Projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).
* In einem Projektbericht, wenn Sie das Feld Geplante Risikokosten zu den Spalten des Berichts hinzufügen.\
  Weitere Informationen zum Erstellen von Berichten in Workfront finden Sie im Artikel [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* Wenn das Projekt in Portfolio Optimizer mit einer Portfolio verknüpft ist, wird es in der Spalte Risiko angezeigt.\
  Die Summe aller potenziellen Risikokosten aller Projekte im Portfolio summiert sich zum Risiko der Portfolio.\
  Weitere Informationen zu Portfolio Optimizer finden Sie im Artikel [Übersicht über Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

Weitere Informationen zum Erstellen von Risiken in einem Projekt finden Sie im Artikel [Erstellen und Bearbeiten von Risiken in Projekten](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)

Weitere Informationen zum Business Case eines Projekts finden Sie im Artikel [Erstellen eines Business Case für ein Projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).
