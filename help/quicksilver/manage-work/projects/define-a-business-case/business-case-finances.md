---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Überblick über Business Case-Finanzfelder
description: Die Unterregisterkarte Business-Case enthält Finanzfelder für das Projekt. Damit einige der Finanzfelder Werte aufweisen, müssen entsprechende Bereiche des Business Case ausgefüllt werden.
author: Becky
feature: Work Management
exl-id: d420fc3e-e98d-47a0-a456-b2df17d72f34
source-git-commit: fa0b4322b9f7c1d506cf194645c7ae50ad8c0f0b
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 2%

---

# Überblick über Business Case-Finanzfelder

Die Unterregisterkarte Business-Case enthält Finanzfelder für das Projekt. Damit einige der Finanzfelder Werte aufweisen, müssen entsprechende Bereiche des Business Case ausgefüllt werden.  

Die folgenden Finanzfelder des Projekts werden im Business Case angezeigt:

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
   <td> <p>Zeigt die Ausrichtung des Projekts entsprechend seiner Scorecard an. Ein hoher Prozentwert zeigt an, dass das Projekt gut auf den Zweck und die Ziele der Organisation abgestimmt ist. <br>Weitere Informationen zur Verwendung von Scorecards finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref">Erstellen einer Scorecard</a>.</p> <p>Dieses Feld wird im Bereich Zusammenfassung des Business-Case angezeigt. </p> </td> 
  </tr> 
  <tr> 
   <td>Budgetierte Kosten</td> 
   <td> <p>Die geschätzten Gesamtkosten, die dem Projekt bei Projektstart zugeordnet sind.</p> <p>Die budgetierten Kosten für das Projekt werden nach folgender Formel berechnet:<br></p> <p><code>Budgeted Cost =&nbsp;Budgeted Expense Cost + Budgeted Labor Cost </code> <br> </p> <p>Adobe Workfront verwendet die budgetierten Stunden aus dem Ressourcenplaner, um die budgetierten Lohnkosten zu berechnen.<br>Weitere Informationen zur Berechnung budgetierter Kosten finden Sie unter <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Budgetierte Kosten berechnen</a>. </p> <p>Dieses Feld wird im Bereich Zusammenfassung des Business-Case angezeigt.</p> </td> 
  </tr> 
  <tr> 
   <td>Budgetierte Ausgaben</td> 
   <td> <p>Die budgetierten Kosten aller Ausgaben für das Projekt. </p> <p>Dies wird nach folgender Formel berechnet:</p> <p><code>Budgeted Expense Cost = SUM(Planned Amount of Expenses on the project) </code></p> <p>Weitere Informationen zur Berechnung von Ausgaben finden Sie unter <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Projektausgaben verwalten </a>.</p> <p>Dieses Feld wird im Bereich Ausgaben angezeigt.</p> </td> 
  </tr> 
  <tr> 
   <td>Budgetierte Lohnkosten</td> 
   <td> <p>Die Kosten, die mit den Ressourcen verbunden sind, die für die Fertigstellung der Arbeit am Projekt zugewiesen wurden.</p> <p>Die budgetierten Lohnkosten für das Projekt werden nach folgender Formel berechnet:<br></p> <p><code>Budgeted Labor Cost = SUM(Estimated/ Budgeted hours for each job role on the project * Cost per Hour rate of each job role on the project) </code><br></p> <p>Workfront verwendet die budgetierten Stunden aus dem Ressourcenplaner, um die budgetierten Lohnkosten zu berechnen.<br>Weitere Informationen zur Berechnung budgetierter Lohnkosten finden Sie unter <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Budgetierte Lohnkosten und budgetierte Stunden für Projekte</a>.</p> <p>Dieses Feld wird im Bereich Ressourcenbudgetierung des Business Case angezeigt. </p> </td> 
  </tr> 
  <tr> 
   <td>Geplante Kosten</td> 
   <td> <p>Dies entspricht den budgetierten Ausgabenkosten. </p> <p>Hinweis: Die geplanten Kosten unterscheiden sich von den geplanten Kosten für das Projekt. Die geplanten Kosten werden anhand des geplanten Aufwands für das Projekt berechnet, während die geplanten Kosten anhand der geplanten Stunden für das Projekt berechnet werden. </p> <p>Dieses Feld wird für jede Ausgabe im Bereich Ausgaben angezeigt.</p> </td> 
  </tr> 
  <tr> 
   <td>Nettowert</td> 
   <td> <p>Dies ist der erwartete Gesamtwert des Projekts nach Berechnung des Nutzens und Entfernung der Kosten.</p> <p>Der Nettowert für das Projekt wird anhand der folgenden Formel berechnet:<br></p> <p><code>Net Value = Planned Benefit - Budgeted Cost - Potential Risk</code>. <br></p> <p>Weitere Informationen zur Berechnung des Nettowerts finden Sie unter <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Nettowert berechnen</a>.<br></p> <p>Dieses Feld wird im Bereich Zusammenfassung des Business-Case angezeigt.</p> </td> 
  </tr> 
  <tr> 
   <td>Geplanter Gewinn</td> 
   <td>Eine manuelle Schätzung des monetären Nutzens für Ihr Unternehmen, wenn dieses Projekt abgeschlossen ist. Sie kann eine beliebige Währung sein und ist für Sie und jedes von Ihnen verwaltete Projekt spezifisch. Der geplante Vorteil darf keinen negativen Wert haben. Dieses Feld wird im Bereich Zusammenfassung eines Business-Case angezeigt und kann im Bereich Projektinformationen des Business-Case bearbeitet werden. </td> 
  </tr> 
  <tr> 
   <td>Mögliche Risikokosten</td> 
   <td> <p>Dies sind die potenziellen Kosten aller Risiken des Projekts. </p> <p>Dies wird anhand der folgenden Formel berechnet:</p> <p><code>Potential Risk = SUM(Potential Cost * Probability of Risk) </code></p> <p>Weitere Informationen zu Risiken im Projekt finden Sie unter <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Erstellen und Bearbeiten von Risiken in Projekten</a>.</p> <p>Dieses Feld wird im Bereich Zusammenfassung des Business-Case angezeigt.</p> </td> 
  </tr> 
  <tr> 
   <td>Potenzielles Risiko</td> 
   <td> <p>In der Zusammenfassung eines Business-Case ist dies der Betrag der Kosten aller Risiken, falls sie eintreten sollten, basierend auf ihrer Wahrscheinlichkeit. Wenn ein Risiko beispielsweise potenzielle Kosten von 100 USD und eine Eintrittswahrscheinlichkeit von 10 % aufweist, beträgt das potenzielle Risiko 10 USD. Das potenzielle Risiko in der Zusammenfassung eines Business-Case wird anhand der folgenden Formel berechnet:</p> <p><code>Potential&nbsp;Risk = SUM(Risk Potential Cost x Probability)</code> für alle Risiken. </p> </td> 
  </tr> 
  <tr> 
   <td>Kosten zur Risikominderung</td> 
   <td> <p>Die Kosten des Minderungsplans für die Risiken, die Sie schätzen, können im Projekt auftreten.<br>Weitere Informationen zu Risiken im Projekt finden Sie unter <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Erstellen und Bearbeiten von Risiken in Projekten</a>.</p> <p>Dieses Feld wird im Bereich Risiken für jedes Risiko angezeigt, das im Projekt angegeben ist.</p> </td> 
  </tr> 
  <tr> 
   <td>Mögliche Kosten für ein Risiko</td> 
   <td> <p>Die geschätzten finanziellen Kosten zum Zeitpunkt, zu dem die für das Projekt definierten Risiken tatsächlich eintreten würden, unabhängig von ihrer Wahrscheinlichkeit. </p> <p>Dies ist ein manuell aktualisiertes Feld, das zu jedem Risiko im Risikobereich des Business-Case angezeigt wird. </p> </td> 
  </tr> 
  <tr> 
   <td>Risiken potenzielle Gesamtkosten</td> 
   <td> <p>Dies sind die geschätzten Gesamtkosten für alle Risiken, die im Projekt zum Zeitpunkt ihres tatsächlichen Eintritts definiert wurden. </p> <p>Dies wird nach folgender Formel berechnet:</p> <p><code>Risks Total Potential Cost = SUM(Potential Cost of all risks on the project) </code></p> <p>Sie wird als Währungsnummer neben dem Titel des Risikobereichs des Business Case angezeigt.</p> </td> 
  </tr> 
 </tbody> 
</table>
