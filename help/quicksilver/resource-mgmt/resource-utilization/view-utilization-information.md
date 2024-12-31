---
product-area: resource-management
navigation-topic: resource-utilization
title: Informationen zur Ressourcenauslastung anzeigen
description: Sie können die Auslastung Ihrer Ressourcen im Auslastungsbericht anzeigen.
author: Lisa
feature: Resource Management
exl-id: 785ee3e9-1b2d-4180-bc78-c41e71c5244d
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '7252'
ht-degree: 0%

---

# Informationen zur Ressourcenauslastung anzeigen

<!-- Audited: 01/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this is linked to the UI from the Utilization report. ALWAYS keep this information. DO NOT DELETE!!)</p>
-->

Sie können die Auslastung Ihrer Ressourcen im Auslastungsbericht anzeigen.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Vazgen's response about these hours ie below and he asked us to NOT document them:</p>
<p>It queries Assignments first to get the tasks, issues, projects to display in the view. And then from those gets the hours.</p>
<p>In some cases, like for Planned Hours, it takes them from Assignments</p>
<p>But Budgeted Hours come from projects.</p>
<p>And Actual Hours are their own object - Hour)</p>
</div>
-->

<!--
<p style="color: #dc143c;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This report displays information about the assignments on work items for projects in your environment, like Planned, Actual, and Budgeted Hours, FTE, or Cost.&nbsp;These are hours,&nbsp;FTE, or costs associated with the assignments and not with the tasks and issues themselves.(PRIVATE NOTE:&nbsp;Vazgen's response about these hours: It queries Assignments first to get the tasks, issues, projects to display in the view. And then from those gets the hours. In some cases, like for Planned Hours, it takes them from Assignments; But Budgeted Hours come from projects. And Actual Hours are their own object - Hour.)</p>
-->

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um auf den Auslastungsbericht zuzugreifen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td><p>Neu: Beliebig</p>
       <p>Oder</p>
       <p>Aktuell: Pro oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Folgendes anzeigen oder höher:</p> 
    <ul> 
     <li> <p>Ressourcenverwaltung </p> </li> 
     <li> <p>Projekte</p> </li> 
     <li> <p>Portfolios</p> </li> 
     <li> <p>Programme</p> </li> 
     <li> <p>Finanzdaten, wenn Informationen nach Kosten angezeigt werden sollen</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zeigen Sie den Zugriff auf Projekte, Portfolios und Programme an, um auf den Abschnitt Nutzung im Bereich Ressourcen zuzugreifen</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-highloighted-350x145.png" style="width: 350;height: 145;"> </p> <p>Verwalten des Zugriffs auf ein Projekt, um auf den Abschnitt Nutzung des Projekts zuzugreifen</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-on-project-highloighted-350x289.png" style="width: 350;height: 289;"> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must have View access to the projects you want to view utilization information for as described in this section. If you are still unable to access this information, contact your Workfront administrator. (NOTE:&nbsp;replaced with above table)</p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Prerequisites for accessing utilization information</h2>
<p>(NOTE: drafted, replaced with above table)</p>
<p>To access utilization information as described in this section, ensure that the following conditions are met:</p>
<ul>
<li>You have at least&nbsp;View access to the project, program, or portfolio for which you want to view the utilization information.</li>
<li>Your Workfront administrator must grant you at least View access to&nbsp;Financial&nbsp;Data in your Access Level to be able to view cost and revenue information in the Utilization report. The Workfront administrator must enable both View Role Billing & Cost Rates as well as View User Billing &&nbsp;Cost Rates when they grant you the View access to Financial Data. For information about granting access to&nbsp;Financial&nbsp;Data, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. </li>
<li>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;drafted. No longer the case.) </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization tab is included on any layout template that is assigned to you and that is applied to either the projects you view or to the Reporting area. </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization section is included on any layout template that is assigned to you and that is applied to either the projects you view or to the Resourcing area. </p>
</li>
<li>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization tab is available by default in the Reporting area if the system administrator has not assigned a custom layout template to you. </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization section is available by default in the Resourcing area if the system administrator has not assigned a custom layout template to you. </p>
</li>
</ul>
</div>
-->

## Überblick über den Auslastungsbericht {#overview-of-the-utilization-report}

Mit dem Auslastungsbericht können Sie den Fortschritt, die Kosten oder den Umsatz eines Projekts, Programms oder Portfolios in einem einzigen Bericht anzeigen. Sie können auch den Umsatz mit den Kosten vergleichen.

Sie können den Auslastungsbericht im Bereich Ressourcen anzeigen, um die Auslastung für mehrere Projekte anzuzeigen, oder Sie können ihn auf Projektebene anzeigen, um die Auslastung für die einzelnen Ressourcen (Aufgabengebiete und Benutzer) anzuzeigen, die mit diesem Projekt verknüpft sind.

Informationen zum Zugriff auf und zur Verwendung des Auslastungsberichts finden Sie [ Abschnitt „Verfolgen von Fortschritt, Kosten und Umsatz mit dem ](#track-progress-cost-and-revenue-with-the-utilization-report)&quot; in diesem Artikel.

### Stunden verfolgen (Fortschritt) {#track-hours-progress}

Sie können den Fortschritt verfolgen, indem Sie sich ansehen, wie die budgetierten und geplanten Stunden mit den tatsächlichen Stunden verglichen werden.

Wenn Sie den Fortschritt eines Projekts, Programms oder Portfolios verfolgen, wird der Fortschritt bei beiden Aufgaben und Problemen im Auslastungsbericht angezeigt.

Beim Verfolgen von Stunden sind im Auslastungsbericht die folgenden Informationen verfügbar:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Spaltentitel beim Anzeigen von Stunden</strong> </th> 
   <th><strong>Funktion</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Budgetierte Stunden</strong> </td> 
   <td scope="col"> <p>Die insgesamt budgetierten Stunden für die eingeschlossenen Projekte. Sie können die budgetierten Gesamtstunden für die Gesamtlebensdauer der eingeschlossenen Projekte anzeigen oder die budgetierten Gesamtstunden nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen einzelnen Monat angeben). </p> <p>Budgetierte Stunden werden aus Informationen ausgefüllt, die im Bereich Ressourcenbudgetierung des Business Case oder des Ressourcenplaners verfügbar sind<em>.</em></p> <p>Budgetierte Stunden werden im Auslastungsbericht in einer der folgenden Zeilen angezeigt:</p> 
    <ul> 
     <li> Budgetierte Stunden werden nach Aufgabengebiet und nach einzelnen Benutzern im Auslastungsbericht wie folgt zusammengefasst:<br><strong>Einzelner Benutzer:</strong> Budgetierte Stunden werden für jeden Benutzer im Auslastungsbericht zusammengefasst. Diese budgetierten Stunden sind mit den Aufgaben und Problemen verknüpft, denen der Benutzer in den eingeschlossenen Projekten zugewiesen ist. (Sie können die Zeile des entsprechenden Aufgabengebiets erweitern, um eine Liste von Benutzern mit diesem Aufgabengebiet anzuzeigen.)<br><strong>Aufgabengebiet: </strong> budgetierte Stunden werden im Auslastungsbericht nach Aufgabengebiet zusammengefasst.<br>Budgetierte Stunden werden in einem bestimmten Aufgabengebiet als Ergebnis eines der folgenden Szenarien angezeigt:
     <ul>
     <li>Das Aufgabengebiet wird als primäres Aufgabengebiet des Benutzers definiert, der der Aufgabe oder dem Problem zugewiesen ist, mit der bzw. dem die budgetierten Stunden verknüpft sind. </li> 
       <li>Wenn Sie Nutzungsinformationen für ein einzelnes Projekt anzeigen, wird das Aufgabengebiet des Benutzers verwendet, dem die Stunden zugewiesen wurden, unabhängig davon, ob für die Aufgabe oder das Problem keine Zuweisung vorhanden ist, ein anderer Benutzer ohne Zuweisung eines Aufgabengebiets zugewiesen wurde, ein anderer Benutzer mit einem anderen Aufgabengebiet zugewiesen wurde oder ein anderes Team zugewiesen wurde.</li> 
       <li>Wenn Sie Nutzungsinformationen für mehrere Projekte, Programme oder Portfolios anzeigen, wird das Aufgabengebiet des Benutzers, dem die Stunden zugewiesen wurden, nur verwendet, wenn das Aufgabengebiet einer Aufgabe oder einem Problem in einem Projekt zugewiesen wurde. </li> 
       <li>Das Aufgabengebiet wird der Aufgabe oder dem Problem zugewiesen, der/dem budgetierte Stunden zugeordnet sind, und dem/der Benutzenden, der/dem die Aufgabe oder das Problem zugewiesen ist, ist im System kein Aufgabengebiet definiert.</li> 
      </ul></li> 
    </ul> 
    <ul> 
     <li> <p><strong>Nicht zugewiesene Stunden</strong>: Budgetierte Stunden werden im Auslastungsbericht im Abschnitt Nicht zugewiesene Stunden angezeigt, wenn budgetierte Stunden mit einer Aufgabe oder einem Problem verknüpft sind und der Aufgabe oder dem Problem kein Benutzer oder keine Funktion zugewiesen ist.<br>Dieser Abschnitt wird nur angezeigt, wenn es Stunden im Projekt gibt, die dieser Beschreibung entsprechen, und wenn der Auslastungsbericht nach oder von einem Projekt angezeigt wird. </p> <p>Dieser Abschnitt wird nur angezeigt, wenn es Stunden im Projekt gibt, die dieser Beschreibung entsprechen, und wenn der Auslastungsbericht nach oder von einem Projekt angezeigt wird. </p> </li> 
    </ul> <p>Weitere Informationen zu budgetierten Stunden finden Sie unter <a href="/help/quicksilver/manage-work/projects/project-finances/budgeted-labor-cost.md#locate-the-budgeted-hours-of-a-project">Suchen der budgetierten Stunden eines Projekts</a> unter <a href="/help/quicksilver/manage-work/projects/project-finances/budgeted-labor-cost.md">Budgetierte Lohnkosten und budgetierte Stunden für Projekte</a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Geplante Stunden</strong> </td> 
   <td scope="col">
