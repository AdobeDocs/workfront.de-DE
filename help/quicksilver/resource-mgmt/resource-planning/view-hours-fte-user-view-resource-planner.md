---
content-type: reference
product-area: resource-management;user-management
navigation-topic: resource-planning
title: Anzeigen der verfügbaren, geplanten und tatsächlichen Stunden oder der FTE im Ressourcenplaner bei Verwendung der Benutzeransicht
description: Zeigen Sie verfügbare, geplante und tatsächliche Stunden oder VZÄ im Ressourcenplaner an, wenn Sie die User viewPlanning-Funktion im RP verwenden. Vielleicht "budgeting resources in the RP"oder "Managing Resources in the RP". usw. - oder müssen Sie möglicherweise von einem anderen POV umgeleitet werden?!)"
author: Alina
feature: Resource Management
exl-id: 6b532aa2-435f-4fda-b7ce-abe0a785638f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1739'
ht-degree: 1%

---

# Anzeigen der verfügbaren, geplanten und tatsächlichen Stunden oder der FTE im Ressourcenplaner bei Verwendung der Benutzeransicht

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Consider renaming this article (probably split already) to something other than "Planning" in the RP" - maybe "budgeting resources in the RP" or "Managing Resources in the RP." etc... - or might need to be repurposed from another POV?!)</p>
-->

Zusätzlich zu den Budgeteinträgen in den Projekt- und Rollenansichten können Sie über die Benutzeransicht des Adobe Workfront-Ressourcenplaners Informationen zu den geplanten, verfügbaren und tatsächlichen Stunden- oder FTE-Werten für Projekte und Ressourcen anzeigen.

## Überblick über die Benutzeransicht im Ressourcenplaner

Beachten Sie beim Anzeigen der Stunden- oder FTE-Informationen im Ressourcenplaner Folgendes:

* Sie können die verfügbaren und geplanten Stunden oder die FTE-Informationen für Benutzer, Arbeitsplatzrollen und Projekte in allen Ansichten des Resource Planers anzeigen.
* Sie können die folgenden Informationen nur in der Benutzeransicht anzeigen:

   * Differenz zwischen der geplanten Stundenzahl oder VZÄ und der Menge der verfügbaren Stunden oder VZÄ. Anschließend können Sie die Zuordnung Ihrer Benutzer entsprechend dieser Differenz in den Ansichten &quot;Projekt&quot;und &quot;Rolle&quot;planen.
   * Die tatsächlichen Stunden oder die VZÄ.

