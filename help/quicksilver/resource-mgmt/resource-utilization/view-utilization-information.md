---
product-area: resource-management
navigation-topic: resource-utilization
title: Informationen zur Ressourcenauslastung anzeigen
description: Sie können die Nutzung Ihrer Ressourcen mit dem Bericht "Nutzung"anzeigen.
author: Alina, Lisa
feature: Resource Management
exl-id: 785ee3e9-1b2d-4180-bc78-c41e71c5244d
source-git-commit: d2b62f2ec2f52c54129b342d68c336c782601242
workflow-type: tm+mt
source-wordcount: '7854'
ht-degree: 0%

---

# Informationen zur Ressourcenauslastung anzeigen

{{highlighted-preview}}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this is linked to the UI from the Utilization report. ALWAYS keep this information. DO NOT DELETE!!)</p>
-->

Sie können die Nutzung Ihrer Ressourcen mit dem Bericht &quot;Nutzung&quot;anzeigen.

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

Sie müssen über Folgendes verfügen, um auf den Bericht &quot;Nutzung&quot;zugreifen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Pro oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zeigen Sie den Zugriff auf Folgendes an oder höher:</p> 
    <ul> 
     <li> <p>Ressourcenverwaltung </p> </li> 
     <li> <p>Projekte</p> </li> 
     <li> <p>Portfolios</p> </li> 
     <li> <p>Programme</p> </li> 
     <li> <p>Finanzdaten , wenn Sie Informationen nach Kosten anzeigen möchten</p> </li> 
    </ul> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen des Zugriffs auf Projekte, Portfolios und Programme für den Zugriff auf den Abschnitt "Nutzung"im Bereich "Ressourcen"</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-highloighted-350x145.png" style="width: 350;height: 145;"> </p> <p>Zugriff auf das Projekt verwalten , um auf den Abschnitt "Nutzung"eines Projekts zuzugreifen</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-on-project-highloighted-350x289.png" style="width: 350;height: 289;"> </p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must have View access to the projects you want to view utilization information for as described in this section. If you are still unable to access this information, contact your Workfront administrator. (NOTE:&nbsp;replaced with above table)</p>
-->

In den folgenden Abschnitten wird beschrieben, wie Sie Nutzungsinformationen anzeigen und verwenden.

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

## Übersicht über den Nutzungsbericht {#overview-of-the-utilization-report}

Mithilfe des Nutzungsberichts können Sie den Fortschritt, die Kosten oder den Umsatz eines Projekts, Programms oder Portfolios in einem einzigen Bericht anzeigen. Sie können auch den Umsatz mit den Kosten vergleichen.

Sie können den Nutzungsbericht im Bereich &quot;Ressourcen&quot;anzeigen, um die Nutzung über mehrere Projekte hinweg anzuzeigen, oder Sie können ihn auf der Ebene eines Projekts anzeigen, um die Nutzung der einzelnen Ressourcen (Auftragsrollen und Benutzer) anzuzeigen, die mit diesem Projekt verbunden sind.

