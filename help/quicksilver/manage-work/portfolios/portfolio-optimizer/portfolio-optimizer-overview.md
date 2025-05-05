---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Übersicht über Portfolio Optimizer
description: Der [!UICONTROL Portfolio Optimizer] ist das Tool, das für die Evaluierung und den Vergleich von Projekten verwendet wird. Beim Überprüfen und Vergleichen von Business Case-Werten für Projekte, die einem Portfolio zugewiesen sind, kann ein Portfolio-Manager Projekte priorisieren und den größten Nutzen für eine Organisation generieren.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1e48a24c-65de-49c2-85a8-dc931ac40c52
source-git-commit: c53e7d2229032c59710a8f955de53cfbd7fc6df4
workflow-type: tm+mt
source-wordcount: '1647'
ht-degree: 0%

---

# [!UICONTROL Portfolio Optimizer] - Übersicht

<!-- Audited: 01/2024 -->

Der [!UICONTROL Portfolio Optimizer] ist das Tool, das für die Evaluierung und den Vergleich von Projekten verwendet wird. Beim Überprüfen und Vergleichen von [!UICONTROL Business Case]-Werten für Projekte, die einem Portfolio zugewiesen sind, kann ein Portfolio-Manager Projekte priorisieren und den größten Nutzen für eine Organisation generieren.

