---
content-type: reference
product-area: projects
navigation-topic: financials
title: Berechnete veranschlagte Kosten
description: Berechnung des budgetierten CostTracking-Projektfortschritts mit einem Nutzungsbericht""
author: Alina
feature: Work Management
exl-id: e96fe38f-58c2-4938-9d2d-81d1109123fa
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 2%

---

# Berechnete veranschlagte Kosten

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked from "Tracking Project Progress with a Utilization Report"</p>
<p>Keep the structure of this article similar to Calculating Budgeted Labor Cost)</p>
</div>
-->

Die budgetierten Kosten eines Projekts sind die Gesamtkosten, die mit dem Projekt verbunden sind, wie bei der Planung des Projekts geschätzt.

## Übersicht über die in einem Projekt veranschlagten Kosten

Sie können die budgetierten Kosten eines Projekts nicht manuell ändern. Adobe Workfront berechnet die budgetierten Kosten anhand der folgenden Formel:

`Budgeted Cost = Resource Planner Budgeted Labor Cost + Budgeted Expenses Cost + Fixed Cost of the project`

* Die in der obigen Berechnung unter **Ressourcenplaner budgetierten Arbeitskosten** angegebenen Kosten entsprechen den Kosten, die mit den Stellenrollen im Projekt verbunden sind.

  Sie können die budgetierten Arbeitskosten eines Projekts im Bereich Ressourcenbudgetierung des Business Case oder im Resource Planer nachverfolgen.

  >[!TIP]
  >
  >  Die budgetierten Arbeitskosten eines Projekts im Geschäftsfall werden in Berichten und Listen als Ressourcenplaner mit budgetierten Arbeitskosten angezeigt.

  Informationen zu den budgetierten Arbeitskosten finden Sie im Artikel [Grundlegendes zu den budgetierten Arbeitskosten und den geplanten Arbeitsstunden für Projekte](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* Die in der obigen Berechnung unter **budgeted Expenses Cost** angegebenen Kosten entsprechen den mit den Projektausgaben verbundenen geplanten Kosten, da sie im Bereich &quot;Ausgaben&quot;des Geschäftsfeldes &quot;Geschäftsszenario&quot;oder im Tab &quot;Ausgaben&quot;des Projekts berechnet werden.\
  Weitere Informationen zu Ausgaben für ein Projekt finden Sie im Artikel [Verwalten von Projektausgaben](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* Die **Feste Kosten** in der obigen Berechnung ist der Festbetrag, der mit den Kosten des Projekts verbunden ist, wie im Bereich &quot;Finanzierungen&quot;des Bereichs Details des Projekts definiert.\
  Weitere Informationen zur Unterregisterkarte &quot;Finanzen&quot;eines Projekts finden Sie im Artikel [Verwalten von Informationen im Bereich &quot;Projekt-Finanzen&quot;](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

>[!NOTE]
>
>Workfront berechnet alle Kosteninformationen unter Verwendung der Projektwährung. Wenn Sie im Ressourcenplaner Budgetzeit für Ihre Ressourcen angeben, ist die Option zum Ändern der Projektwährung deaktiviert.
>
>Weitere Informationen zum Ändern der Währung eines Projekts finden Sie im Artikel [Ändern der Projektwährung](../../../manage-work/projects/project-finances/change-project-currency.md).

## Budgetierte Kosten eines Projekts ermitteln

Die im Ressourcenbudgeting-Bereich des Geschäftsszenarios oder im Ressourcenplaner angezeigten Budgetierungskosten werden in den folgenden Bereichen von Workfront unter folgenden Namen angezeigt:

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>Anzeigename der budgetierten Kosten</strong></td> 
     <td><strong>Gebiet von Workfront</strong></td> 
    </tr> 
    <tr> 
     <td>Budgetierte Kosten</td> 
     <td> <p>Business Case-Zusammenfassung</p> <p> <img src="assets/business-case-summary-qs-350x453.png" style="width: 350;height: 453;"> </p> </td> 
    </tr> 
    <tr> 
     <td>Kosten</td> 
     <td> <p>Portfolio Optimizer</p> <p>Tipp: Die Gesamtsumme aller projektbezogenen budgetierten Kosten ist die Budgetierten Kosten des Portfolios.</p> </td> 
    </tr> 
    <tr> 
     <td>Budgetierte Projektkosten</td> 
     <td> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (NOTE: this was removed with flash)</p>
      --> <p>Projektbericht</p> <p>Bericht über das Projekt (Finanzdaten)</p> <p>Aufgabenbericht</p> <p>Problembericht</p> <p>Bericht "Budgetierte Stunde"</p> <p>Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Benutzerspezifischen Bericht erstellen</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>
