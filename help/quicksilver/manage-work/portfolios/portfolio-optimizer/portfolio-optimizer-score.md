---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Übersicht über die Portfolio Optimizer-Bewertung
description: Sie finden das Portfolio Optimizer-Ergebnis im Portfolio Optimizer. Sie wird im [!UICONTROL Ergebnis] -Spalte für jedes Projekt. Dies stellt einen Wert für jedes Projekt im Portfolio dar.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 4451b1a3-57ae-4c66-a6a1-a85bd51a1648
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 1%

---

# Übersicht über die [!UICONTROL Portfolio Optimizer] Ergebnis

Sie finden die [!UICONTROL Portfolio Optimizer] Wert in [!UICONTROL Portfolio Optimizer]. Sie wird im **[!UICONTROL Ergebnis]** -Spalte für jedes Projekt. Dies stellt einen Wert für jedes Projekt im Portfolio dar.

Informationen zum Auffinden der [!UICONTROL Portfolio Optimizer], siehe Artikel [[!UICONTROL Portfolio Optimizer] Übersicht](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

Informationen zum [!DNL Adobe Workfront] verwendet die Projektbewertung und andere Projektinformationen, um Projekte in der [!UICONTROL Portfolio Optimizer], siehe [Projektoptimierung im Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md).

## Unterschied zwischen der [!UICONTROL Ausrichtungsbewertung] und [!UICONTROL Portfolio Optimizer-Bewertung]

Es gibt einen Unterschied zwischen dem Alignment-Wert und dem Portfolio-Optimierer-Wert eines Projekts.

Der Ausrichtungswert eines Projekts wird anhand der Punkte berechnet, die nach Abschluss der Scorecard ermittelt wurden. Dieser Punktstand wird dann zur Bestimmung des Portfolioausrichtungswerts verwendet. Der Ausrichtungswert wird als Prozentsatz angezeigt.\
Der Ausrichtungswert eines Projekts wird im **[!UICONTROL Ausrichtung]** Spalte [!UICONTROL Portfolio Optimizer] oder in [!UICONTROL Ausrichtung] des [!UICONTROL Zusammenfassung von Geschäftsfällen].

![](assets/business-case-summary-aligned-field-highlighted.png)

![](assets/project-alignment-score-portfolio-optimizer-highlighted-350x174.png)

Weitere Informationen zum Generieren des Ausrichtungswerts eines Projekts finden Sie im Artikel [Anwenden einer Scorecard auf ein Projekt und Generieren einer Alignment-Bewertung](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Die [!UICONTROL Portfoliooptimierung] Das Ergebnis ist ein Rang, der automatisch im [!UICONTROL Portfolio Optimizer] durch die Projekte priorisiert werden können. Das Portfolio-Optimierungsergebnis wird als Indikatorsymbol mit einer Zahl angezeigt und im **[!UICONTROL Ergebnis]** Spalte [!UICONTROL Portfolio Optimizer].

>[!NOTE]
>
>Ein Projekt kann im Abschnitt [!UICONTROL Portfolio Optimizer] nur dann, wenn der Geschäftsfall abgeschlossen ist. Weitere Informationen zum Abschließen eines Geschäftsszenarios finden Sie im Artikel [[!UICONTROL Geschäftsszenario erstellen] für ein Projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

![](assets/portfolio-optimizer-project-score-highlighted-350x132.png)

Die Bewertung für jedes Projekt wird anhand der Wichtigkeit der folgenden Kategorien berechnet:

* [!UICONTROL Kosten]
* [!UICONTROL Ausrichtung]
* [!UICONTROL Nettowert]
* [!UICONTROL Risiko des Nutzens]
* [!UICONTROL ROI]

## Berechnen Sie die [!UICONTROL Portfolio Optimizer] Ergebnis

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This was edited based on this issue, per Anna: https://hub.workfront.com/issue/603d0c58000095ea0bc00ce5e2110693/overview)</p>
-->

[!DNL Workfront] erzeugt eine Punktzahl mit der [!UICONTROL Portfolio Optimizer] ist ein Ranking, der bei der Priorisierung von Projekten hilft. Die Werte im Portfolio basieren auf den Werten, die in die Geschäftsfälle der Projekte eingegeben wurden, und werden zur Berechnung eines Werts für das Projekt verwendet. Projekte mit einem höheren Punktstand könnten als von größerer Bedeutung betrachtet werden, und sie könnten vorrangig abgeschlossen werden.

Gehen Sie wie folgt vor, um die Rangfolge eines Projekts zu ermitteln:

1. Navigieren Sie zu [!UICONTROL Portfolio Optimizer].
1. Bewegen Sie den Mauszeiger über das Ranking-Symbol, um das Portfolio-Optimierungsergebnis für ein Projekt anzuzeigen.

![ranking_icon_in_portfolio_optimizer_new.png](assets/ranking-icon-in-portfolio-optimizer-new-350x160.png)

Der Algorithmus zur Berechnung der Punktzahl berücksichtigt die in den Geschäftsszenarien der Projekte beschriebenen Werte und die von ihnen mitgeführten Gewichtungen. Es gibt jedem Projekt im Optimierer eine Punktzahl und normalisiert diese Punktzahl, sodass immer ein Projekt mit einem Wert von 100 vorhanden ist. Dadurch erhält das beste Projekt einen hohen Punktstand.

**Beispiel:** Wenn Sie beispielsweise [!UICONTROL Höhere Ausrichtung] Der einzige zu berücksichtigende Faktor: Das Projekt mit der höchsten Ausrichtung erhält den Wert von 100.

Im Folgenden finden Sie Kriterien, anhand derer Sie ein Projekt bewerten können:

* [!UICONTROL Kosten]
* [!UICONTROL Ausrichtung]
* [!UICONTROL Wert]
* [!UICONTROL Risiko des Nutzens]
* [!UICONTROL ROI]

![](assets/optimizer-sliding-value-options-350x77.png)

Informationen zur Optimierung von Projekten im Portfolio finden Sie unter [Optimieren von Projekten in der [!UICONTROL Portfolio Optimizer]](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md).

Jedes Kriterium im Konfigurationsbereich ([!UICONTROL Kosten], [!UICONTROL Ausrichtung], [!UICONTROL ROI], [!UICONTROL Nettowert], [!UICONTROL Risiko des Nutzens]) erhalten ihre Gewichte im Bereich 0-100 basierend auf dem, was Sie ausgewählt haben.

Für jedes Projekt mit einem vollständigen Geschäftsfall wird anhand der folgenden Formel ein Ergebnis pro Kriterium generiert:

```
Score Per Criteria = (Project Value For The Criteria - AVG(all the project values for this criteria)) / Standard Deviation of that value for that project
```

**Beispiel:** Für [!UICONTROL Ausrichtungsbewertung] Für Projekt A haben Sie Folgendes:

```
Alignment Score = (Project A Alignment Score - AVG (of all the project Alignments)) / Standard Deviation of alignment score for that project
```

Sobald Sie alle [!UICONTROL Bewertung nach Kriterien] berechnet wurde, können Sie sie unter Berücksichtigung ihrer Gewichtungen hinzufügen, um die volle Punktzahl pro Projekt zu erhalten. Der Punktstand des Projekts wird mit der folgenden Formel berechnet:

```
Score = Cost Score * Cost Weight + Alignment Score * Alignment Weight + ROI Score * ROI Weight + Net Value Score * Net Value Weight + Risk Score * Risk Weight
```

Für die Projektkosten und [!UICONTROL Risiko] Die Logik funktioniert umgekehrt von der Funktionsweise der anderen Kriterien: Wenn Sie möchten, [!UICONTROL Geringe Kosten] für Sie wichtig sein, wird es den Gesamtwert des Projekts nicht erhöhen, sondern verringern durch `Cost Score * Cost Weight`.

Nachdem Sie für jedes Projekt Bewertungen berechnet haben, wird die [!UICONTROL Optimierungsbewertung] wird für die Projekte wie folgt definiert:

1. [!UICONTROL Minimum] und [!UICONTROL Maximum] -Werte definiert werden.
1. Der Bereich zwischen diesen Werten wird berechnet.
1. Für jedes Projekt [!UICONTROL Optimierungsbewertung] wird mit der folgenden Formel berechnet:

   ```
   Optimization Score = Rounded ((Score - Minimum / Range)*100)
   ```