<p>
Die geplanten Stunden für die eingeschlossenen Projekte, die mit den Zuweisungen für jede Aufgabe und jedes Problem verknüpft sind. Sie können die geplanten Gesamtstunden aller Zuweisungen für das Projekt für die gesamte Lebensdauer der eingeschlossenen Projekte anzeigen oder die geplanten Gesamtstunden nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen einzelnen Monat angeben).
</p>
<p>
<strong>TIPP </strong>
</p>
<p>
Die geplanten Stunden für Elemente mit einer Dauer von 0 werden nicht berücksichtigt. 
</p>
<p>
Geplante Stunden im Auslastungsbericht berücksichtigen, ob die geplanten Stunden während der Dauer einer Aufgabe oder eines Problems neu zugewiesen wurden. 
</p>
<p>
Wenn die tägliche Stundenzuordnung des/r Benutzenden mithilfe des Workload Balancer geändert wurde, können die Daten im Auslastungsbericht beeinflusst werden, wenn die im Auslastungsbericht ausgewählten Datumsangaben nur einen Teil der Dauer einer Aufgabe oder eines Problems enthalten. 
</p>
<p>
Informationen zum Ändern der Zuweisungen für Benutzer finden Sie unter <a href="../workload-balancer/manage-user-allocations-workload-balancer.md">Verwalten von Benutzerzuweisungen im Workload-Balancer</a>.


</p>
<p>
„Geplante Stunden“ wird im Auslastungsbericht in einer der folgenden Zeilen angezeigt:
</p>
<ul>

<li>Die geplanten Stunden werden im Auslastungsbericht nach Aufgabengebiet und nach einzelnen Benutzenden wie folgt zusammengefasst: 
<ul>

<li><strong>Einzelner Benutzer</strong>: Die geplanten Stunden werden für jeden Benutzer im Auslastungsbericht zusammengefasst. Diese geplanten Stunden sind mit den Aufgaben und Problemen verknüpft, denen der/die Benutzende in den eingeschlossenen Projekten zugewiesen ist. (Sie können die Zeile des entsprechenden Aufgabengebiets erweitern, um eine Liste von Benutzern mit diesem Aufgabengebiet anzuzeigen.)

<li><strong>Aufgabengebiet</strong>: Die geplanten Stunden werden nach Aufgabengebiet im Auslastungsbericht eines einzelnen Projekts zusammengefasst.<br>Geplante Stunden werden in einem bestimmten Aufgabengebiet als Ergebnis eines der folgenden Szenarien angezeigt:  
<ul>

<li>Das Aufgabengebiet wird als primäres Aufgabengebiet des Benutzers definiert, der der Aufgabe oder dem Problem zugewiesen ist, mit der bzw. dem die geplanten Stunden verknüpft sind.

<li>Wenn Sie Nutzungsinformationen für ein einzelnes Projekt anzeigen, werden die mit einem Aufgabengebiet verknüpften Stunden in den folgenden Szenarien nicht für das Aufgabengebiet angezeigt:   
<ul>

<li>Für die Aufgabe oder das Problem ist keine Zuweisung vorhanden

<li>Einem Benutzer wird kein Aufgabengebiet zugewiesen

<li>Einem Benutzer wird ein anderes Aufgabengebiet zugewiesen

<li>Der Aufgabe oder dem Problem wurde ein Team zugewiesen
</li>   
</ul>

<li>Wenn Sie Nutzungsinformationen für mehrere Projekte, Programme oder Portfolios anzeigen, wird das Aufgabengebiet des Benutzers, dem die Stunden zugewiesen wurden, nur verwendet, wenn das Aufgabengebiet einer Aufgabe oder einem Problem in einem Projekt zugewiesen wurde. Aufgabengebietsstunden werden beim Anzeigen des Auslastungsberichts für mehrere Projekte nicht separat angezeigt.

<li>Das Aufgabengebiet wird der Aufgabe oder dem Problem zugewiesen, der/dem die geplanten Stunden zugeordnet sind, und dem/der Benutzenden, der/dem die Aufgabe oder das Problem zugewiesen ist, ist im System kein Aufgabengebiet definiert.
</li>  
</ul>

