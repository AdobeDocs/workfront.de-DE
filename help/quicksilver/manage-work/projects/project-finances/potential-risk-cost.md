---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Potenzielle Risikokosten berechnen
description: Die potenziellen Risikokosten eines Projekts berücksichtigen die potenziellen Kosten der Projektrisiken und deren Wahrscheinlichkeit des Auftretens.
author: Alina
feature: Work Management
exl-id: f4dc1950-efd8-4936-83fd-1280ee465923
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Potenzielle Risikokosten berechnen

Die potenziellen Risikokosten eines Projekts berücksichtigen die potenziellen Kosten der Projektrisiken und deren Wahrscheinlichkeit des Auftretens.

## Überblick über potenzielle Risikokosten eines Projekts

Adobe Workfront berechnet die potenziellen Risikokosten eines Projekts anhand der folgenden Formel:

```
Potential Risk Cost =SUM(Potential Risk Costs * Risk Probability)
```

Beachten Sie bei der Überprüfung der potenziellen Risikokosten eines Projekts Folgendes:

* Die geplanten Risikokosten eines Projekts entsprechen den potenziellen Risikokosten. 
* Die potenziellen Risikokosten werden nicht in die geplanten Kosten eines Projekts einbezogen. Stattdessen wird er zur Bestimmung seines Nettowerts verwendet. .

## Potenzielle Risikokosten eines Projekts ermitteln

Sie finden die Risiken für ein Projekt und die potenziellen Kosten in den folgenden Bereichen in Workfront:

* Auf der Registerkarte Risiken des Projekts.
* In der Zusammenfassung der Geschäftsszenarios.\
   Weitere Informationen zum Geschäftsfall eines Projekts finden Sie im Artikel [Geschäftsszenario für ein Projekt erstellen](../../../manage-work/projects/define-a-business-case/create-business-case.md).
* In einem Projektbericht, wenn Sie das Feld &quot;Geplante Risikokosten&quot;zu den Spalten des Berichts hinzufügen.\
   Weitere Informationen zum Erstellen von Berichten in Workfront finden Sie im Artikel [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* Wenn das Portfolio-Optimizer mit einem Portfolio verknüpft ist, in der Spalte &quot;Risiko&quot;.\
   Die Summe aller potenziellen Risikokosten aller Projekte im Portfolio erhöht das Risiko des Portfolios.\
   Weitere Informationen zum Portfolio Optimizer finden Sie im Artikel [Übersicht über Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

Weitere Informationen zum Erstellen von Risiken für ein Projekt finden Sie im Artikel [Erstellen und Bearbeiten von Risiken für Projekte](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)

Weitere Informationen zum Geschäftsfall eines Projekts finden Sie im Artikel [Geschäftsszenario für ein Projekt erstellen](../../../manage-work/projects/define-a-business-case/create-business-case.md).
