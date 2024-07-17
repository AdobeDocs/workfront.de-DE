---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Berechnung der Kapitalrendite (ROI)
description: Return On Investment (ROI) ist eine Adobe Workfront-Metrik, mit der Portfolioverwalter schnell feststellen können, wie das Projekt mit dem ursprünglich geplanten Nutzen und den budgetierten Kosten des Projekts funktioniert.
author: Alina
feature: Work Management
exl-id: 1a3d16cb-8cb1-472e-8102-0ea8e0bc0edd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Berechnung der Kapitalrendite (ROI)

Return On Investment (ROI) ist eine Adobe Workfront-Metrik, mit der Portfolioverwalter schnell feststellen können, wie das Projekt mit dem ursprünglich geplanten Nutzen und den budgetierten Kosten des Projekts funktioniert.

## Übersicht über die Kapitalrendite (ROI) des Projekts

Workfront berechnet den ROI anhand der folgenden Formel:

```
Project ROI = [(Project Planned Benefit - Project Budgeted Cost) / Project Budgeted Cost] x 100
```

Die folgenden Felder beeinflussen den ROI eines Projekts:

* **Vorgesehener Projektvorteil**: Dies ist ein manueller Eintrag, der vom Projekteigentümer beim Ausfüllen des Bereichs Projektinfo im Geschäftsfall angegeben wird. Dies ist eine Schätzung dessen, was Sie als Projekteigentümer glauben, dass der Nutzen des Projekts sein könnte, wenn Sie das Projekt abschließen. Dies ist ein bestimmter Währungsbetrag und muss ein positiver Wert sein.\
  Weitere Informationen zum geplanten Nutzen eines Projekts finden Sie im Abschnitt &quot;Projektinfo&quot;im Artikel [Geschäftsszenario für ein Projekt erstellen](../../../manage-work/projects/define-a-business-case/create-business-case.md).

* **Projekt - Budgetierte Kosten**: Dies sind die Gesamtkosten, die mit dem Projekt verbunden sind, wie beim ersten Start des Projekts geschätzt.

  Die **budgeted Cost** verwendet den Wert **Budgeted Labour Cost** , der im Bereich Resource Budgeting des Business Case berechnet wird, und berücksichtigt die für Ihre Stellenrollen im Resource Planer geplanten Stunden sowie die Kosten pro Stunde für jede Jobrolle.\
  Weitere Informationen finden Sie unter [Budgetierte Kosten berechnen](../../../manage-work/projects/project-finances/budgeted-cost.md).

## Finden Sie den ROI (Return on Investment) des Projekts.

Sie können den ROI-Wert für ein Projekt in den folgenden Bereichen in Workfront anzeigen:

* Im Portfolio Optimizer , wenn das Projekt mit einem Portfolio verknüpft ist

  >[!NOTE]
  >
  >Die Gesamtsumme aller Projekt-ROI-Werte ist der ROI des Portfolios.

  Informationen zum Portfolio Optimizer finden Sie im Artikel [Übersicht über Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* Im Feld Projekt-ROI in den folgenden Listen und Berichten: 

   * Projekt
   * Aufgabe
   * Problem
   * Projekt (Finanzdaten)

  Weitere Informationen zum Erstellen von Berichten in Workfront finden Sie im Artikel [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
