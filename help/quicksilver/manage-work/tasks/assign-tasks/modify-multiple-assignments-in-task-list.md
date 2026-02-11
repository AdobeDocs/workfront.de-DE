---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Ändern mehrerer Benutzerzuweisungen in einer Aufgabenliste
description: Beim Verwalten von Aufgabenzuweisungen können Sie diese gleichzeitig für mehrere Aufgaben ändern, indem Sie die Massenbearbeitungsfunktion in einer Liste von Aufgaben verwenden.
author: Lisa
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 21c98e443a6d6ca79045e2f4aba5f792340833cd
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 3%

---

# Mehrere Benutzerzuweisungen in einer Aufgabenliste ändern

<!--Audited: 11/2025-->

<!--remove the old/new experience references when the toggles are removed-->

<!--
this article is similar and updates on this one might need to be repeated here: help/quicksilver/manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md</p>
-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Second Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-release-overview.md).  

</div>-->

Beim Verwalten von Aufgabenzuweisungen können Sie diese gleichzeitig für mehrere Aufgaben ändern, indem Sie die Massenbearbeitungsfunktion in einer Liste von Aufgaben verwenden.

Dieser Artikel bezieht sich auf das Ändern mehrerer Benutzerzuweisungen für mehrere Aufgaben in einer Aufgabenliste. In den folgenden Artikeln finden Sie auch Informationen zum Ändern von Zuweisungen für mehrere Aufgaben in anderen Bereichen:

