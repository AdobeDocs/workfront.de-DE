---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Geplantes Abschlussdatum für das Projekt festlegen
description: Das geplante Abschlussdatum eines Projekts ist das Datum, bis zu dem das Projekt abgeschlossen sein soll.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 996398c5-de92-445e-8e86-36b2efdcf6b5
source-git-commit: fedb0328450896d212081715df4cde7644b169bc
workflow-type: tm+mt
source-wordcount: '591'
ht-degree: 1%

---

# Geplantes Abschlussdatum für das Projekt festlegen

<!-- Audited: 4/2025 -->

Das geplante Abschlussdatum eines Projekts ist das Datum, an dem das Projekt abgeschlossen werden soll.

Der geplante Start und die geplanten Abschlussdaten eines Projekts hängen von den Daten der Aufgaben im Projekt ab. Dieser Artikel beschreibt, wie Sie das geplante Abschlussdatum eines Projekts manuell oder automatisch festlegen können. Weitere Informationen zum geplanten Abschlussdatum einer Aufgabe finden Sie unter [Übersicht über das geplante Abschlussdatum der Aufgabe](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

Das geplante Abschlussdatum eines Projekts kann manuell oder automatisch festgelegt werden, je nachdem, ob Sie das Projekt vom Start- oder vom Abschlussdatum aus planen.

## Zugriffsanforderungen

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>
   Neu: Standard

Oder

Aktuell: Plan </p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für das Projekt</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Manuelles Festlegen des geplanten Abschlussdatums eines Projekts

Sie müssen das geplante Abschlussdatum eines Projekts manuell festlegen, wenn Sie das Projekt ab dem Abschlussdatum planen.

>[!NOTE]
>
>Wenn Sie das geplante Abschlussdatum eines Projekts manuell festlegen, berechnet Workfront automatisch das geplante Startdatum des Projekts auf der Grundlage der Dauer aller Aufgaben.


So planen Sie ein Projekt ab dem Abschlussdatum:

{{step1-to-projects}}

1. Klicken Sie auf **Neues Projekt** und wählen Sie dann **Neues Projekt** aus der angezeigten Dropdown-Liste aus.

   Weitere Informationen zum Erstellen von Projekten finden Sie im Artikel [Erstellen eines Projekts](../../../manage-work/projects/create-projects/create-project.md).

1. Wählen **Projektdetails** im linken Bedienfeld aus.

1. Klicken Sie auf **Projekt bearbeiten**-Symbol ![Bearbeiten](/help/quicksilver/manage-work/projects/planning-a-project/assets/qs-edit-icon.png) in der oberen rechten Ecke und wählen Sie dann **Übersicht** in der angezeigten Dropdown-Liste aus.

1. Klicken Sie **Abschnitt** Projektdaten“ auf das Feld **Planungsmodus** und wählen Sie dann **Abschlussdatum**.

1. Geben Sie **„Geplantes Abschlussdatum** des Projekts an.
1. Klicken Sie auf **Änderungen speichern**.

   Wenn Sie beginnen, Ihrem Projekt Aufgaben hinzuzufügen, wird **„Geplantes Startdatum** des Projekts auf der Grundlage der Gesamtdauer aller Aufgaben berechnet. 

## Automatisches Festlegen des geplanten Abschlussdatums eines Projekts

Das geplante Abschlussdatum eines Projekts wird automatisch von Workfront berechnet, wenn Sie das Projekt ab dem Startdatum planen. 

So planen Sie ein Projekt ab dem Startdatum:

{{step1-to-projects}}

1. Klicken Sie auf **Neues Projekt** und wählen Sie dann **Neues Projekt** aus der angezeigten Dropdown-Liste aus.

   Weitere Informationen zum Erstellen von Projekten finden Sie im Artikel [Erstellen eines Projekts](../../../manage-work/projects/create-projects/create-project.md).

1. Wählen **Projektdetails** im linken Bedienfeld aus.

1. Klicken Sie auf **Projekt bearbeiten**-Symbol ![Bearbeiten](/help/quicksilver/manage-work/projects/planning-a-project/assets/qs-edit-icon.png) in der oberen rechten Ecke und wählen Sie dann **Übersicht** in der angezeigten Dropdown-Liste aus.

1. Klicken Sie **Abschnitt** Projektdaten“ auf das Feld **Planungsmodus** und wählen Sie dann **Startdatum**.

1. Geben Sie **„Geplantes Startdatum** des Projekts an.
1. Klicken Sie auf **Änderungen speichern**.

   Wenn Sie beginnen, Ihrem Projekt Aufgaben hinzuzufügen, wird **Geplantes Abschlussdatum** des Projekts auf der Grundlage der Gesamtdauer aller Aufgaben berechnet. 

   Weitere Informationen zur Aufgabendauer finden Sie im Artikel [Übersicht über die Aufgabendauer und den ](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)).

   Das geplante Abschlussdatum des Projekts fällt in diesem Fall mit dem geplanten Abschlussdatum der letzten Aufgabe im Projekt zusammen.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>The Planned Completion Date of a task</h2>