Informationen zum Zugriff auf und zur Verwendung des Nutzungsberichts finden Sie im Abschnitt [Verfolgen von Fortschritt, Kosten und Umsatz mit dem Nutzungsbericht](#track-progress-cost-and-revenue-with-the-utilization-report) in diesem Artikel.

* [Tracking von Stunden (Fortschritt)](#track-hours-progress)
* [Kosten verfolgen](#track-cost)
* [Umsatz verfolgen](#track-revenue)
* [Vergleich des Umsatzes mit den geplanten und tatsächlichen Kosten](#compare-revenue-against-planned-and-actual-costs)

### Tracking von Stunden (Fortschritt) {#track-hours-progress}

Sie können den Fortschritt verfolgen, indem Sie sich ansehen, wie die geplanten und geplanten Stunden im Vergleich zu den tatsächlichen Stunden verlaufen.

Beim Verfolgen des Fortschritts eines Projekts, Programms oder Portfolios werden die Fortschritte bei Aufgaben und Problemen in den Nutzungsbericht aufgenommen.

Die folgenden Informationen sind beim Verfolgen von Stunden im Nutzungsbericht verfügbar:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Spaltentitel bei Ansicht von Stunden</strong> </th> 
   <th><strong>Funktion</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Budgetierte Stunden</strong> </td> 
   <td scope="col"> <p>Die insgesamt geplanten Stunden für die enthaltenen Projekte. Sie können die geplanten Gesamtstunden für das Gesamtleben der enthaltenen Projekte anzeigen oder die Gesamtanzahl der geplanten Stunden nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen bestimmten Monat angeben). </p> <p>Budgetierte Stunden werden aus Informationen gefüllt, die im neuen Ressourcenbudgeting-Bereich des Business Case oder im Resource Planer verfügbar sind.<em>.</em></p> <p>Die budgetierten Stunden werden im Nutzungsbericht in einer der folgenden Zeilen angezeigt:</p> 
    <ul> 
     <li> Die geplanten Stunden werden nach der Rolle des Auftrags und dem einzelnen Benutzer im Nutzungsbericht wie folgt zusammengefasst:<br><strong>Individueller Benutzer:</strong> Budgetierte Stunden werden für jeden Benutzer im Nutzungsbericht zusammengefasst. Diese budgetierten Stunden sind mit den Aufgaben und Problemen verknüpft, denen der Benutzer für die enthaltenen Projekte zugewiesen ist. (Sie können die Zeile der entsprechenden Auftragsrolle erweitern, um eine Liste der Benutzer mit dieser Auftragsrolle anzuzeigen.)<br><strong>Auftragsrolle:</strong> Die budgetierten Stunden werden im Nutzungsbericht nach der Rolle des Arbeitsplatzes zusammengefasst.<br>Budgetierte Stunden erscheinen als Ergebnis eines der folgenden Szenarien in einer bestimmten Rolle: 
     <li>Die Rolle "Job"wird als primäre Aufgabenrolle des Benutzers definiert, der der Aufgabe oder dem Problem zugewiesen ist, der die Budgetzeit zugeordnet ist. </li> 
       <li>Wenn Sie Nutzungsinformationen für ein einzelnes Projekt anzeigen, wird die Rolle des Benutzers, dem die Stunden zugewiesen sind, verwendet, unabhängig davon, ob es keine Zuweisung für die Aufgabe oder das Problem gibt, ob einem anderen Benutzer keine Aufgabenrollenzuweisung zugewiesen wurde, ein anderer Benutzer mit einer anderen Rolle für den Auftrag zugewiesen wird oder ein anderes Team zugewiesen wird.</li> 
       <li>Wenn Sie Nutzungsinformationen für mehrere Projekte, Programme oder Portfolios anzeigen, wird die Aufgabenrolle des den Stunden zugewiesenen Benutzers nur verwendet, wenn die Rolle einer Aufgabe oder eines Problems in einem Projekt zugewiesen ist. </li> 
       <li>Die Rolle des Auftrags wird der Aufgabe oder dem Problem zugewiesen, der bzw. dem die budgetierten Stunden zugeordnet sind, und der Benutzer, der der Aufgabe oder dem Problem zugewiesen ist, hat keine Rolle im System.</li> 
      </ul></li> 
    </ul> 
    <ul> 
     <li> <p><strong>Nicht zugewiesene Stunden</strong>: Die budgetierten Stunden werden im Nutzungsbericht im Abschnitt Nicht zugewiesene Stunden angezeigt, wenn eine Aufgabe oder ein Problem mit einer budgetierten Stunde verbunden ist und der Aufgabe oder dem Problem kein Benutzer oder keine Rolle zugewiesen ist.<br>Dieser Abschnitt wird nur angezeigt, wenn Stunden am Projekt vorhanden sind, die dieser Beschreibung entsprechen, und wenn der Bericht "Nutzung"nach oder von einem Projekt angezeigt wird. </p> <p>Dieser Abschnitt wird nur angezeigt, wenn Stunden am Projekt vorhanden sind, die dieser Beschreibung entsprechen, und wenn der Bericht "Nutzung"nach oder von einem Projekt angezeigt wird. </p> </li> 
    </ul> <p>Weitere Informationen zu den geplanten Stunden finden Sie im Abschnitt "Budgetierte Stunden eines Projekts suchen"im <a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Budgetierte Arbeitskosten und budgetierte Stunden für Projekte</a> Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Geplante Stunden</strong> </td> 
   <td scope="col"> <!-- Yay, no errors, warnings, or alerts! -->

<p>
Die geplanten Stunden für die enthaltenen Projekte, die mit den Zuweisungen für jede Aufgabe und jedes Problem verknüpft sind. Sie können die gesamten geplanten Stunden aller Zuweisungen im Projekt für die Gesamtdauer der enthaltenen Projekte anzeigen oder die insgesamt geplanten Stunden nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen bestimmten Monat angeben). 
</p>
<p>
<strong>TIPP </strong>
</p>
<p>
Die geplanten Stunden von Artikeln mit einer Dauer von 0 werden nicht berücksichtigt. 
</p>
<p>
Bei geplanten Stunden im Nutzungsbericht wird berücksichtigt, ob die geplanten Stunden über die Dauer einer Aufgabe oder eines Problems hinweg neu zugewiesen wurden. 
</p>
<p>
Wenn die tägliche Zuweisung von Stunden durch den Benutzer mithilfe des Workload Balancer geändert wurde, können die Daten im Auslastungsbericht betroffen sein, wenn die im Auslastungsbericht ausgewählten Daten nur einen Teil der Dauer einer Aufgabe oder eines Problems enthalten. 
</p>
<p>
Informationen zum Ändern der Zuordnung für Benutzer finden Sie unter <a href="../workload-balancer/manage-user-allocations-workload-balancer.md">Verwalten von Benutzerzuordnungen im Lastenausgleich</a>.


</p>
<p>
Geplante Stunden werden im Nutzungsbericht in einer der folgenden Zeilen angezeigt:
</p>
<ul>

<li>Geplante Stunden werden im Nutzungsbericht nach Auftragsrolle und nach individuellem Benutzer wie folgt zusammengefasst: 
<ul>

<li><strong>Individueller Benutzer</strong>: Die geplanten Stunden werden für jeden Benutzer im Nutzungsbericht zusammengefasst. Diese geplanten Stunden sind mit den Aufgaben und Problemen verknüpft, denen der Benutzer für die enthaltenen Projekte zugewiesen ist. (Sie können die Zeile der entsprechenden Auftragsrolle erweitern, um eine Liste der Benutzer mit dieser Auftragsrolle anzuzeigen.)

<li><strong>Auftragsrolle</strong>: Geplante Stunden werden im Nutzungsbericht eines einzelnen Projekts nach der Rolle des Auftrags zusammengefasst.<br>Geplante Stunden erscheinen als Ergebnis eines der folgenden Szenarien in einer bestimmten Rolle:  
<ul>

<li>Die Auftragsrolle ist definiert als die Rolle des Hauptauftrags des Benutzers, der der Aufgabe oder dem Problem zugewiesen ist, mit der bzw. dem die geplanten Stunden verknüpft sind.

<li>Wenn Sie Nutzungsinformationen für ein einzelnes Projekt anzeigen, werden die Stunden, die mit einer Auftragsrolle verknüpft sind, in den folgenden Szenarien nicht für die Auftragsrolle angezeigt:   
<ul>

<li>Es gibt keine Zuweisung zu der Aufgabe oder dem Problem

<li>Ein Benutzer ohne Aufgabenrollenzuweisung wurde zugewiesen.

<li>Dem Benutzer wird eine andere Aufgabenrolle zugewiesen.

<li>Ein Team wird der Aufgabe oder dem Problem zugewiesen
</li>   
</ul>

<li>Wenn Sie Nutzungsinformationen für mehrere Projekte, Programme oder Portfolios anzeigen, wird die Aufgabenrolle des den Stunden zugewiesenen Benutzers nur verwendet, wenn die Rolle einer Aufgabe oder eines Problems in einem Projekt zugewiesen ist. Die Auftragsrollenstunden werden nicht separat angezeigt, wenn der Bericht "Nutzung"für mehrere Projekte angezeigt wird.

<li>Die Rolle "Auftrag"wird der Aufgabe oder dem Problem zugewiesen, der bzw. dem geplante Stunden zugeordnet sind, und der der Aufgabe oder dem Problem zugewiesene Benutzer hat keine Rolle im System.
</li>  
</ul>

<li><strong>Nicht zugewiesene Stunden</strong>: Geplante Stunden werden im Nutzungsbericht im Abschnitt Nicht zugewiesene Stunden angezeigt, wenn geplante Stunden mit einer Aufgabe oder einem Problem verknüpft sind und der Aufgabe oder dem Problem kein Benutzer oder keine Rolle zugewiesen ist. Dieser Abschnitt wird nur angezeigt, wenn Stunden am Projekt vorhanden sind, die dieser Beschreibung entsprechen, und wenn der Bericht "Nutzung"für ein einzelnes Projekt angezeigt wird. <br>Weitere Informationen zu geplanten Stunden finden Sie unter <a href="../../manage-work/tasks/task-information/planned-hours.md">Übersicht über geplante Stunden</a>.
</li> 
</ul>
</li> 
</ul> </td> 
  </tr> 
  <tr> 
   <td><strong>Tatsächliche Stunden</strong> </td> 
   <td> <p> Gesamtstunden der Aufgaben, Probleme, <span>und zum Projekt</span> für die enthaltenen Projekte. Sie können die tatsächlichen Gesamtstunden für die Gesamtdauer der enthaltenen Projekte anzeigen oder die tatsächlichen Gesamtstunden nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen einzelnen Monat angeben). </p> <p>Warnung: Der Nutzungsbericht enthält die am Projekt protokollierten Stunden, untergeordnete Aufgaben, Probleme und übergeordnete Aufgaben mit mindestens einer Zuweisung. Sie enthält keine Stunden, die mit übergeordneten Aufgaben ohne Zuweisungen protokolliert wurden. Es wird empfohlen, keine übergeordneten Aufgaben als Arbeitsaufgaben zu verwenden und Ihren Ressourcen nur untergeordnete Aufgaben zuzuweisen. </p> <p>Die tatsächlichen Stunden werden im Nutzungsbericht in einer der folgenden Zeilen angezeigt:</p> 
    <ul> 
     <li> Die tatsächlichen Stunden werden im Nutzungsbericht eines Projekts nach der Rolle des Auftrags und dem einzelnen Benutzer wie folgt zusammengefasst:<br><strong>Individueller Benutzer:</strong> Die tatsächlichen Stunden werden im Nutzungsbericht in der Zeile des Benutzers angezeigt, der die Stunden protokolliert hat. (Sie können die Zeile der entsprechenden Auftragsrolle erweitern, um eine Liste der Benutzer mit dieser Auftragsrolle anzuzeigen, die Stunden protokolliert haben.)<br><strong>Auftragsrolle:</strong> Die tatsächlichen Stunden, die von Benutzern protokolliert werden, die mit diesen Rollen verknüpft sind, werden im Nutzungsbericht in der Zeile der entsprechenden Vorgangsrolle zusammengefasst.<br>Die tatsächlichen Stunden werden in einer bestimmten Rolle als Ergebnis eines der folgenden Szenarien angezeigt: 
      <ul> 
       <li>Die Auftragsrolle wird als primäre Aufgabenrolle des Benutzers definiert, der die Stunden protokolliert hat.</li> 
       <li>Es gibt keine Zuweisung zu der Aufgabe oder dem Problem</li> 
       <li>Ein anderer Benutzer wurde ohne Aufgabenrollenzuweisung zugewiesen</li> 
       <li>Einem anderen Benutzer wird eine andere Aufgabenrolle zugewiesen.</li> 
       <li> <p>Ein Team wird zugewiesen.</p> </li> 
      </ul></li>  
     <p>Wenn dem Benutzer, der die Stunden protokolliert, keine Arbeitsrolle mit seinem Profil zugeordnet ist, ist die für den Auslastungsbericht verwendete Vorgangsrolle die der Aufgabe oder dem Problem zugewiesene Auftragsrolle, in der Stunden protokolliert werden, oder die mit dem Primären Eigentümer der Aufgabe oder des Problems verknüpfte Auftragsrolle. </p> 
     <li><strong>Sonstige Stunden:</strong> Die tatsächlichen Stunden werden im Nutzungsbericht im Abschnitt Andere Stunden in der Zeile des Benutzers angezeigt, der sich in den Stunden angemeldet hat.<br>Stunden werden in diesem Abschnitt angezeigt, wenn der Benutzer, der die Stunden protokolliert hat, keine Rolle im System definiert hat.<br>Dieser Abschnitt wird nur angezeigt, wenn Stunden am Projekt dieser Beschreibung entsprechen. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>Budgetierte Varianz (für Stunden)</strong> </td> 
   <td> <p>Die insgesamt veranschlagten Stunden abzüglich der tatsächlichen Gesamtstunden für die einbezogenen Projekte. Sie können die gesamte budgetierte Varianz für die gesamte Lebensdauer der eingeschlossenen Projekte anzeigen oder die gesamte budgetierte Varianz nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen bestimmten Monat angeben). </p> <p>Wenn der Wert positiv ist, wird er grün angezeigt. Dies zeigt an, dass die geplanten Gesamtstunden die tatsächlichen Stunden überschreiten.</p> <p>Wenn der Wert negativ ist, wird er rot angezeigt. Dies zeigt an, dass die geplanten Gesamtstunden kleiner als die tatsächlichen Stunden sind.</p> <p> <img src="assets/utilization-variance-budgeted-350x96.png" style="width: 350;height: 96;"> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Geplante Variante (für Stunden)</strong> </td> 
   <td> <p>Die insgesamt geplanten Stunden abzüglich der tatsächlichen Gesamtstunden für die enthaltenen Projekte. Sie können die insgesamt geplante Varianz für die gesamte Lebensdauer der enthaltenen Projekte anzeigen oder die insgesamt geplante Varianz nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen bestimmten Monat angeben).</p> <p>Wenn der Wert positiv ist, wird er grün angezeigt. Dies zeigt an, dass die geplanten Gesamtstunden die tatsächlichen Stunden überschreiten.</p> <p>Wenn der Wert negativ ist, wird er rot angezeigt. Dies zeigt an, dass die geplanten Gesamtstunden weniger als die tatsächlichen Stunden betragen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Kosten verfolgen {#track-cost}

Sie können Kosten nachverfolgen, indem Sie sich ansehen, wie die budgetierten Kosten und geplanten Kosten mit den tatsächlichen Kosten verglichen werden.

Bei der Verfolgung der Kosten eines Projekts, Programms oder Portfolios stammen die Informationen im Nutzungsbericht aus Aufgaben. Kosteninformationen aus Aufgaben sind immer im Nutzungsbericht verfügbar. Die Kosten für Aufgaben werden basierend auf dem Kostentyp der Aufgabe berechnet. Informationen zum Kostentyp von Aufgaben finden Sie unter &quot;Ändern der Kostentypen für einzelne Aufgaben&quot;in [Kosten verfolgen](../../manage-work/projects/project-finances/track-costs.md).

Sie können Kosteninformationen im Bericht &quot;Nutzung&quot;wie folgt anzeigen:

* Für eine bestimmte Woche oder einen bestimmten Monat oder für das gesamte Projekt, Programm oder Portfolio.
* Nach Rolle oder Einzelperson für Projekte.

Die im Nutzungsbericht verwendete Währung wird durch die im Projekt festgelegte Währung bestimmt. Informationen zum Anpassen der Währung für ein Projekt finden Sie unter [Ändern der Projektwährung](../../manage-work/projects/project-finances/change-project-currency.md).

Die folgenden Informationen sind im Nutzungsbericht verfügbar, wenn Kosten verfolgt werden:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Spaltentitel bei Ansicht der Kosten</strong> </th> 
   <th> <p><strong>Funktion</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Budgetierte Kosten</strong> </td> 
   <td scope="col"> <p>Die budgetierten Kosten für die enthaltenen Projekte. Sie können die Gesamtkosten der Budgetierung für die Gesamtdauer der eingeschlossenen Projekte anzeigen oder die Gesamtkosten der Budgetierung nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen einzelnen Monat angeben).</p> <p>Da sich die im Nutzungsbericht veranschlagten Kosten auf Kosten nach Rolle konzentrieren, entspricht die Berechnung den budgetierten Arbeitskosten in anderen Bereichen von Workfront. Informationen zur Berechnung der budgetierten Arbeitskosten finden Sie unter <a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Budgetierte Arbeitskosten und budgetierte Stunden für Projekte</a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Geplante Kosten</strong> </td> 
   <td scope="col"> <p>Gesamtsumme der geplanten Kosten für die enthaltenen Projekte. Sie können die Gesamtsumme der geplanten Kosten für die gesamte Lebensdauer der enthaltenen Projekte anzeigen oder die Gesamtsumme der geplanten Kosten nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen einzelnen Monat angeben).</p> <p><span class="preview">Beachten Sie, dass die geplanten Kosten für die Wochen-, Monats- und vierteljährlichen Ansichten als Durchschnitt des ausgewählten Zeitraums berechnet werden, in dem die Kostensätze für Stellenberufe oder Benutzer datumswirksam sind.</span></p><p>Weitere Informationen zur Berechnung der geplanten Kosten für das Projekt finden Sie im Abschnitt "Wie Workfront geplante, geplante und tatsächliche Kosten berechnet"im Artikel <a href="../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten verfolgen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Istkosten</strong> </td> 
   <td scope="col"> <p>Die tatsächlichen Gesamtkosten der enthaltenen Projekte. Sie können die tatsächlichen Gesamtkosten für die Gesamtdauer der eingeschlossenen Projekte anzeigen oder die tatsächlichen Gesamtkosten nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen einzelnen Monat angeben).</p> <p>Weitere Informationen zur Berechnung der tatsächlichen Kosten für das Projekt finden Sie im Abschnitt "Wie Workfront geplante, geplante und tatsächliche Kosten berechnet"im Artikel <a href="../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten verfolgen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>budgetierte Abweichung (für Kosten)</strong> </td> 
   <td scope="col"> <p>Die gesamten veranschlagten Kosten abzüglich der tatsächlichen Gesamtkosten für die enthaltenen Projekte. Sie können die gesamte budgetierte Varianz für die gesamte Lebensdauer der eingeschlossenen Projekte anzeigen oder die gesamte budgetierte Varianz nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen bestimmten Monat angeben).</p> <p>Wenn der Wert positiv ist, wird er grün angezeigt. Dies deutet darauf hin, dass die gesamten budgetierten Kosten größer sind als die tatsächlichen Kosten.</p> <p>Wenn der Wert negativ ist, wird er rot angezeigt. Dies zeigt an, dass die Gesamtkosten unter den tatsächlichen Kosten liegen.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Geplante Varianz (für Kosten)</strong> </td> 
   <td> <p>Die gesamten geplanten Kosten abzüglich der tatsächlichen Gesamtkosten für die enthaltenen Projekte. Sie können die insgesamt geplante Varianz für die gesamte Lebensdauer der enthaltenen Projekte anzeigen oder die insgesamt geplante Varianz nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen bestimmten Monat angeben). </p> <p>Wenn der Wert positiv ist, wird er grün angezeigt. Dies deutet darauf hin, dass die gesamten geplanten Kosten größer als die tatsächlichen Kosten sind.</p> <p>Wenn der Wert negativ ist, wird er rot angezeigt. Dies zeigt an, dass die Gesamtkosten der geplanten Kosten unter den tatsächlichen Kosten liegen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Umsatz verfolgen {#track-revenue}

Sie können den Umsatz verfolgen, indem Sie anzeigen, wie der geplante und der geplante Umsatz mit dem tatsächlichen Umsatz verglichen werden.

Beim Verfolgen des Umsatzes eines Projekts, Programms oder Portfolios werden nur Umsätze aus Aufgaben im Bericht Verwendung erfasst.

Die Informationen in der folgenden Tabelle sind beim Verfolgen des Umsatzes im Nutzungsbericht verfügbar.

Informationen zu den spezifischen Feldern und deren Berechnung durch Workfront finden Sie in den folgenden Artikeln:

* [Kosten verfolgen](../../manage-work/projects/project-finances/track-costs.md)
* [Übersicht über Rechnungsstellung und Umsatz](../../manage-work/projects/project-finances/billing-and-revenue-overview.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Spaltentitel bei Ansicht des Umsatzes</strong> </th> 
   <th> <strong>Funktion</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Budgetierte Einnahmen</strong> </td> 
   <td scope="col"> <p>Die Gesamtbudgetierten Stunden multipliziert mit dem Role Billing Rate für die einbezogenen Projekte. Sie können den Gesamtumsatz im Budget für die gesamte Lebensdauer der enthaltenen Projekte anzeigen oder den Gesamtumsatz nur für den angegebenen Datumsbereich anzeigen (Sie können eine bestimmte Woche oder einen bestimmten Monat angeben).</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Geplante Einnahmen</strong> </td> 
   <td scope="col"> <p>Der geplante Umsatz im Bericht "Nutzung"ist der Umsatz, der mit den geplanten Stunden verbunden ist und den Ressourcen zugeordnet ist, die den Aufgaben des Projekts zugewiesen sind.</p> <p>Workfront berechnet den geplanten Umsatz des Projekts für den Bericht "Nutzung"anhand der folgenden Formel:</p> <p><code>Project Planned Revenue = SUM&nbsp;(All Tasks Planned Revenue)</code> </p> 
   <p><b>NOTIZ</b>
   <p>Der geplante Umsatz des Projekts, der im Nutzungsbericht angezeigt wird, unterscheidet sich von dem geplanten Umsatz, der im Bereich "Projektdetails"und in den Projektberichten angezeigt wird. </p> <p>Der geplante Umsatz im Bereich "Projektdetails"spiegelt den Umsatz der Aufgabe sowie den festen Umsatz des Projekts wider. Der geplante Umsatz im Nutzungsbericht zeigt den geplanten Umsatz an, der nur mit den Aufgaben im Projekt verbunden ist. </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p>Wenn das Projekt eine Aufgabe mit 10 Stunden umfasst, die einem Berater mit einer Stundenrate von 20 US-Dollar zugewiesen ist und das Projekt einen festen Umsatz von 100 US-Dollar aufweist, zeigt der Nutzungsbericht 200 US-Dollar für den geplanten Umsatz an (den geplanten Umsatz, der mit den Stunden der Aufgabe verknüpft ist). Im Abschnitt Projektdetails werden 300 USD (der geplante Umsatz aus der Aufgabe und der feste Umsatz für das Projekt) angezeigt. </p> 
     </div> <p>Weitere Informationen über die Aufgabe und das Projekt "Geplanter Umsatz"außerhalb des Nutzungsberichts finden Sie unter <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Übersicht über Rechnungsstellung und Umsatz</a>.</p> </p> <p>Die Art und Weise, wie der Nutzungsbericht den geplanten Umsatz für die enthaltenen Projekte berechnet und anzeigt, berücksichtigt den für die Aufgabe festgelegten Umsatztyp. </p> <p>Je nach dem Umsatztyp jeder Aufgabe im Projekt gibt es die folgenden Szenarien: </p> <p><strong>Fester Umsatz:</strong> Unabhängig von der Aufgabenzuweisung wird der Umsatz der Aufgabe immer mit dem Festbetrag berechnet, der in der Aufgabe angegeben ist.</p> <p><b>WICHTIG</b>

Im Gegensatz zu anderen Bereichen von Workfront berechnet der Nutzungsbericht den geplanten Umsatz für feste Umsätze, indem er den festen Umsatz gleichmäßig durch die Anzahl der geplanten Stunden für die Aufgabe teilt. </p> <p>Beispielsweise hat eine Aufgabe einen Umsatz von 200 USD. Wenn die Aufgabe vier geplante Stunden umfasst, beträgt jede Stunde 50 USD. Dies wird auf Benutzer- und Rollenebene verteilt. Diese Verteilung ist für den Bericht &quot;Nutzung&quot;eindeutig.</p> <p><b>NOTIZ</b>

Wenn Sie eine Aufgabe mit festem Umsatz haben und für die Aufgabe keine geplanten Stunden vorgesehen sind, wird der Umsatz nicht im Nutzungsbericht angezeigt, da es keine Möglichkeit gibt, ihn auf die Stunden zu verteilen. Wenn Sie für Aufgaben mit festem Umsatz und ohne Zuweisung geplante Stunden geplant haben, wird der Umsatz als nicht zugewiesener Umsatz angezeigt. </p> <p><strong>Stündliche Rolle:</strong> Der Umsatz aus der Aufgabe wird anhand des für eine bestimmte Rolle festgelegten Abrechnungskurses multipliziert mit der Anzahl der mit dieser Rolle verbundenen geplanten Stunden berechnet. Workfront verwendet die folgende Formel:</p> <p><code>Rolle &quot;Stündlicher geplanter Umsatz&quot;= SUM(geplante Stunden von der Rolle für alle Aufgaben) * Rollenabrechnungsrate</code></p><p><span class="preview"><b>HINWEIS:</b> Der Abrechnungsstundensatz in der Formel berücksichtigt alle Datumsänderungen des Satzes.</span></p>   <p><strong>Benutzer stündlich:</strong> Der Umsatz aus der Aufgabe wird anhand des für einen bestimmten Benutzer festgelegten Abrechnungskurses multipliziert mit der Anzahl der diesem Benutzer zugeordneten geplanten Stunden berechnet. Workfront verwendet die folgende Formel:</p> <p><code>User Stündlich geplanter Umsatz = SUM(geplante Stunden von Benutzern für alle Aufgaben) * Abrechnungsrate für Benutzer</code> </p> <p><span class="preview"><b>HINWEIS:</b> Der Abrechnungsstundensatz in der Formel berücksichtigt alle Datumsänderungen des Satzes.</span></p> <p><b>Stündliche Rolle oder stündlicher Benutzer Plus fest</b> </p> <p><b>WICHTIG</b>

Im Gegensatz zu anderen Bereichen von Workfront berechnet der Nutzungsbericht den geplanten Umsatz, indem er den festen Umsatz gleichmäßig durch die Anzahl der geplanten Stunden für die Aufgabe teilt. </p> <p>Die folgenden Fälle sind vorhanden: </p>
<ul>
<li> <p><strong>Rolle Stündlich Plus fest:</strong> Der Umsatz aus der Aufgabe wird anhand des für eine bestimmte Rolle festgelegten Abrechnungskurses multipliziert mit der Anzahl der geplanten Stunden, die mit der Rolle verbunden sind, berechnet. Darüber hinaus wird der Rollenrate ein fester Betrag hinzugefügt, der für die Aufgabe angegeben ist. Workfront verwendet die folgende Formel:</p> <p><code>Rolle Stündlich plus geplanter Umsatz = [SUM(Geplante Stunden von der Rolle für alle Aufgaben) * Rollenabrechnungsrate] + SUM(Cap or Fixed Amount of the task / Scheduled Hours of the task)</code> </p> </li>
</ul>
<ul>
<li> <p><strong>Benutzerstündlich plus fest:</strong> Die für einen bestimmten Benutzer festgelegte Abrechnungsrate multipliziert mit der Anzahl der geplanten Stunden für die Aufgabe von diesem Benutzer. Darüber hinaus wird der Benutzerrate ein fester Betrag hinzugefügt, der für die Aufgabe angegeben ist. Workfront verwendet die folgende Formel:</p> <p><code>Benutzer Stündlich plus geplanter Umsatz = [SUM(Geplante Stunden für Benutzer aller Aufgaben) * Benutzerabrechnungsrate] + SUM(Cap or Fixed Amount of the task / Scheduled Hours of the task)</code> </p> </li>
</ul> <p><b>Rolle oder Benutzer stündlich mit Cap</b> </p> <p><b>WICHTIG</b>

Im Gegensatz zu anderen Bereichen in Workfront gilt der Betrag über der Obergrenze, wenn der geplante Umsatz die Obergrenze überschreitet, als fester Umsatz. Der geplante Umsatz wird berechnet, indem der feste Umsatz gleichmäßig durch die Anzahl der geplanten Stunden für die Aufgabe dividiert und dann der Höchstbetrag und die Rolle oder der stündliche Umsatz des Benutzers hinzugefügt werden. <br></p> <p>Die folgenden Fälle sind vorhanden: </p>
<ul>
<li> <p><strong>Stündliche Rolle mit Cap:</strong> Aufgaben werden stündlich in Rechnung gestellt, wie in Rolle Stündlich , sie haben jedoch einen maximalen Maximalbetrag, den Sie angeben können. Workfront verwendet die folgende Formel:</p> <p><code>Stündliche Rolle mit geplantem Gesamtumsatz = [SUM(Scheduled Hours from role für alle Aufgaben und Probleme) * Rollenabrechnungsrate] + Sockel Betrag der Aufgabe + SUM(Betrag über den Sockel/Geplante Stunden der Aufgabe)</code> </p> </li>
</ul>
<ul>
<li> <p><strong>Benutzerstündlich mit Begrenzung:</strong> Aufgaben werden stündlich in Rechnung gestellt, wie in Benutzer stündlich, sie haben jedoch eine maximale Obergrenze, die Sie angeben können. Workfront verwendet die folgende Formel: </p> <p><code>Benutzer Stündlich mit geplantem Gesamtumsatz = [SUM(Geplante Stunden für Benutzer aller Aufgaben) * Benutzerabrechnungsrate] + Sockel Betrag der Aufgabe + SUM(Betrag über den Sockel/Geplante Stunden der Aufgabe)</code> </p> </li>
</ul> <p>Weitere Informationen darüber, welche Rolle oder welcher Benutzer bei der Berechnung des geplanten Umsatzes berücksichtigt wird, finden Sie unter <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Übersicht über Rechnungsstellung und Umsatz</a>.</p> </td>
</tr> 
  <tr> 
   <td><strong>Tatsächliche Einnahmen</strong> </td> 
   <td> <p>Der tatsächliche Umsatz ist der Umsatz, der mit den tatsächlichen Stunden der Aufgaben verbunden ist. <span>und des Projekts</span>. Weitere Informationen zum tatsächlichen Umsatz finden Sie im Artikel im Abschnitt "Verfolgen von Umsatzsummen" <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Übersicht über Rechnungsstellung und Umsatz</a>.</p>

<p>Die Berechnung des tatsächlichen Umsatzes für die enthaltenen Projekte durch den Nutzungsbericht hängt vom für die Aufgabe festgelegten Umsatztyp ab, wie folgt:</p> <p><strong>Fester Umsatz:</strong> Unabhängig von der Aufgabenzuweisung wird der Umsatz der Aufgabe immer mit dem Festbetrag berechnet, der in der Aufgabe angegeben ist.</p> <p><b>WICHTIG</b>

Im Gegensatz zu anderen Bereichen von Workfront berechnet der Nutzungsbericht den tatsächlichen Umsatz, indem er den festen Umsatz gleichmäßig durch die Anzahl der Stunden teilt, die bei der Aufgabe protokolliert wurden. </p> <p> </p> <p>Beispielsweise hat eine Aufgabe einen tatsächlichen Umsatz von 200 USD. Wenn die Aufgabe 4 Stunden umfasst, beträgt die Stunde 50 USD. Dies wird auf Benutzer- und Rollenebene verteilt. Diese Verteilung ist für den Bericht &quot;Nutzung&quot;eindeutig.</p> <p><b>NOTIZ</b>

Wenn Sie eine Aufgabe mit festem Umsatz haben und keine tatsächlichen Stunden für die Aufgabe vorhanden sind, wird der tatsächliche Umsatz nicht im Nutzungsbericht angezeigt, da keine Möglichkeit zur Verteilung der Stunden besteht. </p> <p><strong>Stündliche Rolle:</strong> Der Umsatz aus der Aufgabe wird anhand des für eine bestimmte Rolle festgelegten Abrechnungskurses multipliziert mit der Anzahl der tatsächlichen Stunden berechnet.</p> <p>Workfront verwendet die folgende Formel:</p> <p><code>Rolle &quot;Tatsächlicher Umsatz pro Stunde&quot;= SUM(tatsächliche Stunden von der Rolle für alle Aufgaben) * Rolle &quot;Abrechnungsrate&quot;</code> </p> <p><span class="preview"><b>HINWEIS:</b> Der Abrechnungsstundensatz in der Formel berücksichtigt alle Datumsänderungen des Satzes.</span></p> <p><strong>Benutzer stündlich:</strong> Der Umsatz aus der Aufgabe wird anhand des für einen bestimmten Benutzer festgelegten Abrechnungskurses multipliziert mit der Anzahl der Stunden berechnet, die dieser Benutzer mit der Aufgabe protokolliert hat. Workfront verwendet die folgende Formel:</p> <p><code>Benutzerstündlicher tatsächlicher Umsatz = SUM(tatsächliche Stunden vom Benutzer für alle Aufgaben) * Benutzerabrechnungsrate</code></p> <p><span class="preview"><b>HINWEIS:</b> Der Abrechnungsstundensatz in der Formel berücksichtigt alle Datumsänderungen des Satzes.</span></p> <p><b>Rolle oder Benutzer stündlich Plus fest</b> </p> <p><b>WICHTIG</b>

Im Gegensatz zu anderen Bereichen von Workfront berechnet der Nutzungsbericht den tatsächlichen Umsatz, indem er den festen Umsatz gleichmäßig durch die Anzahl der Stunden teilt, die bei der Aufgabe protokolliert wurden. </p> <p>Die folgenden Fälle sind vorhanden: </p>
<ul>
<li> <p><strong>Rolle Stündlich Plus fest:</strong> Die Abrechnungsrate, die für eine bestimmte Rolle festgelegt wurde, multipliziert mit der Anzahl der Stunden, die von einem Benutzer mit dieser Rolle gegen die Aufgabe protokolliert wurden. Darüber hinaus wird der Rollenrate ein fester Betrag hinzugefügt, der für die Aufgabe angegeben ist. </p> <p>Workfront verwendet die folgende Formel:</p> <p><code>Rolle Stündlich plus Fester tatsächlicher Umsatz = [SUM(Tatsächliche Stunden von der Rolle für alle Aufgaben) * Rollenabrechnungsrate] + SUM(Cap or Fixed Amount of the task / Actual Hours of the task)</code> </p> </li>
</ul>
<ul>
<li> <p><strong>Benutzerstündlich plus fest:</strong> Die für einen bestimmten Benutzer festgelegte Abrechnungsrate multipliziert mit der Anzahl der Stunden, die mit der Aufgabe von diesem Benutzer verglichen wurden. Darüber hinaus wird der Benutzerrate ein fester Betrag hinzugefügt, der für die Aufgabe angegeben ist. </p> <p>Workfront verwendet die folgende Formel:</p> <p><code>Benutzerstündlich plus Fester tatsächlicher Umsatz = [SUM(Tatsächliche Stunden von der Rolle für alle Aufgaben) * Benutzerabrechnungsrate] + SUM(Cap or Fixed Amount of the task / User Hours of the task)</code> </p> </li>
</ul> <p><b>Rolle oder Benutzer stündlich mit Cap</b> </p> <p><b>WICHTIG</b>

Im Gegensatz zu anderen Bereichen in Workfront gilt der Betrag über der Obergrenze, wenn der geplante Umsatz die Obergrenze überschreitet, als fester Umsatz. Der geplante Umsatz wird berechnet, indem der feste Umsatz gleichmäßig durch die Anzahl der geplanten Stunden für die Aufgabe dividiert und dann der Höchstbetrag und die Rolle oder der stündliche Umsatz des Benutzers hinzugefügt werden. <br></p> <p>Die folgenden Szenarien existieren:</p>
<ul>
<li> <p><strong>Stündliche Rolle mit Cap:</strong> Aufgaben werden stündlich in Rechnung gestellt, wie in Rolle Stündlich , sie haben jedoch einen maximalen Maximalbetrag, den Sie angeben können. Workfront verwendet die folgende Formel:</p> <p><code>Stündliche Rolle mit tatsächlichem Umsatz = oberste Ebene [SUM(Tatsächliche Stunden von der Rolle für alle Aufgaben und Probleme) * Rollenabrechnungsrate] + Sockel Betrag der Aufgabe + SUM(Betrag über den Sockel/tatsächliche Stunden der Aufgabe)</code></p> </li>
</ul>
<ul>
<li> <p><strong>Benutzerstündlich mit Begrenzung:</strong> Aufgaben werden stündlich in Rechnung gestellt, wie in Benutzer stündlich, sie haben jedoch eine maximale Obergrenze, die Sie angeben können.</p> <p> Workfront verwendet die folgende Formel:</p> <p><code>Benutzer stündlich mit aktuellem Umsatz beschränken = [SUM(Tatsächliche Stunden von der Rolle für alle Aufgaben und Probleme) * Benutzerabrechnungsrate] + Sockel Betrag der Aufgabe + SUM(Betrag über den Sockel/tatsächliche Stunden der Aufgabe)</code> </p> </li>
</ul>
<div>
<p><strong>Projektumsatz</strong>: Der Umsatz, der mit den im Projekt angemeldeten Stunden verbunden ist, wird unter Berücksichtigung der Abrechnung pro Stunde der Betrag der primären Auftragsrolle des Benutzers berechnet, der die Zeit protokolliert. Wir empfehlen keine Protokollierungszeit für das Projekt. </p>
<p><b>NOTIZ</b>

Wenn der Benutzer nicht mit einer Stellenrolle verknüpft ist oder die Abrechnung pro Stunde der Primären Rolle null ist, berechnet Workfront den tatsächlichen Umsatz anhand des Betrags Abrechnung pro Stunde für den Benutzer. Wenn der Benutzer keinen Betrag pro Stunde in seinem Profil hat, ist der tatsächliche Umsatz null. </p>
</div> </td>
</tr> 
  <tr> 
   <td><strong>budgetierte Abweichung (für Umsatz)</strong> </td> 
   <td> <p>Die tatsächlichen Gesamteinnahmen abzüglich der ausgewiesenen Einnahmen aus den einbezogenen Projekten.<br>Sie können die gesamte budgetierte Varianz für die gesamte Lebensdauer der eingeschlossenen Projekte anzeigen oder die gesamte budgetierte Varianz nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen bestimmten Monat angeben).</p> <p>Wenn der Wert positiv ist, wird er grün angezeigt. Dies zeigt an, dass der Gesamtumsatz größer ist als der tatsächliche Umsatz.</p> <p>Wenn der Wert negativ ist, wird er rot angezeigt. Dies zeigt an, dass der Gesamtumsatz geringer ist als der tatsächliche Umsatz.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Geplante Varianz (für Umsatz)</strong> </td> 
   <td> <p>Der tatsächliche Gesamtumsatz abzüglich des gesamten geplanten Umsatzes für die einbezogenen Projekte.<br>Sie können die insgesamt geplante Varianz für die gesamte Lebensdauer der enthaltenen Projekte anzeigen oder die insgesamt geplante Varianz nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen bestimmten Monat angeben). </p> <p>Wenn der Wert positiv ist, wird er grün angezeigt. Dies zeigt an, dass der geplante Gesamtumsatz größer ist als der tatsächliche Umsatz.</p> <p>Wenn der Wert negativ ist, wird er rot angezeigt. Dies zeigt an, dass der geplante Gesamtumsatz kleiner als der tatsächliche Umsatz ist.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--Note from the table about Actual revenue: 
     <p>Actual Revenue is displayed in the Utilization report only after the task is marked as Complete or Done (or a status that equates with Complete).</p>
    -->

