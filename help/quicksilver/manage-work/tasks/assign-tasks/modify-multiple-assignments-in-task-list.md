---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Mehrere Benutzerzuweisungen in einer Aufgabenliste ändern
description: Beim Verwalten von Aufgabenzuweisungen können Sie diese gleichzeitig für mehrere Aufgaben ändern, indem Sie die Massenbearbeitungsfunktion in einer Liste von Aufgaben verwenden.
author: Lisa
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 259fd0e3fdaa07bfdb0301d60bf0d9b1090b4ef7
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 0%

---

# Mehrere Benutzerzuweisungen in einer Aufgabenliste ändern

<!--Audited: 07/2024-->

<!--
<p>There is a similar article in Resource Scheduling and a similar one for Issues; when things change, you might need to update all 3</p>
-->

Beim Verwalten von Aufgabenzuweisungen können Sie diese gleichzeitig für mehrere Aufgaben ändern, indem Sie die Massenbearbeitungsfunktion in einer Liste von Aufgaben verwenden.

Dieser Artikel bezieht sich auf das Ändern mehrerer Benutzerzuweisungen für mehrere Aufgaben in einer Aufgabenliste. In den folgenden Artikeln finden Sie auch Informationen zum Ändern von Zuweisungen für mehrere Aufgaben in anderen Bereichen:

