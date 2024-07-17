---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Nettowert berechnen
description: Der Nettowert eines Projekts ist der erwartete Gesamtwert des Projekts nach der Berechnung seines Vorteils und der Beseitigung der Kosten.
author: Alina
feature: Work Management
exl-id: 44e3f211-c816-4ee1-aafc-c40fc8732f1a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 1%

---

# Nettowert berechnen

Der Nettowert eines Projekts ist der erwartete Gesamtwert des Projekts nach der Berechnung seines Vorteils und der Beseitigung der Kosten. 

## Übersicht über den Projektkostenwert

Adobe Workfront berechnet den Nettowert eines Projekts nach folgender Formel: 

```
Project Net Value = Planned Benefit - Budgeted Cost - Potential Risk Cost
```

Die folgenden Felder können sich auf den Nettowert eines Projekts auswirken:

* **Geplanter Nutzen**: Dies ist ein manueller Eintrag, der vom Projekteigentümer beim Ausfüllen des Bereichs **Projektinfo** im Geschäftsfall angegeben wurde.\
  Weitere Informationen zum geplanten Nutzen eines Projekts finden Sie im Abschnitt [Projektinfo](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) in Artikel [Überblick über die Bereiche des Geschäftsfalls](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* **Budgetierte Kosten**: Dies sind die Gesamtkosten, die mit dem Projekt verbunden sind, wie beim ersten Start des Projekts geschätzt.

  Die **budgeted Cost** verwendet den Wert **Budgeted Labour Cost** , der im Bereich Resource Budgeting des Business Case berechnet wird, und berücksichtigt die für Ihre Stellenrollen im Resource Planer geplanten Stunden sowie die Kosten pro Stunde für jede Jobrolle.\
  Die veranschlagten Kosten wirken sich auf den **Nettowert** des Projekts aus. Weitere Informationen zur Berechnung der budgetierten Kosten finden Sie unter [Budgetierte Kosten berechnen](../../../manage-work/projects/project-finances/budgeted-cost.md).

* **Potenzielle Risikokosten**: Dies sind die Kosten, die mit etwaigen Risiken für das Projekt verbunden sind, wie sie im Geschäftsfall oder auf der Registerkarte Risiken des Projekts definiert sind.\
  Weitere Informationen zur Berechnung der potenziellen Risikokosten eines Projekts finden Sie im Artikel [Berechnen der potenziellen Risikokosten](../../../manage-work/projects/project-finances/potential-risk-cost.md).

   

## Suchen Sie nach dem Projekt-Nettowert

Sie finden den Nettowert eines Projekts in den folgenden Bereichen in Workfront:

* Im Geschäftsfallzusammenfassungsbereich des Geschäftsfalles \
  Weitere Informationen zum Bereich &quot;Business Case Summary&quot;finden Sie im Abschnitt &quot;Understanding the Business Case Summary&quot;im Artikel [Geschäftsszenario für ein Projekt erstellen](../../../manage-work/projects/define-a-business-case/create-business-case.md) [Geschäftsszenario für ein Projekt erstellen](../../../manage-work/projects/define-a-business-case/create-business-case.md).

  ![](assets/net-value-on-business-case-summary-highlighted-350x444.png)

* Im Portfolio Optimizer , wenn das Projekt mit einem Portfolio verknüpft ist

  >[!TIP]
  >
  >Die Gesamtsumme aller Projekt-Nettowerte ist der Nettowert des Portfolios.

  Weitere Informationen zum Portfolio Optimizer finden Sie unter [Übersicht über Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* Im Feld Project Net Value der folgenden Listen und Berichte:

   * Projekt
   * Aufgabe
   * Problem
   * Projekt (Finanzdaten)

  Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