<li><strong>Nicht zugewiesene Stunden</strong>: Geplante Stunden werden im Auslastungsbericht im Abschnitt Nicht zugewiesene Stunden angezeigt, wenn geplante Stunden mit einer Aufgabe oder einem Problem verknüpft sind und der Aufgabe oder dem Problem kein Benutzer oder keine Funktion zugewiesen ist. Dieser Abschnitt wird nur angezeigt, wenn es Stunden im Projekt gibt, die dieser Beschreibung entsprechen, und wenn der Auslastungsbericht für ein einzelnes Projekt angezeigt wird. <br>Weitere Informationen über geplante Stunden finden Sie unter <a href="../../manage-work/tasks/task-information/planned-hours.md">Übersicht über geplante Stunden</a>.
</li> 
</ul>
</li> 
</ul> </td> 
  </tr> 
  <tr> 
   <td><strong>Tatsächliche Stunden</strong> </td> 
   <td> <p> Die Gesamtstunden, die für die Aufgaben, Probleme <span> das Projekt für </span> eingeschlossenen Projekte protokolliert wurden. Sie können die tatsächlichen Gesamtstunden für die Gesamtlebensdauer der eingeschlossenen Projekte anzeigen oder die tatsächlichen Gesamtstunden nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen einzelnen Monat angeben). </p> <p><strong>Warnung</strong> Der Auslastungsbericht enthält Stunden, die für das Projekt protokolliert wurden, untergeordnete Aufgaben, Probleme und übergeordnete Aufgaben mit mindestens einer Zuweisung. Sie enthält keine Stunden, die ohne Zuweisungen bei übergeordneten Aufgaben protokolliert wurden. Es wird empfohlen, keine übergeordneten Aufgaben als Arbeitsaufgaben zu verwenden und Ihren Ressourcen nur untergeordnete Aufgaben zuzuweisen. </p> <p>Tatsächliche Stunden werden im Auslastungsbericht in einer der folgenden Zeilen angezeigt:</p> 
    <ul> 
     <li> Die tatsächlichen Stunden werden nach Aufgabengebiet und nach einzelnen Benutzenden im Auslastungsbericht eines Projekts wie folgt zusammengefasst:<br><strong>Einzelner Benutzer:</strong> Die tatsächlichen Stunden werden im Auslastungsbericht in der Zeile des Benutzers angezeigt, der die Stunden protokolliert hat. (Sie können die Zeile des entsprechenden Aufgabengebiets erweitern, um eine Liste von Benutzern mit diesem Aufgabengebiet anzuzeigen, die Stunden protokolliert haben.)<br><strong>Aufgabengebiet: </strong> tatsächlichen Stunden, die von Benutzenden erfasst wurden, die diesen Aufgabengebieten zugeordnet sind, werden im Auslastungsbericht in der Zeile des entsprechenden Aufgabengebiets zusammengefasst.<br>Tatsächliche Stunden werden in einem bestimmten Aufgabengebiet als Ergebnis eines der folgenden Szenarien angezeigt: 
      <ul> 
       <li>Das Aufgabengebiet wird als primäres Aufgabengebiet des Benutzers definiert, der die Stunden protokolliert hat</li> 
       <li>Für die Aufgabe oder das Problem ist keine Zuweisung vorhanden</li> 
       <li>Einem anderen Benutzer wurde kein Aufgabengebiet zugewiesen</li> 
       <li>Einem anderen Benutzer wird ein anderes Aufgabengebiet zugewiesen</li> 
       <li> <p>Ein Team wird zugewiesen</p> </li> 
      </ul></li>  
     <p>Wenn dem/der Benutzenden, der/die die Stunden protokolliert, kein Aufgabengebiet mit seinem/ihrem Profil zugeordnet ist, ist das für den Auslastungsbericht verwendete Aufgabengebiet das Aufgabengebiet, das der Aufgabe oder dem Problem zugewiesen wurde, in der/dem die Stunden protokolliert werden, oder das Aufgabengebiet, das dem/der Primären Verantwortlichen der Aufgabe oder des Problems zugeordnet ist. </p> 
     <li><strong>Sonstige Stunden: </strong> tatsächlichen Stunden werden im Auslastungsbericht im Abschnitt Sonstige Stunden in der Zeile der Benutzerin oder des Benutzers angezeigt, die bzw. der sich in den Stunden angemeldet hat.<br>Stunden werden in diesem Abschnitt angezeigt, wenn für den Benutzer, der die Stunden protokolliert hat, im System kein Aufgabengebiet definiert ist.<br>Dieser Abschnitt wird nur angezeigt, wenn das Projekt Stunden enthält, die dieser Beschreibung entsprechen. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>Budgetierte Abweichung (für Stunden)</strong> </td> 
   <td> <p>Die insgesamt budgetierten Stunden abzüglich der tatsächlichen Gesamtstunden für die eingeschlossenen Projekte. Sie können die budgetierte Gesamtabweichung für die gesamte Lebensdauer der eingeschlossenen Projekte anzeigen oder die budgetierte Gesamtabweichung nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen einzelnen Monat angeben). </p> <p>Wenn der Wert positiv ist, wird er in grün angezeigt. Dies zeigt an, dass die budgetierten Gesamtstunden größer sind als die tatsächlichen Stunden.</p> <p>Wenn der Wert negativ ist, wird er rot angezeigt. Dies zeigt an, dass die budgetierten Gesamtstunden kleiner als die tatsächlichen Stunden sind.</p> <p> <img src="assets/utilization-variance-budgeted-350x96.png" style="width: 350;height: 96;"> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Geplante Abweichung (für Stunden)</strong> </td> 
   <td> <p>Die geplanten Gesamtstunden abzüglich der tatsächlichen Gesamtstunden für die eingeschlossenen Projekte. Sie können die geplante Gesamtabweichung für die gesamte Lebensdauer der eingeschlossenen Projekte anzeigen oder die geplante Gesamtabweichung nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen einzelnen Monat angeben).</p> <p>Wenn der Wert positiv ist, wird er in grün angezeigt. Dies zeigt an, dass die geplanten Gesamtstunden größer sind als die tatsächlichen Stunden.</p> <p>Wenn der Wert negativ ist, wird er rot angezeigt. Dies zeigt an, dass die geplanten Gesamtstunden geringer sind als die tatsächlichen Stunden.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Kosten nachverfolgen {#track-cost}

Sie können Kosten nachverfolgen, indem Sie sich ansehen, wie die budgetierten Kosten und geplanten Kosten mit den Istkosten verglichen werden.

Beim Nachverfolgen der Kosten eines Projekts, Programms oder Portfolios stammen die Informationen im Auslastungsbericht aus Aufgaben. Kosteninformationen aus Aufgaben sind immer im Auslastungsbericht verfügbar. Die Kosten für Aufgaben werden anhand des Kostentyps der Aufgabe berechnet. Weitere Informationen zum Kostentyp von Aufgaben finden Sie unter [So berechnet Workfront Kostentypen für Aufgaben](/help/quicksilver/manage-work/projects/project-finances/track-costs.md#how-workfront-calculates-cost-types-for-tasks) in [Kosten nachverfolgen](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

Sie können Kosteninformationen im Auslastungsbericht wie folgt anzeigen:

* Für eine bestimmte Woche oder einen bestimmten Monat oder für das gesamte Projekt, Programm oder Portfolio
* Nach Rolle oder Person, für Projekte

Die Währung im Auslastungsbericht wird durch die im Projekt festgelegte Währung bestimmt. Informationen zum Anpassen der Währung für ein Projekt finden Sie unter [Ändern der ](../../manage-work/projects/project-finances/change-project-currency.md).

Die folgenden Informationen sind im Auslastungsbericht beim Verfolgen der Kosten verfügbar:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Spaltentitel bei der Anzeige der Kosten</strong> </th> 
   <th> <p><strong>Funktion</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Budgetierte Kosten</strong> </td> 
   <td scope="col"> <p>Die budgetierten Kosten der eingeschlossenen Projekte. Sie können die budgetierten Gesamtkosten für die gesamte Lebensdauer der eingeschlossenen Projekte anzeigen oder die budgetierten Gesamtkosten nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen einzelnen Monat angeben).</p> <p>Da sich die budgetierten Kosten im Auslastungsbericht auf die Kosten nach Funktion konzentrieren, entspricht die Berechnung den budgetierten Lohnkosten in anderen Bereichen von Workfront. Informationen zur Berechnung budgetierter Lohnkosten finden Sie unter <a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Budgetierte Lohnkosten und budgetierte Stunden für Projekte </a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Geplante Kosten</strong> </td> 
   <td scope="col"> <p>Die geplanten Gesamtkosten der eingeschlossenen Projekte. Sie können die geplanten Gesamtkosten für die gesamte Lebensdauer der eingeschlossenen Projekte anzeigen oder die geplanten Gesamtkosten nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen einzelnen Monat angeben).</p> <p>Beachten Sie, dass die geplanten Kosten für die Wochen-, Monats- und Vierteljahresansichten als Durchschnitt des ausgewählten Zeitraums berechnet werden, in dem die Kostensätze für Aufgabengebiete oder Benutzer zum Datum des Wirksamwerdens gelten.</p><p>Weitere Informationen zur Berechnung der geplanten Kosten für das Projekt finden Sie unter <a href="/help/quicksilver/manage-work/projects/project-finances/track-costs.md#how-workfront-calculates-planned-budgeted-and-actual-costs">So berechnet Workfront geplante, budgetierte und Istkosten</a> in <a href="/help/quicksilver/manage-work/projects/project-finances/track-costs.md">Kosten nachverfolgen</a>.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"><strong>Ist-Kosten</strong> </td> 
   <td scope="col"> <p>Die Ist-Gesamtkosten für die eingeschlossenen Projekte. Sie können die Ist-Gesamtkosten für die gesamte Lebensdauer der eingeschlossenen Projekte anzeigen oder die Ist-Gesamtkosten nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen einzelnen Monat angeben).</p> <p>Weitere Informationen zur Berechnung der Istkosten für das Projekt finden Sie unter <a href="/help/quicksilver/manage-work/projects/project-finances/track-costs.md#how-workfront-calculates-planned-budgeted-and-actual-costs">So berechnet Workfront geplante, budgetierte und Istkosten</a> in <a href="/help/quicksilver/manage-work/projects/project-finances/track-costs.md">Kosten nachverfolgen</a>.</p> </td>
  </tr> 
  <tr> 
   <td><strong>Budgetierte Abweichung (für Kosten)</strong> </td> 
   <td scope="col"> <p>Die budgetierten Gesamtkosten abzüglich der Ist-Gesamtkosten für die eingeschlossenen Projekte. Sie können die budgetierte Gesamtabweichung für die gesamte Lebensdauer der eingeschlossenen Projekte anzeigen oder die budgetierte Gesamtabweichung nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen einzelnen Monat angeben).</p> <p>Wenn der Wert positiv ist, wird er in grün angezeigt. Dies zeigt an, dass die budgetierten Gesamtkosten größer sind als die Ist-Kosten.</p> <p>Wenn der Wert negativ ist, wird er rot angezeigt. Dies zeigt an, dass die budgetierten Gesamtkosten geringer sind als die Ist-Kosten.</p> </td>
  </tr> 
  <tr> 
   <td><strong>Geplante Abweichung (für Kosten)</strong> </td> 
   <td> <p>Die geplanten Gesamtkosten abzüglich der Ist-Gesamtkosten für die eingeschlossenen Projekte. Sie können die geplante Gesamtabweichung für die gesamte Lebensdauer der eingeschlossenen Projekte anzeigen oder die geplante Gesamtabweichung nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen einzelnen Monat angeben). </p> <p>Wenn der Wert positiv ist, wird er in grün angezeigt. Dies zeigt an, dass die geplanten Gesamtkosten größer sind als die Ist-Kosten.</p> <p>Wenn der Wert negativ ist, wird er rot angezeigt. Dies zeigt an, dass die geplanten Gesamtkosten niedriger sind als die Ist-Kosten.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Umsatz nachverfolgen {#track-revenue}

Sie können den Umsatz verfolgen, indem Sie anzeigen, wie der budgetierte und der geplante Umsatz mit dem tatsächlichen Umsatz verglichen werden.

Beim Verfolgen des Umsatzes eines Projekts, Programms oder Portfolios wird der Umsatz nur aus Aufgaben in den Auslastungsbericht einbezogen.

Die Informationen in der folgenden Tabelle sind im Auslastungsbericht beim Verfolgen des Umsatzes verfügbar.

Informationen zu den spezifischen Feldern und wie Workfront sie berechnet, finden Sie auch unter [Kosten ](../../manage-work/projects/project-finances/track-costs.md) und [Übersicht über Abrechnung und Umsatz](../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Spaltentitel beim Anzeigen des Umsatzes</strong> </th> 
   <th> <strong>Funktion</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Budgetierte Einnahmen</strong> </td> 
   <td scope="col"> <p>Die insgesamt budgetierten Stunden multipliziert mit dem Abrechnungssatz der Funktion für die eingeschlossenen Projekte. Sie können die budgetierten Gesamteinnahmen für die gesamte Lebensdauer der eingeschlossenen Projekte anzeigen oder die budgetierten Gesamteinnahmen nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen einzelnen Monat angeben).</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Geplante Einnahmen</strong> </td> 
   <td scope="col"> <p>Geplanter Umsatz im Auslastungsbericht ist der Umsatz, der mit den geplanten Stunden verknüpft ist, die den Ressourcen zugeordnet wurden, die den Aufgaben im Projekt zugewiesen wurden.</p> <p>Workfront berechnet die geplanten Projekteinnahmen für den Auslastungsbericht anhand der folgenden Formel:</p> <p><code>Project Planned Revenue = SUM (All Tasks Planned Revenue)</code> </p> 
   <p><b>HINWEIS</b>
   <p>Der im Auslastungsbericht angezeigte geplante Projektumsatz unterscheidet sich von dem geplanten Umsatz, der im Bereich „Projektdetails“ und in den Projektberichten angezeigt wird. </p> <p>Die geplanten Einnahmen im Bereich Projektdetails spiegeln die Einnahmen aus der Aufgabe sowie die Festeinnahmen des Projekts wider. Der Bericht „Geplanter Umsatz“ zeigt den geplanten Umsatz an, der nur mit den Aufgaben im Projekt verknüpft ist. </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p>Wenn das Projekt 1 Aufgabe mit 10 Stunden hat, einem Berater mit einem Stundensatz von 20 US-Dollar zugewiesen ist und das Projekt einen festen Umsatz von 100 US-Dollar hat, zeigt der Auslastungsbericht 200 US-Dollar für den geplanten Umsatz an (der geplante Umsatz, der mit den Stunden für die Aufgabe verknüpft ist). Im Abschnitt Projektdetails werden 300 $ angezeigt (der geplante Umsatz aus der Aufgabe und der feste Umsatz für das Projekt). </p> 
     </div> <p>Weitere Informationen zu den geplanten Aufgaben- und Projekteinnahmen außerhalb des Auslastungsberichts finden Sie unter <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Übersicht über Abrechnung und Umsatz</a>.</p> </p> <p>Die Art und Weise, wie der Auslastungsbericht die geplanten Einnahmen für die eingeschlossenen Projekte berechnet und anzeigt, berücksichtigt den für die Aufgabe festgelegten Umsatztyp. </p> <p>Je nach Umsatztyp jeder Aufgabe im Projekt sind die folgenden Szenarien vorhanden: </p> <p><strong>Fester Umsatz</strong> Unabhängig von den Aufgabenzuordnungen wird der Umsatz für die Aufgabe immer anhand des für die Aufgabe angegebenen Festbetrags berechnet.</p> <p><b>WICHTIG</b>

Im Gegensatz zu anderen Bereichen von Workfront berechnet der Auslastungsbericht den geplanten Umsatz für Festeinnahmenaufgaben, indem der Festeinnahme-Wert gleichmäßig durch die Anzahl der für die Aufgabe geplanten Stunden geteilt wird. </p> <p>Beispielsweise hat eine Aufgabe einen Umsatz von 200 $. Wenn für die Aufgabe vier geplante Stunden vorhanden sind, würde jede Stunde 50 $ betragen. Dieser wird auf Benutzer- und Rollenebene verteilt. Diese Verteilung ist im Auslastungsbericht eindeutig.</p> <p><b>HINWEIS</b>

Wenn Sie eine Aufgabe mit festem Umsatz haben und keine geplanten Stunden für die Aufgabe vorhanden sind, wird der Umsatz nicht im Auslastungsbericht angezeigt, da es keine Möglichkeit gibt, ihn auf die Stunden zu verteilen. Wenn Sie für Aufgaben mit Festeinnahmen und ohne Zuweisungen geplante Stunden haben, wird der Umsatz als Nicht zugewiesener Umsatz angezeigt. </p> <p><strong>Funktion pro Stunde:</strong> Der Umsatz aus der Aufgabe wird anhand des Abrechnungssatzes berechnet, der für eine bestimmte Funktion festgelegt wurde, multipliziert mit der Anzahl der geplanten Stunden, die mit dieser Funktion verknüpft sind. Workfront verwendet die folgende Formel:</p> <p><code>Stundensatz nach Funktion - Geplanter Umsatz = SUMME (Geplante Stunden aus Funktion für alle Aufgaben) * Abrechnungssatz für Funktion</code></p><p><b>HINWEIS</b> Der Stundensatz für die Abrechnung in der Formel berücksichtigt alle Datumsänderungen, die mit Wirkung vom Tag des Inkrafttretens des Satzes vorgenommen werden.</p>   <p><strong>Benutzer pro Stunde:</strong> Der Umsatz aus der Aufgabe wird anhand des Abrechnungssatzes berechnet, der für einen bestimmten Benutzer festgelegt wurde, multipliziert mit der Anzahl der geplanten Stunden, die mit diesem Benutzer verknüpft sind. Workfront verwendet die folgende Formel:</p> <p><code>Geplanter Umsatz des Benutzers pro Stunde = SUMME(Geplante Stunden der Benutzer für alle Aufgaben) * Abrechnungssatz des Benutzers</code> </p> <p><b>HINWEIS</b> Der Stundensatz für die Abrechnung in der Formel berücksichtigt alle Datumsänderungen, die mit Wirkung vom Tag des Inkrafttretens des Satzes vorgenommen werden.</p> <p><b>Stundensatz nach Funktion oder Stundensatz nach Benutzer plus fest</b> </p> <p><b>WICHTIG</b>

Im Gegensatz zu anderen Bereichen von Workfront berechnet der Auslastungsbericht den geplanten Umsatz, indem er die Festeinnahmen gleichmäßig durch die Anzahl der für die Aufgabe geplanten Stunden teilt. </p> <p>Die folgenden Fälle liegen vor: </p>
<ul>
<li> <p><strong>Funktion „Stündlich plus fest“</strong> Der Umsatz für die Aufgabe wird anhand des Abrechnungssatzes berechnet, der für eine bestimmte Funktion festgelegt wurde, multipliziert mit der Anzahl der geplanten Stunden, die mit der Funktion verknüpft sind. Darüber hinaus wird ein fester Betrag, der für die Aufgabe angegeben ist, zum Rollensatz hinzugefügt. Workfront verwendet die folgende Formel:</p> <p><code>Funktion pro Stunde plus fester geplanter Umsatz = [SUM(Geplante Stunden aus Funktion für alle Aufgaben) * Funktion Abrechnungssatz] + SUM(Obergrenze oder fester Betrag der Aufgabe / Geplante Stunden der Aufgabe)</code> </p> </li>
<li> <p><strong>Benutzer pro Stunde plus fest</strong> Der Abrechnungssatz, der für einen bestimmten Benutzer festgelegt wurde, multipliziert mit der Anzahl der geplanten Stunden für die Aufgabe von diesem Benutzer. Darüber hinaus wird ein fester Betrag, der für die Aufgabe angegeben ist, zur Benutzerrate hinzugefügt. Workfront verwendet die folgende Formel:</p> <p><code>Benutzer pro Stunde plus fester geplanter Umsatz = [SUM(Geplante Stunden des Benutzers für alle Aufgaben) * Benutzer-Abrechnungssatz] + SUM(Obergrenze oder fester Betrag der Aufgabe / Geplante Stunden der Aufgabe)</code> </p> </li>
</ul> <p><b>Funktion oder Benutzer pro Stunde mit Obergrenze</b> </p> <p><b>WICHTIG</b>

Im Gegensatz zu anderen Bereichen von Workfront gilt der Betrag über dem Höchstbetrag als Festeinnahme, wenn die geplanten Einnahmen den Höchstbetrag überschreiten. Der geplante Umsatz wird berechnet, indem der feste Umsatz gleichmäßig durch die Anzahl der geplanten Stunden für die Aufgabe geteilt und dann der Begrenzungsbetrag und der Funktion oder der Benutzer-Stundenumsatz hinzugefügt werden. <br></p> <p>Die folgenden Fälle liegen vor: </p>
<ul>
<li> <p><strong>Stundensatz nach Funktion mit Obergrenze: </strong> Aufgaben werden stündlich wie in der Stundensatz-Funktion in Rechnung gestellt, sie haben jedoch einen maximalen Höchstbetrag, den Sie angeben können. Workfront verwendet die folgende Formel:</p> <p><code>Funktion Stündlich mit Obergrenze Geplanter Umsatz = [SUMME(Geplante Stunden aus Funktion für alle Aufgaben und Probleme) * Funktion Abrechnungssatz] + Obergrenze Betrag der Aufgabe + SUMME(Betrag über Obergrenze Betrag / Geplante Stunden der Aufgabe)</code> </p> </li>
<li> <p><strong>Benutzer stündlich mit Obergrenze: </strong> Aufgaben werden stündlich wie im Benutzer stündlich in Rechnung gestellt, sie haben jedoch einen maximalen Begrenzungsbetrag, den Sie angeben können. Workfront verwendet die folgende Formel: </p> <p><code>Benutzer pro Stunde mit Obergrenze Geplanter Umsatz = [SUMME(Geplante Stunden des Benutzers für alle Aufgaben) * Benutzer-Abrechnungssatz] + Obergrenze der Aufgabe + SUMME(Betrag über dem Begrenzungsbetrag / Geplante Stunden der Aufgabe)</code> </p> </li>
</ul> <p>Weitere Informationen dazu, welche Funktion oder welcher Benutzer bei der Berechnung des geplanten Umsatzes berücksichtigt wird, finden Sie unter <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Übersicht über Abrechnung und Umsatz</a>.</p> </td>
</tr> 
  <tr> 
   <td><strong>Tatsächliche Einnahmen</strong> </td>
   <td> <p>Die tatsächlichen Einnahmen sind die Einnahmen, die mit den tatsächlichen Stunden der Aufgaben und des Projekts verknüpft sind. Weitere Informationen zu den tatsächlichen Einnahmen finden Sie unter <a href="/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md#track-revenue-amounts">Verfolgen der </a>" in <a href="/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md">Übersicht über Abrechnung und Umsatz</a>.</p>

<p>Die Methode, mit der der Auslastungsbericht die tatsächlichen Einnahmen für die eingeschlossenen Projekte berechnet, hängt vom für die Aufgabe festgelegten Umsatztyp ab und sieht wie folgt aus:</p> <p><strong>Fester Umsatz</strong> Unabhängig von den Aufgabenzuordnungen wird der Umsatz für die Aufgabe immer anhand des für die Aufgabe angegebenen Festbetrags berechnet.</p> <p><b>WICHTIG</b>

Im Gegensatz zu anderen Bereichen von Workfront berechnet der Auslastungsbericht den tatsächlichen Umsatz, indem er die festen Einnahmen gleichmäßig durch die Anzahl der für die Aufgabe protokollierten Stunden teilt. </p> <p> </p> <p>Beispielsweise hat eine Aufgabe einen tatsächlichen Umsatz von 200 USD. Wenn die Aufgabe 4 Stunden umfasst, würde jede Stunde 50 $ betragen. Dieser wird auf Benutzer- und Rollenebene verteilt. Diese Verteilung ist im Auslastungsbericht eindeutig.</p> <p><b>HINWEIS</b>

Wenn Sie eine Aufgabe mit festem Umsatz haben und keine tatsächlichen Stunden für die Aufgabe vorhanden sind, wird der tatsächliche Umsatz nicht im Auslastungsbericht angezeigt, da keine Möglichkeit besteht, Stunden zu verteilen. </p> <p><strong>Stundensatz nach Funktion: </strong> Der Umsatz aus der Aufgabe wird anhand des Abrechnungssatzes berechnet, der für eine bestimmte Funktion festgelegt wurde, multipliziert mit der Anzahl der tatsächlichen Stunden.</p> <p>Workfront verwendet die folgende Formel:</p> <p><code>Stundensatz nach Funktion - Tatsächlicher Umsatz = SUMME (Tatsächliche Stunden aus Funktion für alle Aufgaben) * Abrechnungssatz der Funktion</code> </p> <p><b>HINWEIS</b> Der Stundensatz für die Abrechnung in der Formel berücksichtigt alle Datumsänderungen, die mit Wirkung vom Tag des Inkrafttretens des Satzes vorgenommen werden.</p> <p><strong>Benutzer pro Stunde:</strong> Der Umsatz aus der Aufgabe wird anhand des Abrechnungssatzes berechnet, der für einen bestimmten Benutzer festgelegt wurde, multipliziert mit der Anzahl der Stunden, die für die Aufgabe von diesem Benutzer protokolliert wurden. Workfront verwendet die folgende Formel:</p> <p><code>Benutzer pro Stunde - Tatsächlicher Umsatz = SUM(Tatsächliche Stunden des Benutzers für alle Aufgaben) * Benutzer-Abrechnungssatz</code></p> <p><b>HINWEIS</b> Der Stundensatz für die Abrechnung in der Formel berücksichtigt alle Datumsänderungen, die mit Wirkung vom Tag des Inkrafttretens des Satzes vorgenommen werden.</p> <p><b>Stundensatz nach Funktion oder Benutzer plus fest</b> </p> <p><b>WICHTIG</b>

Im Gegensatz zu anderen Bereichen von Workfront berechnet der Auslastungsbericht den tatsächlichen Umsatz, indem er die festen Einnahmen gleichmäßig durch die Anzahl der für die Aufgabe protokollierten Stunden teilt. </p> <p>Die folgenden Fälle liegen vor: </p>
<ul>
<li> <p><strong>Funktion „Stündlich plus fest“</strong> Der für eine bestimmte Funktion festgelegte Abrechnungssatz, multipliziert mit der Anzahl der Stunden, die für die Aufgabe von einem Benutzer mit dieser Funktion protokolliert wurden. Darüber hinaus wird ein fester Betrag, der für die Aufgabe angegeben ist, zum Rollensatz hinzugefügt. </p> <p>Workfront verwendet die folgende Formel:</p> <p><code>Funktion Stündlich plus Fester tatsächlicher Umsatz = [SUM(Tatsächliche Stunden aus Funktion für alle Aufgaben) * Funktion Abrechnungssatz] + SUM(Obergrenze oder Fester Betrag der Aufgabe / Tatsächliche Stunden der Aufgabe)</code> </p> </li>
<li> <p><strong>Benutzer pro Stunde plus fest</strong> Der Abrechnungssatz, der für einen bestimmten Benutzer festgelegt wurde, multipliziert mit der Anzahl der Stunden, die dieser Benutzer für die Aufgabe protokolliert hat. Darüber hinaus wird ein fester Betrag, der für die Aufgabe angegeben ist, zur Benutzerrate hinzugefügt. </p> <p>Workfront verwendet die folgende Formel:</p> <p><code>Benutzer pro Stunde plus fester tatsächlicher Umsatz = [SUM(Tatsächliche Stunden aus Funktion für alle Aufgaben) * Benutzer-Abrechnungssatz] + SUM(Obergrenze oder fester Betrag der Aufgabe / Benutzerstunden der Aufgabe)</code> </p> </li>
</ul> <p><b>Funktion oder Benutzer pro Stunde mit Obergrenze</b> </p> <p><b>WICHTIG</b>

Im Gegensatz zu anderen Bereichen von Workfront gilt der Betrag über dem Höchstbetrag als Festeinnahme, wenn die geplanten Einnahmen den Höchstbetrag überschreiten. Der geplante Umsatz wird berechnet, indem der feste Umsatz gleichmäßig durch die Anzahl der geplanten Stunden für die Aufgabe geteilt und dann der Begrenzungsbetrag und der Funktion oder der Benutzer-Stundenumsatz hinzugefügt werden. <br></p> <p>Die folgenden Fälle liegen vor:</p>
<ul>
<li> <p><strong>Stundensatz nach Funktion mit Obergrenze: </strong> Aufgaben werden stündlich wie in der Stundensatz-Funktion in Rechnung gestellt, sie haben jedoch einen maximalen Höchstbetrag, den Sie angeben können. Workfront verwendet die folgende Formel:</p> <p><code>Funktion Stündlich mit Obergrenze des tatsächlichen Umsatzes = [SUM(Tatsächliche Stunden aus der Funktion für alle Aufgaben und Probleme) * Funktion Abrechnungssatz] + Obergrenze des Vorgangs + SUM(Betrag über der Obergrenze des Betrags / Tatsächliche Stunden der Aufgabe)</code></p> </li>
<li> <p><strong>Benutzer stündlich mit Obergrenze: </strong> Aufgaben werden stündlich wie im Benutzer stündlich in Rechnung gestellt, sie haben jedoch einen maximalen Begrenzungsbetrag, den Sie angeben können.</p> <p> Workfront verwendet die folgende Formel:</p> <p><code>Benutzer pro Stunde mit Begrenzung des tatsächlichen Umsatzes = [SUM(Tatsächliche Stunden aus der Funktion für alle Aufgaben und Probleme) * Benutzer-Abrechnungssatz] + Obergrenze der Aufgabe + SUM(Betrag über dem Begrenzungsbetrag / Tatsächliche Stunden der Aufgabe)</code> </p> </li>
</ul>
<p><strong>Projektumsatz</strong>: Der Umsatz in Verbindung mit den für das Projekt protokollierten Stunden wird unter Berücksichtigung des Betrags für „Abrechnung pro Stunde“ für das primäre Aufgabengebiet des Benutzers berechnet, der die Zeit protokolliert. Es wird nicht empfohlen, die Zeit im Projekt zu erfassen. </p>
<p><b>HINWEIS</b>

Wenn der Benutzer keinem Aufgabengebiet zugeordnet ist oder die Fakturierung pro Stunde für die Primäre Funktion null ist, berechnet Workfront den tatsächlichen Umsatz anhand des Betrags für die Fakturierung pro Stunde für den Benutzer. Wenn der/die Benutzende keinen Betrag „Abrechnung pro Stunde“ in seinem/ihrem Profil hat, ist der tatsächliche Umsatz gleich null. </p>
</td> 
  </tr> 
  <tr> 
   <td><strong>Budgetierte Abweichung (für Einnahmen)</strong> </td> 
   <td> <p>Die tatsächlichen Gesamteinnahmen abzüglich der budgetierten Einnahmen für die eingeschlossenen Projekte.<br>Sie können die budgetierte Gesamtabweichung für die gesamte Lebensdauer der eingeschlossenen Projekte anzeigen oder die budgetierte Gesamtabweichung nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen einzelnen Monat angeben).</p> <p>Wenn der Wert positiv ist, wird er in grün angezeigt. Dies zeigt an, dass die budgetierten Gesamteinnahmen höher sind als die tatsächlichen Einnahmen.</p> <p>Wenn der Wert negativ ist, wird er rot angezeigt. Dies zeigt an, dass die budgetierten Gesamteinnahmen geringer sind als die tatsächlichen Einnahmen.</p> </td>
  </tr> 
  <tr> 
   <td><strong>Geplante Abweichung (für Umsatz)</strong> </td> 
   <td> <p>Die tatsächlichen Gesamteinnahmen abzüglich der geplanten Gesamteinnahmen für die eingeschlossenen Projekte.<br>Sie können die geplante Gesamtabweichung für die gesamte Lebensdauer der eingeschlossenen Projekte anzeigen oder die geplante Gesamtabweichung nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen einzelnen Monat angeben). </p> <p>Wenn der Wert positiv ist, wird er in grün angezeigt. Dies zeigt an, dass die geplanten Gesamteinnahmen höher sind als die tatsächlichen Einnahmen.</p> <p>Wenn der Wert negativ ist, wird er rot angezeigt. Dies zeigt an, dass die geplanten Gesamteinnahmen geringer sind als die tatsächlichen Einnahmen.</p> </td>
  </tr> 
 </tbody> 