<!--More notes from the table: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;the note below is duplicated in this article: /Content/Manage work/Projects/Project Finances/billing-and-revenue-overview.html and in the glossary)</p>
   -->

### Vergleich des Umsatzes mit den geplanten und tatsächlichen Kosten {#compare-revenue-against-planned-and-actual-costs}

Sie können die geplanten oder tatsächlichen Kosten neben dem geplanten Umsatz anzeigen. Die Marge (%) wird ebenfalls angezeigt (die Marge wird als Umsatz - Kosten/Umsatz berechnet).

Die folgenden Informationen sind im Nutzungsbericht beim Vergleich von Umsatz mit geplanten und tatsächlichen Kosten verfügbar:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Spaltentitel bei Anzeige von Umsatz vs. Kosten (geplant)</strong> </th> 
   <th> <strong>Funktion</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Geplante Kosten</strong> </td> 
   <td scope="col"> Gesamtsumme der geplanten Kosten für die enthaltenen Projekte. Sie können die Gesamtsumme der geplanten Kosten für die gesamte Lebensdauer der enthaltenen Projekte anzeigen oder die Gesamtsumme der geplanten Kosten nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen einzelnen Monat angeben). </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Geplante Einnahmen</strong> </td> 
   <td scope="col"> <p>Der geplante Umsatz ist der Umsatz, der mit den geplanten Stunden der Aufgaben verbunden ist. </p> <p>Die Berechnung und Anzeige des geplanten Umsatzes für die enthaltenen Projekte durch den Nutzungsbericht hängt vom für die Aufgabe festgelegten Umsatztyp ab, wie im Abschnitt <a href="#track-revenue" class="MCXref xref">Umsatz verfolgen</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Rand</strong> </td> 
   <td scope="col"> <p>Der Prozentsatz der Spanne wird wie folgt berechnet:</p> <p><code>Planned Revenue - Planned Cost / Planned Revenue * 100. </code></p> <p><b>NOTIZ</b>

