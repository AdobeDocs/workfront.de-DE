---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Übersicht über Portfolio Optimizer
description: Der [!UICONTROL Portfolio Optimizer] ist das Tool für die Projektbewertung und -vergleich. Der Prozess der Überprüfung und des Vergleichs von Geschäftsfallwerten für Projekte, die einem Portfolio zugewiesen sind, ist die Art und Weise, wie ein Portfolioverwalter Projekte priorisieren und den größtmöglichen Nutzen für eine Organisation generieren kann.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1e48a24c-65de-49c2-85a8-dc931ac40c52
source-git-commit: 1fd3b135682c096f1715e5da0455fed12e882582
workflow-type: tm+mt
source-wordcount: '1629'
ht-degree: 0%

---

# Überblick über [!UICONTROL Portfolio Optimizer]

<!-- Audited: 01/2024 -->

Der [!UICONTROL Portfolio Optimizer] ist das Tool für die Projektbewertung und -vergleich. Der Prozess der Überprüfung und des Vergleichs von [!UICONTROL Geschäftsfall] -Werten für Projekte, die einem Portfolio zugewiesen werden, besteht darin, wie ein Portfolioverwalter Projekte priorisieren und den größtmöglichen Wert für eine Organisation generieren kann.

![](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

Der [!UICONTROL Portfoliooptimierer] soll eine Schnittstelle bereitstellen, über die ein Portfolioverwalter, ein Lenkungsausschuss oder ein Produktverwaltungsbüro zusammenfassende Informationen über den Geschäftsfall jedes Projekts anzeigen kann. Projekte können dann nach strategischen Werten und Zielen oder nach ihrem Gesamtergebnis priorisiert werden.

Der [!UICONTROL Portfolio Optimizer] kann Ihnen nur dann helfen, wenn Sie die folgenden Voraussetzungen erfüllt haben:

* Die [!UICONTROL geschäftlichen Fälle] wurden für die Projekte abgeschlossen. Weitere Informationen finden Sie in den Artikeln unter [Definieren eines Geschäftsfalls: Artikelindex](../../projects/define-a-business-case/define-business-case.md).
* Ein Portfolio wird im Bereich Projektübersicht im Abschnitt Projektdetails für die Projekte definiert, die Sie überprüfen möchten.
* Sie haben das Projektbudget und den geplanten Nutzen für die Projekte angegeben, die Sie überprüfen möchten. Feste Kosten und fester Umsatz sind optional, fügen jedoch zusätzlichen Wert hinzu. Weitere Informationen finden Sie unter [Projekte finanzieren Felder](../../projects/project-finances/project-finances-overview-1.md).

Informationen zum Auffinden des [!UICONTROL Portfolio Optimizer] finden Sie unter [Suchen des [!UICONTROL Portfolio Optimizer]](../../../manage-work/portfolios/portfolio-optimizer/locate-portfolio-optimizer.md).

## Finanzierungen im [!UICONTROL Portfolio Optimizer]

Bei Verwendung des [!UICONTROL Portfolio Optimizer] können Sie jederzeit während der Projektlaufzeit den Finanzstatus Ihres Portfolios anzeigen.

Beachten Sie Folgendes beim Arbeiten mit Finanzen im [!UICONTROL Portfolio Optimizer]:

* Jedem Portfolio wird eine Punktzahl zugewiesen, wenn seine [!UICONTROL Geschäftsszenarios] gemäß den Kriterien abgeschlossen werden, die im [!UICONTROL  Optimizer] übereinstimmen. Beispielsweise erhalten Projekte mit niedrigen Kosten oder hoher Ausrichtung ein höheres Ergebnis.

  Weitere Informationen zur Berechnung des Portfolio-Optimierungswerts eines Projekts finden Sie unter [Überblick über den [!UICONTROL Portfolio Optimizer] Score](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).

* Die Finanzberechnungen für den [!UICONTROL Portfolio Optimizer] verwenden die [!UICONTROL budgetierten Kosten] im [!UICONTROL Geschäftsszenario] des Projekts.
* Sie können Ihre Projekte im [!UICONTROL Portfolio Optimizer] manuell priorisieren und dabei alle Informationen zu ihnen berücksichtigen. Dazu gehören beispielsweise Finanzdaten, die Ausrichtung an ihren Scorecards und der ROI.

### Die Finanzbereiche im [!UICONTROL Portfolio Optimizer] {#the-financial-areas-in-the-portfolio-optimizer}

Sie können Finanzinformationen in den folgenden Bereichen von [!UICONTROL Portfolio Optimizer] anzeigen:

* **[!UICONTROL Portfolio-Header]**: Dieser Bereich zeigt Finanzinformationen an, die aus allen Projekten des Portfolios erfasst wurden. Sie wird auf jeder Registerkarte des Portfolio-Objekts angezeigt.
* **[!UICONTROL Projektfinanzierung für ausgewählte Portfolios]**: Dieser Bereich zeigt Finanzinformationen an, die aus den im [!UICONTROL Projektoptimierer] ausgewählten Projekten gesammelt wurden. Sie können Projekte hinzufügen oder entfernen und verstehen, wie sich dies auf die Finanzen des Portfolios auswirkt, indem Sie die Informationen in diesem Bereich ansehen.
* **[!UICONTROL Projektfinanzierung]**: Dieser Bereich zeigt die Finanzinformationen der einzelnen Projekte an, die im [!UICONTROL Portfolio Optimizer] aufgelistet sind.

### Die Finanzfelder im [!UICONTROL Portfolio Optimizer] {#the-financial-fields-in-the-portfolio-optimizer}

Die folgenden Finanzfelder werden im [!UICONTROL Portfolio Optimizer] angezeigt:

* [Portfolio-Kopfzeile](#portfolio-header)
* [Finanzierung ausgewählter Portfolios](#portfolio-finances-for-selected-projects)

#### Portfolio-Kopfzeile {#portfolio-header}

![](assets/portfolio-header-nwe-350x14.png)

[!DNL Adobe Workfront] berechnet die Finanzfelder im Portfolioheader anhand von Informationen aus Projekten mit Status, die nur mit [!UICONTROL Genehmigt] oder [!UICONTROL Aktuell] übereinstimmen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Name des Felds</strong> </th> 
   <th><strong>Beschreibung</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Einschaltzeit]</td> 
   <td> <p>Der Prozentsatz der Projekte im Portfolio, die als [!UICONTROL On Time] betrachtet werden. Dies ist auf jeder Registerkarte in einem Portfolio sichtbar.</p> <p>Ein Projekt gilt als [!UICONTROL On Time], wenn die Projektbedingung <strong>[!UICONTROL Condition]</strong> <strong>[!UICONTROL On Target]</strong> lautet. <br>Weitere Informationen zu [!UICONTROL Projektbedingungen] finden Sie im Artikel <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Überblick über Projektbedingungen und Bedingungstyp</a>.</p> <p>Der Prozentsatz <strong>[!UICONTROL On Time]</strong> wird mit der folgenden Formel berechnet:</p> <p><em>[!UICONTROL On Time Portfolio Percentage] = Anzahl der [!UICONTROL On Time] Projekte/ Gesamtanzahl der  in einem [!UICONTROL Current]- oder [!UICONTROL Approved]-Status</em> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL on Budget]</td> 
   <td> <p>Der Prozentsatz der Projekte im Portfolio, die als [!UICONTROL On Budget] betrachtet werden. Dies ist in jeder Registerkarte innerhalb eines [!UICONTROL Portfolios] sichtbar.</p> <p>Projekte sind <strong>[!UICONTROL On Budget]</strong>, wenn sie ihr vordefiniertes Budget nicht überschritten haben. <br>Weitere Informationen zum Budget eines Projekts finden Sie im Artikel <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">[!UICONTROL Verwalten] Informationen im Bereich "Projekt-Finanzen"</a>.</p> <p>Der [!UICONTROL On Budget]-Prozentsatz wird anhand der folgenden Formel berechnet:</p> <p><em>[!UICONTROL On Budget Portfolio Percentage] = Anzahl der [!UICONTROL On Budget] Projekte/ Gesamtprojektanzahl </em><em>in einem [!UICONTROL Current]- oder [!UICONTROL Approved]-Status</em> </p> </td> 
  </tr> 
  <tr> 
   <td>ROI (für Portfolio)</td> 
   <td> <p>Die [!UICONTROL Return on Investment] (ROI) für das Portfolio wird unter Berücksichtigung des [!UICONTROL Nutzens] des [!UICONTROL Portfolios] und der [!UICONTROL Budgetierten Kosten] der Projekte berechnet. Dies ist auf jeder Registerkarte in einem Portfolio sichtbar.</p> <p>Der ROI-Wert des Portfolios wird mit der folgenden Formel berechnet:</p> <p><em>Portfolio-ROI = ([!UICONTROL Gesamtnutzen] - [!UICONTROL Gesamtkosten])/ [!UICONTROL Gesamtkosten] * 100</em> </p> <p>Weitere Informationen zur Berechnung des ROI für ein Projekt finden Sie im Artikel <a href="../../../manage-work/projects/project-finances/calculate-roi.md" class="MCXref xref">Return On Investment (ROI) berechnen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aligned] oder [!UICONTROL Alignment Score] </td> 
   <td> <p>Ein Durchschnitt aller [!UICONTROL Project Alignment Score]-Werte, die nach Abschluss der [!UICONTROL Scorecard] im [!UICONTROL Business Case] des Projekts berechnet werden. Der Alignment-Wert der einzelnen Projekte wird in der Spalte [!UICONTROL Alignment] des [!UICONTROL Portfolio Optimizer] aufgeführt. Dies ist auf jeder Registerkarte in einem Portfolio sichtbar.</p> <p>Weitere Informationen zum Generieren eines Ausrichtungswerts für ein Projekt finden Sie im Artikel <a href="../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md" class="MCXref xref">Anwenden einer Scorecard auf ein Projekt und Generieren einer Alignment-Bewertung</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nettowert]</td> 
   <td> <p>Die Summe aller [!UICONTROL Netzwerte] aller Projekte im Portfolio. Dies ist auf jeder Registerkarte in einem Portfolio sichtbar.</p> <p>Weitere Informationen zur Berechnung des [!UICONTROL Nettowerts] für ein Projekt finden Sie im Artikel <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Nettowert berechnen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Finanzierung ausgewählter Portfolios {#portfolio-finances-for-selected-projects}

![](assets/portfolio-finances-for-selected-projects-in-optimizer-nwe-350x29.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Name des Felds</strong> </th> 
   <th><strong>Beschreibung</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Anzahl der Projekte]</td> 
   <td> <p>Die Gesamtzahl der aktiven Projekte im Portfolio. Projekte, die als in einem Portfolio aktiv betrachtet werden, können einen der folgenden Status aufweisen:</p> 
    <ul> 
     <li>[!UICONTROL Aktuell]</li> 
     <li>[!UICONTROL Planung]</li> 
     <li>[!UICONTROL Genehmigt]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budget]</td> 
   <td>Sie können dieses Feld manuell aktualisieren, um anzugeben, welches Gesamtbudget für das gesamte Portfolio verwendet wird. Dieses Budget wird für alle Projekte innerhalb des Portfolios verwendet. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Verbleibend]</td> 
   <td> <p>Das verbleibende Budget, nachdem alle [!UICONTROL Budgeted Costs] für alle Projekte innerhalb des Portfolios aus dem Portfolio abgezogen wurden.</p> <p>Das [!UICONTROL Portfolio Budget] wird nach folgender Formel berechnet:</p> <p><em>[!UICONTROL Verbleibendes Portfolio-Budget] = [!UICONTROL Portfolio-Gesamtbudget] - Gesamtkosten [!UICONTROL Geplante Kosten] aller Portfolio-Projekte</em> </p> <p>Die Gesamtkosten (!UICONTROL Budgeted Cost) aller Projekte im Portfolio werden in der Indikatorleiste im Feld Budget dargestellt. </p> <p>Weitere Informationen zu Tracking-Kosten für ein Projekt finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten-Tracking</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gesamtkosten]</td> 
   <td> <p>Die Summe der Kosten aller im [!UICONTROL Portfolio Optimizer] angezeigten Projekte. Die Kosten für jedes Projekt entsprechen den [!UICONTROL Budgeted Cost] des Projekts, die in der [!UICONTROL Geschäftsfallzusammenfassung] angezeigt werden. </p> <p>Weitere Informationen zu den Finanzfeldern von Projekten im [!UICONTROL Geschäftsfall] finden Sie im Abschnitt "Grundlagen zu den Finanzfeldern im Geschäftsfall"im Artikel <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Geschäftsszenario für ein Projekt erstellen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risiko] </td> 
   <td> <p>Die Summe aller [!UICONTROL Potenziellen Risikokosten] aller Projekte im Portfolio. Die [!UICONTROL Potenziellen Risikokosten] eines jeden Portfolios sind in der [!UICONTROL Risiko]-Spalte des [!UICONTROL  Optimizer] aufgeführt. </p> <p>Weitere Informationen zur Berechnung von Risiken für Projekte finden Sie im Artikel <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Berechnen von potenziellen Risikokosten</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benefit]</td> 
   <td> <p>Die Summe aller [!UICONTROL Geplanten Nutzenwerte] aller Projekte im Portfolio. Der Wert des geplanten Nutzens eines jeden Projekts wird in der Spalte [!UICONTROL Portfolio Optimizer] in der Spalte [!UICONTROL Benefit] aufgeführt. </p> <p>Weitere Informationen zum geplanten [!UICONTROL Nutzen] eines Projekts finden Sie im Artikel <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Überblick über den geplanten Nutzen des Projekts</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Indikator [!UICONTROL Risiko-Nettowert]</td> 
   <td> <p>Ermittelt den [!UICONTROL Potenziellen Risiko]-Wert unter Berücksichtigung des [!UICONTROL Nettowerts], der von allen Projekten im Portfolio bereitgestellt wird. Um die höchste Effizienz im Portfolio zu erzielen, möchten Sie sehen, dass der [!UICONTROL Risiko]-Indikator niedrig ist und der [!UICONTROL Net Value]-Indikator hoch ist. </p> <p>Weitere Informationen zur Berechnung des Risikos in [!UICONTROL Net Value] finden Sie im Artikel <a href="../../../manage-work/portfolios/portfolio-optimizer/calculate-risk-to-net-value-in-portfolio.md" class="MCXref xref">Berechnung des Nettowertrisikos in einem Portfolio</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anpassen des [!UICONTROL Portfolio Optimizer]

