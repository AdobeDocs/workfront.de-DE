---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Übersicht über die Portfolio Optimizer-Bewertung
description: Sie finden das Portfolio Optimizer-Ergebnis im Portfolio Optimizer. Er wird für jedes Projekt in der Spalte [!UICONTROL Punktzahl] angezeigt. Dies stellt einen Wert für jedes Projekt im Portfolio dar.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 4451b1a3-57ae-4c66-a6a1-a85bd51a1648
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 0%

---

# Überblick über die [!UICONTROL Portfolio Optimizer]-Punktzahl

Sie finden den Punktstand [!UICONTROL Portfolio Optimizer] im [!UICONTROL Portfolio Optimizer]. Er wird für jedes Projekt in der Spalte **[!UICONTROL Punktzahl]** angezeigt. Dies stellt einen Wert für jedes Projekt im Portfolio dar.

Informationen zum Auffinden des [!UICONTROL Portfolio Optimizer] finden Sie im Artikel [[!UICONTROL Übersicht über Portfolio Optimizer]](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md) .

Informationen dazu, wie [!DNL Adobe Workfront] die Projektbewertung und andere Projektinformationen verwendet, um Portfolios im [!UICONTROL Projektoptimierer] zu optimieren, finden Sie unter [Projektoptimierung im Portfolio-Optimizer](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md).

## Unterschied zwischen dem [!UICONTROL Alignment-Score] und dem [!UICONTROL Portfolio Optimizer-Score]

Es gibt einen Unterschied zwischen dem Alignment-Wert und dem Portfolio-Optimierer-Wert eines Projekts.

Der Ausrichtungswert eines Projekts wird anhand der Punkte berechnet, die nach Abschluss der Scorecard ermittelt wurden. Dieser Punktstand wird dann zur Bestimmung des Portfolioausrichtungswerts verwendet. Der Ausrichtungswert wird als Prozentsatz angezeigt.\
Der Alignment-Wert eines Portfolios wird in der Spalte **[!UICONTROL Ausrichtung]** des [!UICONTROL Projektoptimierers] oder im Feld [!UICONTROL Ausrichtung] der [!UICONTROL Zusammenfassung der Geschäftsszenarios] angezeigt.

![](assets/business-case-summary-aligned-field-highlighted.png)

![](assets/project-alignment-score-portfolio-optimizer-highlighted-350x174.png)