Wenn der geplante Umsatz gleich 0 ist, wird der Rand als 0 angezeigt. </p> </td>
</tr> 
  <tr> 
   <td scope="col"> <p scope="col"><strong>Spaltentitel bei Ansicht von Umsatz vs. Kosten (tatsächlich)</strong> </p>  </td> 
   <td scope="col"><p><strong>Funktion</strong></p></td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Istkosten</strong> </td> 
   <td scope="col"> <p>Die tatsächlichen Gesamtkosten der enthaltenen Projekte. Sie können die tatsächlichen Gesamtkosten für die Gesamtdauer der eingeschlossenen Projekte anzeigen oder die tatsächlichen Gesamtkosten nur für den angegebenen Datumsbereich anzeigen (Sie können eine einzelne Woche oder einen einzelnen Monat angeben).</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Tatsächliche Einnahmen</strong> </td> 
   <td> <p>Der tatsächliche Umsatz ist der Umsatz, der mit den tatsächlichen Stunden der Aufgaben verbunden ist.</p> <p>Der tatsächliche Umsatz wird im Nutzungsbericht erst angezeigt, nachdem die Aufgabe als abgeschlossen oder Fertig markiert wurde (oder ein Status, der mit Abgeschlossen übereinstimmt).</p> <p>Die Berechnung des tatsächlichen Umsatzes für die enthaltenen Projekte durch den Nutzungsbericht hängt vom für die Aufgabe festgelegten Umsatztyp ab, wie im Abschnitt <a href="#track-revenue" class="MCXref xref">Umsatz verfolgen</a> in diesem Artikel. </p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Rand</strong> </td> 
   <td> <p>Der Prozentsatz der Spanne wird wie folgt berechnet:</p> <p>Tatsächlicher Umsatz - Tatsächliche Kosten / Tatsächlicher Umsatz * 100. </p> <p><b>NOTIZ</b>