![Portfolio Optimizer mit Projekten](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

Der [!UICONTROL Portfolio-Optimizer] bietet eine Schnittstelle, über die ein Portfoliomanager, ein Lenkungsausschuss oder ein Produktmanagementbüro zusammenfassende Informationen über den Business Case jedes Projekts anzeigen kann. Die Projekte können dann nach strategischen Werten und Zielen oder nach ihrem Gesamtergebnis priorisiert werden.

Der [!UICONTROL Portfolio Optimizer] kann Ihnen nur helfen, wenn Sie die folgenden Voraussetzungen erfüllt haben:

* Die [!UICONTROL Business Cases] wurden für die Projekte abgeschlossen. Weitere Informationen finden Sie in den Artikeln unter [Definieren eines Business-Case: Artikelindex](../../projects/define-a-business-case/define-business-case.md).
* Ein Portfolio wird im Bereich Projektübersicht des Abschnitts Projektdetails für die Projekte definiert, die Sie überprüfen möchten.
* Sie haben das Projektbudget und den geplanten Nutzen für die Projekte angegeben, die Sie überprüfen möchten. Festkosten und Festeinnahmen sind optional, bieten jedoch einen zusätzlichen Mehrwert. Weitere Informationen finden Sie unter [Felder für die Projektfinanzierung](../../projects/project-finances/project-finances-overview-1.md).

Informationen zum Auffinden von [!UICONTROL Portfolio Optimizer] finden Sie unter [Suchen von [!UICONTROL Portfolio Optimizer]](../../../manage-work/portfolios/portfolio-optimizer/locate-portfolio-optimizer.md).

## Finanzen im [!UICONTROL Portfolio Optimizer]

Bei Verwendung des [!UICONTROL Portfolio Optimizer] können Sie den Finanzstatus Ihres Portfolios jederzeit während der Laufzeit Ihrer Projekte einsehen.

Beachten Sie beim Arbeiten mit Finanzen in [!UICONTROL Portfolio Optimizer Folgendes]:

* Projekte erhalten jeweils eine Bewertung, wenn ihre [!UICONTROL Business Cases] gemäß den Kriterien abgeschlossen werden, die sie im [!UICONTROL Portfolio Optimizer&rbrace; &#x200B;]. Niedrige Kosten oder Projekte mit hoher Ausrichtung erhalten beispielsweise eine höhere Punktzahl.

  Weitere Informationen zur Berechnung des Portfolio-Optimizer-Scores eines Projekts finden Sie unter [Übersicht über den [!UICONTROL Portfolio Optimizer]-Score](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).

* Die Finanzberechnungen für den [!UICONTROL Portfolio Optimizer] verwenden [!UICONTROL Budgetierte Kosten] im [!UICONTROL Business Case] des Projekts.
* Sie können Ihre Projekte in [!UICONTROL Portfolio Optimizer] manuell priorisieren, wobei alle zugehörigen Informationen berücksichtigt werden. Dazu gehören beispielsweise Finanzdaten, die Ausrichtung an den Scorecards und der ROI.

### Die Finanzbereiche im [!UICONTROL Portfolio Optimizer] {#the-financial-areas-in-the-portfolio-optimizer}

Finanzinformationen finden Sie in den folgenden Bereichen von [!UICONTROL Portfolio Optimizer]:

* **[!UICONTROL Portfolio-Kopfzeile]**: Dieser Bereich zeigt Finanzinformationen an, die aus allen Projekten im Portfolio gesammelt wurden. Er wird auf jeder Registerkarte des Portfolio-Objekts angezeigt.
* **[!UICONTROL Portfolio-Finanzen für ausgewählte Projekte]**: Dieser Bereich zeigt Finanzinformationen an, die aus den Projekten gesammelt wurden, die in [!UICONTROL Portfolio Optimizer&rbrace; ausgewählt &#x200B;]. Sie können Projekte hinzufügen oder entfernen und verstehen, wie sich dies auf die Finanzen des Portfolios auswirkt, indem Sie die Informationen in diesem Bereich anzeigen.
* **[!UICONTROL Projektfinanzen]**: In diesem Bereich werden die Finanzinformationen der einzelnen Projekte angezeigt, die in [!UICONTROL Portfolio Optimizer&rbrace; &#x200B;] sind.

### Die Finanzfelder im [!UICONTROL Portfolio Optimizer] {#the-financial-fields-in-the-portfolio-optimizer}

Die folgenden Finanzfelder werden in [!UICONTROL Portfolio Optimizer] angezeigt:

* [Portfolio-Kopfzeile](#portfolio-header)
* [Portfolio-Finanzen für ausgewählte Projekte](#portfolio-finances-for-selected-projects)

#### Portfolio-Kopfzeile {#portfolio-header}

![Portfolio-Kopfzeile](assets/portfolio-header-nwe-350x14.png)

[!DNL Adobe Workfront] berechnet die Finanzfelder in der Portfoliokopfzeile anhand von Informationen aus Projekten mit Status, die nur mit &quot;[!UICONTROL &quot; &#x200B;] &quot;[!UICONTROL &quot; &#x200B;].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Feldname</strong> </th> 
   <th><strong>Beschreibung</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL on time]</td> 
   <td> <p>Der Prozentsatz der Projekte im Portfolio, die als [!UICONTROL On Time] betrachtet werden. Dies ist auf jeder Registerkarte innerhalb eines Portfolios sichtbar.</p> <p>Ein Projekt gilt als [!UICONTROL On Time], wenn die <strong>[!UICONTROL condition]</strong> des Projekts <strong>[!UICONTROL On Target]</strong>. <br>Weitere Informationen zu [!UICONTROL Projektbedingungen] finden Sie im Artikel <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Übersicht über Projektbedingung und Bedingungstyp</a>.</p> <p>Der <strong>[!UICONTROL On Time]</strong>Prozentsatz wird anhand der folgenden Formel berechnet:</p> <p><em>[!UICONTROL On Time Portfolio Percentage] = Anzahl der [!UICONTROL On Time] Projekte/Gesamtzahl der Projekte mit [!UICONTROL Aktuell]- oder [!UICONTROL Genehmigt]-Status</em> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL für Budget]</td> 
   <td> <p>Der Prozentsatz der Projekte im Portfolio, die als [!UICONTROL On Budget] betrachtet werden. Dies ist auf jeder Registerkarte innerhalb eines [!UICONTROL -Portfolios] sichtbar.</p> <p>Projekte werden <strong>[!UICONTROL On Budget]</strong>, wenn sie ihr vordefiniertes Budget nicht überschritten haben. <br>Weitere Informationen zum Budget eines Projekts finden Sie im Artikel <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">[!UICONTROL Manage] Informationen im Bereich Projektfinanzierung</a>.</p> <p>Der [!UICONTROL On Budget]-Prozentsatz wird anhand der folgenden Formel berechnet:</p> <p><em>[!UICONTROL on budget Portfolio percentage] = Anzahl der [!UICONTROL on budget] Projekte/Gesamtzahl der Projekte (</em><em> Status [!UICONTROL Aktuell] oder [!UICONTROL Genehmigt]</em> </p> </td> 
  </tr> 
  <tr> 
   <td>ROI (für Portfolio)</td> 
   <td> <p>Der [!UICONTROL Return on Investment] (ROI) für das Portfolio wird unter Berücksichtigung des gesamten [!UICONTROL Benefits] des [!UICONTROL Portfolio] und der Summe der [!UICONTROL budgetierten Kosten] der Projekte berechnet. Dies ist auf jeder Registerkarte innerhalb eines Portfolios sichtbar.</p> <p>Der ROI-Wert von Portfolio wird anhand der folgenden Formel berechnet:</p> <p><em>Portfolio-ROI = ([!UICONTROL Gesamtnutzen] - [!UICONTROL Budgetierte Gesamtkosten])/ [!UICONTROL Gesamtkosten] * 100</em> </p> <p>Weitere Informationen zur Berechnung des ROI für ein Projekt finden Sie im Artikel <a href="../../../manage-work/projects/project-finances/calculate-roi.md" class="MCXref xref">Berechnung des ROI)</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Alignment] oder [!UICONTROL Alignment Score] </td> 
   <td> <p>Ein Durchschnitt aller [!UICONTROL Project Alignment Score]-Werte, die nach Abschluss der [!UICONTROL Scorecard] im [!UICONTROL Business Case] des Projekts berechnet werden. Der Alignment-Score jedes Projekts wird in der Spalte [!UICONTROL Alignment] im [!UICONTROL Portfolio Optimizer] aufgeführt. Dies ist auf jeder Registerkarte innerhalb eines Portfolios sichtbar.</p> <p>Weitere Informationen zum Generieren eines Ausrichtungswerts für ein Projekt finden Sie im Artikel <a href="../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md" class="MCXref xref">Anwenden einer Scorecard auf ein Projekt und Generieren eines Ausrichtungswerts</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nettowert]</td> 
   <td> <p>Die Summe aller [!UICONTROL Net Values] aller Projekte im Portfolio. Dies ist auf jeder Registerkarte innerhalb eines Portfolios sichtbar.</p> <p>Weitere Informationen zur Berechnung von [!UICONTROL Net Value] für ein Projekt finden Sie im Artikel <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Calculate Net Value</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Portfolio-Finanzen für ausgewählte Projekte {#portfolio-finances-for-selected-projects}

![Finanzen von Portfolio](assets/portfolio-finances-for-selected-projects-in-optimizer-nwe-350x29.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Feldname</strong> </th> 
   <th><strong>Beschreibung</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Anzahl der Projekte]</td> 
   <td> <p>Die Gesamtzahl der aktiven Projekte im Portfolio. Projekte, die in einem Portfolio als aktiv betrachtet werden, können einen der folgenden Status aufweisen:</p> 
    <ul> 
     <li>[!UICONTROL Aktuell]</li> 
     <li>[!UICONTROL Planung]</li> 
     <li>[!UICONTROL genehmigt]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budget]</td> 
   <td>Sie können dieses Feld manuell aktualisieren, um das Gesamtbudget für das gesamte Portfolio anzugeben. Dieses Budget wird für alle Projekte innerhalb des Portfolios verwendet. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL verbleibt]</td> 
   <td> <p>Das verbleibende Budget nach den [!UICONTROL Gesamtkosten] für alle Projekte innerhalb des Portfolios wurde vom Budget des Portfolios abgezogen.</p> <p>Das [!UICONTROL Verbleibendes Portfolio-Budget] wird nach folgender Formel berechnet:</p> <p><em>[!UICONTROL Verbleibendes Portfolio-Budget] = [!UICONTROL Portfolio-Gesamtbudget] - [!UICONTROL budgetierte Gesamtkosten] aller Portfolio-Projekte</em> </p> <p>Das Portfoliobudget ist ein manueller Eintrag im Feld Budget von Portfolio Optimizer. </p> <p>Weitere Informationen zum Nachverfolgen von Kosten für ein Projekt finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten nachverfolgen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gesamtkosten]</td> 
   <td> <p>Die Summe der Kosten aller Projekte, die in [!UICONTROL Portfolio Optimizer] angezeigt werden. Die Kosten jedes Projekts entsprechen den [!UICONTROL Budgetierte Kosten] des Projekts, wie sie in der [!UICONTROL Business Case Summary] angezeigt werden. </p> <p>Weitere Informationen zu den Finanzfeldern von Projekten im [!UICONTROL Business Case] finden Sie im Abschnitt „Verstehen von Finanzfeldern im Business Case“ im Artikel <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Erstellen eines Business Case für ein Projekt</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risiko] </td> 
   <td> <p>Die Summe aller [!UICONTROL Potenzielle Risikokosten] aller Projekte im Portfolio. Die [!UICONTROL Mögliche Risikokosten] jedes Projekts sind in der Spalte [!UICONTROL Risiko] des [!UICONTROL Portfolio Optimizer] aufgeführt. </p> <p>Weitere Informationen zur Berechnung von Risiken für Projekte finden Sie im Artikel <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Berechnung potenzieller Risikokosten</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL -Vorteil]</td> 
   <td> <p>Die Summe aller [!UICONTROL Geplanter Nutzen]-Werte aller Projekte im Portfolio. Der Wert des geplanten Nutzens jedes Projekts wird in der Spalte [!UICONTROL Benefit] des [!UICONTROL Portfolio Optimizer] aufgeführt. </p> <p>Weitere Informationen zum [!UICONTROL Geplanter Nutzen] eines Projekts finden Sie im Artikel <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Übersicht über den geplanten Nutzen eines Projekts</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Indikator [!UICONTROL Risiko zum Nettowert]</td> 
   <td> <p>Misst den Wert [!UICONTROL Potenzielles Risiko] unter Berücksichtigung des von allen Projekten im Portfolio bereitgestellten [!UICONTROL Nettowerts]. Um innerhalb des Portfolios die größte Effizienz zu erzielen, sollte der Indikator [!UICONTROL Risk] niedrig und der Indikator [!UICONTROL Net Value] hoch sein. </p> <p>Weitere Informationen zur Berechnung des Risikos für [!UICONTROL Nettowert] finden Sie im Artikel <a href="../../../manage-work/portfolios/portfolio-optimizer/calculate-risk-to-net-value-in-portfolio.md" class="MCXref xref">Berechnung des Risikos für den Nettowert eines Portfolios</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anpassen des [!UICONTROL Portfolio Optimizer]