Sie können nur den Projektlistenbereich von [!UICONTROL Portfolio Optimizer] anpassen, indem Sie Einstellungen verwenden, um die Informationen in der Liste zu ändern.

Die folgenden Symbole und Optionen sind für den [!UICONTROL Portfolio Optimizer] verfügbar:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Symbol im Portfolio Optimizer</strong></td> 
   <td><strong>Name</strong></td> 
   <td><strong>Funktion</strong></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-set-priority-icon.png"> </td> 
   <td>[!UICONTROL Projektpriorität festlegen]</td> 
   <td>Verwenden Sie dieses Symbol, wenn Sie die Projektreihenfolge basierend auf ihrer Priorität speichern möchten. </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-optimize-icon-in-optimizer.png"> </td> 
   <td>[!UICONTROL Optimierungsportfolio]</td> 
   <td>Verwenden Sie dieses Symbol, um das Portfolio basierend auf den folgenden finanziellen Werten der Projekte zu optimieren:
    <ul>
     <li>[!UICONTROL Cost]</li>
     <li>[!UICONTROL Ausrichtung]</li>
     <li>[!UICONTROL Wert]</li>
     <li>[!UICONTROL Risiko des Nutzens]</li>
     <li>[!UICONTROL ROI]</li>
    </ul><p>Weitere Informationen zur Optimierung Ihres Portfolios finden Sie im Artikel <a href="../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md" class="MCXref xref">Projektoptimierung im [!UICONTROL Portfolio Optimizer]</a>.</p></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-undo-redo-icons-optimizer.png"> </td> 
   <td>Symbole [!UICONTROL Rückgängig]/ [!UICONTROL Wiederherstellen]</td> 
   <td>Verwenden Sie diese Symbole, um die Änderungen, die Sie vor dem Speichern an [!UICONTROL Portfolio Optimizer] vorgenommen haben, abzubrechen oder erneut durchzuführen.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/hide-show-unselected-portfolio-optimizer-142x74.png" alt="hide_show_unselected_portfolio_optimizer.png" style="width: 142;height: 74;"> </td> 
   <td>[!UICONTROL Einblenden]/[!UICONTROL Ausblenden] deaktiviert Projekte</td> 
   <td>Verwenden Sie diese Symbole, um die Projekte im Portfolio, die Sie deaktiviert haben, ein- oder auszublenden.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-export-optimizer-icon-350x173.png" style="width: 350;height: 173;"> </td> 
   <td>[!UICONTROL Export] </td> 
   <td> <p>Verwenden Sie dieses Symbol, um die Daten im Bereich [!UICONTROL Project Priorization] des [!UICONTROL Portfolio Optimizer] zu exportieren. Sie können sie in die folgenden Formate exportieren:</p> 
    <ul> 
     <li>PDF</li> 
     <li>[!DNL Excel]</li> 
     <li>[!UICONTROL Tab] Getrennt</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/preferences-portfolio-optimizer.png" alt="preferences_portfolio_optimizer.png"> </td> 
   <td>[!UICONTROL Voreinstellungen]</td> 
   <td> <p>Verwenden Sie dieses Symbol, um die in den Spalten des [!UICONTROL Portfolio Optimizer] angezeigten Projektfelder zu ändern oder um zu ändern, welche Projekte im [!UICONTROL Optimizer] je nach Status angezeigt werden. </p> <p>Tipp:  
     <ul> 
      <li> <p>Es sind nicht alle Standardfelder von [!DNL Workfront] verfügbar, die in die Spalten eingefügt werden können. </p> </li> 
     </ul> 
     <ul> 
      <li> <p>Sie können nur die benutzerdefinierten Felder hinzufügen, die einen anderen Wert als null in einem der Projekte im Portfolio haben.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>
