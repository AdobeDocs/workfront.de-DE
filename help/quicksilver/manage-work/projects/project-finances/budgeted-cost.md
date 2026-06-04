---
content-type: reference
product-area: projects
navigation-topic: financials
title: Berechnen der budgetierten Kosten
description: Budgetierte Kostenverfolgung des Projektfortschritts mit einem Auslastungsbericht berechnen
author: Lisa
feature: Work Management
exl-id: e96fe38f-58c2-4938-9d2d-81d1109123fa
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/20gQnapiR9T6hm3WCv6-8ymhphOOEcZWqUi-05a4CUU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 395
ht-degree: 7%

---

# Berechnen der budgetierten Kosten

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked from "Tracking Project Progress with a Utilization Report"</p>
<p>Keep the structure of this article similar to Calculating Budgeted Labor Cost)</p>
</div>
-->

Die budgetierten Kosten eines Projekts entsprechen den Gesamtkosten, die mit dem Projekt verbunden sind und zum Zeitpunkt der Planung des Projekts geschätzt werden.

## Übersicht über budgetierte Kosten in einem Projekt

Die budgetierten Kosten eines Projekts können nicht manuell geändert werden. Adobe Workfront berechnet die budgetierten Kosten anhand der folgenden Formel:

`Budgeted Cost = Resource Planner Budgeted Labor Cost + Budgeted Expenses Cost + Fixed Cost of the project`

* Der **Ressourcenplaner budgetierte Lohnkosten** in der obigen Berechnung entspricht den Kosten, die mit den Aufgabengebieten im Projekt verknüpft sind.

  Sie können die budgetierten Lohnkosten eines Projekts im Bereich Ressourcenbudgetierung des Business Case oder des Ressourcenplaners verfolgen.

  >[!TIP]
  >
  >  Die budgetierten Lohnkosten eines Projekts im Business Case werden in Berichten und Listen als Ressourcenplaner „budgetierte Lohnkosten“ angezeigt.

  Informationen zu budgetierten Lohnkosten finden Sie im Artikel [Budgetierte Lohnkosten und budgetierte Stunden für Projekte](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* Die **budgetierten Kosten** in der obigen Berechnung sind die geplanten Kosten, die mit den Ausgaben für das Projekt verbunden sind, da sie im Bereich Ausgaben des Business Case oder auf der Registerkarte Ausgaben des Projekts berechnet werden.\
  Weitere Informationen zu Ausgaben für ein Projekt finden Sie im Artikel [Verwalten von Projektausgaben](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* Die **Fixkosten** in der obigen Berechnung ist der feste Betrag, der mit den Kosten des Projekts verknüpft ist, wie im Bereich „Finanzen“ des Abschnitts „Details“ des Projekts definiert.\
  Weitere Informationen zur Unterregisterkarte „Finanzen“ eines Projekts finden Sie im Artikel [Verwalten von Informationen im Bereich „Projektfinanzierung](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

>[!NOTE]
>
>Workfront berechnet alle Kosteninformationen anhand der Projektwährung. Wenn Sie im Ressourcenplaner budgetierte Stunden für Ihre Ressourcen angeben, ist die Option zum Ändern der Projektwährung deaktiviert.
>
>Weitere Informationen zum Ändern der Währung eines Projekts finden Sie im Artikel [Ändern der Projektwährung](../../../manage-work/projects/project-finances/change-project-currency.md).

## Budgetierte Kosten eines Projekts suchen

Die budgetierten Kosten, wie sie im Bereich Ressourcenbudgetierung des Business Case oder des Ressourcenplaners angezeigt werden, werden in den folgenden Bereichen von Workfront unter den folgenden Namen angezeigt:

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
     <td> <p>Portfolio Optimizer</p> <p>Tipp: Die Summe aller budgetierten Kostenwerte des Projekts entspricht den budgetierten Kosten des Portfolios.</p> </td> 
    </tr> 
    <tr> 
     <td>Budgetierte Projektkosten</td> 
     <td>
     <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (NOTE: this was removed with flash)</p>
      -->
      <p>Projektbericht</p> <p>Bericht zu Projekten (Finanzdaten)</p> <p>Aufgabenbericht</p> <p>Problembericht</p> <p>Bericht zu budgetierten Stunden</p> <p>Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Erstellen eines benutzerdefinierten Berichts</a>.</p> </td>
    </tr> 
   </tbody> 
  </table>