</table>

<!--Note from the table about Actual revenue: 
     <p>Actual Revenue is displayed in the Utilization report only after the task is marked as Complete or Done (or a status that equates with Complete).</p>
    -->

<!--More notes from the table: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;the note below is duplicated in this article: /Content/Manage work/Projects/Project Finances/billing-and-revenue-overview.html and in the glossary)</p>
   -->

### Einnahmen mit geplanten Kosten und Istkosten vergleichen {#compare-revenue-against-planned-and-actual-costs}

Sie können die geplanten Kosten oder Istkosten zusammen mit dem geplanten Umsatz anzeigen. Die Spanne (%) wird ebenfalls angezeigt (die Spanne wird als Umsatz - Kosten/Umsatz berechnet).

Der Auslastungsbericht enthält folgende Informationen zum Vergleich der Einnahmen mit den geplanten Kosten und den Istkosten:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Spaltentitel bei der Ansicht Umsatz vs. Kosten (geplant)</strong> </th> 
   <th> <strong>Funktion</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Geplante Kosten</strong> </td> 
   <td scope="col"> Die geplanten Gesamtkosten der eingeschlossenen Projekte. Sie können die geplanten Gesamtkosten für die gesamte Lebensdauer der eingeschlossenen Projekte anzeigen oder die geplanten Gesamtkosten nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen einzelnen Monat angeben). </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Geplante Einnahmen</strong> </td> 
   <td scope="col"> <p>Geplanter Umsatz ist der Umsatz, der mit den geplanten Stunden der Aufgaben verknüpft ist. </p> <p>Die Art und Weise, wie der Auslastungsbericht die geplanten Einnahmen für die eingeschlossenen Projekte berechnet und anzeigt, unterscheidet sich je nach dem für die Aufgabe festgelegten Umsatztyp, wie im Abschnitt <a href="#track-revenue" class="MCXref xref">Verfolgen von </a>" in diesem Artikel beschrieben.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Spanne</strong> </td> 
   <td scope="col"> <p>Die Spanne in Prozent wird wie folgt berechnet:</p> <p><code>Planned Revenue - Planned Cost / Planned Revenue * 100. </code></p> <p><b>NOTIZ</b>

