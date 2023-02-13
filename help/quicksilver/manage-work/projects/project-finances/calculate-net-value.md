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

* **Geplanter Vorteil**: Dies ist ein manueller Eintrag, der vom Projekteigentümer beim Abschließen der **Projektinformationen** -Bereich des Geschäftsfalls.\
   Weitere Informationen über den geplanten Nutzen eines Projekts finden Sie im [Projektinformationen](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) Artikel [Überblick über die Bereiche des Geschäftsfalles](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* **Geplante Kosten**: Dies sind die mit dem Projekt verbundenen Gesamtkosten, wie beim ersten Start des Projekts geschätzt.

   Die **Geplante Kosten** verwendet die **Geplante Arbeitskosten** -Wert, der im Bereich Resource Budgeting des Business Case berechnet wird, und berücksichtigt die für Ihre Arbeitsplatzrollen im Resource Planer vorgesehenen Stunden sowie die Kosten pro Stunde für jede Stellenrolle.\
   Die budgetierten Kosten wirken sich auf die **Nettowert** des Projekts. Weitere Informationen zur Berechnung der budgetierten Kosten finden Sie unter [Berechnete veranschlagte Kosten](../../../manage-work/projects/project-finances/budgeted-cost.md).

* **Potenzielle Risikokosten**: Dies sind die Kosten, die mit etwaigen Risiken für das Projekt verbunden sind, wie sie im Geschäftsfall oder im Tab Risiken des Projekts definiert sind.\
   Weitere Informationen zur Berechnung der potenziellen Risikokosten eines Projekts finden Sie im Artikel [Potenzielle Risikokosten berechnen](../../../manage-work/projects/project-finances/potential-risk-cost.md).

    

## Suchen Sie nach dem Projekt-Nettowert .

Sie finden den Nettowert eines Projekts in den folgenden Bereichen in Workfront:

* Im Geschäftsfallzusammenfassungsbereich des Geschäftsfalles \
   Weitere Informationen zum Bereich &quot;Zusammenfassung von Geschäftsfällen&quot;finden Sie im Abschnitt &quot;Grundlagen zur Zusammenfassung von Geschäftsfällen&quot;im Artikel [Geschäftsszenario für ein Projekt erstellen](../../../manage-work/projects/define-a-business-case/create-business-case.md) [Geschäftsszenario für ein Projekt erstellen](../../../manage-work/projects/define-a-business-case/create-business-case.md).

   ![](assets/net-value-on-business-case-summary-highlighted-350x444.png)

* Im Portfolio Optimizer , wenn das Projekt mit einem Portfolio verknüpft ist

   >[!TIP]
   >
   >Die Gesamtsumme aller Projekt-Nettowerte ist der Nettowert des Portfolios.

   Weitere Informationen zum Portfolio Optimizer finden Sie unter [Übersicht über Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* Im Feld Project Net Value der folgenden Listen und Berichte:

   * Projekt
   * Aufgabe
   * Anfrage
   * Projekt (Finanzdaten)
   Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
