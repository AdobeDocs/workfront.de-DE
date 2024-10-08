---
product-area: resource-management
navigation-topic: resource-planning
title: Berechnen der Kosten im Ressourcenplaner
description: Sie können Ihre Ressourcen im Adobe Workfront Resource Planer mit Kostenwerten anstelle von Stunden- oder FTE-Werten einsetzen. Kostenwerte sind nicht für die Ansicht "Nach Benutzer anzeigen"im Ressourcenplaner verfügbar.
author: Lisa
feature: Resource Management
exl-id: 2f3ca8c2-51b3-4282-af8b-7f433365d386
source-git-commit: 3c3175c347431b10aed1a6034df6c756056399b3
workflow-type: tm+mt
source-wordcount: '1421'
ht-degree: 0%

---

# Kosten im Ressourcenplaner berechnen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)</p>
-->

<!--'(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)'-->

Sie können Ihre Ressourcen im Adobe Workfront Resource Planer mit Kostenwerten anstelle von Stunden- oder FTE-Werten einsetzen. Kostenwerte sind nicht für die Ansicht **Nach Benutzer anzeigen** im Ressourcenplaner verfügbar.

>[!IMPORTANT]
>
>Sie müssen Benutzer und Stellenrollen mit den Kosten pro Stunde-Raten verknüpfen, um Kosteninformationen im Ressourcenplaner anzuzeigen.\
>Weitere Informationen zum Zuordnen der Kosten pro Stunde zu Auftragsrollen finden Sie unter [Erstellen und Verwalten von Auftragsrollen](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
>Weitere Informationen zum Zuordnen der Kosten pro Stunde zu Benutzern finden Sie unter [Profil eines Benutzers bearbeiten](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Bevor Sie Ihre Ressourcen in den Budgets einplanen, sollten Sie wissen, welche Aufgaben zu erledigen sind (geplante Stunden, FTE oder Kosten) und wann Ihre Benutzer zur Arbeit bereit sind (Verfügbare Stunden, FTE oder Kosten).\
Weitere Informationen zum Verständnis der Informationen im Ressourcenplaner bei der Budgetierung nach Stunden oder VZÄ finden Sie unter [Überblick über Stunden, VZÄ und Kosteninformationen in den Projekt- und Rollenansichten des Ressourcenplaners](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
    <td><p>Neu: Beliebig</p>
       <p>oder</p>
       <p>Aktuell: Pro oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>oder</p>
       <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Bearbeiten Sie den Zugriff auf das Ressourcen-Management, das Zugriff auf die Option "Prioritäten bearbeiten"und die Budgetzeiten im Ressourcenplaner enthält.</p> <p>Zugriff auf Finanzdaten, Projekte und Benutzer bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für die Projekte, für die Informationen zum Budget bereitgestellt werden sollen, mit der Möglichkeit, die Finanzen zu verwalten</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anzeigen von Informationen im Ressourcenplaner nach Kosten

Standardmäßig werden die Verfügbarkeits- und Zuordnungsinformationen in Stunden im Ressourcenplaner angezeigt.

So zeigen Sie verfügbare, geplante und budgetierte Informationen nach Kosten im Ressourcenplaner an:

{{step1-to-resourcing}}

1. Wechseln Sie zum Ressourcen-Planer.
1. (Bedingt) Wählen Sie **Nach Projekt anzeigen** oder **Nach Rolle anzeigen** aus.\
   Standardmäßig ist **Nach Projekt anzeigen** ausgewählt.\
   Die Informationen zur Zuordnung und Verfügbarkeit werden in Stunden angezeigt.

1. Wählen Sie aus dem Dropdownmenü **Stunden** die Option **Kosten** aus.

   Wenn Sie keinen Zugriff auf Finanzdaten in Ihrer Zugriffsebene haben, ist diese Option nicht verfügbar.\
   Wenn Projekte eine andere Währung als das System haben, werden die Kosten für diese Projekte im Ressourcenplaner angezeigt, der in die Währung des Systems konvertiert wurde. Ihr Systemadministrator definiert die Systemwährung.\
   Weitere Informationen zur Einrichtung der Systemwährung in Workfront und zu Konversionsraten finden Sie unter [Einrichten von Wechselkursen](../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).\
   ![cost_in_the_planner_with_no_budgeting.png](assets/costs-in-the-planner-with-no-budgeting-350x240.png)

## Verfügbare Kosten im Ressourcenplaner berechnen

Um die Werte der verfügbaren Kosten im Ressourcenplaner anzuzeigen, müssen Sie über Folgendes verfügen:

* Kosten pro Stunde für Benutzer und Rollen
* Informationen zur Benutzerverfügbarkeit.

  Das Ermitteln von Informationen zur Benutzerverfügbarkeit hängt davon ab, wie Ihr Workfront-Administrator die Voreinstellungen für die Ressourcenverwaltung konfiguriert.\
  Weitere Informationen zum Berechnen der Benutzerverfügbarkeit und Festlegen von Voreinstellungen für die Ressourcenverwaltung finden Sie unter [Voreinstellungen für die Ressourcenverwaltung konfigurieren](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

Die folgende Tabelle zeigt, wie die verfügbaren Kosten im Ressourcenplaner berechnet werden:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Verfügbare Kosten</strong> </th> 
   <th><strong>Berechnung</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Verfügbare Benutzerkosten</td> 
   <td> <p>Die verfügbaren Kosten pro Benutzer werden mit der folgenden Formel berechnet:</p> <p><code>Available User Cost = User Available Hours * User Cost per Hour Rate</code> </p> <p><b>NOTIZ</b>

Wenn der Benutzer in seinem Profil keine Kostensätze pro Stunde angibt, wird in der Berechnung der Kostensatz pro Stunde für die Rolle des Auftrags verwendet, unter der er aufgeführt ist. Wenn dem Benutzer keine Rolle zugeordnet ist, belaufen sich die verfügbaren Benutzerkosten auf 0 USD. </p> </td>
</tr> 
  <tr> 
   <td>Verfügbare Rollenkosten</td> 
   <td> <p>Die verfügbaren Kosten pro Rolle werden anhand der folgenden Formel berechnet:</p> <p><code>Available Role Cost = Role Available Hours * Role Cost per Hour Rate</code> </p> <p><b>NOTIZ</b>

Wenn die Rolle keine Kosten pro Stunde hat, beträgt die verfügbare Rollenkostenzahl 0 USD.</p> </td>
</tr> 
  <tr> 
   <td>Verfügbare Projektkosten</td> 
   <td> <p>Die pro Projekt verfügbaren Kosten werden mit der folgenden Formel berechnet:</p> <p><code>Available Project Cost = SUM(User Available Hours * User Cost per Hour Rate)</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Planete Kosten im Ressourcenplaner berechnen

Obwohl Sie Aufgabeninformationen nicht im Ressourcenplaner anzeigen können, werden die für Benutzer, Rollen und Projekte geplanten Kosten unter Berücksichtigung der folgenden Aufgabeninformationen berechnet:

* Der Typ der Zuweisung für die Aufgabe.\
  Sie können eine Aufgabe nicht zugewiesen lassen oder die folgenden Entitäten einer Aufgabe zuweisen:

   * Ein Benutzer (mit oder ohne Job-Rolle)
   * Eine Rolle
   * Ein Team\
     Eine einem Team zugewiesene Aufgabe wird aus der Sicht des Ressourcenplaners als nicht zugewiesen betrachtet.

* Der **Kostentyp** der Aufgaben im Projekt.\
  Weitere Informationen zum Kostentyp einer Aufgabe finden Sie unter [Kosten verfolgen](../../manage-work/projects/project-finances/track-costs.md).

* Die tatsächlichen Daten der Kostensätze für die Rollen und Benutzer im Auftrag.

  Wenn beispielsweise die Rolle oder der Benutzer im Februar 10 geplante Stunden und im März 10 geplante Stunden hat, sich der Kostensatz jedoch von 12 auf 20 USD im März geändert hat, beträgt der Wert für die geplanten Kosten im Februar 120 USD, im März beträgt der Wert für die geplanten Kosten 200 USD.

>[!NOTE]
>
>Benutzergeplante Kosten beeinflussen die geplanten Projektkosten nicht. Nur die Kosten der geplanten Rolle wirken sich auf die geplanten Kosten des Projekts im Ressourcenplaner aus.

Bei der Berechnung der geplanten Kosten für Benutzer, Rollen und das Projekt gibt es die folgenden Szenarien:

* Wenn der **Kostentyp** **Benutzer stündlich **ist und die Aufgabe **keine Zuweisung** enthält:

   * **Rolle und vom Benutzer geplante Kosten**:

     Die Kosten für Rolle und Anwender, die geplant sind, betragen 0,00 USD.

   * **Projektgeplante Kosten**:

     Die geplanten Projektkosten belaufen sich auf 0,00 USD.

* Wenn der **Kostentyp** **Benutzer stündlich** ist und eine **Benutzerzuweisung** für die Aufgabe vorhanden ist:

   * **Rolle und vom Benutzer geplante Kosten**:

     Die vom Benutzer geplanten Kosten werden mit der folgenden Formel berechnet:

     `User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate`

     Wenn ein Benutzer in seinem Profil einen Kostensatz hat, wird dieser Satz zur Berechnung der geplanten Kosten verwendet. Andernfalls werden die Kosten pro Stunde auf Systemebene der Primären Rolle verwendet.

     >[!NOTE]
     >
     >Der Benutzer kann der Aufgabe mit einer seiner sekundären Job-Rollen zugewiesen werden, aber hier wird die Rate der Rolle des Hauptauftrags verwendet.

     Die Berechnung der Plankosten für die Rolle erfolgt anhand der folgenden Formel:

     `Role Planned Cost = SUM(User Planned Cost)`

   * **Projektgeplante Kosten**:

     Die geplanten Projektkosten belaufen sich auf 0,00 USD.

* Wenn der **Kostentyp** **Benutzer stündlich** ist und die Aufgabe eine **Aufgabenrollenzuweisung** enthält:

   * **Rolle und vom Benutzer geplante Kosten**:

     Die vom Benutzer geplanten Kosten betragen 0,00 USD.

     Die Berechnung der Plankosten für die Rolle erfolgt anhand der folgenden Formel:

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     Die Kosten pro Stunde auf Systemebene der der Aufgabe zugewiesenen Auftragsrolle wird zur Berechnung der geplanten Kosten verwendet.

   * **Projektgeplante Kosten**:

     Die geplanten Projektkosten belaufen sich auf 0,00 USD.

* Wenn der **Kostentyp** **Rolle pro Stunde** ist und die Aufgabe **keine Zuweisung** enthält:

   * **Rolle und vom Benutzer geplante Kosten**:

     Die Kosten für Rolle und Anwender, die geplant sind, betragen 0,00 USD.

   * **Projektgeplante Kosten**:

     Die geplanten Projektkosten belaufen sich auf 0,00 USD.

* Wenn der **Kostentyp** **Stündliche Rolle** ist und eine **Benutzerzuweisung** für die Aufgabe vorhanden ist:

   * **Rolle und vom Benutzer geplante Kosten**:

     Die vom Benutzer geplanten Kosten betragen 0,00 USD.

     Die Berechnung der Plankosten für die Rolle erfolgt nach folgender Formel:

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     Workfront untersucht die Rolle, die der Benutzer bei der Berechnung der geplanten Kosten für die Rolle spielt.

     Wenn der Benutzer keiner Rolle für die Aufgabe zugeordnet ist, beträgt die Anzahl der geplanten Kosten 0,00 USD.

   * **Projektgeplante Kosten**:

     Die geplanten Projektkosten werden mit der folgenden Formel berechnet:

     `Project Planned Cost = SUM(Role Planned Costs)`

* Wenn der **Kostentyp** **Stündliche Rolle** ist und die Aufgabe eine **Aufgabenrollenzuweisung** enthält:

   * **Rolle und vom Benutzer geplante Kosten**:

     Die vom Benutzer geplanten Kosten betragen 0,00 USD.

     Die Berechnung der Plankosten für die Rolle erfolgt nach folgender Formel:

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     Workfront untersucht die Rolle, die der Benutzer bei der Berechnung der geplanten Kosten für die Rolle spielt.

   * **Projektgeplante Kosten**:

     Die geplanten Projektkosten werden mit der folgenden Formel berechnet:

     `Project Planned Cost = SUM(Role Planned Costs)`

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(table below ideal but drafted because it does not display correctly in Markdown)</p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<col>
<col>
<tbody>
<tr>
<td rowspan="2">&nbsp;</td>
<td colspan="3"> <p><strong>Cost Type = User Hourly</strong> </p><strong>User Planned Cost</strong> </td>
<td colspan="3"> <p><strong>Cost Type = Role Hourly</strong> </p><strong>Role Planned Cost</strong> </td>
</tr>
<tr>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
</tr>
<tr>
<td> <p><strong>User and Role Planned Cost</strong> </p> <p> </p> </td>
<td> <p>The Role and User Planned Costs are $0.00.</p> </td>
<td> <p> The User Planned Cost is calculated using the following formula: </p> <p><code> User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate </code> </p> <p> If a user has a cost rate in their profile, then that rate is used to calculate Planned Cost. Otherwise, the system-level Cost per Hour rate of their Primary Role is used. <br><note type="note">
The user can be assigned to the task with one of their secondary job roles, but the rate of the primary job role is used here instead.
</note></p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code>Role Planned Cost = SUM(User Planned Cost)</code> </p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code> Role Planned Cost = Role Planned Hours * Role Cost per Hours </code> </p> <p> The system-level Cost per Hour rate of the job role assigned to the task is used to calculate Planned Cost. </p> </td>
<td> <p>The Role and User Planned Costs are $0.00.</p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> If the user is not associated with any role on the task, the Planned Cost is $0.00. </p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> </p> <p> </p> </td>
</tr>
<tr>
<td rowspan="2"> <p><strong>Project Planned Cost</strong> </p> <p> </p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td colspan="2"> <p> The Project Planned Cost is calculated using the following formula: </p> <p><code> Project Planned Cost = SUM(Role Planned Costs) </code> </p> <p> </p> </td>
</tr>
<tr>
<td colspan="6"> <note type="note">
User Planned Costs do not influence the Project Planned Cost. Only the Role Planned costs affect the Project Planned Costs, in the Resource Planner.
</note> </td>
</tr>
</tbody>
</table>
-->

## Berechnung der budgetierten Kosten im Ressourcenplaner

Um im Ressourcenplaner budgetierte Kostenwerte anzuzeigen, müssen Sie über Folgendes verfügen:

* Budgetierte Stunden für Rollen, Benutzer und Projekte.
* Kosten pro Stunde für Benutzer und Rollen.

>[!NOTE]
>
>Die Budgetzeit für die Projekte wird auf der Grundlage der Budgetierten Stunden für die Rollen berechnet, nicht auf der Grundlage der Benutzerrollen.

Die folgende Tabelle zeigt, wie die Budgetierung von Kosten im Ressourcenplaner erfolgt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Budgetierte Kosten</strong> </th> 
   <th><strong>Berechnung</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Benutzerbudgetierte Kosten</td> 
   <td> <p>Die budgetierten Kosten pro Benutzer werden mit der folgenden Formel berechnet:</p> <p><code>Budgeted User Cost = User Budgeted Hours * User Cost per Hour Rate</code> </p> <p> <p><b>NOTIZ</b>

Wenn der Benutzer in seinem Profil keine Kosten pro Stunde angibt, beträgt die Budgetierung der Benutzerkosten 0,00 USD.</p> </p> </td>
</tr> 
  <tr> 
   <td>Geplante Kosten der Rolle</td> 
   <td> <p>Die Berechnung der Kosten für die Rolle wird mit der folgenden Formel vorgenommen:</p> <p><code>Role Budgeted Cost = Role Budgeted Hours * Role Cost per Hour Rate</code> </p> <p> <p><b>NOTIZ</b>

Wenn die Rolle keinen Kostensatz pro Stunde aufweist, betragen die Kosten für die geplante Rolle 0,00 USD.</p> </p> </td>
</tr> 
  <tr> 
   <td>Budgetierte Projektkosten</td> 
   <td> <p>Die budgetierten Kosten pro Projekt werden mit der folgenden Formel berechnet:</p> <p><code>Project Budgeted Cost = SUM(Role Budgeted Cost). </code> </p> </td> 
  </tr> 
 </tbody> 
</table>