Ist der geplante Umsatz gleich 0, wird die Spanne als 0 angezeigt. </p> </td>
</tr> 
  <tr> 
   <td scope="col"> <p scope="col"><strong>Spaltentitel beim Anzeigen von Umsatz und Kosten (Ist-Kosten)</strong> </p>  </td> 
   <td scope="col"><p><strong>Funktion</strong></p></td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Ist-Kosten</strong> </td> 
   <td scope="col"> <p>Die Ist-Gesamtkosten für die eingeschlossenen Projekte. Sie können die Ist-Gesamtkosten für die gesamte Lebensdauer der eingeschlossenen Projekte anzeigen oder die Ist-Gesamtkosten nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen einzelnen Monat angeben).</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Tatsächliche Einnahmen</strong> </td> 
   <td> <p>Der tatsächliche Umsatz ist der Umsatz, der mit den tatsächlichen Stunden der Aufgaben verknüpft ist.</p> <p>Der tatsächliche Umsatz wird im Auslastungsbericht erst angezeigt, nachdem die Aufgabe als „Abgeschlossen“ oder „Fertig“ (oder in einem Status, der „Abgeschlossen“ entspricht) gekennzeichnet wurde.</p> <p>Die Methode, mit der der tatsächliche Umsatz für die eingeschlossenen Projekte im Auslastungsbericht berechnet wird, hängt vom für die Aufgabe festgelegten Umsatztyp ab, wie im Abschnitt <a href="#track-revenue" class="MCXref xref">Verfolgen des </a>" in diesem Artikel beschrieben. </p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Spanne</strong> </td> 
   <td> <p>Die Spanne in Prozent wird wie folgt berechnet:</p> <p>Tatsächliche Einnahmen - Tatsächliche Kosten/Tatsächliche Einnahmen * 100. </p> <p><b>NOTIZ</b>