* Informationen zum Zuweisen von Aufgaben mit dem Workload Balancer finden Sie unter [Übersicht über das Zuweisen von Arbeit im Workload Balancer](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Informationen zum Zuweisen einer Aufgabe zu einer Ressource in einer Liste finden Sie unter [Aufgaben zuweisen](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neu: Standard</p>
   <p>Aktuell: Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte und Aufgaben bearbeiten</p> <p>Anzeigen von oder höherem Zugriff auf Benutzer</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Contribute oder höhere Berechtigungen für Aufgaben</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on tasks</h2>
<p>(NOTE: moved to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>You might want to modify the user assignments for multiple tasks for a variety of reasons, including the following:</p>
<ul>
<li>Users join or leave your team</li>
<li> <p>A user takes a vacation that extends beyond task due dates</p> <note type="note">
When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks. For information about schedules, see
<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.
</note> </li>
<li>A specific role or user is set as the assignee for multiple tasks and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
<p><strong>How removing assignees affects task hours and allocation percentages</strong></p>
<p>(NOTE: move to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration Types:</p>
<ul>
<li> <p><strong>Simple:</strong> The planned hours assigned to that user are subtracted from the task's total planned hours.</p> <note type="important">
<span class="s1">This could negatively affect your project plan because it changes the total planned hours for the task and the project.</span>
</note> </li>
<li><span class="s1"><strong>Effort Driven:</strong> The allocation percentage does not change for other users.</span> </li>
<li><span class="s1"><strong>Calculated Assignment:</strong> The allocation percentages of other users are adjusted so that the total equals 100%.</span> </li>
<li><span class="s1"><strong>Calculated Work:</strong> The allocation percentage does not change for other users.</span> </li>
</ul>
</div>
-->

## Zuweisungen für mehrere Aufgaben ändern

1. Navigieren Sie zur Liste mit den Aufgaben, für die Sie Zuweisungen ändern möchten.
1. (Optional) Erstellen Sie einen Filter, um nur Aufgaben anzuzeigen, die dem Verantwortlichen zugewiesen sind, den Sie ändern möchten.

   Wenn Ihr Projekt beispielsweise eine bestimmte Rolle als standardmäßigen Bearbeiter für mehrere Aufgaben enthält, können Sie einen Filter erstellen, um nur Aufgaben mit dieser Rolle als Beauftragten anzuzeigen. Anschließend können Sie die Rolle durch einen bestimmten Benutzer ersetzen.

   Informationen zum Erstellen eines Filters finden Sie unter [Filter erstellen oder bearbeiten](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).


1. Um nach einer Rolle zu filtern, wählen Sie **Arbeitsauftrag - Rollen** und klicken Sie dann auf **ID**.

   >[!TIP]
   >
   >Verwenden Sie nicht das Feld **Zugewiesen an**. Dadurch wird nur der Primäre Verantwortliche für die Aufgabe gefunden, nicht aber für die ihnen zuweisbaren Rollen.

   Oder

   Um nach einem Benutzer zu filtern, wählen Sie **Arbeitsauftrag - Benutzer** und klicken Sie dann auf **ID.**

   >[!TIP]
   >
   >Verwenden Sie nicht das Feld **Zugewiesen an**. Dadurch wird nur der Primäre Verantwortliche für die Aufgabe gefunden, nicht aber einer der Benutzenden, die ihnen zugewiesen werden könnten.

1. Wählen Sie die Aufgaben aus, für die Sie Zuweisungen ändern möchten, und klicken Sie dann auf das **Bearbeiten**-Symbol ![](assets/edit-icon.png).

   Die Seite Aufgaben bearbeiten wird angezeigt. Die Elemente, die Sie bearbeiten, werden in der oberen linken Ecke der Seite angezeigt.

1. Navigieren Sie zum Abschnitt **Arbeitsaufträge** .
1. Führen Sie einen der folgenden Schritte aus, um Verantwortliche hinzuzufügen oder zu entfernen:

   >[!IMPORTANT]
   >
   >Das Entfernen von Zugewiesenen kann sich auf die Aufgabenstunden und die Zuordnungsprozentsätze auswirken. Weitere Informationen finden Sie im Abschnitt [Wie sich das Entfernen von Verantwortlichen auf die Aufgabenstunden und Zuordnungsprozentsätze auswirkt](#how-removing-assignees-affects-task-hours-and-allocation-percentages) in diesem Artikel.

   * So fügen Sie einen neuen Bevollmächtigten hinzu:

      1. Wählen Sie **Abschnitt** Arbeitsaufträge“ **Verantwortlicher** aus.

         Es werden Informationen angezeigt, die für alle ausgewählten Aufgaben gelten. Wenn beispielsweise allen Aufgaben derselbe Benutzer zugewiesen ist, wird dieser Benutzer in der Spalte &quot;**&quot;**. Wenn die Informationen für die ausgewählten Aufgaben nicht gleich sind, werden keine Informationen angezeigt.

      1. Beginnen Sie mit der Eingabe des Namens eines Benutzers, einer Rolle oder eines Teams und wählen Sie ihn aus, wenn er/sie in der Liste angezeigt wird. Die Zuweisung wird hinzugefügt und ersetzt nicht die aktuellen Zuweisungen für die ausgewählten Aufgaben.


     >[!TIP]
     >
     > * Sie können mehrere Benutzer, Aufgabengebiete oder Teams zuweisen. Sie können nur aktive Benutzer, Aufgabengebiete und Teams zuweisen.
     >   
     > * Beachten Sie beim Hinzufügen einer Benutzerzuweisung den Avatar, die Primäre Rolle des Benutzers oder seine E-Mail-Adresse, um zwischen Benutzern mit identischen Namen zu unterscheiden. Benutzende müssen mindestens einem Aufgabengebiet zugeordnet sein, damit sie es beim Hinzufügen anzeigen können. Die Einstellung Kontaktinformationen anzeigen muss in Ihrer Zugriffsebene aktiviert sein, damit Benutzer die E-Mails von Benutzern anzeigen können. Weitere Informationen finden Sie unter [Gewähren des Benutzerzugriffs](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
     > 
     >   Wenn ein(e) Benutzende(r), ein Aufgabengebiet oder ein Team zugewiesen wurde, bevor sie/er deaktiviert wurden, bleiben sie/sie dem Arbeitselement zugewiesen. In diesem Fall empfehlen wir Folgendes:
     >   
     >     * Weisen Sie das Arbeitselement den aktiven Ressourcen neu zu.
     >     * Verknüpfen Sie die Benutzer in einem deaktivierten Team mit einem aktiven Team und weisen Sie das Arbeitselement dem aktiven Team zu.


   * So entfernen Sie einzelne Zugewiesene:

      1. Klicken Sie auf das **X**-Symbol neben dem Namen des Verantwortlichen, den Sie entfernen möchten, wenn der Verantwortliche in der Zuweisungsliste angezeigt wird.

         Oder

         (Bedingt) Wenn der Verantwortliche, den Sie entfernen möchten, nicht im Abschnitt Zuweisungen angezeigt wird, da der Verantwortliche nur einigen der ausgewählten Aufgaben zugewiesen ist, klicken Sie auf **Verantwortlichen entfernen** und geben Sie den Namen des Verantwortlichen ein, den Sie entfernen möchten. Klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.

   * So entfernen Sie alle vorhandenen Zugewiesenen:

      1. Klicken Sie **Alle vorhandenen Bevollmächtigten entfernen** und klicken Sie dann auf **Ja, Alle Bevollmächtigten löschen**.

         Dadurch werden nicht nur die allgemeinen Bevollmächtigten (Bevollmächtigte, die im Dialogfeld „Bearbeiten“ angezeigt werden) entfernt, sondern auch alle Bevollmächtigten für alle ausgewählten Aufgaben.

     Das Entfernen von Benutzern aus Aufgaben kann sich auf die Aufgabenstunden und Zuordnungsprozentsätze auswirken.

     Weitere Informationen finden Sie unter [Übersicht über das Ändern von ](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)).

1. (Optional) Ändern Sie eine der folgenden Optionen für Verantwortliche:

   * (Bedingt) **Zuordnung % oder Stunden**: Geben Sie einen neuen Zuordnungsprozentsatz oder neue Stunden an.

     >[!NOTE]
     >
     >Diese Option kann nur geändert werden, wenn der Dauertyp für alle Aufgaben, die bearbeitet werden, gleich ist. Wenn als Dauertyp „Berechnete Arbeit“ oder „Leistungsgesteuert“ festgelegt ist, können Sie die Zuordnung % aktualisieren. Wenn der Dauertyp „Einfach“ ist, können Sie die Stunden aktualisieren. Informationen zum Dauertyp finden Sie unter [Übersicht über die Aufgabendauer und den Dauertyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
     >
     >
     >Wenn das Feld leer ist, bedeutet dies, dass der Wert in allen Aufgaben unterschiedlich ist. Sie können ihn jedoch weiterhin ändern.

   * **Aufgabenbesitzer**: Wählen Sie diese Option aus, um den Verantwortlichen zum Besitzer der Aufgabe für alle bearbeiteten Aufgaben zu machen.
   * **Rolle des Verantwortlichen**: Wählen Sie eine Rolle aus der Dropdown-Liste aus. Wenn die Option deaktiviert bleibt, wählt Adobe Workfront automatisch die Primäre Rolle des Benutzers aus.

1. Klicken Sie **Änderungen speichern.**