Weitere Informationen zum Generieren des Ausrichtungswerts eines Projekts finden Sie im Artikel [Anwenden einer Scorecard auf ein Projekt und Generieren einer Alignment-Bewertung](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Der Punktstand [!UICONTROL Portfoliooptimierer] ist ein im [!UICONTROL Portfolio Optimizer] automatisch berechneter Rang, anhand dessen Projekte priorisiert werden können. Das Portfolio-Optimierer-Ergebnis wird als Indikatorsymbol zusammen mit einer Zahl angezeigt und in der Spalte **[!UICONTROL Punktzahl]** des [!UICONTROL Portfolio-Optimizer] angezeigt.

>[!NOTE]
>
>Ein Portfolio kann nur dann im [!UICONTROL Projektoptimierer] bewertet werden, wenn sein Geschäftsfall abgeschlossen ist. Weitere Informationen zum Abschließen eines Geschäftsszenarios finden Sie im Artikel [[!UICONTROL Geschäftsszenario erstellen] für ein Projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

![](assets/portfolio-optimizer-project-score-highlighted-350x132.png)

Der Punktstand für jedes Projekt wird anhand der Wichtigkeit der folgenden Kategorien berechnet:

* [!UICONTROL Kosten]
* [!UICONTROL Ausrichtung]
* [!UICONTROL Nettowert]
* [!UICONTROL Nutzen-Risiko]
* [!UICONTROL ROI]

## Berechnen der [!UICONTROL Portfolio Optimizer]-Punktzahl

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This was edited based on this issue, per Anna: https://hub.workfront.com/issue/603d0c58000095ea0bc00ce5e2110693/overview)</p>
-->

[!DNL Workfront] erzeugt mit dem [!UICONTROL Portfolio Optimizer] eine Punktzahl, die eine Rangfolge darstellt, die bei der Priorisierung von Projekten hilft. Die Werte im Portfolio basieren auf den Werten, die in die Geschäftsfälle der Projekte eingegeben wurden, und werden zur Berechnung eines Werts für das Projekt verwendet. Projekte mit einem höheren Punktstand könnten als von größerer Bedeutung betrachtet werden, und sie könnten vorrangig abgeschlossen werden.

Gehen Sie wie folgt vor, um die Rangfolge eines Projekts zu ermitteln:

1. Wechseln Sie zum [!UICONTROL Portfolio Optimizer].
1. Bewegen Sie den Mauszeiger über das Ranking-Symbol, um das Portfolio-Optimierungsergebnis für ein Projekt anzuzeigen.

![ranking_icon_in_portfolio_optimizer_new.png](assets/ranking-icon-in-portfolio-optimizer-new-350x160.png)

Der Algorithmus zur Berechnung der Punktzahl berücksichtigt die in den Geschäftsszenarien der Projekte beschriebenen Werte und die von ihnen mitgeführten Gewichtungen. Es gibt jedem Projekt im Optimierer eine Punktzahl und normalisiert diese Punktzahl, sodass immer ein Projekt mit einem Wert von 100 vorhanden ist. Dadurch erhält das beste Projekt einen hohen Punktstand.

**Beispiel:** Wenn Sie beispielsweise die [!UICONTROL höhere Ausrichtung] als einzigen Faktor betrachten, erhält das Projekt mit der höchsten Ausrichtung den Wert von 100.

Im Folgenden finden Sie Kriterien, anhand derer Sie ein Projekt bewerten können:

* [!UICONTROL Kosten]
* [!UICONTROL Ausrichtung]
* [!UICONTROL Wert]
* [!UICONTROL Nutzen-Risiko]
* [!UICONTROL ROI]

![](assets/optimizer-sliding-value-options-350x77.png)

Informationen zur Projektoptimierung im Portfolio finden Sie unter [Projektoptimierung im [!UICONTROL Portfolio Optimizer]](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md).

Jedes Kriterium im Konfigurationsbereich ([!UICONTROL Kosten], [!UICONTROL Ausrichtung], [!UICONTROL ROI], [!UICONTROL Nettowert], [!UICONTROL Nutzen-Risiko]) erhält seine Gewichtungen im Bereich 0-100 basierend auf dem, was Sie ausgewählt haben.

Für jedes Projekt mit einem vollständigen Geschäftsfall wird anhand der folgenden Formel ein Ergebnis pro Kriterium generiert:

```
Score Per Criteria = (Project Value For The Criteria - AVG(all the project values for this criteria)) / Standard Deviation of that value for that project
```

**Beispiel:** Für die [!UICONTROL Alignment-Bewertung] für Projekt A haben Sie Folgendes:

```
Alignment Score = (Project A Alignment Score - AVG (of all the project Alignments)) / Standard Deviation of alignment score for that project
```

Nachdem Sie alle [!UICONTROL Bewertungskriterien pro Kriterium] berechnet haben, können Sie sie unter Berücksichtigung ihrer Gewichtung hinzufügen, um das vollständige Ergebnis pro Projekt zu erhalten. Der Punktstand des Projekts wird mit der folgenden Formel berechnet:

```
Score = Cost Score * Cost Weight + Alignment Score * Alignment Weight + ROI Score * ROI Weight + Net Value Score * Net Value Weight + Risk Score * Risk Weight
```

Für die Projektkosten und das [!UICONTROL Risiko] funktioniert die Logik umgekehrt von der Funktionsweise der anderen Kriterien: Wenn Sie möchten, dass die [!UICONTROL niedrigen Kosten] für Sie wichtig sind, wird der Gesamtwert des Projekts nicht um `Cost Score * Cost Weight` erhöht, sondern verringert.

Nachdem Sie für jedes Projekt Bewertungen berechnet haben, wird die [!UICONTROL Optimierungsbewertung] für die Projekte wie folgt definiert:

1. Die Werte [!UICONTROL Minimum] und [!UICONTROL Maximum] werden definiert.
1. Der Bereich zwischen diesen Werten wird berechnet.
1. Für jedes Projekt wird die [!UICONTROL Optimierungsbewertung] anhand der folgenden Formel berechnet:

   ```
   Optimization Score = Rounded ((Score - Minimum / Range)*100)
   ```