Wenn der tatsächliche Umsatz 0 entspricht, wird die Spanne als 0 angezeigt. </p> </td>
</tr> 
 </tbody> 
</table>

<!--Note from the table from above "Function" header in the middle of the table; right after the "Planned Revenue"/"Margin" definition: 
     <p scope="col" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This needs to be either split in two tables of formatted differently)</p>
    -->

## Verfolgen Sie Fortschritt, Kosten und Umsatz mit dem Nutzungsbericht {#track-progress-cost-and-revenue-with-the-utilization-report}

Sie können den Fortschritt oder die Kosten eines Projekts, Programms oder Portfolios verfolgen.

Sie können Informationen zum Auslastungsbericht für eine bestimmte Woche oder einen bestimmten Monat oder für die Gesamtlebensdauer der Projekte anzeigen.

So verfolgen Sie den Fortschritt oder die Kosten eines oder mehrerer Projekte mit einem Auslastungsbericht:

1. Führen Sie einen der folgenden Schritte aus, je nachdem, ob Sie Nutzungsinformationen für ein einzelnes Projekt, mehrere Projekte, ein Programm oder ein Portfolio anzeigen:

   * So zeigen Sie Nutzungsinformationen für ein einzelnes Projekt an:

      1. Gehen Sie zu einem Projekt, für das Sie Nutzungsinformationen anzeigen möchten, und klicken Sie dann auf **Weitere Informationen anzeigen > Nutzung**.
      1. Nutzungsinformationen werden beim Anzeigen eines einzelnen Projekts automatisch angezeigt und das Anwenden eines Filters ist nicht erforderlich.\
         Wenn Sie den Auslastungsbericht filtern möchten, können Sie einen Filter anwenden und dann auf &quot;**&quot;**.\
         Informationen zum Filtern des Auslastungsberichts finden Sie unter [Filtern von ](#filter-utilization-information)) in diesem Artikel.\
         Nutzungsinformationen werden für einzelne Benutzer und Rollen angezeigt (Benutzer werden innerhalb ihrer zugehörigen Rolle gruppiert).

   * So zeigen Sie Nutzungsinformationen für mehrere Projekte an:

     {{step1-to-utilization-report}}

      1. Wenden Sie einen Filter auf den Nutzungsbericht an und klicken Sie dann auf **Ausführen**.
Sie müssen ein oder mehrere Projekte im Filter angeben, bevor Sie den Auslastungsbericht ausführen. Informationen zum Filtern des Auslastungsberichts finden Sie unter [Filtern von ](#filter-utilization-information)) in diesem Artikel.\
         Nutzungsinformationen werden für einzelne Rollen und Projekte angezeigt (Rollen sind in ihrem zugehörigen Projekt gruppiert).

   * So zeigen Sie Nutzungsinformationen für ein Programm an:

     {{step1-to-utilization-report}}

      1. Klicken Sie **Anzeigen**>**Programme**.
      1. Wenden Sie einen Filter auf den Nutzungsbericht an und klicken Sie dann auf **Ausführen**.\
         Sie müssen ein oder mehrere Programme im Filter angeben, bevor Sie den Auslastungsbericht ausführen. Informationen zum Filtern des Auslastungsberichts finden Sie unter [Filtern von ](#filter-utilization-information)) in diesem Artikel.\
         Auslastungsinformationen werden für einzelne Projekte und Programme angezeigt (Projekte werden innerhalb ihres zugehörigen Programms gruppiert).

   * So zeigen Sie Nutzungsinformationen für ein Portfolio an:

     {{step1-to-utilization-report}}

      1. Klicken Sie **Anzeigen**>**Portfolios**.
      1. Wenden Sie einen Filter auf den Nutzungsbericht an und klicken Sie dann auf **Ausführen**.\
         Sie müssen ein oder mehrere Portfolios im Filter angeben, bevor Sie den Auslastungsbericht ausführen. Informationen zum Filtern des Auslastungsberichts finden Sie unter [Filtern von ](#filter-utilization-information)) in diesem Artikel.\
         Nutzungsinformationen werden für einzelne Projekte, Programme und Portfolios angezeigt (Projekte werden innerhalb ihres zugehörigen Programms gruppiert, Programme innerhalb ihres zugehörigen Portfolios).

1. Klicken Sie oben rechts im Auslastungsbericht auf **Anzeigen** und wählen Sie dann im Menü Folgendes aus:

   * **Kosten**
   * **Stunden**
   * **Umsatz**
   * **Einnahmen vs. Kosten (geplant)**
   * **Einnahmen vs. Kosten (tatsächlich)**

   Die von Ihnen ausgewählte Option bestimmt, welche Spalten und Informationen im Bericht verfügbar sind.
   ![Optionen anzeigen](assets/utilization-view-dropdown.png)

1. (Optional) Wählen Sie den Datumsbereich aus, für den Nutzungsinformationen angezeigt werden sollen. Sie können Informationen für eine bestimmte Woche oder einen bestimmten Monat links neben der Spalte &quot;**&quot;**. Informationen zum gesamten Projekt, Programm oder Portfolio werden immer in der Spalte **Allgemein** angezeigt.\
   Weitere Informationen finden Sie unter [Anpassen des Datumsbereichs, für den Informationen angezeigt werden](#adjust-the-date-range-for-which-information-is-displayed) in diesem Artikel.

1. (Optional) Klicken Sie auf einen Spaltentitel, um den Auslastungsbericht nach den Informationen in dieser Spalte zu sortieren. Die Sortierung funktioniert nur, wenn Sie mehrere Elemente in Ihren Bericht einbeziehen. Sie können beispielsweise die Ergebnisse Ihres Berichts sortieren, wenn Sie mehr als ein Projekt (oder Portfolio oder Programm) betrachten. Sie können die Ergebnisse nicht sortieren, wenn Sie nur ein Projekt (oder ein Portfolio oder ein Programm) auf einmal betrachten.
1. Verwenden Sie die Informationen im Abschnitt [Überblick über den Auslastungsbericht](#overview-of-the-utilization-report) in diesem Artikel, um mehr über die einzelnen Spalten im Auslastungsbericht zu erfahren.

## Filtern von Nutzungsinformationen {#filter-utilization-information}

Sie können den Inhalt filtern, der in einem Auslastungsbericht für ein Projekt angezeigt wird. Sie können nach Aufgaben, Problemen, Rollen und benutzerdefinierten Daten filtern. Wenn Sie einen Filter anwenden, enthält der Auslastungsbericht Informationen, die auf den von Ihnen ausgewählten Kriterien basieren.

Sie können einen neuen Filter erstellen oder einen zuvor erstellten Filter anwenden.

### Filter erstellen oder ändern {#create-or-modify-a-filter}

Wenn Sie einen Filter erstellen, haben alle Workfront-Benutzenden, die Zugriff auf den Auslastungsbericht haben, auch Zugriff auf den von Ihnen erstellten Filter. Wenn Sie einen vorhandenen Filter ändern, wird der Filter entsprechend für alle Benutzenden geändert, die Zugriff auf den Auslastungsbericht haben.

So erstellen oder ändern Sie einen Filter:

1. Öffnen Sie den Auslastungsbericht.
Siehe [Verfolgen von Fortschritt, Kosten und Umsatz mit dem Auslastungsbericht](#track-progress-cost-and-revenue-with-the-utilization-report), um dies zu tun.

1. Klicken Sie auf **Filter**-Symbol, um die Filteroptionen anzuzeigen.
1. (Bedingt) Um einen vorhandenen Filter zu ändern, klicken Sie auf **Dropdown** Menü Filter und wählen Sie dann den Filter aus, den Sie ändern möchten.
1. Geben Sie die folgenden Informationen an, um den Filter zu erstellen oder zu ändern:

   * **Portfolios:** Sie den Namen des Portfolios ein, das die Informationen enthält, die Sie in den Auslastungsbericht aufnehmen möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird\
     Wiederholen Sie diesen Vorgang, um Informationen aus mehreren Portfolios in den Auslastungsbericht aufzunehmen.\
     Um alle Portfolios aus Ihrem System in Ihren Filter einzubeziehen, klicken Sie auf **Alle hinzufügen**. (Diese Option ist nur verfügbar, wenn Sie weniger als 10 Portfolios in Ihrem System haben.)

   * **Programme:** Beginnen Sie mit der Eingabe des Programmnamens, der die Informationen enthält, die Sie in den Auslastungsbericht aufnehmen möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.\
     Wiederholen Sie diesen Vorgang, um Informationen aus mehreren Aufgaben in den Auslastungsbericht aufzunehmen.\
     Wenn Sie bereits Portfolios im Filter festgelegt haben, muss das angegebene Programm aus den bereits im Filter enthaltenen Portfolios stammen. Ist dies nicht der Fall, werden die Daten aus dem Programm nicht in den Auslastungsbericht aufgenommen.\
     Um alle Programme aus Ihrem System in Ihren Filter einzubeziehen, klicken Sie auf **Alle hinzufügen**. (Diese Option ist nur verfügbar, wenn weniger als 20 Programme im System vorhanden sind.)

   * **Projekte:** Sie den Namen des Projekts ein, das die Informationen enthält, die Sie in den Auslastungsbericht aufnehmen möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.\
     Wiederholen Sie diesen Vorgang, um Informationen aus mehreren Projekten in den Auslastungsbericht aufzunehmen.\
     Wenn Sie bereits Portfolios oder Programme im Filter angegeben haben, muss das angegebene Projekt aus einem der Portfolios oder Programme stammen, die bereits im Filter enthalten sind. Ist dies nicht der Fall, werden die Daten aus dem Projekt nicht in den Auslastungsbericht aufgenommen.\
     Um alle Projekte aus Ihrem System in Ihren Filter einzubeziehen, klicken Sie auf **Alle hinzufügen**. (Diese Option ist nur verfügbar, wenn Ihr System weniger als 250 Projekte umfasst.)

   * **Aufgaben:** Sie den Namen der Aufgabe ein, die die Informationen enthält, die Sie in den Auslastungsbericht aufnehmen möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.\
     Wiederholen Sie diesen Vorgang, um Informationen aus mehreren Aufgaben in den Auslastungsbericht aufzunehmen.\
     Wenn Sie bereits Portfolios, Programme oder Projekte im Filter angegeben haben, muss die angegebene Aufgabe aus einem der Portfolios, Programme oder Projekte stammen, die bereits im Filter enthalten sind. Ist dies nicht der Fall, werden die Daten aus der Aufgabe nicht in den Auslastungsbericht aufgenommen.

   * **Probleme:** Sie den Namen des Problems ein, das die Informationen enthält, die Sie in den Auslastungsbericht aufnehmen möchten, und klicken Sie dann auf den Namen, wenn es in der Dropdown-Liste angezeigt wird.\
     Wiederholen Sie diesen Vorgang, um Informationen aus mehreren Problemen in den Auslastungsbericht aufzunehmen.\
     Wenn Sie bereits Portfolios, Programme oder Projekte im Filter angegeben haben, muss das angegebene Problem aus einem der Portfolios, Programme oder Projekte stammen, die bereits im Filter enthalten sind. Ist dies nicht der Fall, werden die Daten des Problems nicht in den Auslastungsbericht aufgenommen.\
     Kosteninformationen für Probleme sind nicht immer im Auslastungsbericht enthalten. Weitere Informationen dazu, wann Kosteninformationen für Probleme im Auslastungsbericht enthalten sind, finden Sie unter [Verfolgen von Fortschritt, Kosten und Umsatz mit dem Auslastungsbericht](#track-progress-cost-and-revenue-with-the-utilization-report) in diesem Artikel.

   * **Rollen:** Sie den Namen der Rolle ein, die Sie im Auslastungsbericht darstellen möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird. Wiederholen Sie diesen Vorgang, um weitere Rollen einzuschließen.
Der Auslastungsbericht enthält nur Informationen zu den von Ihnen angegebenen Rollen. Eine Aufgabe enthält beispielsweise zehn tatsächliche Stunden. Sechs dieser Stunden stammen aus einer Designer-Rolle und vier aus einer Entwicklerrolle. Wenn Sie den Auslastungsbericht nach Rolle für Designer filtern, werden die vier Stunden aus der Entwicklerrolle aus dem Bericht ausgeschlossen.

   * **Filterregel hinzufügen:** Klicken Sie auf **Filterregel hinzufügen** klicken Sie in das Textfeld und geben Sie den Feldnamen ein, nach dem Sie filtern möchten. Wenn das Feld verfügbar ist, wird es für jedes Objekt ausgefüllt, mit dem es verknüpft werden kann. Klicken Sie auf den Namen des Felds, um es dem Filter hinzuzufügen.

     >[!IMPORTANT]
     >
     >Sie müssen den Feldnamen und nicht die Feldbezeichnung eingeben. Die Feldbezeichnung wird in einem benutzerdefinierten Formular angezeigt, das an ein Objekt angehängt ist. Informationen zum Unterschied zwischen der Bezeichnung und dem Namen eines benutzerdefinierten Felds finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

     Weitere Informationen zu den Feldern, die Sie in den Spalten sehen, finden Sie unter [Glossar der Adobe Workfront-Terminologie](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).\
     Wählen Sie die Filter- und Bedingungsmodifikatoren für den Filter aus. Die verfügbaren Modifikatoren werden unter [Filter- und Bedingungsmodifikatoren](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md) beschrieben.

1. Um einen neuen Filter zu erstellen, klicken Sie auf **Filter speichern**.\
   Oder\
   Um einen vorhandenen Filter zu ändern, klicken Sie auf den Pfeil neben der Schaltfläche **Filter speichern** und anschließend auf **Neuen Filter speichern**.
Geben **im Feld** einen Namen für den Filter ein und klicken Sie auf **Speichern**.
Der Bereich Nutzung wird mit den Informationen gefiltert, die Sie im Filter enthalten haben.

### Anwenden eines gespeicherten Filters {#apply-a-saved-filter}

1. Öffnen Sie den Auslastungsbericht.
Siehe [Verfolgen von Fortschritt, Kosten und Umsatz mit dem Auslastungsbericht](#track-progress-cost-and-revenue-with-the-utilization-report), um dies zu tun.

1. Klicken Sie **Gespeicherte Filter** und wählen Sie dann aus der Dropdown-Liste den Filter aus, den Sie anwenden möchten.

### Duplizieren von Filtern {#duplicate-a-filter}

1. Öffnen Sie den Auslastungsbericht.
Siehe [Verfolgen von Fortschritt, Kosten und Umsatz mit dem Auslastungsbericht](#track-progress-cost-and-revenue-with-the-utilization-report), um dies zu tun.

1. Klicken Sie auf **Gespeicherte Filter** bewegen Sie den Mauszeiger über den Filter, den Sie duplizieren möchten, und klicken Sie auf das Symbol **Duplizieren**.

   ![Symbol „Duplizieren“](assets/utilization-filter-duplicate.png)

   Das Dialogfeld Filter duplizieren wird angezeigt.

1. Geben **im Feld** einen Namen für den neuen Filter ein und klicken Sie auf **Speichern**.

### Umbenennen von Filtern {#rename-a-filter}

Wenn Sie einen Filter umbenennen, sehen alle Workfront-Benutzenden, die Zugriff auf den Auslastungsbericht haben, den von Ihnen eingegebenen neuen Namen.

So benennen Sie einen Filter um:

1. Öffnen Sie den Auslastungsbericht.
Siehe [Verfolgen von Fortschritt, Kosten und Umsatz mit dem Auslastungsbericht](#track-progress-cost-and-revenue-with-the-utilization-report), um dies zu tun.

1. Klicken Sie auf **Gespeicherte Filter** bewegen Sie den Mauszeiger über den Filter, den Sie umbenennen möchten, und klicken Sie auf das Symbol **Umbenennen**.

   ![Filtersymbol umbenennen](assets/utilization-filter-rename.png)

   Das Dialogfeld Filter umbenennen wird angezeigt.

1. Geben **im Feld** einen Namen für den neuen Filter ein und klicken Sie auf **Speichern**.

### Filter löschen {#delete-a-filter}

Wenn Sie einen Filter löschen, wird der Filter für alle Workfront-Benutzenden gelöscht, die Zugriff auf den Auslastungsbericht haben.

So löschen Sie einen Filter:

1. Öffnen Sie den Auslastungsbericht.
Siehe [Verfolgen von Fortschritt, Kosten und Umsatz mit dem Auslastungsbericht](#track-progress-cost-and-revenue-with-the-utilization-report), um dies zu tun.

1. Klicken Sie auf **Gespeicherte Filter** bewegen Sie den Mauszeiger über den Filter, den Sie löschen möchten, und klicken Sie auf das Symbol **Löschen**.

   ![Löschsymbol](assets/utilization-filter-delete.png)

1. Klicken Sie auf **Löschen** wenn Sie gefragt werden, ob Sie den Filter löschen möchten.

## Anpassen des Datumsbereichs, für den Informationen angezeigt werden {#adjust-the-date-range-for-which-information-is-displayed}

Sie können den Datumsbereich anpassen, für den Nutzungsinformationen angezeigt werden. Sie können ein vergangenes oder künftiges Datum auswählen. Von Ihnen vorgenommene Änderungen sind nur für Sie sichtbar.

1. Öffnen Sie den Auslastungsbericht.
Siehe [Verfolgen von Fortschritt, Kosten und Umsatz mit dem Auslastungsbericht](#track-progress-cost-and-revenue-with-the-utilization-report), um dies zu tun.

1. Klicken Sie auf den Datumsbereich neben der Schaltfläche **Exportieren**.

   Die aktuelle Woche ist standardmäßig ausgewählt.

1. Wählen Sie aus den folgenden Optionen:

   * **Woche:** Wählen Sie diese Option, um eine bestimmte Woche (von Sonntag bis Samstag) auszuwählen.
   * **Monat:** Wählen Sie diese Option, um einen bestimmten Monat auszuwählen.

   Der ausgewählte Datumsbereich wird im Auslastungsbericht links neben der Spalte **Gesamt** angezeigt.\
   Workfront speichert, ob eine Wochen- oder Monatsansicht angezeigt werden soll. Wenn Sie das nächste Mal auf den Auslastungsbericht zugreifen, wird je nach ausgewählter Option die aktuelle Woche oder der aktuelle Monat angezeigt.

## Informationen zur Exportauslastung

Sie können Nutzungsinformationen für ein Projekt, ein Programm oder ein Portfolio aus Workfront exportieren. Informationen können nur in den Formaten XLSX, TSV und PDF exportiert werden.

In Microsoft Excel werden negative Zahlen in Klammern angezeigt.

So exportieren Sie Nutzungsinformationen:

1. Öffnen Sie den Auslastungsbericht.
Siehe [Verfolgen von Fortschritt, Kosten und Umsatz mit dem Auslastungsbericht](#track-progress-cost-and-revenue-with-the-utilization-report), um dies zu tun.

1. Klicken **oben links** Bericht auf „Exportieren“.

1. Wählen Sie aus den folgenden Optionen aus:

   * **PDF:** Exportiert den Bericht im PDF-Format. Dies ist das empfohlene Format, wenn Sie den Bericht drucken möchten.\
     Wählen Sie entweder **Brief - Hochformat**, **Brief - Querformat** oder **Andere Größen** (bietet Optionen für den Export in Legal (8,5“ x 14„), Ledger (11“ x 17„) und A4).
Je nach verwendetem Betriebssystem haben Sie möglicherweise die Möglichkeit, die Datei zu öffnen oder zu speichern. Entweder öffnen Sie die Datei mit der zugehörigen Anwendung oder speichern Sie sie auf Ihrem Computer.

   * **Excel:** Exportiert den Bericht im XLSX-Format. Dies ist das empfohlene Format, wenn Sie die Daten in Excel weiter analysieren möchten.
Je nach verwendetem Betriebssystem haben Sie möglicherweise die Möglichkeit, die Datei zu öffnen oder zu speichern. Entweder öffnen Sie die Datei mit der zugehörigen Anwendung oder speichern Sie sie auf Ihrem Computer.

   * **Durch Tabulatoren getrennt:** Exportiert den Bericht im TSV-Format. Dies ist das empfohlene Format, wenn Sie planen, die Daten zur weiteren Analyse in Software von Drittanbietern zu importieren.
Je nach verwendetem Betriebssystem haben Sie möglicherweise die Möglichkeit, die Datei zu öffnen oder zu speichern. Entweder öffnen Sie die Datei mit der zugehörigen Anwendung oder speichern Sie sie auf Ihrem Computer.

1. Lesen Sie die Informationen im Artikel [Exportieren von Daten](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md), um zu verstehen, wie die exportierte Datei verwendet wird.

## Anzeigen von Nutzungsinformationen in einem Diagramm

Sie können die Daten aus dem Auslastungsbericht in einer Diagrammansicht visualisieren.

1. Öffnen Sie den Auslastungsbericht.
Siehe [Verfolgen von Fortschritt, Kosten und Umsatz mit dem Auslastungsbericht](#track-progress-cost-and-revenue-with-the-utilization-report), um dies zu tun.

1. Klicken Sie oben rechts im Auslastungsbericht auf das Symbol **Diagramm**.

   ![Diagrammsymbol](assets/utilization-chart.png)

   Der Auslastungsbericht wird in einer Diagrammansicht angezeigt.

1. (Optional) Konfigurieren Sie das Diagramm so, dass Projekte, Programme oder Portfolios angezeigt werden, indem Sie die entsprechende Option aus dem Dropdown **Menü „Anzeigen** auswählen.
1. (Optional) Bewegen Sie den Mauszeiger über einen bestimmten Zeitpunkt im Bericht, um Daten für diesen Zeitpunkt anzuzeigen.

   ![Bewegen Sie den Mauszeiger über einen Datenpunkt](assets/utilization-chart-hover.png)

1. (Optional) Passen Sie die Filter an, um zu ändern, welche Informationen im Diagramm angezeigt werden. Informationen zum Anpassen der Filter finden Sie unter [Informationen zur Filterauslastung](#filter-utilization-information) in diesem Artikel.
1. (Optional) Konfigurieren Sie den Zeitrahmen des Diagrammberichts, wie in [Anpassen des Datumsbereichs, für den Informationen angezeigt werden](#adjust-the-date-range-for-which-information-is-displayed) in diesem Artikel beschrieben.