* Sie können die Differenz zwischen dem verfügbaren Benutzer und der Anzahl der geplanten Stunden oder FTE entweder als Zahl oder als Prozentwert in der Benutzeransicht anzeigen.
* Sie können die Informationen nicht in der Ansicht Benutzer nach Kosten anzeigen.
* Adobe Workfront füllt Verfügbare Stunden oder VZÄ entsprechend der Arbeitszeit aus, die den Benutzern in ihren Zeitplänen zugewiesen ist.\
  Benutzer, die keinem Zeitplan zugeordnet sind, zeigen die Verfügbarkeit gemäß dem Standardplan an.\
  Weitere Informationen zum Standardzeitplan finden Sie unter [Erstellen eines Zeitplans](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Workfront füllt geplante Stunden oder VZÄ aus den Informationen zu den Aufgaben und Problemstellungen der Projekte aus.
* Workfront füllt &quot;Tatsächliche Stunden&quot;mit der tatsächlichen Zeit, die Aufgaben und Problemen von den ihnen zugewiesenen Benutzern zugewiesen wurde. Dies umfasst die Zeit, die bei einem Projekt angemeldet ist.
* In der Ansicht &quot;User&quot;haben Sie folgende Möglichkeiten:

   * Erweitern Sie jeden Benutzer, um eine Liste der Projekte anzuzeigen, denen dieser Benutzer zugewiesen ist.

     >[!NOTE]
     >
     >Nur Benutzer, die mit den in den Filtern enthaltenen Projekten verknüpft sind, können erweitert werden.

   * Erweitern Sie jedes Projekt, um eine Liste der Vorgangsrollen anzuzeigen, die der Benutzer für diese Projekte ausführen kann.
   * Erweitern Sie jede Rolle, um eine Liste der Aufgaben anzuzeigen, denen der Benutzer in dieser Rolle zugewiesen ist.

  Wenn den Benutzern keine Vorgangsrollen zugeordnet sind, werden ihre Verfügbaren, Geplanten und tatsächlichen Stunden oder FTE im Abschnitt **Keine Rolle** aufgelistet.\
  Informationen dazu, welche Felder und Elemente beim Anwenden der Benutzeransicht auf den Ressourcenplaner angezeigt werden, finden Sie im Abschnitt &quot;Auswahl der Projekt-/Rolle-/Benutzeransicht&quot;in der Navigationsübersicht für den Ressourcenplaner ](../../resource-mgmt/resource-planning/resource-planner-navigation.md).[

## Übersicht über die Felder, die in der Benutzeransicht des Ressourcen-Planers angezeigt werden

In den folgenden Tabellen finden Sie Informationen zu den Informationen, die in der Ansicht &quot;User&quot;des Ressourcenplaners angezeigt werden. Die Informationen werden in Stunden- oder FTE-Werten angezeigt.

* [Die (verfügbare) AVL Spalte](#the-avl-available-column)
* [Die Spalte PLN (Geplant)](#the-pln-planned-column)
* [Die (tatsächliche) Spalte ACT](#The%C2%A0ACT)
* [Die DIF-Spalte (Differenz)](#the-dif-difference-column)
* [Die Spalte % (Prozentsatz der geplanten Stundenzuordnung)](#the-planned-hours-allocation-percentage-column)

### Die Spalte AVL (verfügbar) {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Angezeigt von</strong> </td> 
   <td> <p><strong>Beschreibung</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Benutzerin oder Benutzer</td> 
   <td>Die Gesamtanzahl verfügbarer Stunden oder FTE für den Benutzer gemäß seinem Zeitplan. </td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td>Diese Informationen sind für das Projekt nicht verfügbar, wenn die Benutzeransicht auf den Ressourcenplaner angewendet wird. </td> 
  </tr> 
  <tr> 
   <td>Funktion</td> 
   <td> <p>Die Gesamtanzahl verfügbarer Stunden oder FTE für die Rolle gemäß dem Benutzerplan und dem <strong>Prozentsatz der FTE-Verfügbarkeit</strong> der Rolle.</p> </td> 
  </tr> 
  <tr> 
   <td>Aufgabe oder Problem</td> 
   <td>Diese Informationen sind für die Aufgabe oder das Problem nicht verfügbar. </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen dazu, wie die Verfügbarkeit von Benutzern und Rollen basierend auf dem Zeitplan des Benutzers und dem Prozentsatz der Verfügbarkeit der Rolle in der VZÄ berechnet wird, finden Sie unter [Übersicht über die Berechnungsstunden und die VZÄ für Benutzer und Rollen im Ressourcenplaner](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

### Die Spalte PLN (Geplant) {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Angezeigt von</strong> </td> 
   <td> <p><strong>Beschreibung</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Benutzerin oder Benutzer</td> 
   <td> Die Gesamtanzahl aller geplanten Stunden oder FTE aus allen Aufgaben oder Ausgaben, die dem Benutzer für alle Projekte zugewiesen wurden.<br><p>Dazu gehören Aufgaben und Probleme, die dem Benutzer zugewiesen sind, aber keiner Auftragsrolle und Aufgaben oder Probleme zugeordnet sind, die sich nicht auf Projekte beziehen, auf die Sie Zugriff auf "Verwalten"haben.</p><p>Wenn die Benutzerzuordnung für Stunden mithilfe des Lastenausgleichs geändert wurde, können die Daten im Ressourcenplaner beeinträchtigt werden, wenn die ausgewählten Daten nur einen Teil einer Aufgabe oder eines Problems enthalten. Informationen zum Ändern der Zuordnungen für Benutzer finden Sie unter <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Verwalten von Benutzerzuordnungen im Arbeitslastausgleich</a> . </p></td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td> Die Gesamtanzahl aller geplanten Stunden oder FTE aus allen Aufgaben und Problemen, die einem bestimmten Benutzer im Projekt zugewiesen sind.<br><p>Hinweis: Dies umfasst nicht die geplanten Stunden oder die FTE aus Aufgaben oder Problemen, die Benutzern nicht zugewiesen sind. </p></td> 
  </tr> 
  <tr> 
   <td>Funktion</td> 
   <td> <p>Die Gesamtanzahl aller geplanten Stunden oder FTE aus allen Aufgaben und Problemen, die dem Benutzer mit dieser Rolle im Projekt zugewiesen sind.</p> <p> <p>Hinweis: Dies umfasst nicht die geplanten Stunden oder die FTE aus Aufgaben oder Problemen, die dieser Rolle, aber nicht diesem Benutzer in dieser Rolle zugewiesen sind. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Aufgabe oder Problem</td> 
   <td>Die geplanten Stunden oder die FTE, die mit der Aufgabe oder dem Problem im Projekt verbunden sind.</td> 
  </tr> 
 </tbody> 
</table>

Beachten Sie bei der Anzeige der geplanten Stunden Folgendes:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view)</p>
-->

* Die geplanten Stunden werden für jede ihnen zugewiesene Ressource innerhalb der Dauer der Aufgaben und Probleme gleichmäßig auf jeden Tag verteilt. Die Aufgaben- oder Problemdauer basiert auf ihren geplanten Start- und Abschlussdaten und umfasst jeden Kalendertag innerhalb dieses Zeitraums.\
  Workfront berücksichtigt den Zeitplan des Benutzers oder des Projekts bei der Verteilung von geplanten Stunden an Benutzer oder Projekte. In diesem Fall werden geplante Stunden innerhalb der Dauer von Aufgaben oder Problemen, ausgenommen Wochenenden, Vertreibungen und geplante Ausnahmen, gleichmäßig auf jeden Tag verteilt.

  Wenn Sie beispielsweise den Ressourcenplaner nach Woche anzeigen und Aufgaben mit mehreren Wochen Projektdauer haben, hängt die Anzahl der geplanten Stunden pro Woche davon ab, wie viele Tage innerhalb dieser Woche Teil der Aufgabendauer sind. Dies funktioniert auf ähnliche Weise, wenn der Ressourcenplaner nach Monat oder Quartal angezeigt wird und Aufgaben mehrere Monate oder Quartale umfassen.\
  Wochenendtage, zeitgesteuerte Ausnahmen und Verfallstage sind von dieser Verteilung ausgeschlossen.

* Die folgenden Aufgabenkategorien werden bei der Berechnung der geplanten Stunden für jede Ressource berücksichtigt:

   * Aufgaben, die Benutzern in Ressourcen-Pools, Jobrollen oder Teams im Projekt zugewiesen wurden.

     >[!TIP]
     >
     >Wenn Teams Aufgaben zugewiesen sind, wird ihre Zuordnung unter den Abschnitten **Keine Rolle** und **Kein Benutzer** angezeigt. Sie können die mit Teams verknüpften geplanten Stunden sehen, aber Sie können die Stunden nicht einplanen, da weder Rollen noch Benutzer mit den Aufgaben verbunden sind.

* Geplante Stunden im Ressourcenplaner enthalten keine geplanten Stunden, die mit den folgenden Punkten verknüpft sind:

   * Übergeordnete Aufgaben
   * nicht zugewiesene Aufgaben
   * Probleme, wenn die Einstellung **Stunden aus Problemen einschließen** deaktiviert ist.

* Geplante Stunden werden nicht im Ressourcenplaner angezeigt, wenn die Aufgaben- oder Problemdauer null ist.
* Für deaktivierte Benutzer zugeordnete geplante Stunden werden nicht angezeigt.

Weitere Informationen zu geplanten Stunden und FTE im Ressourcenplaner finden Sie unter [Übersicht über Stunden, FTE und Kosten-Informationen in den Projekt- und Rollenansichten des Ressourcenplaners](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

### Die Spalte ACT (Tatsächlich)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Angezeigt von</strong> </td> 
   <td> <p><strong>Beschreibung</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Benutzerin oder Benutzer </td> 
   <td> <p>Die Zeit, die der Benutzer bei allen ihm zugewiesenen Aufgaben oder Problemen protokolliert.</p> <p>Dazu gehört Folgendes:</p> 
    <ul> 
     <li>Aufgaben und Probleme, die dem Benutzer zugewiesen, aber keiner Auftragsrolle zugeordnet sind.</li> 
     <li>Aufgaben und Probleme, die sich nicht auf Projekte beziehen, für die Sie Zugriff auf "Verwalten"haben. </li> 
    </ul> <p>Dies umfasst die im Projekt angemeldete Zeit nur, wenn der Benutzer Aufgaben oder Problemen in diesem Projekt zugewiesen ist.  </p> </td> 
  </tr> 
  <tr> 
   <td>Projekt </td> 
   <td> <p>Die Zeit, die der Benutzer bei allen Aufgaben und Problemen protokolliert, die ihm im Projekt zugewiesen sind.</p> <p>Dies umfasst jede Zeit, in der sie sich direkt beim Projekt angemeldet haben.</p> <p>Dies umfasst nicht Folgendes:</p> 
    <ul> 
     <li> <p>Zeit protokolliert für Aufgaben und Probleme, die Benutzern nicht zugewiesen sind. </p> </li> 
     <li> <p>Zeit, die bei übergeordneten Aufgaben protokolliert wird. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Funktion</td> 
   <td> <p>Die Zeit, die bei allen Aufgaben oder Problemen protokolliert wird, die dem Benutzer in dieser Rolle zugewiesen sind. </p> <p>Dies umfasst nicht Folgendes:</p> 
    <ul> 
     <li>Zeit protokolliert für Aufgaben und Probleme, die dieser Rolle zugewiesen sind, aber nicht diesem Benutzer in dieser Rolle.</li> 
     <li>Die direkt für das Projekt oder die übergeordneten Aufgaben protokollierte Zeit. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aufgabe oder Problem </td> 
   <td> <p>Die Zeit, die von dem Benutzer, der ihnen auch zugewiesen ist, bei Aufgaben und Problemen protokolliert wird. </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>Die protokollierte Zeit wird in dem Zeitrahmen angezeigt, der dem Startdatum des Stundeneintrags entspricht, unabhängig vom Zeitrahmen der Aufgabe, des Problems oder des Projekts, in dem die Stunden protokolliert werden.

Weitere Informationen zu den tatsächlichen Stunden finden Sie unter [Tatsächliche Stunden anzeigen](../../manage-work/tasks/task-information/actual-hours.md).

### Die DIF-Spalte (Differenz) {#the-dif-difference-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Angezeigt von</strong> </td> 
   <td> <p><strong>Beschreibung</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Benutzerin oder Benutzer</td> 
   <td> <p>Der Unterschied zwischen den verfügbaren und geplanten Stunden oder der FTE des Benutzers. </p> <p>Die Differenz zwischen Stunde und FTE wird anhand der folgenden Formel berechnet:</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <p>Hinweis: Wenn der Wert in negativen roten Zahlen angezeigt wird, wird der Benutzer übergeordnet. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td>Diese Informationen sind für das Projekt nicht verfügbar. </td> 
  </tr> 
  <tr> 
   <td>Funktion</td> 
   <td> <p>Der Unterschied zwischen den verfügbaren und geplanten Stunden oder der FTE der Stellenfunktion. </p> <p>Die Differenz zwischen Stunde und FTE wird anhand der folgenden Formel berechnet:</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <p>Hinweis: Wenn der Wert in negativen roten Zahlen angezeigt wird, wird die Rolle übergeordnet. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Aufgabe oder Problem</td> 
   <td>Diese Informationen sind nicht für die Aufgabe, das Problem oder das Projekt verfügbar. </td> 
  </tr> 
 </tbody> 
</table>

### Die Spalte % (Prozentsatz der geplanten Stundenzuordnung) {#the-planned-hours-allocation-percentage-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Angezeigt von</strong> </td> 
   <td> <p><strong>Beschreibung</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Benutzerin oder Benutzer</td> 
   <td> <p>Die Zuweisung der geplanten Stunden oder der VZÄ in Prozent der verfügbaren Stunden. Der Prozentsatz der geplanten Stundenzuweisung wird anhand der folgenden Formel berechnet:</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>Dieselbe Berechnung wird für FTE-Werte verwendet. </p> </td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td>Diese Informationen sind für das Projekt nicht verfügbar, wenn die Ansicht <strong>Nach Benutzer anzeigen</strong> auf den Ressourcenplaner angewendet wird.</td> 
  </tr> 
  <tr> 
   <td>Funktion</td> 
   <td> Die Zuweisung der geplanten Stunden oder der VZÄ in Prozent der verfügbaren Stunden. <p>Der Prozentsatz der geplanten Stundenzuweisung wird anhand der folgenden Formel berechnet:</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>Dieselbe Berechnung wird für FTE-Werte verwendet.</p></td> 
  </tr> 
  <tr> 
   <td>Aufgabe oder Problem</td> 
   <td>Diese Informationen sind nicht für die Aufgabe, das Problem oder das Projekt verfügbar. </td> 
  </tr> 
 </tbody> 
</table>

Wenn der Wert der geplanten Stunden oder VZÄ null ist, beträgt die Prozentzuweisung 0 %. Wenn der Wert der Verfügbaren Stunden oder VZÄ null ist, kann die Prozentzuweisung nicht berechnet werden.

Weitere Informationen zu geplanten Stunden und FTE sowie dazu, wie sie im Ressourcenplaner angezeigt werden, finden Sie unter [Budgetressourcen im Ressourcenplaner unter Verwendung der Projekt- und Rollenansichten](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this table is ideal but it does not render in Markdown) </p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Column Name (Hours or FTE)</strong> </td>
<td><strong>Displayed By</strong> </td>
<td> <p><strong>Description</strong> </p> </td>
</tr>
<tr>
<td rowspan="5">AVL <br>(Available Hours or FTE)</td>
<td>User</td>
<td>The total of Available Hours or FTE for the user according to their schedule. </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the User view to the Resource Planner. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Available Hours or FTE for the role according to the schedule of the user and the <strong>Percentage of FTE Availability</strong> of the role.</p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project.</td>
</tr>
<tr>
<td colspan="2"> <p colspan="2">For more information about how user and role availability is calculated based on the schedule of the user and the Percentage of FTE Availability of the role, see <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">PLN <br>(Planned Hours or FTE)</td>
<td>User</td>
<td> The total of Planned Hours or FTE from all the tasks or issues assigned to the user on all the projects.<br><p>This includes tasks and issues that are assigned to the user but not associated with any job role and tasks or issues that are not on projects that you have access to Manage.</p><p>When the user allocation for hours has been modified using the Workload Balancer, the data in the Resource Planner can be affected if the dates selected contain only a portion of a task or issue. For information about modifying allocations for users, see <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a> . </p></td>
</tr>
<tr>
<td>Project</td>
<td> The total of Planned Hours or FTE from all the tasks and issues assigned to a specific user on the project.<br><note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are not assigned to any users.
</note></td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Planned Hours or FTE from all the tasks and issues assigned to the user in this role on the project.</p> <p> <note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are assigned to this role but not to this user in this role.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>The Planned Hours or FTE associated with the task or the issue on the project.</td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when viewing Planned Hours:</p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view))</p>
<ul>
<li> <p>Planned Hours are equally distributed to each day within the Duration of tasks and issues , for each resource assigned to them. The task or issue Duration is based on their Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks or issues excluding weekends, time-off days, and schedule exceptions.</p> <p>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li>
<li> <p>The following categories of tasks are included in calculating the Planned Hours for each resource: </p>
<ul>
<li> <p> tasks assigned to users in Resource Pools, job roles, or teams on the project.</p> <note type="tip">
If tasks are assigned to teams, their allocation will appear under
<strong>No Role</strong> and
<strong>No User</strong> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks.
</note> </li>
</ul> </li>
</ul>
<ul>
<li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following:
<ul>
<li>parent tasks</li>
<li>unassigned tasks</li>
<li>issues, when the <strong>Include hours from Issues</strong> setting is disabled.</li>
</ul></li>
<li>Planned Hours do not display in the Resource Planner if the task or issue Duration is zero.</li>
<li>Planned Hours associated with deactivated users do not display. </li>
</ul> <p>For more information about Planned Hours and FTE in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">ACT<br>(Actual Hours or FTE) </td>
<td>User </td>
<td> <p>The time logged by the user on all the tasks or issues assigned to them.</p> <p>This includes the following:</p>
<ul>
<li>Tasks and issues that are assigned to the user but not associated with any job role.</li>
<li>Tasks and issues that are not on projects for which you have access to Manage.. </li>
</ul> <p>This does not include time logged directly on the project or on parent tasks. </p> </td>
</tr>
<tr>
<td>Project </td>
<td> <p>The time logged by the user on all the tasks and issues assigned to them on the project.</p> <p>This includes any time that they logged directly on the project.</p> <p>This does not include the following:</p>
<ul>
<li> <p>Time logged on tasks and issues that are not assigned to any users. </p> </li>
<li> <p>Time logged on parent tasks. </p> </li>
</ul> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The time logged on all the tasks or issues assigned to the user in this role. </p> <p>This does not include the following:</p>
<ul>
<li>Time logged on tasks and issues assigned to this role but not to this user in this role.<em> </em></li>
<li>Time logged directly on the project or parent tasks. </li>
</ul> </td>
</tr>
<tr>
<td>Task or Issue </td>
<td> <p>The time logged on tasks and issues by the user who is also assigned to them. </p> </td>
</tr>
<tr>
<td colspan="2"> <p> <note type="important">
The time logged is displayed in the timeframe corresponding to the Entry Date of the hour entry, regardless of the timeframe of the task, issue, or project where the hours are logged.
</note> </p> <p>For more information about Actual Hours, see <a href="../../manage-work/tasks/task-information/actual-hours.md" class="MCXref xref">View Actual Hours</a></p> </td>
</tr>
<tr>
<td rowspan="4">DIF <br>(Hour or FTE Difference) <br><br></td>
<td>User</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the user. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <note type="note">
If the value displays in negative red numbers, the user is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the job role. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <note type="note">
If the value is displayed in negative red numbers, the role is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td rowspan="5">Planned Hours or FTE Allocation Percentage (%)</td>
<td>User</td>
<td> <p>The allocation of the Planned Hours or FTE as a percentage of the Available Hours. The percentage of the Planned Hours Allocation is calculated using the following formula:</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>The same calculation is used for FTE values. </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the <strong>View by User</strong> view to the Resource Planner.</td>
</tr>
<tr>
<td>Role</td>
<td> The allocation of the Planned Hours or FTE as a percentage of the Available Hours. <p>The percentage of the Planned Hours Allocation is calculated using the following formula:</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>The same calculation is used for FTE values.</p></td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td colspan="2"> <p> If the value of the Planned Hours or FTE is zero, the Percentage Allocation is 0%. If the value of the Available Hours or FTE is zero, the Percentage Allocation cannot be calculated. </p> <p>For more information about Planned Hours and FTE and how they are displayed in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>. </p> </td>
</tr>
</tbody>
</table>
-->