* Informationen zum Zuweisen von Aufgaben mit dem Workload Balancer finden Sie unter [Übersicht über das Zuweisen von Arbeit im Workload Balancer](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Informationen zum Zuweisen einer Aufgabe zu einer Ressource in einer Liste finden Sie unter [Aufgaben zuweisen](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p>
   <p>Work oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte und Aufgaben bearbeiten</p> <p>Anzeigen von oder höherem Zugriff auf Benutzer</p> </td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td>
   <td>Mitwirken an oder höhere Berechtigungen für die Aufgaben</td>
  </tr>
 </tbody>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

   ODER

   Um nach einem Benutzer zu filtern, wählen Sie **Arbeitsauftrag - Benutzer** und klicken Sie dann auf **ID.**

   >[!TIP]
   >
   >Verwenden Sie nicht das Feld **Zugewiesen an**. Dadurch wird nur der Primäre Verantwortliche für die Aufgabe gefunden, nicht aber einer der Benutzenden, die ihnen zugewiesen werden könnten.

1. Wählen Sie die Aufgaben aus, für die Sie Zuweisungen ändern möchten, und klicken Sie dann auf das **Bearbeiten**-Symbol ![Bearbeiten](assets/edit-icon.png).

   1. Um Verantwortliche hinzuzufügen oder zu entfernen, führen Sie einen der folgenden Schritte aus:

      * Um Verantwortliche hinzuzufügen, fangen Sie an, den Namen eines Verantwortlichen in das Feld **Personen, Rollen oder Teams suchen** einzugeben und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.

        Der neue Verantwortliche wird den vorhandenen Aufgaben in den ausgewählten Aufgaben hinzugefügt.
      * Um Verantwortliche zu entfernen, klicken Sie im Feld **Verantwortlichen entfernen** auf den Namen eines Verantwortlichen

        ODER

        Klicken Sie **Alle vorhandenen Zugewiesenen entfernen**.

        Bevollmächtigte werden aus allen ausgewählten Aufgaben entfernt.

        Das Entfernen von Benutzern aus Aufgaben kann sich auf die Aufgabenstunden und Zuordnungsprozentsätze auswirken.

        Weitere Informationen finden Sie unter [Übersicht über das Ändern von &#x200B;](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)).


        >[!TIP]
        >
        >* Sie können mehrere Benutzer, Aufgabengebiete oder Teams zuweisen. Sie können nur aktive Benutzer, Aufgabengebiete und Teams zuweisen.
        >   
        >* Beachten Sie beim Hinzufügen einer Benutzerzuweisung den Avatar, die Primäre Rolle des Benutzers oder seine E-Mail-Adresse, um zwischen Benutzern mit identischen Namen zu unterscheiden. Benutzende müssen mindestens einem Aufgabengebiet zugeordnet sein, damit sie es beim Hinzufügen anzeigen können. Die Einstellung Kontaktinformationen anzeigen muss in Ihrer Zugriffsebene aktiviert sein, damit Benutzer die E-Mails von Benutzern anzeigen können. Weitere Informationen finden Sie unter [Gewähren des Benutzerzugriffs](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
        > 
        >   Wenn ein(e) Benutzende(r), ein Aufgabengebiet oder ein Team zugewiesen wurde, bevor sie/er deaktiviert wurden, bleiben sie/sie dem Arbeitselement zugewiesen. In diesem Fall empfehlen wir Folgendes:
        >   
        >* Weisen Sie das Arbeitselement den aktiven Ressourcen neu zu.
        >* Verknüpfen Sie die Benutzer in einem deaktivierten Team mit einem aktiven Team und weisen Sie das Arbeitselement dem aktiven Team zu.


   1. (Optional) Ändern Sie eine der folgenden Optionen für Verantwortliche:

      * (Bedingt) **Zuordnung % oder Stunden**: Geben Sie einen neuen Zuordnungsprozentsatz oder neue Stunden an.

      >[!NOTE]
      >
      >Diese Option kann nur geändert werden, wenn der Dauertyp für alle Aufgaben, die bearbeitet werden, gleich ist. Wenn als Dauertyp „Berechnete Arbeit“ oder „Leistungsgesteuert“ festgelegt ist, können Sie die Zuordnung % aktualisieren. Wenn der Dauertyp „Einfach“ ist, können Sie die Stunden aktualisieren. Informationen zum Dauertyp finden Sie unter [Übersicht über die Aufgabendauer und den Dauertyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
      >
      >
      >Wenn das Feld leer ist, bedeutet dies, dass der Wert in allen Aufgaben unterschiedlich ist. Sie können ihn jedoch weiterhin ändern.

      * **Primär machen**: Bewegen Sie den Mauszeiger über die ausgewählten Aufgaben und wählen Sie diese Option aus, um den Verantwortlichen zum Besitzer der Aufgabe für alle Aufgaben zu machen, die bearbeitet werden.
      * **Rolle des Verantwortlichen**: Wählen Sie eine Rolle aus der Dropdown-Liste aus. Wenn die Option deaktiviert bleibt, wählt Adobe Workfront automatisch die Primäre Rolle des Benutzers aus.
      * **Dauertyp**
      * **Dauer**
      * **Geplante Stunden**

   1. Klicken Sie auf **Speichern**.

<!-- temporary content - for Assignments redesign:

Editing assignments on tasks differs depending on which environment you choose. 

1. (Conditional) If you are using the Production environment to assign tasks, the **Edit Tasks** box opens in the new experience. Do the following in the Production environment: 

   1. To add or remove assignees, do one of the following:

      * To add assignees, start typing the name of an assignee in the **Search people, roles, or teams** field, then select them when they display in the list. 
      * To remove assignees, click the **x** icon to the right of their name. Only assignees that are common to all tasks display in the list. 
      * Click Assign to me to assign the selected tasks to yourself.

   1. (Conditional) When using the new experience, click **Save**.

   1. (Optional) Click **Switch to old experience** at the bottom of the **Edit Tasks** box.
      
      The **Edit Tasks** box opens in the old experience.

   1. (Conditional) In the old experience, do the following to modify the assignees:

      1. Go to the **Assignments** section.

         >[!IMPORTANT]
         >
         >Removing assignees can affect the task hours and allocation percentages. For more information, see the section [How removing assignees affects task hours and allocation percentages](#how-removing-assignees-affects-task-hours-and-allocation-percentages) in this article.

      1. Do one of the following to add or remove assignees:

         * To add a new assignee:

            1. In the **Assignments** section, select **Assignee**.

               Information that is common across all tasks selected displays. For example, if the same user is assigned to all tasks, that user displays in the **Assignee** column. If information is not common across the tasks selected, no information displays.
            
            1. Start typing the name of a user, role, or team, then select it when it displays in the list. The assignment is added and does not replace the current assignments on the selected tasks.

            >[!TIP]
            >
            > * You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams.
            >   
            > * When adding a user assignment, notice the avatar, the user's Primary Role, or their email address to distinguish between users with identical names. Users must be associated with at least one job role to view it as you add them. You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
            > 
            >   If a user, job role, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:
            >   
            >     * Reassign the work item to active resources.
            >     * Associate the users in a deactivated team with an active team and reassign the work item to the active team.


         * To remove individual assignees:

            1. Click the **X icon** next to the name of the assignee that you want to remove if the assignee displays in the Assignments list.

               Or

               (Conditional) If the assignee that you want to remove does not display in the Assignments section because the assignee is assigned to only some of the tasks that you have selected, click **Remove Assignee** and start typing the name of the assignee that you want to remove, then click the name when it appears in the drop-down list.

         * To remove all existing assignees:

            1. Click **Remove All Existing Assignees**, then click **Yes, Delete All Assignees**.

               This removes not only common assignees (assignees that are displayed in the edit dialog box), but also all assignees on all the selected tasks.

            Removing users from tasks can affect task hours and allocation percentages.
            
            For more information, see [Overview of modifying task assignments](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

      1. (Optional) Modify any of the following options for assignees:

         * (Conditional) **Allocation % or Hours**: Specify a new allocation percentage or hours.

         >[!NOTE]
         >
         >This option can be modified only if the Duration Type is the same across all tasks that are being edited. When the Duration Type is Calculated Work or Effort Driven you can update the Allocation %. When the Duration Type is Simple you can update the Hours. For information about Duration Type, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
         >
         >
         >If the field is blank, this means that the value is different across tasks; however, you are still able to modify it.

         * **Task Owner**: Select this option to make the assignee the owner of the task for all tasks being edited.
         * **Assignee's Role**: Select a role from the drop-down list. If left unselected, Adobe Workfront automatically selects the Primary Role of the user. 

      1. Click **Save Changes.**
        

1. <span class="preview">(Conditional) If you are using the Preview environment to assign tasks, the **Edit Tasks** box opens. Do the following in the Preview environment: </span>

   <div class="preview">-->





