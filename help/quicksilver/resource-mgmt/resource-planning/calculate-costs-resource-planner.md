---
product-area: resource-management
navigation-topic: resource-planning
title: Kosten im Ressourcenplaner berechnen
description: Sie können Ihre Ressourcen im Adobe Workfront-Ressourcenplaner budgetieren, indem Sie Kostenwerte anstelle von Stunden- oder FTE-Werten verwenden. Kostenwerte sind für die Ansicht **Nach Benutzer anzeigen** im Ressourcenplaner nicht verfügbar.
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

Sie können Ihre Ressourcen im Adobe Workfront-Ressourcenplaner budgetieren, indem Sie Kostenwerte anstelle von Stunden- oder FTE-Werten verwenden. Kostenwerte sind für die Ansicht &quot;**nach Benutzer“** Ressourcenplaner nicht verfügbar.

>[!IMPORTANT]
>
>Sie müssen Benutzer und Aufgabengebiete mit Kosten pro Stunde verknüpfen, um Kosteninformationen im Ressourcenplaner anzeigen zu können.\
>Weitere Informationen zum Verknüpfen der Stundensätze für Kosten pro Stunde mit Aufgabengebieten finden Sie unter [Erstellen und Verwalten von Aufgabengebieten](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
>Weitere Informationen zum Verknüpfen von Stundensätzen mit Benutzern finden Sie unter [Benutzerprofil bearbeiten](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Stellen Sie vor der Budgetierung Ihrer Ressourcen sicher, dass Sie ein gutes Verständnis davon haben, welche Arbeit erledigt werden muss (geplante Stunden, FTE oder Kosten) und zu welcher Zeit Ihre Benutzer für die Arbeit offen sind (verfügbare Stunden, FTE oder Kosten).\
Weitere Informationen zum Verständnis der Informationen im Ressourcenplaner bei der Budgetierung nach Stunden oder FTE finden Sie unter [Übersicht über Stunden, FTE und Kosteninformationen in den Projekt- und Rollenansichten des Ressourcenplaners](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
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
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf das Ressourcenmanagement bearbeiten, der den Zugriff auf die Bearbeitung von Prioritäten und Budgetstunden im Ressourcenplaner beinhaltet</p> <p>Zugriff auf Finanzdaten, Projekte und Benutzer bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten Sie Berechtigungen für die Projekte, für die Sie Informationen budgetieren möchten, mit der Möglichkeit, Finanzen zu verwalten.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Informationen im Ressourcenplaner nach Kosten anzeigen

Standardmäßig werden die Verfügbarkeits- und Zuordnungsinformationen im Ressourcenplaner in Stunden angezeigt.

So zeigen Sie verfügbare, geplante und budgetierte Informationen nach Kosten im Ressourcenplaner an:

{{step1-to-resourcing}}

1. Wechseln Sie zum Ressourcenplaner.
1. (Bedingt) Wählen Sie **Nach Projekt anzeigen** oder **Nach Rolle anzeigen** aus.\
   Standardmäßig ist **Nach Projekt anzeigen** ausgewählt.\
   Die Informationen zu Zuordnung und Verfügbarkeit werden in Stunden angezeigt.

1. Wählen Sie **Dropdown** Menü „Stunden“ die Option **Kosten**.

   Wenn Sie auf Ihrer Zugriffsebene keinen Zugriff auf Finanzdaten haben, ist diese Option nicht verfügbar.\
   Wenn Projekte eine andere Währung als die Systemwährung haben, werden die Kosten für diese Projekte im Ressourcenplaner in die Systemwährung umgerechnet angezeigt. Ihr Systemadministrator definiert die Systemwährung.\
   Weitere Informationen zum Einrichten der Systemwährung in Workfront und zu Konversionskursen finden Sie unter [Einrichten von Wechselkursen](../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).\
   ![cost_in_the_planner_with_no_budgeting.png](assets/costs-in-the-planner-with-no-budgeting-350x240.png)

## Verfügbare Kosten im Ressourcenplaner berechnen

Um verfügbare Kostenwerte im Ressourcenplaner anzuzeigen, benötigen Sie Folgendes:

* Kosten pro Stunde für die Benutzer und Rollen
* Informationen zur Benutzerverfügbarkeit.

  Das Erhalten von Informationen zur Benutzerverfügbarkeit hängt davon ab, wie der Workfront-Administrator die Voreinstellungen für die Ressourcenverwaltung konfiguriert.\
  Weitere Informationen zum Berechnen der Benutzerverfügbarkeit und Festlegen der Voreinstellungen für die Ressourcenverwaltung finden Sie [Konfigurieren der Voreinstellungen für die &#x200B;](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)&quot;.

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
   <td>Verfügbare Kosten des Benutzers</td> 
   <td> <p>Die verfügbaren Kosten pro Benutzer werden anhand der folgenden Formel berechnet:</p> <p><code>Available User Cost = User Available Hours * User Cost per Hour Rate</code> </p> <p><b>NOTIZ</b>

Wenn der/die Benutzende keinen Stundensatz „Kosten pro Stunde“ in seinem/ihrem Profil hat, wird der Stundensatz „Kosten pro Stunde“ des Aufgabengebiets, in dem er/sie aufgeführt ist, in der Berechnung verwendet. Wenn dem Benutzer keine Rolle zugeordnet ist, betragen die verfügbaren Benutzerkosten 0 $. </p> </td>
</tr> 
  <tr> 
   <td>Verfügbare Kosten der Funktion</td> 
   <td> <p>Die verfügbaren Kosten pro Funktion werden anhand der folgenden Formel berechnet:</p> <p><code>Available Role Cost = Role Available Hours * Role Cost per Hour Rate</code> </p> <p><b>NOTIZ</b>

Wenn für das Aufgabengebiet kein Stundensatz „Kosten pro Stunde“ festgelegt wurde, betragen die Kosten für das verfügbare Aufgabengebiet 0 USD.</p> </td>
</tr> 
  <tr> 
   <td>Projektkosten</td> 
   <td> <p>Die verfügbaren Kosten pro Projekt werden anhand der folgenden Formel berechnet:</p> <p><code>Available Project Cost = SUM(User Available Hours * User Cost per Hour Rate)</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Geplante Kosten im Ressourcenplaner berechnen

Obwohl Sie keine Aufgabeninformationen im Ressourcenplaner anzeigen können, werden die geplanten Kosten für Benutzer, Funktionen und die Projekte unter Berücksichtigung der folgenden Aufgabeninformationen berechnet:

* Der Typ der Zuweisung für die Aufgabe.\
  Sie können die Zuweisung einer Aufgabe aufheben oder die folgenden Entitäten einer Aufgabe zuweisen:

   * Ein Benutzer (mit oder ohne Aufgabengebiet)
   * Eine Rolle
   * Ein Team\
     Eine einem Team zugewiesene Aufgabe gilt aus Sicht des Ressourcenplaners als nicht zugewiesen.

* Der **Kostentyp** der Aufgaben im Projekt.\
  Weitere Informationen zum Kostentyp einer Aufgabe finden Sie unter [Kosten nachverfolgen](../../manage-work/projects/project-finances/track-costs.md).

* Die Gültigkeitsdaten der Kostensätze für Aufgabengebiete und Benutzer.

  Wenn beispielsweise die Funktion oder der Benutzer im Februar 10 geplante Stunden und im März 10 geplante Stunden hat, der Kostensatz sich jedoch von 12 auf 20 Dollar im März geändert hat, beträgt der Wert für die geplanten Kosten im Februar 120 Dollar und im März 200 Dollar.

>[!NOTE]
>
>Die geplanten Kosten des Benutzers haben keinen Einfluss auf die geplanten Projektkosten. Nur die geplanten Kosten der Funktion wirken sich auf die geplanten Projektkosten im Ressourcenplaner aus.

Bei der Berechnung der geplanten Kosten für Benutzer, Funktionen und das Projekt gibt es die folgenden Szenarien:

* Wenn der **Kostentyp** „Benutzer pro Stunde **&#x200B; lautet &#x200B;** und es **„keine Zuweisung** für die Aufgabe gibt:

   * **Geplante Kosten für Funktion und Benutzer**:

     Die geplanten Kosten für Rolle und Benutzer betragen 0,00 $.

   * **Geplante Projektkosten**:

     Die geplanten Projektkosten betragen 0,00 $.

* Wenn der **Kostentyp** &quot;**pro**&quot; lautet und eine **Benutzerzuweisung** auf der Aufgabe vorhanden ist:

   * **Geplante Kosten für Funktion und Benutzer**:

     Die geplanten Kosten für den Benutzer werden anhand der folgenden Formel berechnet:

     `User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate`

     Wenn ein(e) Benutzende(r) einen Kostensatz in seinem Profil hat, wird dieser Satz zur Berechnung der geplanten Kosten verwendet. Andernfalls wird der Kostensatz pro Stunde auf Systemebene für die Primäre Funktion verwendet.

     >[!NOTE]
     >
     >Der Benutzer kann der Aufgabe mit einem seiner sekundären Aufgabengebiete zugewiesen werden, hier wird jedoch stattdessen die Rate des primären Aufgabengebiets verwendet.

     Die geplanten Kosten für die Funktion werden anhand der folgenden Formel berechnet:

     `Role Planned Cost = SUM(User Planned Cost)`

   * **Geplante Projektkosten**:

     Die geplanten Projektkosten betragen 0,00 $.

* Wenn der **Kostentyp** &quot;**pro**&quot; lautet und eine **Aufgabenrollenzuweisung** auf der Aufgabe vorhanden ist:

   * **Geplante Kosten für Funktion und Benutzer**:

     Die geplanten Kosten für den Benutzer betragen 0,00 $.

     Die geplanten Kosten für die Funktion werden anhand der folgenden Formel berechnet:

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     Die Kosten pro Stunde auf Systemebene des Aufgabengebiets, das der Aufgabe zugewiesen wurde, wird zur Berechnung der geplanten Kosten verwendet.

   * **Geplante Projektkosten**:

     Die geplanten Projektkosten betragen 0,00 $.

* Wenn der **Kostentyp** „Funktion **/Stündlich** lautet und **keine Zuweisung** auf der Aufgabe vorhanden ist:

   * **Geplante Kosten für Funktion und Benutzer**:

     Die geplanten Kosten für Rolle und Benutzer betragen 0,00 $.

   * **Geplante Projektkosten**:

     Die geplanten Projektkosten betragen 0,00 $.

* Wenn der **Kostentyp** &quot;**pro Stunde“** und eine **Benutzerzuweisung** für die Aufgabe vorhanden ist:

   * **Geplante Kosten für Funktion und Benutzer**:

     Die geplanten Kosten für den Benutzer betragen 0,00 $.

     Die geplanten Kosten für die Funktion werden nach folgender Formel berechnet:

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     Workfront ermittelt anhand des Aufgabengebiets, das der Benutzer für die Aufgabe erfüllt, die geplanten Kosten für die Funktion.

     Wenn der/die Benutzende mit keiner Funktion in der Aufgabe verknüpft ist, betragen die geplanten Kosten 0,00 $.

   * **Geplante Projektkosten**:

     Die geplanten Projektkosten werden nach folgender Formel berechnet:

     `Project Planned Cost = SUM(Role Planned Costs)`

* Wenn der **Kostentyp** „Funktion **/Stündlich** lautet und eine **Aufgabenrollenzuweisung** auf der Aufgabe vorhanden ist:

   * **Geplante Kosten für Funktion und Benutzer**:

     Die geplanten Kosten für den Benutzer betragen 0,00 $.

     Die geplanten Kosten für die Funktion werden nach folgender Formel berechnet:

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     Workfront ermittelt anhand des Aufgabengebiets, das der Benutzer für die Aufgabe erfüllt, die geplanten Kosten für die Funktion.

   * **Geplante Projektkosten**:

     Die geplanten Projektkosten werden nach folgender Formel berechnet:

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

## Budgetierte Kosten im Ressourcenplaner berechnen

Um budgetierte Kostenwerte im Ressourcenplaner anzuzeigen, benötigen Sie Folgendes:

* Budgetierte Stunden für Funktionen, Benutzer und Projekte.
* Kosten pro Stunde für Benutzer und Rollen.

>[!NOTE]
>
>Die budgetierten Stunden für die Projekte werden auf der Grundlage der budgetierten Stunden für die Funktionen berechnet, nicht basierend auf den budgetierten Stunden der Benutzer.

Die folgende Tabelle zeigt, wie budgetierte Kosten im Ressourcenplaner berechnet werden:

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
   <td>Vom Benutzer budgetierte Kosten</td> 
   <td> <p>Die budgetierten Kosten pro Benutzer werden anhand der folgenden Formel berechnet:</p> <p><code>Budgeted User Cost = User Budgeted Hours * User Cost per Hour Rate</code> </p> <p> <p><b>NOTIZ</b>

Wenn der/die Benutzende keinen Stundensatz in seinem/ihrem Profil hat, betragen die budgetierten Benutzerkosten 0,00 USD.</p> </p> </td>
</tr> 
  <tr> 
   <td>Budgetierte Kosten der Funktion</td> 
   <td> <p>Die in der Funktion budgetierten Kosten werden anhand der folgenden Formel berechnet:</p> <p><code>Role Budgeted Cost = Role Budgeted Hours * Role Cost per Hour Rate</code> </p> <p> <p><b>NOTIZ</b>

Wenn für die Funktion kein Stundensatz „Kosten pro Stunde“ festgelegt wurde, betragen die budgetierten Kosten der Funktion 0,00 US-Dollar.</p> </p> </td>
</tr> 
  <tr> 
   <td>Budgetierte Projektkosten</td> 
   <td> <p>Die budgetierten Kosten pro Projekt werden anhand der folgenden Formel berechnet:</p> <p><code>Project Budgeted Cost = SUM(Role Budgeted Cost). </code> </p> </td> 
  </tr> 
 </tbody> 
</table>