<p>(NOTE: drafted because I created a new article, here: /Content/Manage work/Tasks/Task information/task-planned-completion-date.htm)</p>
<p>You can either specify the Planned Completion Date of a task, or you can leave it up to Workfront to calculate it depending on certain criteria.&nbsp;</p>
<ul>
<li><a href="#manually-set-the-planned-completion-date-of-a-task" class="MCXref xref">Manually set the Planned Completion Date of a task</a> </li>
<li><a href="#how-the-planned-completion-date-is-calculated-for-a-task" class="MCXref xref">How the Planned Completion Date is calculated for a task</a> </li>
</ul>
<p><strong>Manually set the Planned Completion Date of a task</strong></p>
<p>Setting the Planned Completion Date of a task depends on the type of Task Constraint you assign to the task.&nbsp;</p>
<p>You can manually set the Planned Completion Date&nbsp;when creating a task, as described in&nbsp;the article <a href="../../../manage-work/tasks/create-tasks/create-tasks-in-project.md" class="MCXref xref">Create tasks in a project</a>.</p>
<p>You can manually specify the Planned Completion Date when you select any of the following Task Constraints:&nbsp;</p>
<table border="1" cellspacing="15" cellpadding="1">
<col>
<col>
<thead>
<tr>
<th> <p><strong>Task Constraint Type</strong> </p> </th>
<th> <p><strong>Effect of Manually Changing the Planned Completion Date</strong> </p> </th>
</tr>
</thead>
<tbody>
<tr>
<td> <p>Must Finish On</p> <p>Finish No Later Than</p> <p>Finish No Earlier Than</p> </td>
<td> <p><span class="s1">The Planned Start Date is adjusted in order to keep the Duration the same.</span> </p> </td>
</tr>
<tr>
<td> <p>Fixed Dates</p> </td>
<td> <p>The Duration is adjusted in order to keep the Planned Start Date the same.</p> </td>
</tr>
</tbody>
</table>
<p><strong>How the Planned Completion Date is calculated for a task</strong></p>
<p>When it is calculated automatically by the system, the following can influence the Planned Completion Date of a Task:</p>
<ul>
<li> <p>Task Constraint</p> <p>For more information about Task Constraints, see the article <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>.</p> </li>
<li> <p>Task predecessor relationship</p> <p>For more information about task predecessors, see the article <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p> </li>
<li>Project Completion Date, when the project is scheduled from Completion Date.</li>
<li> <p>The time off schedule of the Primary&nbsp;Assignee of the task. </p> <p>When the Primary Assignee has time off scheduled during the duration of the task, the planned dates of the task adjust accordingly when the <strong>Consider user time off in task durations</strong> setting is selected for the <strong>User Time Off</strong> field. New projects inherit this setting from the Project&nbsp;Preferences area, but you can edit the setting at the project level. </p> <p>For example, if a task with a Constraint of As Soon As Possible is scheduled to start on June 1 and complete on June 3, and the Primary Assignee has June 2 marked for Time-off, the task Planned Completion Date becomes June 4. </p> <p>For information about the <strong>User Time Off</strong> preference, see the articles <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a> or <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p> </li>
</ul>
<p>When set automatically, the Planned Completion Date&nbsp;is determined based on the following calculation:&nbsp;</p>
<p><code>Planned Completion Date = Planned Start Date + Duration</code> </p>
<p>For example, if your task has a start date of September 16 and a duration of 10 days, the Planned Completion Date is September 26.</p> <note type="note">
&nbsp;The Update Type for the project must also be&nbsp;set to Automatic and On Change or Automatically in order for the Planned Hours and Duration to be automatically&nbsp;adjusted.
<br>For more information about the Update Type, see the article
<a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.
</note>
</div>
-->
