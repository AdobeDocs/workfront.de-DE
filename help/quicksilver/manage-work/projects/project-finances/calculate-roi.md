---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Berechnen des ROI
description: Der Return on Investment (ROI) ist eine Adobe Workfront-Metrik, mit der Portfoliomanager schnell feststellen können, wie das Projekt im Vergleich zum ursprünglichen geplanten Nutzen und den budgetierten Kosten des Projekts abschneidet.
author: Lisa
feature: Work Management
exl-id: 1a3d16cb-8cb1-472e-8102-0ea8e0bc0edd
TQID: https://experienceleague.adobe.com/x7MGrAZbtlDd0oTePPgRdLQfUg8-M4GkkQdeWXUTyh4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 348
ht-degree: 4%

---

# Berechnen des ROI

Der Return on Investment (ROI) ist eine Adobe Workfront-Metrik, mit der Portfoliomanager schnell feststellen können, wie das Projekt im Vergleich zum ursprünglichen geplanten Nutzen und den budgetierten Kosten des Projekts abschneidet.

## Überblick über den Return on Investment (ROI) des Projekts

Workfront berechnet den ROI anhand der folgenden Formel:

```
Project ROI = [(Project Planned Benefit - Project Budgeted Cost) / Project Budgeted Cost] x 100
```

Die folgenden Felder wirken sich auf den ROI eines Projekts aus:

* **Geplanter Projektnutzen**: Dies ist ein manueller Eintrag, der vom Projektinhaber beim Ausfüllen des Bereichs „Projektinformationen“ des Business Case angegeben wird. Hierbei handelt es sich um eine Schätzung dessen, was Sie als Projektbesitzer glauben, dass das Projekt Vorteile bringen könnte, wenn Sie das Projekt abschließen. Dies ist ein bestimmter Währungsbetrag und muss ein positiver Wert sein.\
  Weitere Informationen zum geplanten Nutzen eines Projekts finden Sie im Abschnitt „Projektinformationen“ im Artikel „Erstellen [ Business Case für ein Projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

* **Budgetierte Projektkosten**: Dies sind die Gesamtkosten, die mit dem Projekt verbunden sind und zum Zeitpunkt des ersten Starts des Projekts geschätzt werden.

  Die **budgetierte Kosten** verwendet den Wert **Budgetierte Arbeitskosten** der im Bereich Ressourcenbudgetierung des Business Case berechnet wird. Dabei werden die für Ihre Aufgabengebiete im Ressourcenplaner budgetierten Stunden und der Stundensatz pro Stunde für jedes Aufgabengebiet berücksichtigt.\
  Weitere Informationen finden Sie unter [Budgetierte Kosten berechnen](../../../manage-work/projects/project-finances/budgeted-cost.md).

## Suchen des Projekts nach Return on Investment (ROI)

Sie können den ROI-Wert für ein Projekt in den folgenden Bereichen in Workfront anzeigen:

* In Portfolio Optimizer, wenn das Projekt mit einem Portfolio verknüpft ist

  >[!NOTE]
  >
  >Die Summe aller ROI-Werte des Projekts entspricht der ROI des Portfolios.

  Informationen zum Portfolio Optimizer finden Sie im Artikel [Übersicht über Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* Im Feld Projekt-ROI in den folgenden Listen und Berichten:

   * Projekt
   * Aufgabe
   * Problem
   * Projekt (Finanzdaten)

  Weitere Informationen zum Erstellen von Berichten in Workfront finden Sie im Artikel [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
