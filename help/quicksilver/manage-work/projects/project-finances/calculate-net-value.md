---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Berechnen des Nettowerts
description: Der Nettowert eines Projekts entspricht dem erwarteten Gesamtwert des Projekts nach Berechnung des Nutzens und Entfernung der Kosten.
author: Lisa
feature: Work Management
exl-id: 44e3f211-c816-4ee1-aafc-c40fc8732f1a
TQID: https://experienceleague.adobe.com/Bj8-Lz2cRE0HeMF7xGryTucaqddQW25DzyPpbzWQR94
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 402
ht-degree: 6%

---

# Berechnen des Nettowerts

Der Nettowert eines Projekts entspricht dem erwarteten Gesamtwert des Projekts nach Berechnung des Nutzens und Entfernung der Kosten.

## Übersicht über den Nettowert des Projekts

Adobe Workfront berechnet den Nettowert eines Projekts anhand der folgenden Formel:

```
Project Net Value = Planned Benefit - Budgeted Cost - Potential Risk Cost
```

Die folgenden Felder können sich auf den Nettowert eines Projekts auswirken:

* **Geplanter Nutzen**: Dies ist ein manueller Eintrag, der vom Projektinhaber beim Ausfüllen **Bereichs „Projektinformationen** des Business Case angegeben wird.\
  Weitere Informationen zum geplanten Nutzen eines Projekts finden Sie im Abschnitt [Projektinformationen](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) im Artikel [Überblick über die Bereiche des Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* **Budgetierte Kosten**: Dies sind die Gesamtkosten, die mit dem Projekt verbunden sind und zum Zeitpunkt des ersten Starts des Projekts geschätzt werden.

  Die **budgetierte Kosten** verwendet den Wert **Budgetierte Arbeitskosten** der im Bereich Ressourcenbudgetierung des Business Case berechnet wird. Dabei werden die für Ihre Aufgabengebiete im Ressourcenplaner budgetierten Stunden und der Stundensatz pro Stunde für jedes Aufgabengebiet berücksichtigt.\
  Die budgetierten Kosten wirken sich auf **Nettowert** Projekts aus. Weitere Informationen zur Berechnung der budgetierten Kosten finden Sie unter [Budgetierte Kosten berechnen](../../../manage-work/projects/project-finances/budgeted-cost.md).

* **Mögliche Risikokosten**: Dies sind die Kosten, die mit allen Risiken im Projekt verbunden sind, wie sie im Business Case oder auf der Registerkarte „Risiken“ des Projekts definiert sind.\
  Weitere Informationen zur Berechnung der potenziellen Risikokosten eines Projekts finden Sie im Artikel [Berechnung potenzieller Risikokosten](../../../manage-work/projects/project-finances/potential-risk-cost.md).



## Suchen Sie das Projekt „Nettowert“

Den Nettowert für ein Projekt finden Sie in den folgenden Bereichen in Workfront:

* Im Business Case-Zusammenfassungsbereich des Business Case\
  Weitere Informationen zum Bereich „Zusammenfassung eines Business-Case“ finden Sie im Abschnitt „Grundlagen zur Zusammenfassung eines Business-Case“ im Artikel [Erstellen eines Business-Case für &#x200B;](../../../manage-work/projects/define-a-business-case/create-business-case.md) Projekt[Erstellen eines Business-Case für ein Projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

  ![Nettowert im Business Case](assets/net-value-on-business-case-summary-highlighted-350x444.png)

* In Portfolio Optimizer, wenn das Projekt mit einem Portfolio verknüpft ist

  >[!TIP]
  >
  >Die Summe aller Projekt-Nettowerte ist der Nettowert des Portfolios.

  Weitere Informationen zu Portfolio Optimizer finden Sie unter [Übersicht über Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* Im Feld Nettowert des Projekts der folgenden Listen und Berichte:

   * Projekt
   * Aufgabe
   * Problem
   * Projekt (Finanzdaten)

  Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