Wenn der tatsächliche Umsatz gleich 0 ist, wird der Rand als 0 angezeigt. </p> </td>
</tr> 
 </tbody> 
</table>

<!--Note from the table from above "Function" header in the middle of the table; right after the "Planned Revenue"/"Margin" definition: 
     <p scope="col" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This needs to be either split in two tables of formatted differently)</p>
    -->

## Verfolgen von Fortschritt, Kosten und Umsatz mit dem Nutzungsbericht {#track-progress-cost-and-revenue-with-the-utilization-report}

Sie können den Fortschritt oder die Kosten eines Projekts, Programms oder Portfolios verfolgen.

Sie können Informationen zum Nutzungsbericht für eine bestimmte Woche oder einen bestimmten Monat oder für die Gesamtdauer der Projekte anzeigen.

So verfolgen Sie den Fortschritt oder die Kosten eines oder mehrerer Projekte mit einem Nutzungsbericht:

1. Führen Sie je nachdem, ob Sie Nutzungsinformationen für ein einzelnes Projekt, mehrere Projekte, ein Programm oder ein Portfolio anzeigen, einen der folgenden Schritte aus:

   * So zeigen Sie Nutzungsinformationen für ein einzelnes Projekt an:

      1. Wechseln Sie zu einem Projekt, für das Sie Nutzungsinformationen anzeigen möchten, und klicken Sie dann auf **Mehr anzeigen > Nutzung**.
      1. Informationen zur Verwendung werden automatisch angezeigt, wenn Sie ein einzelnes Projekt anzeigen. Es ist nicht erforderlich, einen Filter anzuwenden.\
         Wenn Sie den Bericht &quot;Nutzung&quot;filtern möchten, können Sie einen Filter anwenden und dann auf **Ausführen**.\
         Informationen zum Filtern des Nutzungsprotokolls finden Sie im Abschnitt . [Informationen zur Filterauslastung](#filter-utilization-information) in diesem Artikel.\
         Die Informationen zur Verwendung werden für einzelne Benutzer und Rollen angezeigt (Benutzer werden in ihrer zugehörigen Rolle gruppiert).

   * So zeigen Sie Nutzungsinformationen für mehrere Projekte an:

      1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Ressourcen**, dann **Nutzung** im linken Bereich.
      1. Anwenden eines Filters auf den Bericht &quot;Nutzung&quot;und klicken Sie dann auf **Ausführen**.\
         Sie müssen mindestens ein Projekt im Filter angeben, bevor Sie den Bericht &quot;Nutzung&quot;ausführen. Informationen zum Filtern des Nutzungsprotokolls finden Sie im Abschnitt . [Informationen zur Filterauslastung](#filter-utilization-information) in diesem Artikel.\
         Informationen zur Verwendung werden für einzelne Rollen und Projekte angezeigt (Rollen sind innerhalb des zugehörigen Projekts gruppiert).

   * So zeigen Sie Nutzungsinformationen für ein Programm an:

      1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Ressourcen**, dann **Nutzung** im linken Bereich und klicken Sie auf die **Anzeigen**>**Programme**.
      1. Anwenden eines Filters auf den Bericht &quot;Nutzung&quot;und klicken Sie dann auf **Ausführen**.\
         Sie müssen ein oder mehrere Programme im Filter angeben, bevor Sie den Bericht &quot;Nutzung&quot;ausführen. Informationen zum Filtern des Nutzungsprotokolls finden Sie im Abschnitt . [Informationen zur Filterauslastung](#filter-utilization-information) in diesem Artikel.\
         Informationen zur Nutzung werden für einzelne Projekte und Programme angezeigt (Projekte sind in ihrem jeweiligen Programm gruppiert).

   * So zeigen Sie Nutzungsinformationen für ein Portfolio an:

      1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Ressourcen**, dann **Nutzung** Klicken Sie im linken Bereich auf **Anzeigen**>**Portfolios**.
      1. Anwenden eines Filters auf den Bericht &quot;Nutzung&quot;und klicken Sie dann auf **Ausführen**.\
         Sie müssen mindestens ein Portfolio im Filter angeben, bevor Sie den Bericht &quot;Nutzung&quot;ausführen. Informationen zum Filtern des Nutzungsprotokolls finden Sie im Abschnitt . [Informationen zur Filterauslastung](#filter-utilization-information) in diesem Artikel.\
         Informationen zur Nutzung werden für einzelne Projekte, Programme und Portfolios angezeigt (Projekte werden innerhalb ihres zugehörigen Programms gruppiert und Programme innerhalb ihres zugehörigen Portfolios gruppiert).

1. Klicken Sie in der rechten oberen Ecke des Nutzungsberichts auf die Schaltfläche **Ansicht** aus dem Dropdown-Menü und wählen Sie dann aus den folgenden Optionen aus:

   * **Kosten**
   * **Stunden**
   * **Einnahmen**
   * **Einnahmen vs. Kosten (geplante Kosten)**
   * **Umsatz vs. Kosten (realisiert)**.

   Die ausgewählte Option bestimmt, welche Spalten und Informationen im Bericht verfügbar sind. Weitere Informationen zu den in den einzelnen Spalten verfügbaren Informationen finden Sie in der Tabelle in Schritt 5.\
   ![](assets/utilization-view-dropdown.png)

1. (Optional) Wählen Sie den Datumsbereich aus, für den die Nutzungsinformationen angezeigt werden. Sie können Informationen für eine bestimmte Woche oder einen bestimmten Monat links neben dem **Insgesamt** Spalte. Informationen für das gesamte Projekt, Programm oder Portfolio werden immer im **Insgesamt** Spalte.\
   Weitere Informationen finden Sie im Abschnitt . [Anpassen des Datumsbereichs, für den Informationen angezeigt werden](#adjust-the-date-range-for-which-information-is-displayed) in diesem Artikel.

1. (Optional) Klicken Sie auf einen beliebigen Spaltentitel, um den Nutzungsbericht nach den Informationen in dieser Spalte zu sortieren. Die Sortierung funktioniert nur, wenn Sie mehrere Elemente in Ihren Bericht aufnehmen. Sie können beispielsweise die Ergebnisse Ihres Berichts sortieren, wenn Sie mehr als ein Projekt (oder Portfolio oder Programm) betrachten. Sie können die Ergebnisse nicht sortieren, wenn Sie jeweils nur ein Projekt (oder ein Portfolio oder ein Programm) betrachten.
1. Verwenden Sie die Informationen im Abschnitt . [Übersicht über den Nutzungsbericht](#overview-of-the-utilization-report) in diesem Artikel , um mehr über die einzelnen Spalten im Nutzungsbericht zu erfahren.

## Informationen zur Filterauslastung {#filter-utilization-information}

Sie können die in einem Nutzungsbericht angezeigten Inhalte nach einem Projekt filtern. Sie können nach Aufgaben, Problemen, Rollen und benutzerdefinierten Daten filtern. Wenn Sie einen Filter auf den Bericht &quot;Nutzung&quot;anwenden, enthält der Bericht &quot;Nutzung&quot;Informationen, die auf den von Ihnen ausgewählten Kriterien basieren.

Sie können einen Filter erstellen oder einen zuvor erstellten Filter anwenden.

* [Filter erstellen oder ändern](#create-or-modify-a-filter)
* [Anwenden eines gespeicherten Filters](#apply-a-saved-filter)
* [Filter duplizieren](#duplicate-a-filter)
* [Filter umbenennen](#rename-a-filter)
* [Filter löschen](#delete-a-filter)

### Filter erstellen oder ändern {#create-or-modify-a-filter}

Wenn Sie einen Filter erstellen, haben alle Workfront-Benutzer, die Zugriff auf den Bericht &quot;Nutzung&quot;haben, auch Zugriff auf den von Ihnen erstellten Filter. Wenn Sie einen vorhandenen Filter ändern, wird der Filter für alle Benutzer geändert, die Zugriff auf den Bericht &quot;Verwendung&quot;haben.

So erstellen oder ändern Sie einen Filter:

1. Um Nutzungsinformationen für ein einzelnes Projekt zu filtern, gehen Sie zu dem Projekt, für das Sie Nutzungsinformationen filtern möchten, und klicken Sie dann auf **Weitere Informationen anzeigen > Verwendung** im linken Bereich.

   Oder

   Um Nutzungsinformationen für mehrere Projekte, für ein Programm oder für ein Portfolio zu filtern, klicken Sie auf das Symbol Hauptmenü . ![](assets/main-menu-icon.png) in der oberen rechten Ecke von Workfront, **Ressourcen**, **Nutzung** im linken Bereich, dann **Anzeigen**>**Programme** oder **Portfolios** oder **Projekte**.

1. Klicken Sie auf **Filter** -Symbol, um die Filteroptionen anzuzeigen.

1. (Bedingt) Um einen vorhandenen Filter zu ändern, klicken Sie auf die Schaltfläche **Filter** und wählen Sie dann den zu ändernden Filter aus.
1. Geben Sie die folgenden Informationen an, um den Filter zu erstellen oder zu ändern:

   * **Portfolios:** Beginnen Sie mit der Eingabe des Namens des Portfolios, das die Informationen enthält, die Sie in den Nutzungsbericht aufnehmen möchten, und klicken Sie dann auf den Namen, wenn er im Dropdown-Menü angezeigt wird.\
     Wiederholen Sie diesen Vorgang, um Informationen aus mehreren Portfolios in den Nutzungsbericht aufzunehmen.\
     Um alle Portfolios aus Ihrem System in Ihren Filter aufzunehmen, klicken Sie auf **Alle hinzufügen**. (Diese Option ist nur verfügbar, wenn Ihr System weniger als 10 Portfolios enthält.)

   * **Programme:** Beginnen Sie mit der Eingabe des Programmnamens, der die Informationen enthält, die Sie in den Bericht &quot;Nutzung&quot;aufnehmen möchten, und klicken Sie dann auf den Namen, wenn er im Dropdown-Menü angezeigt wird.\
     Wiederholen Sie diesen Vorgang, um Informationen aus mehreren Aufgaben in den Bericht &quot;Nutzung&quot;aufzunehmen.\
     Wenn Sie bereits Portfolios im Filter benannt haben, muss das von Ihnen angegebene Programm aus den bereits im Filter enthaltenen Portfolios stammen. Ist dies nicht der Fall, werden die Daten aus dem Programm nicht in den Bericht &quot;Nutzung&quot;aufgenommen.\
     Um alle Programme aus Ihrem System in Ihren Filter aufzunehmen, klicken Sie auf **Alle hinzufügen**. (Diese Option ist nur verfügbar, wenn Ihr System weniger als 20 Programme enthält.)

   * **Projekte:** Beginnen Sie mit der Eingabe des Namens des Projekts, das die Informationen enthält, die Sie in den Nutzungsbericht aufnehmen möchten, und klicken Sie dann auf den Namen, wenn er im Dropdown-Menü angezeigt wird.\
     Wiederholen Sie diesen Vorgang, um Informationen aus mehreren Projekten in den Nutzungsbericht aufzunehmen.\
     Wenn Sie bereits Portfolios oder Programme im Filter benannt haben, muss das von Ihnen angegebene Projekt aus einem der Portfolios oder Programme stammen, die bereits im Filter enthalten sind. Ist dies nicht der Fall, werden die Daten aus dem Projekt nicht in den Bericht &quot;Nutzung&quot;aufgenommen.\
     Um alle Projekte aus Ihrem System in Ihren Filter aufzunehmen, klicken Sie auf **Alle hinzufügen**. (Diese Option ist nur verfügbar, wenn Ihr System weniger als 250 Projekte enthält.)

   * **Aufgaben:** Beginnen Sie mit der Eingabe des Namens der Aufgabe, die die Informationen enthält, die Sie in den Bericht &quot;Nutzung&quot;aufnehmen möchten, und klicken Sie dann auf den Namen, wenn er im Dropdown-Menü angezeigt wird.\
     Wiederholen Sie diesen Vorgang, um Informationen aus mehreren Aufgaben in den Bericht &quot;Nutzung&quot;aufzunehmen.\
     Wenn Sie bereits Portfolios, Programme oder Projekte im Filter benannt haben, muss die Aufgabe aus einem der Portfolios, Programme oder Projekte stammen, die bereits im Filter enthalten sind. Ist dies nicht der Fall, werden die Daten aus der Aufgabe nicht in den Bericht &quot;Nutzung&quot;aufgenommen.

   * **Probleme:** Beginnen Sie mit der Eingabe des Namens des Problems, das die Informationen enthält, die Sie in den Nutzungsbericht aufnehmen möchten, und klicken Sie dann auf den Namen, wenn er im Dropdown-Menü angezeigt wird.\
     Wiederholen Sie diesen Vorgang, um Informationen aus mehreren Problemen in den Bericht &quot;Nutzung&quot;aufzunehmen.\
     Wenn Sie bereits Portfolios, Programme oder Projekte im Filter benannt haben, muss das von Ihnen angegebene Problem aus einem der Portfolios, Programme oder Projekte stammen, die bereits im Filter enthalten sind. Ist dies nicht der Fall, werden die Daten aus dem Problem nicht in den Nutzungsbericht aufgenommen.\
     Kosteninformationen für Probleme werden nicht immer im Nutzungsbericht aufgeführt. Weitere Informationen dazu, wann im Nutzungsbericht Kosteninformationen für Probleme enthalten sind, finden Sie im Abschnitt [Verfolgen von Fortschritt, Kosten und Umsatz mit dem Nutzungsbericht](#track-progress-cost-and-revenue-with-the-utilization-report) in diesem Artikel.

   * **Rollen:** Beginnen Sie mit der Eingabe des Namens der Rolle, die Sie im Nutzungsbericht darstellen möchten, und klicken Sie dann auf den Namen, wenn er im Dropdown-Menü angezeigt wird. Wiederholen Sie diesen Vorgang, um weitere Rollen hinzuzufügen.\
     Der Nutzungsbericht enthält nur Informationen zu den von Ihnen angegebenen Rollen. Beispielsweise enthält eine Aufgabe 10 tatsächliche Stunden. 6 dieser Stunden stammen aus einer Designer-Rolle und 4 aus einer Entwicklerrolle. Wenn Sie den Nutzungsbericht nach Rolle für Designer filtern, werden die 4 Stunden, die aus der Entwicklerrolle stammen, aus dem Bericht ausgeschlossen.

   * **Filterregel hinzufügen:** Klicken **Filterregel hinzufügen**, klicken Sie in das erste Feld und geben Sie dann den Feldnamen ein, nach dem Sie filtern möchten. Wenn das Feld verfügbar ist, wird es für jedes Objekt gefüllt, mit dem es verknüpft werden kann. Klicken Sie auf den Namen des Felds, um es dem Filter hinzuzufügen.

     >[!IMPORTANT]
     >
     >Sie müssen den Feldnamen und nicht die Feldbezeichnung eingeben. Die Feldbezeichnung wird in einem benutzerdefinierten Formular angezeigt, das an ein Objekt angehängt ist. Informationen zum Unterschied zwischen der Beschriftung und dem Namen eines benutzerdefinierten Felds finden Sie unter  [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

     Weitere Informationen zu den Feldern, die in den Spalten angezeigt werden, finden Sie unter [Glossar der Adobe Workfront-Terminologie](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).\
     Wählen Sie die Filter- und Bedingungsmodifikatoren für den Filter aus. Die verfügbaren Modifikatoren werden unter [Filter- und Bedingungs-Modifikatoren](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. Um einen neuen Filter zu erstellen, klicken Sie auf **Filter speichern**.\
   Oder\
   Um einen vorhandenen Filter zu ändern, klicken Sie auf den Dropdown-Pfeil neben dem **Filter speichern** und klicken Sie auf **Neuen Filter speichern**.\
   Im **Filtername** ein, geben Sie einen Namen für den Filter ein und klicken Sie auf **Speichern**.\
   Der Bereich Verwendung wird mit den Informationen gefiltert, die Sie in den Filter aufgenommen haben.

### Anwenden eines gespeicherten Filters {#apply-a-saved-filter}

1. Um einen Filter auf den Nutzungsbericht für ein einzelnes Projekt anzuwenden, gehen Sie zu dem Projekt, nach dem Sie filtern möchten, und klicken Sie dann auf **Weitere Informationen anzeigen > Verwendung** im linken Bereich.

   Oder

   Wenn Sie einen Filter auf den Nutzungsbericht anwenden möchten, klicken Sie auf die Schaltfläche **Hauptmenü** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von Workfront, **Ressourcen**, **Nutzung** im linken Bereich, dann **Anzeigen**>**Programme** oder **Portfolios** oder **Projekte**.

1. Klicken **Gespeicherte Filter** und wählen Sie dann im Dropdown-Menü den anzuwendenden Filter aus.

### Filter duplizieren {#duplicate-a-filter}

1. Um einen Filter für den Nutzungsbericht für ein einzelnes Projekt zu duplizieren, gehen Sie zu dem Projekt, für das Sie den Filter duplizieren möchten, und klicken Sie dann auf **Weitere Informationen anzeigen > Verwendung** im linken Bereich.

   Oder

   Um einen Filter für den Nutzungsbericht für mehrere Projekte, für ein Programm oder für ein Portfolio zu duplizieren, klicken Sie auf die Schaltfläche **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Ressourcen**, dann **Nutzung** im linken Bereich.

1. Klicken **Gespeicherte Filter**, bewegen Sie den Mauszeiger im Dropdown-Menü über den Filter, den Sie duplizieren möchten, und klicken Sie dann auf **Duplizieren** Symbol.

   ![](assets/utilization-filter-duplicate.png)\
   Das Dialogfeld Filter duplizieren wird angezeigt.

1. Im **Filtername** ein, geben Sie einen Namen für den neuen Filter ein und klicken Sie auf **Speichern**.

### Filter umbenennen {#rename-a-filter}

Wenn Sie einen Filter umbenennen, sehen alle Workfront-Benutzer, die Zugriff auf den Bericht &quot;Verwendung&quot;haben, den von Ihnen gewählten neuen Namen.

So benennen Sie einen Filter um:

1. Um einen Filter für den Nutzungsbericht für ein einzelnes Projekt umzubenennen, gehen Sie zu dem Projekt, für das Sie den Filter umbenennen möchten, und klicken Sie dann auf **Weitere Informationen anzeigen > Verwendung** im linken Bereich.

   Oder

   Um einen Filter für den Nutzungsbericht für mehrere Projekte, für ein Programm oder für ein Portfolio umzubenennen, klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Ressourcen**, dann **Nutzung** im linken Bereich.

1. Klicken **Gespeicherte Filter**, bewegen Sie den Mauszeiger im Dropdown-Menü über den Filter, den Sie duplizieren möchten, und klicken Sie dann auf **Umbenennen** Symbol.\
   ![](assets/utilization-filter-rename.png)\
   Das Dialogfeld Filter umbenennen wird angezeigt.

1. Im **Filtername** ein, geben Sie einen Namen für den neuen Filter ein und klicken Sie auf **Speichern**.

### Filter löschen {#delete-a-filter}

Wenn Sie einen Filter löschen, wird der Filter für alle Workfront-Benutzer gelöscht, die Zugriff auf den Bericht &quot;Verwendung&quot;haben.

So löschen Sie einen Filter:

1. Um einen Filter für den Nutzungsbericht für ein einzelnes Projekt zu löschen, gehen Sie zu dem Projekt, für das Sie den Filter löschen möchten, und klicken Sie dann auf **Weitere Informationen anzeigen > Verwendung** im linken Bereich.

   Oder

   Um einen Filter für den Nutzungsbericht für mehrere Projekte, für ein Programm oder für ein Portfolio zu löschen, klicken Sie auf die Schaltfläche **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Ressourcen**, dann **Nutzung** im linken Bereich.

1. Klicken **Gespeicherte Filter**, bewegen Sie den Mauszeiger im Dropdown-Menü über den Filter, den Sie duplizieren möchten, und klicken Sie dann auf **Löschen** Symbol.

   ![](assets/utilization-filter-delete.png)

1. Klicken **Löschen** angezeigt, wenn Sie gefragt werden, ob Sie den Filter löschen möchten.

## Anpassen des Datumsbereichs, für den Informationen angezeigt werden {#adjust-the-date-range-for-which-information-is-displayed}

Sie können den Datumsbereich anpassen, für den die Nutzungsinformationen angezeigt werden. Sie können ein vergangenes oder künftiges Datum auswählen. Änderungen, die Sie vornehmen, sind nur für Sie sichtbar.

1. Um den Datumsbereich des Nutzungsberichts für ein einzelnes Projekt anzupassen, gehen Sie zu dem Projekt, für das Sie den Datumsbereich anpassen möchten, und klicken Sie dann auf **Weitere Informationen anzeigen > Verwendung** im linken Bereich.

   Oder

   Um den Datumsbereich des Berichts &quot;Nutzung&quot;für mehrere Projekte, für ein Programm oder für ein Portfolio anzupassen, klicken Sie auf die Schaltfläche **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Ressourcen**, dann **Nutzung** im linken Bereich.

1. Klicken Sie auf den Datumsbereich neben dem **Export** Schaltfläche.

   Die aktuelle Woche ist standardmäßig ausgewählt.

1. Wählen Sie aus den folgenden Optionen aus:

   * **Woche:** Wählen Sie diese Option aus, um eine bestimmte Woche (von Sonntag bis Samstag) auszuwählen.
   * **Monat:** Wählen Sie diese Option aus, um einen bestimmten Monat auszuwählen.

   Der ausgewählte Datumsbereich wird im Nutzungsbericht links neben dem **Insgesamt** Spalte.\
   Workfront merkt sich, ob Sie eine Wochen- oder Monatsansicht anzeigen möchten. Wenn Sie das nächste Mal auf den Nutzungsbericht zugreifen, wird je nach ausgewählter Option die aktuelle Woche oder der aktuelle Monat angezeigt.

## Informationen zur Exportauslastung

Sie können Nutzungsinformationen für ein Projekt, Programm oder Portfolio aus Workfront exportieren. Informationen können nur in den Formaten XLSX, TSV und PDF exportiert werden.

In Microsoft Excel werden negative Zahlen in Klammern angezeigt.

Informationen zur Exportauslastung:

1. Um Auslastungsinformationen für ein einzelnes Projekt zu exportieren, gehen Sie zu dem Projekt, für das Sie Auslastungsinformationen exportieren möchten, und klicken Sie dann auf das **Nutzung** Registerkarte (abhängig von Ihren Layouteinstellungen, befindet sich dies möglicherweise unter der **Mehr** Registerkarte).

   Oder

   Um Nutzungsinformationen für mehrere Projekte, für ein Programm oder für ein Portfolio zu exportieren, klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Ressourcen**, dann **Nutzung** im linken Bereich.

1. Klicken **Export**, befindet sich in der linken oberen Ecke der **Nutzung** Registerkarte.

1. Wählen Sie aus den folgenden Optionen aus:

   * **PDF:** Exportiert den Bericht im PDF-Format. Dies ist das empfohlene Format, wenn Sie den Bericht drucken möchten.\
     Wählen Sie entweder **Brief - Hochformat**, **Brief - Querformat** oder **Sonstige Größen** (bietet Optionen für den Export in Legal (8,5&quot; x 14&quot;), Ledger (11&quot; x 17&quot;) und A4).\
     Je nach verwendetem Betriebssystem haben Sie möglicherweise die Möglichkeit, die Datei zu öffnen oder zu speichern. Öffnen Sie die Datei mit der zugehörigen Anwendung oder speichern Sie sie auf Ihrer Festplatte.

   * **Excel:** Exportiert den Bericht im XLSX-Format. Dies ist das empfohlene Format, wenn Sie die Daten in Excel weiter analysieren möchten.\
     Je nach verwendetem Betriebssystem haben Sie möglicherweise die Möglichkeit, die Datei zu öffnen oder zu speichern. Öffnen Sie die Datei mit der zugehörigen Anwendung oder speichern Sie sie auf Ihrer Festplatte.

   * **Tabulatorgetrennt:** Exportiert den Bericht im TSV-Format. Dies ist das empfohlene Format, wenn Sie die Daten zur weiteren Analyse in die Software von Drittanbietern importieren möchten.\
     Je nach verwendetem Betriebssystem haben Sie möglicherweise die Möglichkeit, die Datei zu öffnen oder zu speichern. Öffnen Sie die Datei mit der zugehörigen Anwendung oder speichern Sie sie auf Ihrer Festplatte.

1. Informationen in diesem Artikel lesen [Daten exportieren](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md) , um zu verstehen, wie die exportierte Datei verwendet wird.

## Anzeigen von Nutzungsinformationen in einer Grafik

Sie können die Daten aus dem Nutzungsbericht in einer Diagrammansicht visualisieren.

1. Um einen Nutzungsbericht für ein einzelnes Projekt in einem Diagrammformat anzuzeigen, gehen Sie zu dem Projekt, das Sie anzeigen möchten, und klicken Sie dann auf **Mehr anzeigen > Nutzung** im linken Bereich.

   Oder

   Wenn Sie einen Nutzungsbericht im Diagrammformat für mehrere Projekte, für ein Programm oder für ein Portfolio anzeigen möchten, klicken Sie auf **Berichterstellung** in der Leiste &quot;Globale Navigation&quot;, um zum Bereich &quot;Berichterstellung&quot;zu wechseln, und klicken Sie dann auf das **Nutzung** Registerkarte.

1. Klicken Sie in der rechten oberen Ecke des Nutzungsberichts auf die Schaltfläche **Diagramm** Symbol.\
   ![](assets/utilization-chart.png)\
   Der Nutzungsbericht wird in einer Diagrammansicht angezeigt.

1. (Optional) Konfigurieren Sie diese Option, um Projekte, Programme oder Portfolios anzuzeigen, indem Sie die entsprechende Option aus dem **Anzeigen** Dropdown-Menü.
1. (Optional) Bewegen Sie den Mauszeiger über einen bestimmten Zeitpunkt im Bericht, um Daten zu diesem Zeitpunkt anzuzeigen.

   ![](assets/utilization-chart-hover-350x176.png)

1. (Optional) Passen Sie die Filter an, um festzulegen, welche Informationen im Diagramm angezeigt werden. Informationen zum Anpassen der Filter finden Sie im Abschnitt . [Informationen zur Filterauslastung](#filter-utilization-information) in diesem Artikel.
1. (Optional) Konfigurieren Sie den Zeitrahmen des Diagrammberichts, wie im Abschnitt beschrieben. [Anpassen des Datumsbereichs, für den Informationen angezeigt werden](#adjust-the-date-range-for-which-information-is-displayed) in diesem Artikel.
