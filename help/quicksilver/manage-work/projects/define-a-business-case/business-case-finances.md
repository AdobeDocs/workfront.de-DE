---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Überblick über die Finanzfelder für Geschäftsfälle
description: Der Untertab Geschäftsfall enthält Finanzfelder für das Projekt. Damit einige der Finanzfelder Werte aufweisen können, müssen die entsprechenden Bereiche des Geschäftsszenarios ausgefüllt werden.
author: Alina
feature: Work Management
exl-id: d420fc3e-e98d-47a0-a456-b2df17d72f34
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 2%

---

# Überblick über die Finanzfelder für Geschäftsfälle

Der Untertab Geschäftsfall enthält Finanzfelder für das Projekt. Damit einige der Finanzfelder Werte aufweisen können, müssen die entsprechenden Bereiche des Geschäftsszenarios ausgefüllt werden.  

Die folgenden finanziellen Felder des Projekts werden im Geschäftsfall angezeigt:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="col">Feldname</th> 
   <th scope="col">Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Abgestimmt </td> 
   <td> <p>Zeigt die Ausrichtung des Projekts nach seiner Scorecard an. Ein hoher Prozentwert zeigt an, dass das Projekt gut mit dem Zweck und den Zielen der Organisation abgestimmt ist. <br>Weitere Informationen zur Verwendung von Scorecards finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref">Scorecard erstellen</a>.</p> <p>Dieses Feld wird im Bereich "Zusammenfassung der Geschäftsfälle"angezeigt. </p> </td> 
  </tr> 
  <tr> 
   <td>Budgetierte Kosten</td> 
   <td> <p>Die Gesamtkosten, die bei Projektstart schätzungsweise mit dem Projekt verbunden sind.</p> <p>Die für das Projekt veranschlagten Kosten werden anhand der folgenden Formel berechnet:<br></p> <p><code>Budgeted Cost =&nbsp;Budgeted Expense Cost + Budgeted Labor Cost </code> <br> </p> <p>Adobe Workfront verwendet die budgetierten Stunden aus dem Ressourcenplaner, um die budgetierten Arbeitskosten zu berechnen.<br>Weitere Informationen zur Berechnung der budgetierten Kosten finden Sie unter <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Berechnete veranschlagte Kosten</a>. </p> <p>Dieses Feld wird im Bereich "Zusammenfassung der Geschäftsfälle"angezeigt.</p> </td> 
  </tr> 
  <tr> 
   <td>Budgetierte Ausgaben</td> 
   <td> <p>Die veranschlagten Kosten aller Ausgaben für das Projekt. </p> <p>Dies wird anhand der folgenden Formel berechnet:</p> <p><code>Budgeted Expense Cost = SUM(Planned Amount of Expenses on the project) </code></p> <p>Weitere Informationen zur Berechnung der Ausgaben finden Sie unter <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Verwalten von Projektausgaben </a>.</p> <p>Dieses Feld wird im Bereich Ausgaben angezeigt.</p> </td> 
  </tr> 
  <tr> 
   <td>Budgetierte Lohnkosten</td> 
   <td> <p>Die Kosten, die mit den für die Durchführung der Arbeiten am Projekt zugewiesenen Ressourcen verbunden sind.</p> <p>Die für das Projekt veranschlagten Arbeitskosten werden anhand der folgenden Formel berechnet:<br></p> <p><code>Budgeted Labor Cost = SUM(Estimated/ Budgeted hours for each job role on the project * Cost per Hour rate of each job role on the project) </code></p> <p>Workfront verwendet die budgetierten Stunden aus dem Ressourcenplaner, um die budgetierten Arbeitskosten zu berechnen.<br>Weitere Informationen zur Berechnung der budgetierten Arbeitskosten finden Sie unter <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Budgetierte Arbeitskosten und budgetierte Stunden für Projekte</a>.</p> <p>Dieses Feld wird im Bereich Ressourcenbudgetierung des Geschäftsfalls angezeigt. </p> </td> 
  </tr> 
  <tr> 
   <td>Geplante Kosten</td> 
   <td> <p>Dies entspricht den budgetierten Kosten. </p> <p>Hinweis: Die geplanten Kosten unterscheiden sich von den für das Projekt geplanten Kosten. Die geplanten Kosten werden anhand der geplanten Kosten des Projekts berechnet, während die geplanten Kosten anhand der geplanten Stunden im Projekt berechnet werden. </p> <p>Dieses Feld wird für jede Ausgabe im Bereich Ausgaben angezeigt.</p> </td> 
  </tr> 
  <tr> 
   <td>Nettowert</td> 
   <td> <p>Dies ist der erwartete Gesamtwert des Projekts nach der Berechnung seines Vorteils und der Beseitigung der Kosten.</p> <p>Der Nettowert des Projekts wird anhand der folgenden Formel berechnet:<br></p> <p><code>Net Value = Planned Benefit - Budgeted Cost - Potential Risk</code>. <br></p> <p>Weitere Informationen zur Berechnung des Nettowerts finden Sie unter <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Nettowert berechnen</a>.<br></p> <p>Dieses Feld wird im Bereich "Zusammenfassung der Geschäftsfälle"angezeigt.</p> </td> 
  </tr> 
  <tr> 
   <td>Geplanter Gewinn</td> 
   <td>Eine manuelle Schätzung des finanziellen Nutzens für Ihre Organisation nach Abschluss dieses Projekts. Es kann sich um einen beliebigen Währungsbetrag handeln, der für Sie und jedes von Ihnen verwaltete Projekt spezifisch ist. Der geplante Vorteil darf keinen negativen Wert haben. Dieses Feld wird im Bereich "Zusammenfassung von Geschäftsfällen"angezeigt und kann im Bereich "Projektinfo"des Geschäftsfalls bearbeitet werden. </td> 
  </tr> 
  <tr> 
   <td>Potenzielle Kosten von Risiken</td> 
   <td> <p>Dies sind die potenziellen Kosten aller Risiken für das Projekt. </p> <p>Dies wird mit der folgenden Formel berechnet:</p> <p><code>Potential Risk = SUM(Potential Cost * Probability of Risk) </code></p> <p>Weitere Informationen zu Risiken für das Projekt finden Sie unter <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Erstellen und Bearbeiten von Risiken für Projekte</a>.</p> <p>Dieses Feld wird im Bereich "Zusammenfassung der Geschäftsfälle"angezeigt.</p> </td> 
  </tr> 
  <tr> 
   <td>Potenzielles Risiko</td> 
   <td> <p>In der Zusammenfassung der Geschäftsfälle ist dies der Betrag der Kosten aller Risiken, falls sie auftreten sollten, basierend auf ihrer Wahrscheinlichkeit. Wenn ein Risiko beispielsweise die potenziellen Kosten von 100 $ und die Wahrscheinlichkeit eines Auftretens von 10 % aufweist, beträgt das potenzielle Risiko 10 $. Das potenzielle Risiko in der Zusammenfassung der Geschäftsszenarios wird anhand der folgenden Formel berechnet:</p> <p><code>Potential&nbsp;Risk = SUM(Risk Potential Cost x Probability)</code> für alle Risiken. </p> </td> 
  </tr> 
  <tr> 
   <td>Risikominderungskosten</td> 
   <td> <p>Die Kosten des Minderungsplans für die von Ihnen geschätzten Risiken können im Projekt anfallen.<br>Weitere Informationen zu Risiken für das Projekt finden Sie unter <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Erstellen und Bearbeiten von Risiken für Projekte</a>.</p> <p>Dieses Feld wird im Bereich Risiken für jedes im Projekt angegebene Risiko angezeigt.</p> </td> 
  </tr> 
  <tr> 
   <td>Potenzielle Kosten für ein Risiko</td> 
   <td> <p>Die geschätzten finanziellen Kosten, zu denen die für das Projekt definierten Risiken tatsächlich eintreten würden, unabhängig von ihrer Wahrscheinlichkeit. </p> <p>Dies ist ein manuell aktualisiertes Feld, das zu jedem Risiko im Risikobereich des Geschäftsfalls angezeigt wird. </p> </td> 
  </tr> 
  <tr> 
   <td>Risiken Gesamte potenzielle Kosten</td> 
   <td> <p>Dies sind die geschätzten Gesamtkosten aller Risiken, die zum Zeitpunkt des tatsächlichen Eintretens des Projekts für das Projekt definiert wurden. </p> <p>Dies wird anhand der folgenden Formel berechnet:</p> <p><code>Risks Total Potential Cost = SUM(Potential Cost of all risks on the project) </code></p> <p>Sie wird als Währungsnummer neben dem Titel des Risikobereichs des Geschäftsfalls angezeigt.</p> </td> 
  </tr> 
 </tbody> 
</table>