Sie können nur den Projektlistenbereich von [!UICONTROL Portfolio Optimizer] anpassen, indem Sie Einstellungen verwenden, um die Informationen in der Liste zu ändern.

Die folgenden Symbole und Optionen sind für den [!UICONTROL Portfolio Optimizer verfügbar]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Symbol in Portfolio Optimizer</strong></td> 
   <td><strong>Name</strong></td> 
   <td><strong>Funktion</strong></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-set-priority-icon.png"> </td> 
   <td>[!UICONTROL Projektpriorität festlegen]</td> 
   <td><p>Verwenden Sie dieses Symbol, wenn Sie die Projektreihenfolge basierend auf ihrer Priorität speichern möchten.</p>
   <p>Sie müssen über Verwaltungsberechtigungen für alle Projekte in der Liste verfügen, um „Projektpriorität festlegen<b> verwenden zu </b></p>.
    </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-optimize-icon-in-optimizer.png"> </td> 
   <td>[!UICONTROL Portfolio optimieren]</td> 
   <td>Verwenden Sie dieses Symbol, um das Portfolio basierend auf den folgenden finanziellen Werten der Projekte zu optimieren:
    <ul>
     <li>[!UICONTROL Kosten]</li>
     <li>[!UICONTROL -Ausrichtung]</li>
     <li>[!UICONTROL -Wert]</li>
     <li>[!UICONTROL Risiko-Nutzen-Verhältnis]</li>
     <li>[!UICONTROL ROI]</li>
    </ul><p>Weitere Informationen zur Portfoliooptimierung finden Sie im Artikel <a href="../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md" class="MCXref xref">Optimieren von Projekten in [!UICONTROL Portfolio Optimizer]</a>.</p></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-undo-redo-icons-optimizer.png"> </td> 
   <td>[!UICONTROL Rückgängig]/ [!UICONTROL Wiederholen] Symbole</td> 
   <td>Verwenden Sie diese Symbole, um die Änderungen, die Sie am [!UICONTROL Portfolio Optimizer] vor dem Speichern vorgenommen haben, abzubrechen oder wiederherzustellen.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/hide-show-unselected-portfolio-optimizer-142x74.png" alt="hide_show_unselected_portfolio_optimizer.png" style="width: 142;height: 74;"> </td> 
   <td>[!UICONTROL Anzeigen]/[!UICONTROL Ausblenden] nicht aktivierte Projekte</td> 
   <td>Verwenden Sie diese Symbole, um die Projekte im Portfolio, die Sie deaktiviert haben, anzuzeigen oder auszublenden.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-export-optimizer-icon-350x173.png" style="width: 350;height: 173;"> </td> 
   <td>[!UICONTROL -Export] </td> 
   <td> <p>Verwenden Sie dieses Symbol, um die Daten im Bereich [!UICONTROL Projektpriorisierung] von [!UICONTROL Portfolio Optimizer] zu exportieren. Sie können sie in die folgenden Formate exportieren:</p> 
    <ul> 
     <li>PDF</li> 
     <li>[!DNL Excel]</li> 
     <li>Durch [!UICONTROL tab] getrennt</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/preferences-portfolio-optimizer.png" alt="preferences_portfolio_optimizer.png"> </td> 
   <td>[!UICONTROL -Voreinstellungen]</td> 
   <td> <p>Mit diesem Symbol können Sie die in den Spalten von [!UICONTROL Portfolio Optimizer] angezeigten Projektfelder ändern oder je nach Status ändern, welche Projekte Sie in [!UICONTROL Optimizer] anzeigen. </p> <p>Tipp:  
     <ul> 
      <li> <p>Es stehen nicht alle [!DNL Workfront] Standardfelder zur Verfügung, die in den Spalten hinzugefügt werden können. </p> </li> 
     </ul> 
     <ul> 
      <li> <p>Sie können nur die benutzerdefinierten Felder hinzufügen, die in einem der Projekte im Portfolio einen anderen Wert als null aufweisen.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>
