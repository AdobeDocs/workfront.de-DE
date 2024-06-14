---
product-area: templates
navigation-topic: templates-navigation-topic
title: Bearbeiten von Projektvorlagen
description: Sie können Projektvorlagen bearbeiten, um Änderungen in Projektprozessen und -einstellungen widerzuspiegeln.
author: Alina
feature: Work Management
exl-id: da0fca31-6a50-4862-ad9a-a453ef968773
source-git-commit: 5cb07cb42c3264c6629bc0a038c0e70ffc2cb509
workflow-type: tm+mt
source-wordcount: '4721'
ht-degree: 2%

---

# Bearbeiten von Projektvorlagen

<!-- Audited: 2/2024 -->

<!--The Resource Pools part also duplicates in the "Working with Resource Pools" article-->

Sie können Projektvorlagen bearbeiten, um Änderungen in Projektprozessen und -einstellungen widerzuspiegeln. Nachdem Sie die Änderungen auf einer Vorlage aktualisiert und gespeichert haben, sind die neuen Änderungen in neuen Projekten sichtbar, wenn die Projekte mit der Vorlage erstellt werden. Die Änderungen, die Sie an der Vorlage vornehmen, beziehen sich nicht auf das Projekt, das diese Vorlage verwendet.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen</td> 
   <td>
      <p>Neu: Standard</p>
      <p>Oder</p>
      <p>Aktuell: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene</td> 
   <td> <p>Zugriff auf Vorlagen bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> 
    <ul> 
     <li> <p>Beitragen Sie Berechtigungen zu einer Vorlage, um sie auf der Registerkarte "Vorlagendetails"zu bearbeiten</p> </li> 
     <li> <p>Berechtigungen für eine Vorlage verwalten, um sie im Feld "Vorlage bearbeiten"zu bearbeiten</p> </li> 
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vorlagen bearbeiten {#edit-a-template}

<!--
Editing a template differs depending on what environment you choose. 

### Edit a template in the Production environment {#edit-a-template-in-the-production-environment} 

1. Go to the template you want to edit.
1. (Conditional) To edit limited information about the template,  click **Template Details** in the left panel, then go to the areas listed in the left panel to edit information for each area. 
1. To edit information in the Details section, click the **Edit** icon ![](assets/edit-icon.png), then select from any of the areas below, or click **Edit all** to edit information in all areas:

   * Overview
   * Custom Forms

     Names of customs forms display only if there are custom forms attached to the object.
   
   * Finance

   >[!TIP]
   >
   >For information about all fields that display in the Details area, continue with editing all fields using the Edit Template box below.

1. (Conditional) To edit all information about the template, click the **More** menu ![](assets/qs-more-icon-on-an-object.png) next to the name of the template, then click **Edit**.

   The **Edit Template** box opens. The sections in this box contain the same fields available in  the Template Details section .

1. Consider editing information in any of the following sections:

   * [Overview](#overview) 
   * [Finance](#finance) 
   * [Portfolio](#portfolio) 
   * [Settings](#settings) 
   * [Access](#access) 
   * [Custom Forms](#custom-forms) 
   * [Tasks](#tasks) 
   * [Issues](#issues) 
   * [Comment](#comment)

### Overview {#overview}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Overview**.

   ![](assets/edit-template-overview-with-tasks-and-issues-350x210.png)

1. Update the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong></td> 
      <td>Specify a name for the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Description</strong></td> 
      <td>Add additional information about the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Active</strong></td> 
      <td><p>Select this checkbox if you want the template to be active. Other users can find this template and attach it to projects when creating projects. Deselect this checkbox if you want to deactivate templates that are no longer used. Deactivated templates cannot be attached to projects. This is enabled by default. </p><p><b>TIP</b>
      
      You can deactivate a template from the template header as described in the [Activate or deactivate a template](#activate-or-deactivate-a-template) section in this article.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong></td> 
      <td>Specify a web link that relates to information about this template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Schedule From</strong></td> 
      <td><p>Specify whether the project using this template is scheduled from the <strong>Start Date</strong>, or from the <strong>Completion Date</strong>. This selection determines the planned dates of the future tasks on the project using this template. </p><p>Select from the following: </p> 
       <ul> 
        <li><p><strong>Schedule From Start Date</strong>: The Start Date of the template is actually the Start Day. When you schedule a template from Start Date, Adobe Workfront calculates the Completion Day of the template based on the Duration of all the template tasks. The Start Day of the template becomes the Planned Start Date of the future project.</p></li> 
        <li><p><strong>Schedule from Completion Date</strong>: The Completion Date of the template is actually the Completion Day. When you schedule a template from Completion Date, Workfront calculates the Start Day of the template based on the Duration of all the template tasks. The Completion Day of the template becomes the Planned Completion Date of the future project. </p></li> 
       </ul><p>For more information about the Start and Completion Days of template tasks, see <a href="../../../manage-work/projects/create-and-manage-templates/overview-of-start-completion-day-on-template.md" class="MCXref xref">Overview of Start and Completion Days in a template</a>. </p><p>The Schedule From setting for templates is similar to that of projects. Your Workfront administrator selects the default Schedule From setting for the projects in your system. For information about setting project defaults, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Condition Type</strong></td> 
      <td><p>Select between the following Condition Types:</p> 
       <ul> 
        <li><strong>Manual:</strong> The project owner sets the Condition of the project on the project manually. <strong></strong></li> 
        <li><strong>Progress Status:</strong> Workfront automatically sets the Condition of the future project based on the Progress Status of tasks on the Critical Path. For more information about understanding Progress Status, see <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Task Progress Status overview</a>.</li> 
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priority</strong></td> 
      <td><p>This is just a visual flag for you which allows you to prioritize your future projects. Select from the following options:</p> 
       <ul> 
        <li><p><strong>None</strong></p></li> 
        <li><p><strong>Low</strong></p></li> 
        <li><p><strong>Normal</strong></p></li> 
        <li><p><strong>High</strong></p></li> 
        <li><p><strong>Urgent</strong></p></li> 
       </ul><p><p>Depending on the Project Preferences selected by your Workfront administrator, the names of priorities might be different for you. For more information about editing priorities, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Create and customize priorities</a>.</p></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Template Owner</strong></td> 
      <td><p>The user who is designated as the Template Owner must be a Workfront active user. </p><p>Consider the following about the user designated as the Template Owner: </p> 
       <ul> 
        <li>They are automatically given Manage permissions to the template. </li> 
        <li>They are added to the project team and are automatically given Manage permissions to the project created from the template. </li> 
        <li>They become the Project Owner, when the project is created from this template. </li> 
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Template Sponsor</strong></td> 
      <td><p>The user specified in this field becomes the Project Sponsor, when the template is added to the project. This user is added to the project team and is automatically given view permissions to the project. The user who is designated as the Template Sponsor must be a Workfront active user. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Resource Manager</strong></td> 
      <td><p>The specified users are automatically given manage permissions to the future projects and can assign resources to the tasks and issues of the projects. You can specify more than one Resource Manager. </p></td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>Group</strong></td> 
      <td><p>In the drop-down list, select the group that you want to be associated with projects created from the template. It can be a group of any level. </p><p>You can make sure you are selecting the right group by hovering over it and clicking the information icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.</p> <p><b>NOTES</b>
      
    <ul> 
    <li><p>In the Projects area on a group's page, when someone creates a project using a template that doesn't have a group selected, the system associates the currently open group with the project.</p><p>This is different from other areas where the system associates a user's Home Group with the project when the user creates the project using a template that doesn't have a group selected.</p>
    </li> 
      <li><p>If a user selects a template that has a group selected while creating a project—or while converting a task or issue to a project—the user can choose a different group for the project.</p></li> 
      <li>Though this field is available in templates only in the new Adobe Workfront experience, you can see it in lists and reports both there and in Adobe Workfront Classic. </li> 
      </ul> </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Company</strong></td> 
      <td><p>Specify the Company that you want to associate with the template. Only active companies display in the list.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Finance {#finance}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Finance**.

   ![](assets/edit-template-finance-with-tasks-and-issues-350x259.png)

1. Update the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Performance Index Method</strong></td> 
      <td><p>Specify whether the Earned Value metrics of the future project are calculated using hours or costs. For more information about the Performance Index Method, see <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Set the Performance Index Method (PIM)</a>. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Budget</strong></td> 
      <td><p>Specify a Budget for the projects that are created from this template.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fixed Cost</strong></td> 
      <td><p>Specify the Fixed Cost for the projects that are created from this template. This is different than the Labor Cost which comes from the hours on the project and the Expense Cost which comes from the amount of expenses on the project. The Fixed Cost of a project is taken into account when calculating the Net Value of a project and it is part of the Budgeted Cost.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fixed Revenue</strong></td> 
      <td><p>Specify the Fixed Revenue for the projects that are created from this template.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Template Currency</strong></td> 
      <td><p>Specify the currency for the future project, if it is different than the default currency of your system. This field is not visible if you have only the default currency in the system.<br>For more information about currency, see <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Require time to be approved for this project</strong></td> 
      <td><p>Select this option to require the Project Owner of the future project created from this template to approve time logged on the project. If you are using Billing Records and you select this option, only the approved hours on the project appear as available billable hours for the Billing Records. Approving time on the project is independent of approving timesheets. For more information about requiring time to be approved on a project, see <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" class="MCXref xref">Require time to be approved for a project</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Portfolio {#portfolio}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Portfolio**.

   ![](assets/edit-template-portfolio-with-tasks-and-issues-350x228.png)

1. Update the following fields:

   <table style="table-layout:auto">
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Portfolio</strong></td> 
      <td><p>Specify a Portfolio for the projects that are created from this template. You must create a Portfolio first, before it appears in the drop-down list. </p><p>Only active portfolios display in the list. For more information about creating portfolios, see <a href="../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md" class="MCXref xref">Create a portfolio </a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Program</strong></td> 
      <td><p>If you selected a Portfolio for the template, specify a <strong>Program</strong> for the future project. Some Portfolios might not have Programs. You must create a Program first, before it appears in this drop-down list. Only active programs display in the list.</p><p>For more information about creating programs, see <a href="../../../manage-work/portfolios/create-and-manage-programs/create-program.md" class="MCXref xref">Create a program</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Planned Benefit</strong></td> 
      <td><p>Specify the Planned Benefit of the projects that are created from this template. The Planned Benefit is used in the Business Case of the project and the Portfolio Optimizer. </p><p>For more information about the Planned Benefit of a project, see <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Overview of project Planned Benefit</a>. The Planned Benefit of a project is taken into account when the Net Value of a project is calculated. </p><p>For more information about using the Portfolio Optimizer, see <a href="../../../manage-work/portfolios/portfolio-optimizer/manage-projects-in-portfolio-optimizer.md" class="MCXref xref">Manage projects in the Portfolio Optimizer</a> </p></td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Settings {#settings}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Settings**.

   ![](assets/edit-template-settings-with-tasks-and-issues-350x336.png)

1. Update the following fields: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Milestone Path</strong> </td> 
      <td> <p>Select a Milestone Path for the template. Only active milestone paths display in the list.<br>For more information about Milestone Paths, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Create a milestone path</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Completion Mode</strong> </td> 
      <td> <p>Controls how the future project will be marked as Complete. <br>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>Automatic</strong>: The project is marked Complete when all the tasks and issues are completed.</p> </li> 
        <li> <p><strong>Manual</strong>: You have to manually select the Complete status for the project, when all the tasks and issues are completed. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Summary Completion Mode</strong> </td> 
      <td> <p>Controls how the parent tasks on the future project are marked as Complete. <br>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>Automatic</strong>: The parent tasks are marked Complete and they update their percent complete automatically, as the children tasks are completed and the percent complete of the children is updated. </p> </li> 
        <li> <p><strong>Manual</strong>: You have to manually update the percent complete and the status of the parent tasks, independently of what changes are made to the children tasks. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Update Type</strong> </td> 
      <td> <p>Controls when the changes you make to the timeline of the future project are saved on the project. </p> 
       <b>EXAMPLE </b> 
        <p>The following changes to the project trigger an update to the timeline of the project:</p> 
        <ul> 
         <li> <p>update the dates of tasks</p> </li> 
         <li> <p>change predecessor relationships<br></p> </li> 
         <li> <p>change parent-child relationships</p> </li> 
         <li> <p>add or remove assignments in addition to changing the task constraint or duration type.</p> </li> 
        </ul> 
       </div> <p>Select from the following options:<br></p> 
       <ul> 
        <li> <p><strong>Automatic and On Change</strong> (Default setting): The future project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on (On Change). The project timeline is also updated each night (Automatic).<br>This is the recommended setting for this field because it ensures that the project timeline is always up to date.<br>When you perform an action on a task or project that triggers a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer recalculations display briefly as a question mark (between 1 and 5 seconds, or up to a minute for large projects). This indicates that the recalculation is not yet finished, and the dates are subject to change.<br></p> </li> 
       </ul> 
       <ul> 
        <li> <p><strong>Change Only</strong>: The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. You might want to select this option if changes rarely occur in the project or in other projects that the timeline is dependent on.<br></p> </li> 
       </ul> 
       <ul> 
        <li> <p><strong>Automatic Only</strong>: The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if many changes occur each day in the project or in other projects that the timeline is dependent on. However, be aware that you chose this setting, as the project will not update at the same time that the changes are made.<br></p> </li> 
       </ul> 
       <ul> 
        <li> <p><strong>Manual Only</strong>: The project timeline is updated only when you select the option to Recalculate Timelines, as described in <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalculate project timelines</a>.<br></p> </li> 
       </ul> <p>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Schedule</strong> </td> 
      <td> <p>Select a schedule for your template. This will become the schedule of the project that is created from this template. This should be the same schedule assigned to most people that are working on the project. You must create a schedule before you can assign it to a template.<br>For more information about creating schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>. <br>If you have not created custom schedules in your system, the Default Schedule is selected. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>User Time Off</strong> </td> 
      <td> <p>Determines whether the time off of the Primary Assignee of a task adjusts the task planned dates. When you attach the template to an existing project, and the template has a different setting for this field than the project, the setting on the project remains unchanged. The default option for this setting for a new template is the same as the system-level project preference. </p> <p>For information about the project preferences at the System level, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p> <p>For information about how this setting affects the task dates on a project, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.<br>Select from the following options:<br></p> 
       <ul> 
        <li> <p><strong>Consider user time off in task durations</strong>: When selecting this option, the planned dates of the tasks on the project created from this template adjust according to the time off of the Primary Assignee of the task, if the time off occurs during the duration of the task. </p> </li> 
        <li> <p><strong>Ignore user time off in task durations</strong>: When selecting this option, the planned dates of the tasks on the project created from this template remain as originally planned, even if the Primary Assignee of the task has time off during the duration of the task. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Resource Leveling Mode</strong> </td> 
      <td> <p>Select from the following options:<br></p> 
       <ul> 
        <li> <p><strong>Manual</strong>: you must manually level your resources on the project created from this template (this is the default setting)</p> </li> 
        <li> <p><strong>Automatic:</strong> Workfront levels the resources on the future project. <br>For more information about Resource Leveling, see <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md" class="MCXref xref">Level Resources in the Gantt Chart </a>. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Risk</strong> </td> 
      <td> <p>Define the level of risk of the projects created from this template. The risk is just an indicator of how risky a project can be. You can prioritize the execution of your projects based on the level of risk.<br>Consider selecting from the following levels of risk:<br></p> 
       <ul> 
        <li> <p><strong>Very Low</strong> </p> </li> 
        <li> <p><strong>Low</strong> </p> </li> 
        <li> <p><strong>Medium</strong> </p> </li> 
        <li> <p><strong>High</strong> </p> </li> 
        <li> <p><strong>Very High</strong> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Resource Pools</strong> </td> 
      <td> <p>Specify the resource pools associated with the template. Resource pools are collections of users that are needed at the same time for the completion of a project. For more information about resource pools, see <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resource pools overview </a>.</p> <p> <p><b>NOTE</b> 
      
      When you edit templates in bulk, only the resource pools that are common to all the templates selected appear in this field. If the templates selected have no shared resource pools, this field will be empty. The resource pools you specify here will overwrite the templates' individual resource pools.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Approval Process</strong> </td> 
      <td> <p>Select the approval process you want to associate with the template. Your Workfront administrator or a user with administrative access to Approval Processes must define system-level or group-level project approval processes before you can associate them with a template. For more information about creating approval processes, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Create an approval process for work items</a>.</p> <p>Consider the following when adding approval processes: </p> 
      <ul> 
      <li>Only active approval processes display in the list. </li> 
      <li> <p>System-wide and group-specific approval processes display in the list. An approval process associated with a group other than that of the template does not display in the list.</p> <p><b>IMPORTANT</b> 
      
      If the group associated with the template changes, the group-specific approval process becomes a single-use approval process. For more information about how changes to the group of the project or changes in the approval process affect approval settings, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">How group and approval process changes affect assigned approval processes</a>. </p> </li> 
      <li> <p>If you added a single-use approval process, it displays as "Custom" in this field. For information, see <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associate a new or existing approval process with work</a>. </p> 
      </li> 
      <li> <p>When bulk-editing templates, the following scenarios exist:</p> 
      <ul> 
         <li> <p>When you select templates from the same group, both system-level and group-level approval processes display in this field.</p> </li> 
         <li> <p>When you select templates from different groups, only system-level approval processes display in this field.</p> </li> 
         <li> <p>When any of the templates has a single-use approval process attached, it is replaced by the system-level you select. </p> </li> 
      </ul> </li> 
      </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Filter Hour Types</strong> </td> 
      <td> <p>Consider the following:</p> <p>Select <strong>No</strong> to make all project-specific hour types available on the future project. (This is the default selection)</p> <p>Or</p> <p>Select <strong>Yes</strong> to make only a subset of the project-specific hour types available on the future project, then select the hour types you want to make available. (Hold the Shift key to select multiple hour types.)</p> <p>If you select this option, only the hour types you select are made available to select when logging hours on the project (or on tasks and issues within the project). You must select at least one hour type; if you select this option and you do not select any hour types, all hour types are made available on the project.</p> <p>The same hour type selections must be made at the individual user level in order for the user to see these hour type options on the project. </p> <p>For more information about defining hour types at the user level, see the section <a href="../../../timesheets/create-and-manage-timesheets/log-time.md#understa" class="MCXref xref">Log time</a> in <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Log time</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Reminder Notification</strong> </td> 
      <td>Select the Reminder Notification that should be associated with the future project. You must configure Reminder Notifications for projects for this field to appear during editing a template. <br>For more information about configuring Reminder Notifications, see <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Set up reminder notifications</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.  
   Or
1. Click **Save Changes**.

### Access {#access}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Access**.

   ![](assets/edit-template-access-with-tasks-and-issues-350x241.png)

   The Access you specify for your template will become the Access of users associated with the project when the template is used to create a project.

   Specify the following **Access** information for the template:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>When someone is assigned to a task</strong> </td> 
      <td> <p>Select from <strong>View</strong>, <strong>Contribute,</strong> or <strong>Manage</strong> access to a task. The user assigned to a task is automatically granted this access to the task. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Also grant access to the project</strong> </td> 
      <td> <p> Select from <strong>View</strong>, <strong>Contribute</strong>, or <strong>Manage</strong> access to the project. The user assigned to a task is automatically granted this access to the project, as well. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>When someone is assigned to an issue</strong> </td> 
      <td> <p>Select from <strong>View</strong>, <strong>Contribute,</strong> or <strong>Manage</strong> access to an issue. The user assigned to an issue is automatically granted this access to the issue. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Also grant access to the project</strong> </td> 
      <td> <p> Select from <strong>View</strong>, <strong>Contribute</strong>, or <strong>Manage</strong> access to the project. The user assigned to an issue is automatically granted this access to the project, as well. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>When someone submits a request: Give them access</strong> </td> 
      <td> <p> Select from <strong>View</strong>, <strong>Contribute</strong>, or <strong>Manage</strong> access to the request. When they submit a request to the project, they are granted this access to the request they submitted. For more information, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>People from the same company will inherit the same permissions for all requests</strong> </td> 
      <td> <p>Select this field if you want people from the same company to have the same access to all the requests on the project, whether they submitted them or not.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>When someone is given access to this project: Give them access to ...</strong> </td> 
      <td> <p>Select the access options that you want users to have on the project, if the project is shared with them. Select the specific options for their access, if they are designated as <strong>Viewers</strong>, <strong>Contributors</strong>, or <strong>Managers</strong> when sharing the project with them. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Custom Forms {#custom-forms}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Custom Forms**.

   ![edit_tempate_custom_forms.png](assets/edit-tempate-custom-forms-tasks-with-issues-sections-350x136.png)

1. Select the custom form or forms that you want to associate with the template. You must build the custom forms before they are available to select in this field.

   Only active custom forms display in the list. For more information about building custom forms, see [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   You can add up to ten custom forms to a template.

   The forms will be added to the project that is created from this template. 

1. (Optional) Continue editing the following section, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Tasks {#tasks}

You can define the defaults that will be associated with all the new tasks when you add them to a project that is created from the template.

For information about how these settings affect creating new tasks, see [Create tasks overview](../../../manage-work/tasks/create-tasks/create-tasks-overview.md).

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Tasks**.

   ![](assets/edit-template-with-tasks-and-issue-sections-350x144.png)

1. In the **Task Default Approval Process** box, select the Approval Process you want to associate with all new tasks when you add them to a project created from this template. You must create an Approval Process for tasks before you can associate it with tasks. Only active approval processes display in the list. For more information about creating Approval Processes, see [Creating Approval Processes](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
1. In the **Task Default Custom Forms** box, select the custom form or forms that you want to associate with all new tasks when you add them to a project created from this template. You must build the custom forms before they are available to select in this field. Only active custom forms display in the list. For more information about building custom forms, see [Creating Custom Forms](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). You can associate up to ten custom forms with a task.
1. (Optional) **Select Use Work Effort to automatically calculate task Planned Hours** if you want to enable managing task effort by using&nbsp;Work Effort instead of Planned Hours in the project created from the template.
1. (Conditional and optional) If you selected Use Work Effort to automatically calculate task Planned Hours, click the drop-down menu to update the percentage for each level of Work Effort. The following percentage values are the defaults:
 
   | Work Effort level |Percentage value|
   |---|---|
   | Small |25% |
   | Medium |50% |
   | Large |75% |

  For information about using Work Effort to manage the effort on tasks on projects, see [Work Effort overview](../../../manage-work/tasks/task-information/work-effort.md).

1. (Optional) Continue editing the following section, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Issues {#issues}

By editing issue settings, you can prevent users from adding issues inline in the future project created from the template.

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Issues**.

   ![](assets/edit-template-box-with-issues-nwe-350x171.png)

1. (Optional) Deselect the **Allow users to add issues inline** option. It is enabled by default.

   When disabling this option users cannot add issues inline to the project or the tasks in the Issues section, when the project is created from the template.

   >[!TIP]
   >
   >Disable this option if you want to enforce users to complete the New Issue Fields or the custom forms associated with new issues.

   When disabling this option, users with permissions to add issues to the project created from the template can do so by using the New Issue button or a request queue associated with the project.

   For more information about configuring issue settings on projects, see the [Issue Settings](../../../manage-work/projects/manage-projects/edit-projects.md#issue) section in the article [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

   For information about creating issues on projects, see [Create issues](../../../manage-work/issues/manage-issues/create-issues.md). 

1. (Optional) Continue editing the following section, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Comment {#comment}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Comment**.

   ![edit_templates_comment.png](assets/edit-templates-comment-with-tasks-and-issues-350x177.png)

1. Specify a comment that you want to display in the updates stream of the template in the available field.

   This comment is visible for everyone with View access to the template and with access to view Notes.

1. Click **Save Changes**.

   Your changes will be submitted for this template.

   Now, when you use this template to create a project all these settings will transfer to the new project.


   <!--drafted section below for the edit template story: 
   remove this tag and add the Preview blurb at the top of this article in yellow, if it's not already there. Keep the "div class" tags below until 23.1 production: 


### Edit a template in the Preview environment {#edit-a-template-in-the-preview-environment}
-->

1. Markieren Sie die Vorlage, die Sie bearbeiten möchten.
1. (Bedingt) Klicken Sie zum Bearbeiten begrenzter Informationen über die Vorlage auf **Vorlagendetails** Navigieren Sie im linken Bereich zu den Bereichen, die im linken Bereich aufgeführt sind, um Informationen für jeden Bereich zu bearbeiten.
1. Um Informationen im Bereich Details zu bearbeiten, klicken Sie auf das **Bearbeiten** icon ![](assets/edit-icon.png), wählen Sie dann einen der folgenden Bereiche aus oder klicken Sie auf **Alle bearbeiten** um Informationen in allen Bereichen zu bearbeiten:

   * Übersicht
   * Benutzerdefinierte Formulare

   Namen von Zollformularen werden nur angezeigt, wenn benutzerdefinierte Formulare an das Objekt angehängt sind.

   * Finanzielle Details

   >[!TIP]
   >
   >Informationen zu allen Feldern, die im Bereich &quot;Details&quot;angezeigt werden, erhalten Sie, wenn Sie mit der Bearbeitung aller Felder über das Feld &quot;Vorlage bearbeiten&quot;weiter unten fortfahren.

1. (Bedingt) Um alle Informationen über die Vorlage zu bearbeiten, klicken Sie auf **Mehr** Menü ![](assets/qs-more-icon-on-an-object.png) neben dem Namen der Vorlage klicken Sie auf **Bearbeiten**.

   Die **Vorlage bearbeiten** wird geöffnet. Die Abschnitte in diesem Feld enthalten dieselben Felder, die im Abschnitt Vorlagendetails verfügbar sind.

1. Ziehen Sie Informationen in einen der folgenden Abschnitte:

   * [Vorlagenname](#template-name)
   * [Übersicht](#overview-preview)
   * [Finanzen](#finance-preview)
   * [Benutzerdefinierte Formulare](#custom-forms-preview)
   * [Projekteinstellungen](#project-settings)
   * [Aufgabeneinstellungen](#task-settings)
   * [Problemeinstellungen](#issue-settings)
   * [Zugriff](#access-preview)


### Vorlagenname{#template-name}

1. Beginnen Sie mit der Bearbeitung Ihrer Vorlage wie oben beschrieben.
1. Im **Vorlage bearbeiten** Feld, klicken Sie auf **Vorlagenname**.
1. (Optional) Fahren Sie je nach den zu ändernden Informationen mit der Bearbeitung der folgenden Abschnitte fort

   Oder

   Klicken Sie auf **Speichern**.



### Übersicht {#overview-preview}

1. Beginnen Sie mit der Bearbeitung Ihrer Vorlage wie oben beschrieben.
1. Im **Vorlage bearbeiten** Feld, klicken Sie auf **Übersicht**.

   ![](assets/edit-template-box-overview-section.png)

1. Aktualisieren Sie die folgenden Felder:

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
         <tr> 
         <td role="rowheader"><strong>Beschreibung</strong></td> 
         <td>Fügen Sie zusätzliche Informationen zur Vorlage hinzu.</td> 
       </tr> 
         <tr> 
         <td role="rowheader"><strong>Priorität</strong></td> 
         <td><p>Dies ist nur ein visuelles Flag für Sie, mit dem Sie Ihre zukünftigen Projekte priorisieren können. Wählen Sie aus den folgenden Optionen aus:</p> 
         <ul> 
         <li><p><strong>Keine</strong></p></li> 
         <li><p><strong>Niedrig</strong></p></li> 
         <li><p><strong>Normal</strong></p></li> 
         <li><p><strong>Hoch</strong></p></li> 
         <li><p><strong>Dringend</strong></p></li> 
         </ul><p><p>Je nach den von Ihrem Workfront-Administrator ausgewählten Projekteinstellungen können die Prioritätsnamen für Sie unterschiedlich sein. Weitere Informationen zu Bearbeitungsprioritäten finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Erstellen und Anpassen von Prioritäten</a>.</p></p></td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>URL</strong></td> 
         <td>Geben Sie einen Web-Link an, der sich auf Informationen zu dieser Vorlage bezieht.</td> 
       </tr>
       <tr> 
       <td role="rowheader"><strong>Bedingungstyp</strong></td> 
       <td><p>Wählen Sie zwischen den folgenden Bedingungstypen aus:</p> 
         <ul> 
         <li><strong>Manuell:</strong> Der Projekteigentümer legt die Projektbedingung für das Projekt manuell fest. <strong></strong></li> 
         <li><strong>Fortschrittsstatus:</strong> Workfront legt die Bedingung des künftigen Projekts automatisch auf der Grundlage des Fortschrittsstatus von Aufgaben auf dem kritischen Pfad fest. Weitere Informationen zum Fortschrittsstatus finden Sie unter <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Übersicht über den Task Progress Status</a>.</li> 
       </ul>
         </td> 
         </tr> 
       <tr> 
         <td role="rowheader"><strong>Zeitplanmodus</strong></td> 
         <td><p>Geben Sie an, ob das Projekt, das diese Vorlage verwendet, über die <strong>Startdatum</strong>oder von der <strong>Abschlussdatum</strong>. Diese Auswahl bestimmt die geplanten Daten der künftigen Aufgaben für das Projekt anhand dieser Vorlage. </p><p>Wählen Sie aus den folgenden Optionen aus: </p> 
       <ul> 
       <li><p><strong>Zeitplan ab Startdatum</strong>: Das Startdatum der Vorlage ist tatsächlich der Starttag. Wenn Sie eine Vorlage vom Startdatum an planen, berechnet Adobe Workfront den Fertigungstag der Vorlage basierend auf der Dauer aller Vorlagenaufgaben. Der Starttag der Vorlage wird zum geplanten Startdatum des künftigen Projekts.</p></li> 
       <li><p><strong>Zeitplan ab Abschlussdatum</strong>: Das Abschlussdatum der Vorlage ist tatsächlich der Abschlussdatum. Wenn Sie eine Vorlage ab dem Abschlussdatum planen, berechnet Workfront den Starttag der Vorlage basierend auf der Dauer aller Vorlagenaufgaben. Der Abschlusstag der Vorlage wird zum geplanten Abschlussdatum des künftigen Projekts. </p></li> 
       </ul><p>Weitere Informationen zu den Start- und Fertigungstagen von Vorlagenaufgaben finden Sie unter <a href="../../../manage-work/projects/create-and-manage-templates/overview-of-start-completion-day-on-template.md" class="MCXref xref">Übersicht über Start- und Endtage in einer Vorlage</a>. </p><p>Die Einstellung "Zeitplan ab"für Vorlagen ähnelt der für Projekte. Ihr Workfront-Administrator wählt die Standardeinstellung "Zeitplan ab"für die Projekte in Ihrem System aus. Weitere Informationen zum Festlegen der Projektstandards finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projektvoreinstellungen konfigurieren</a>.</p></td> 
       </tr>

   <tr> 
         <td role="rowheader"><strong>Portfolio</strong></td> 
         <td><p>Geben Sie ein Portfolio für die aus dieser Vorlage erstellten Projekte an. Sie müssen zuerst ein Portfolio erstellen, bevor es in der Dropdownliste angezeigt wird. </p><p>In der Liste werden nur aktive Portfolios angezeigt. Weitere Informationen zum Erstellen von Portfolios finden Sie unter <a href="../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md" class="MCXref xref">Erstellen eines Portfolios </a>.</p></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Programm</strong></td> 
         <td><p>Wenn Sie ein Portfolio für die Vorlage ausgewählt haben, geben Sie eine <strong>Programm</strong> für das künftige Projekt. Einige Portfolios haben möglicherweise keine Programme. Sie müssen zunächst ein Programm erstellen, bevor es in dieser Dropdown-Liste angezeigt wird. In der Liste werden nur aktive Programme angezeigt.</p><p>Weitere Informationen zum Erstellen von Programmen finden Sie unter <a href="../../../manage-work/portfolios/create-and-manage-programs/create-program.md" class="MCXref xref">Programm erstellen</a>.</p></td> 
       </tr>  
       <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
         <td role="rowheader"><strong>Gruppe</strong></td> 
         <td><p>Wählen Sie in der Dropdown-Liste die Gruppe aus, die Sie mit in der Vorlage erstellten Projekten verknüpfen möchten. Es kann sich um eine Gruppe beliebiger Ebenen handeln. </p><p>Sie können sicherstellen, dass Sie die richtige Gruppe auswählen, indem Sie den Mauszeiger darüber bewegen und auf das Informationssymbol klicken <img src="assets/info-icon.png"> , das daneben angezeigt wird. Dadurch wird eine QuickInfo mit Informationen zur Gruppe angezeigt, z. B. die Hierarchie der Gruppen darüber und deren Administratoren.</p> <p><b>HINWEISE</b>

   <ul> 
       <li><p>Wenn im Bereich "Projekte"auf der Seite einer Gruppe ein Projekt erstellt wird, für das eine Vorlage verwendet wird, für die keine Gruppe ausgewählt ist, ordnet das System die derzeit geöffnete Gruppe dem Projekt zu.</p><p>Dies unterscheidet sich von anderen Bereichen, in denen das System die Startseite eines Benutzers mit dem Projekt verknüpft, wenn der Benutzer das Projekt mit einer Vorlage erstellt, für die keine Gruppe ausgewählt ist.</p></li> 
       <li><p>Wenn ein Benutzer eine Vorlage auswählt, für die eine Gruppe beim Erstellen eines Projekts ausgewählt wurde - oder während der Konvertierung einer Aufgabe oder eines Problems in ein Projekt -, kann der Benutzer eine andere Gruppe für das Projekt auswählen.</p></li> 
       <li>Dieses Feld ist zwar nur in den Vorlagen des neuen Adobe Workfront-Erlebnisses verfügbar, Sie können es jedoch sowohl dort als auch in Adobe Workfront Classic in Listen und Berichten sehen. </li> 
         </ul> </p></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Firma</strong></td> 
         <td><p>Geben Sie das Unternehmen an, das Sie mit der Vorlage verknüpfen möchten. In der Liste werden nur aktive Unternehmen angezeigt.</p></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Inhaber der Vorlage</strong></td> 
         <td><p>Der Benutzer, der als Vorlageneigentümer bestimmt wurde, muss ein aktiver Workfront-Benutzer sein. </p><p>Beachten Sie Folgendes zu dem Benutzer, der als Vorlageneigentümer festgelegt wurde: </p> 
         <ul> 
         <li>Sie erhalten automatisch Verwaltungsberechtigungen für die Vorlage. </li> 
         <li>Sie werden dem Projektteam hinzugefügt und erhalten automatisch Verwaltungsberechtigungen für das Projekt, das aus der Vorlage erstellt wurde. </li> 
         <li>Sie werden zum Projekteigentümer, wenn das Projekt aus dieser Vorlage erstellt wird. </li> 
         <li> Wenn der Benutzer, der als Vorlageninhaber benannt wurde, von seiner Zugriffsebene aus eingeschränkten Zugriff auf Vorlagen oder Projekte hat, sind seine Verwaltungsberechtigungen für die Vorlage und die Projekte eingeschränkt. Wenn sie beispielsweise nur Zugriff auf Vorlagen oder Projekte in ihrer Zugriffsebene haben, erhalten sie automatisch Anzeigeberechtigungen für die Vorlage und das Projekt, wenn sie als Vorlageneigentümer bestimmt sind.</li>
         </ul></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Vorlagen-Sponsor</strong></td> 
         <td><p>Der in diesem Feld angegebene Benutzer wird zum Projektsponsor, wenn die Vorlage zum Projekt hinzugefügt wird. Dieser Benutzer wird dem Projektteam hinzugefügt und erhält automatisch Anzeigeberechtigungen für das Projekt. Der Benutzer, der als Vorlagen-Sponsor benannt wurde, muss ein aktiver Workfront-Benutzer sein. </p></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Ressourcenmanager</strong></td> 
         <td><p>Die angegebenen Benutzer erhalten automatisch Verwaltungsberechtigungen für zukünftige Projekte und können den Aufgaben und Problemen der Projekte Ressourcen zuweisen. Sie können mehr als einen Ressourcen-Manager angeben. </p></td> 
       </tr> 
      </table>

1. (Optional) Fahren Sie je nach den zu ändernden Informationen mit der Bearbeitung der folgenden Abschnitte fort.

   Oder

   Klicken Sie auf **Speichern**.

### Finanzielle Details {#finance-preview}

1. Beginnen Sie mit der Bearbeitung Ihrer Vorlage wie oben beschrieben.
1. Im **Vorlage bearbeiten** Feld, klicken Sie auf **Finanzen**.

   ![](assets/edit-template-box-finance-section.png)

1. Aktualisieren Sie die folgenden Felder:

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody>
       <tr> 
         <td role="rowheader"><strong> Währung</strong></td> 
         <td><p>Geben Sie die Währung für das zukünftige Projekt an, wenn sie sich von der Standardwährung Ihres Systems unterscheidet. Dieses Feld ist nicht sichtbar, wenn Sie nur die Standardwährung im System haben.<br>Weitere Informationen zur Währung finden Sie unter <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Wechselkurse einrichten</a>.</p></td> 
       </tr>
       <tr> 
       <td role="rowheader"><strong>Budget</strong></td> 
       <td><p>Geben Sie ein Budget für die Projekte an, die aus dieser Vorlage erstellt werden.</p></td> 
       </tr>  
       <tr> 
         <td role="rowheader"><strong>Performance-Index-Methode</strong></td> 
         <td><p>Wählen Sie aus, wie Workfront die Metriken für den Earned Value des künftigen Projekts berechnet. Wählen Sie aus den folgenden Optionen:
         <ul>
         <li>Stundenbasiert</li>
         <li>Kostenbasiert</li>
         </ul>

   Weitere Informationen zur Leistungsindex-Methode finden Sie unter <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Leistungsindex-Methode (PIM) festlegen</a>. </p></td>
   </tr> 
         <tr> 
         <td role="rowheader"><strong>Geplanter Gewinn</strong></td> 
         <td><p>Geben Sie den geplanten Nutzen der Projekte an, die anhand dieser Vorlage erstellt werden. Der geplante Nutzen wird im Geschäftsfall des Portfolios und im Projektoptimierer verwendet. </p><p>Weitere Informationen über den geplanten Nutzen eines Projekts finden Sie unter <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Übersicht über den geplanten Nutzen des Projekts</a>. Der geplante Nutzen eines Projekts wird bei der Berechnung des Nettowerts eines Projekts berücksichtigt. </p><p>Weitere Informationen zur Verwendung des Portfolio Optimizer finden Sie unter <a href="../../../manage-work/portfolios/portfolio-optimizer/manage-projects-in-portfolio-optimizer.md" class="MCXref xref">Verwalten von Projekten im Portfolio Optimizer</a> </p></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Fixkosten</strong></td> 
         <td><p>Geben Sie die Festkosten für die Projekte an, die aus dieser Vorlage erstellt werden. Dies unterscheidet sich von den Arbeitskosten, die sich aus den Stunden auf dem Projekt ergeben, und den Kosten, die aus den Kosten des Projekts entstehen. Die Fixkosten eines Projekts werden bei der Berechnung des Nettowerts eines Projekts berücksichtigt und sind Teil der Budgetierten Kosten.</p></td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Festeinnahmen</strong></td> 
       <td><p>Geben Sie den festen Umsatz für die Projekte an, die aus dieser Vorlage erstellt werden.</p></td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Genehmigung des Zeitaufwands für dieses Projekt verlangen</strong></td> 
       <td><p>Wählen Sie diese Option aus, damit der Projekteigentümer des anhand dieser Vorlage erstellten künftigen Projekts die im Projekt angemeldete Zeit genehmigen kann. Wenn Sie Rechnungsdatensätze verwenden und diese Option auswählen, werden nur die genehmigten Stunden im Projekt als verfügbare Abrechnungszeiten für die Rechnungsdatensätze angezeigt. Die Genehmigung der Zeit für das Projekt ist unabhängig von der Genehmigung von Timesheets. Weitere Informationen dazu, wie Sie eine Genehmigung für ein Projekt benötigen, finden Sie unter <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" class="MCXref xref">Genehmigung für ein Projekt erforderlich</a>.</p></td> 
       </tr> 
       </tbody> 
      </table>

1. (Optional) Fahren Sie je nach den zu ändernden Informationen mit der Bearbeitung der folgenden Abschnitte fort.

   Oder

   Klicken Sie auf **Speichern**.

### Benutzerdefinierte Formulare {#custom-forms-preview}

1. Beginnen Sie mit der Bearbeitung Ihrer Vorlage wie oben beschrieben.
1. Im **Vorlage bearbeiten** Feld, klicken Sie auf **Benutzerdefinierte Forms**.

   ![](assets/edit-template-box-custom-forms-section.png)

   Die Namen der benutzerdefinierten Formulare, die bereits an die Vorlage angehängt sind, werden im linken Bereich angezeigt.

1. Klicken Sie in die **Benutzerdefiniertes Formular hinzufügen** und wählen Sie das benutzerdefinierte Formular oder die Formulare aus, die Sie mit der Vorlage verknüpfen möchten. Sie müssen die benutzerdefinierten Formulare erstellen, bevor sie in diesem Feld ausgewählt werden können.

   In der Liste werden nur aktive benutzerdefinierte Formulare angezeigt. Weitere Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   Sie können einer Vorlage bis zu zehn benutzerdefinierte Formulare hinzufügen.

   Die Formulare werden dem Projekt hinzugefügt, das aus dieser Vorlage erstellt wird.

1. (Optional) Aktualisieren Sie Informationen in einem der Felder in den benutzerdefinierten Formularen. Die Informationen werden an die Projekte übermittelt, die aus der Vorlage erstellt werden.

1. (Optional) Klicken Sie auf die **x** rechts neben dem Namen eines benutzerdefinierten Formulars klicken Sie auf **Entfernen** , um es aus der Vorlage zu entfernen.

1. (Optional) Fahren Sie je nach den zu ändernden Informationen mit der Bearbeitung des folgenden Abschnitts fort.

   Oder

   Klicken Sie auf **Speichern**.

### Projekteinstellungen {#project-settings}

1. Beginnen Sie mit der Bearbeitung Ihrer Vorlage wie oben beschrieben.
1. Im **Vorlage bearbeiten** Feld, klicken Sie auf **Projekteinstellungen**.

   ![](assets/edit-template-box-project-settings-section.png)

1. Aktualisieren Sie die folgenden Felder:

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
       <tr> 
       <td role="rowheader"><strong>Milestone-Pfad</strong> </td> 
       <td> <p>Wählen Sie einen Milestone-Pfad für die Vorlage aus. In der Liste werden nur aktive Meilensteinpfade angezeigt.<br>Weitere Informationen zu Meilensteinpfaden finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Meilensteinpfad erstellen</a>.</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Abschlussmodus</strong> </td> 
         <td> <p>Steuert, wie das zukünftige Projekt als abgeschlossen markiert wird. <br>Wählen Sie aus den folgenden Optionen aus:</p> 
         <ul> 
         <li> <p><strong>Automatisch</strong>: Das Projekt wird als abgeschlossen markiert, wenn alle Aufgaben und Probleme abgeschlossen sind.</p> </li> 
         <li> <p><strong>Manuell</strong>: Sie müssen den Status Abgeschlossen für das Projekt manuell auswählen, wenn alle Aufgaben und Probleme abgeschlossen sind. </p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Modus für Zusammenfassungsabschluss</strong> </td> 
       <td> <p>Steuert, wie die übergeordneten Aufgaben im künftigen Projekt als abgeschlossen markiert werden. <br>Wählen Sie aus den folgenden Optionen aus:</p> 
       <ul> 
       <li> <p><strong>Automatisch</strong>: Die übergeordneten Aufgaben sind als abgeschlossen markiert und aktualisieren ihren Prozentsatz automatisch, da die untergeordneten Aufgaben abgeschlossen und der Prozentsatz der abgeschlossenen Kinder aktualisiert wird. </p> </li> 
       <li> <p><strong>Manuell</strong>: Sie müssen den prozentualen Abschluss und den Status der übergeordneten Aufgaben manuell aktualisieren, unabhängig davon, welche Änderungen an den untergeordneten Aufgaben vorgenommen werden. </p> </li> 
       </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Aktualisierungstyp</strong> </td> 
         <td> <p>Steuert, wann die Änderungen, die Sie an der Zeitleiste des künftigen Projekts vornehmen, im Projekt gespeichert werden. </p> 
         <b>BEISPIEL </b> 
         <p>Die folgenden Änderungen am Projekt-Trigger ermöglichen eine Aktualisierung der Timeline des Projekts:</p> 
         <ul> 
         <li> <p>Datum der Aufgaben aktualisieren</p> </li> 
         <li> <p>Ändern von Vorgängerbeziehungen<br></p> </li> 
         <li> <p>Ändern von übergeordneten und untergeordneten Beziehungen</p> </li> 
         <li> <p>Hinzufügen oder Entfernen von Zuweisungen zusätzlich zur Änderung der Aufgabenbegrenzung oder des Dauertyps.</p> </li> 
         </ul> 
         </div> <p>Wählen Sie aus den folgenden Optionen aus:<br></p> 
         <ul> 
         <li> <p><strong>Automatisch und Bei Änderung</strong> (Standardeinstellung): Die zukünftige Projekt-Timeline wird jedes Mal aktualisiert, wenn eine Änderung im Projekt oder in einem anderen Projekt erfolgt, von dem die Timeline abhängig ist (Bei Änderung). Die Projekt-Timeline wird auch jede Nacht aktualisiert (automatisch).<br>Dies ist die empfohlene Einstellung für dieses Feld, da dadurch sichergestellt wird, dass die Projekt-Timeline immer auf dem neuesten Stand ist.<br>Wenn Sie eine Aktion für eine Aufgabe oder ein Projekt ausführen, für die eine Timeline-Neuberechnung Trigger wird, werden alle verfügbaren Daten sofort angezeigt, sodass Sie mit der Arbeit fortfahren können. Bei Projekten mit mehr als 100 Aufgaben werden Daten, die eine längere Neuberechnung erfordern, kurz als Fragezeichen angezeigt (zwischen 1 und 5 Sekunden oder bis zu einer Minute bei großen Projekten). Dies bedeutet, dass die Neuberechnung noch nicht abgeschlossen ist und sich die Daten ändern können.<br></p> </li> 
         </ul> 
         <ul> 
         <li> <p><strong>Nur ändern</strong>: Die Projekt-Timeline wird jedes Mal aktualisiert, wenn eine Änderung im Projekt oder in einem anderen Projekt erfolgt, von dem die Timeline abhängig ist. Sie können diese Option auswählen, wenn Änderungen selten im Projekt oder in anderen Projekten auftreten, von denen die Timeline abhängig ist.<br></p> </li> 
         </ul> 
         <ul> 
         <li> <p><strong>Nur Automatisch</strong>: Die Projekt-Timeline wird jede Nacht aktualisiert. Sie wird nicht sofort aktualisiert, nachdem Änderungen vorgenommen wurden.<br>Sie können diese Option auswählen, wenn täglich im Projekt oder in anderen Projekten, von denen die Timeline abhängig ist, viele Änderungen vorgenommen werden. Beachten Sie jedoch, dass Sie diese Einstellung ausgewählt haben, da das Projekt nicht gleichzeitig mit den Änderungen aktualisiert wird.<br></p> </li> 
         </ul> 
         <ul> 
         <li> <p><strong>Nur manuell</strong>: Die Projekt-Timeline wird nur aktualisiert, wenn Sie die Option zum Neuberechnen von Zeitleisten auswählen, wie unter <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Projektzeitpläne neu berechnen</a>.<br></p> </li> 
         </ul> <p>Sie können diese Option auswählen, wenn Sie gleichzeitig viele Änderungen am Projekt vornehmen und möchten, dass die Timeline-Neuberechnung erfolgt, nachdem alle Änderungen vorgenommen wurden (und nicht nach jeder einzelnen Änderung).</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Zeitplan</strong> </td> 
         <td> <p>Wählen Sie einen Zeitplan für Ihre Vorlage aus. Dies wird zum Zeitplan des Projekts, das anhand dieser Vorlage erstellt wird. Dieser Zeitplan sollte mit dem für die meisten Personen übereinstimmen, die an dem Projekt arbeiten. Sie müssen einen Zeitplan erstellen, bevor Sie ihn einer Vorlage zuweisen können.<br>Weitere Informationen zum Erstellen von Zeitplänen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Zeitplan erstellen</a>. <br>Wenn Sie keine benutzerdefinierten Zeitpläne in Ihrem System erstellt haben, wird der Standardzeitplan ausgewählt. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Zeitlimit für Benutzer</strong> </td> 
         <td> <p>Bestimmt, ob die Zeitdauer des Primären Verantwortlichen einer Aufgabe die geplanten Aufgabendaten anpasst. Wenn Sie die Vorlage an ein vorhandenes Projekt anhängen und die Vorlage für dieses Feld eine andere Einstellung hat als das Projekt, bleibt die Einstellung für das Projekt unverändert. Die Standardoption für diese Einstellung für eine neue Vorlage ist dieselbe wie für die Projektanvoreinstellung auf Systemebene. </p> <p>Weitere Informationen zu den Projektvoreinstellungen auf Systemebene finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projektvoreinstellungen konfigurieren</a>. </p> <p>Informationen dazu, wie sich diese Einstellung auf die Aufgabendaten in einem Projekt auswirkt, finden Sie unter <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Projekte bearbeiten</a>.<br>Wählen Sie aus den folgenden Optionen aus:<br></p> 
         <ul> 
         <li> <p><strong>Benutzerzeitlimit in Aufgabendauern berücksichtigen</strong>: Wenn Sie diese Option auswählen, werden die geplanten Termine der Projektaufgaben, die mit dieser Vorlage erstellt wurden, entsprechend der Zeitspanne des Primären Aufgabenempfängers angepasst, wenn die Zeitspanne während der Aufgabendauer abgelaufen ist. </p> </li> 
         <li> <p><strong>Ignorieren der Benutzerzeit in der Aufgabendauer</strong>: Wenn Sie diese Option auswählen, bleiben die geplanten Termine der Aufgaben für das anhand dieser Vorlage erstellte Projekt wie ursprünglich geplant, auch wenn der Primäre Verantwortliche der Aufgabe während der Dauer der Aufgabe über eine Zeitverzögerung verfügt. </p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Ressourcenstufenmodus</strong> </td> 
         <td> <p>Wählen Sie aus den folgenden Optionen aus:<br></p> 
         <ul> 
         <li> <p><strong>Manuell</strong>: Sie müssen Ihre Ressourcen manuell auf das aus dieser Vorlage erstellte Projekt überprüfen (dies ist die Standardeinstellung).</p> </li> 
         <li> <p><strong>Automatisch:</strong> Workfront legt die Ressourcen für das künftige Projekt fest. <br>Weitere Informationen zur Ressourcenebene finden Sie unter <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md" class="MCXref xref">Level Resources in Gantt Chart </a>. </p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Risiko</strong> </td> 
         <td> <p>Definieren Sie das Risiko der auf dieser Vorlage basierenden Projekte. Das Risiko ist nur ein Indikator dafür, wie riskant ein Projekt sein kann. Sie können die Ausführung Ihrer Projekte je nach Risikograd priorisieren.<br>Wählen Sie aus den folgenden Risikostufen aus:<br></p> 
         <ul> 
         <li> <p><strong>Sehr niedrig</strong> </p> </li> 
         <li> <p><strong>Niedrig</strong> </p> </li> 
         <li> <p><strong>Mittel</strong> </p> </li> 
         <li> <p><strong>Hoch</strong> </p> </li> 
         <li> <p><strong>Sehr hoch</strong> </p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Ressourcenpools</strong> </td> 
         <td> <p>Geben Sie die mit der Vorlage verknüpften Ressourcen-Pools an. Ressourcen-Pools sind Sammlungen von Benutzern, die zum Abschluss eines Projekts gleichzeitig benötigt werden. Weitere Informationen zu Ressourcen-Pools finden Sie unter <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Ressourcen-Pools - Übersicht </a>.</p> <p> <p><b>NOTIZ</b>

   Wenn Sie Vorlagen stapelweise bearbeiten, werden in diesem Feld nur die Ressourcen-Pools angezeigt, die für alle ausgewählten Vorlagen gelten. Wenn die ausgewählten Vorlagen keine gemeinsamen Ressourcen-Pools aufweisen, ist dieses Feld leer. Die Ressourcen-Pools, die Sie hier angeben, überschreiben die einzelnen Ressourcen-Pools der Vorlagen.</p> </p> </td>
   </tr>
       <tr> 
         <td role="rowheader"><strong>Art der Filterstunde</strong> </td> 
         <td> <p>Beachten Sie Folgendes:</p> <p>Auswählen <strong>Nein</strong> , um alle projektspezifischen Stundentypen für das zukünftige Projekt verfügbar zu machen. (Dies ist die Standardauswahl)</p> <p>Oder</p> <p>Auswählen <strong>Ja</strong> , um nur eine Untergruppe der projektspezifischen Stundentypen für das zukünftige Projekt verfügbar zu machen, wählen Sie dann die Stundentypen aus, die verfügbar gemacht werden sollen. (Halten Sie die Umschalttaste gedrückt, um mehrere Stundentypen auszuwählen.)</p> <p>Wenn Sie diese Option auswählen, stehen nur die ausgewählten Stundentypen zur Verfügung, die bei der Protokollierung von Stunden im Projekt (oder bei Aufgaben und Problemen im Projekt) ausgewählt werden. Sie müssen mindestens einen Stundentyp auswählen. Wenn Sie diese Option wählen und keine Stundentypen auswählen, werden alle Stundentypen für das Projekt zur Verfügung gestellt.</p> <p>Dieselbe Stundentyp muss auf der Ebene der einzelnen Benutzer ausgewählt werden, damit der Benutzer diese Stundenoptionen im Projekt sehen kann. </p> <p>Weitere Informationen zum Definieren von Stundentypen auf Benutzerebene finden Sie im Abschnitt . <a href="../../../timesheets/create-and-manage-timesheets/log-time.md#understa" class="MCXref xref">Protokollzeit</a> in <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Protokollzeit</a>.</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Validierungsprozess</strong> </td> 
         <td> <p>Wählen Sie den Validierungsprozess aus, den Sie mit der Vorlage verknüpfen möchten. Ihr Workfront-Administrator oder ein Benutzer mit Administratorzugriff auf Genehmigungsprozesse muss die Projektgenehmigungsverfahren auf System- oder Gruppenebene definieren, bevor Sie sie mit einer Vorlage verknüpfen können. Weitere Informationen zum Erstellen von Genehmigungsprozessen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Erstellen eines Genehmigungsprozesses für Arbeitselemente</a>.</p> <p>Beachten Sie beim Hinzufügen von Validierungsprozessen Folgendes: </p> 
         <ul> 
         <li>In der Liste werden nur aktive Validierungsprozesse angezeigt. </li> 
         <li> <p>Systemweite und gruppenspezifische Validierungsprozesse werden in der Liste angezeigt. Ein Validierungsprozess, der einer anderen Gruppe als der Vorlage zugeordnet ist, wird nicht in der Liste angezeigt.</p> <p><b>WICHTIG</b>

   Wenn sich die mit der Vorlage verknüpfte Gruppe ändert, wird der gruppenspezifische Validierungsprozess zu einem Validierungsprozess für die einmalige Verwendung. Weitere Informationen dazu, wie sich Änderungen an der Projektgruppe oder Änderungen im Genehmigungsprozess auf die Validierungseinstellungen auswirken, finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">Auswirkungen von Änderungen am Gruppen- und Genehmigungsprozess auf zugewiesene Genehmigungsprozesse</a>. </p> </li>
   <li> <p>Wenn Sie einen Validierungsprozess für die einmalige Verwendung hinzugefügt haben, wird dieser in diesem Feld als "Benutzerdefiniert"angezeigt. Weitere Informationen finden Sie unter <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit</a>. </p> 
         </li> 
         <li> <p>Bei der Massenbearbeitung von Vorlagen gibt es die folgenden Szenarien:</p> 
         <ul> 
            <li> <p>Wenn Sie Vorlagen aus derselben Gruppe auswählen, werden in diesem Feld sowohl Validierungsprozesse auf Systemebene als auch auf Gruppenebene angezeigt.</p> </li> 
            <li> <p>Wenn Sie Vorlagen aus unterschiedlichen Gruppen auswählen, werden in diesem Feld nur Validierungsprozesse auf Systemebene angezeigt.</p> </li> 
            <li> <p>Wenn an eine Vorlage ein Validierungsprozess für die einmalige Verwendung angehängt ist, wird sie durch die von Ihnen ausgewählte Systemebene ersetzt. </p> </li> 
         </ul> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Erinnerungsbenachrichtigung</strong> </td> 
         <td>Wählen Sie die Erinnerungsbenachrichtigung aus, die mit dem künftigen Projekt verknüpft werden soll. Sie müssen Erinnerungsbenachrichtigungen für Projekte konfigurieren, damit dieses Feld während der Bearbeitung einer Vorlage angezeigt wird. <br>Weitere Informationen zum Konfigurieren von Erinnerungsbenachrichtigungen finden Sie unter <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Einrichten von Erinnerungsbenachrichtigungen</a>.</td> 
       </tr> 
       </tbody> 
      </table>

1. (Optional) Fahren Sie je nach den zu ändernden Informationen mit der Bearbeitung der folgenden Abschnitte fort.\
   Oder
1. Klicken Sie auf **Speichern**.

### Einstellungen für die Aufgabe {#task-settings}

Sie können die Standardeinstellungen definieren, die mit allen neuen Aufgaben verknüpft werden sollen, wenn Sie sie zu einem Projekt hinzufügen, das aus der Vorlage erstellt wird.

Informationen dazu, wie sich diese Einstellungen auf die Erstellung neuer Aufgaben auswirken, finden Sie unter [Übersicht über Aufgaben erstellen](../../../manage-work/tasks/create-tasks/create-tasks-overview.md).

1. Beginnen Sie mit der Bearbeitung Ihrer Vorlage wie oben beschrieben.
1. Im **Vorlage bearbeiten** Feld, klicken Sie auf **Aufgabeneinstellungen**.

   ![](assets/edit-template-box-tax-settings-section.png)

1. Im **Standardgenehmigungsverfahren für Aufgaben** Wählen Sie den Validierungsprozess aus, den Sie allen neuen Aufgaben zuweisen möchten, wenn Sie sie zu einem Projekt hinzufügen, das mit dieser Vorlage erstellt wurde. Sie müssen einen Genehmigungsprozess für Aufgaben erstellen, bevor Sie ihn mit Aufgaben verknüpfen können. In der Liste werden nur aktive Validierungsprozesse angezeigt. Weitere Informationen zum Erstellen von Genehmigungsprozessen finden Sie unter [Erstellen von Validierungsprozessen](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
1. Im **Benutzerdefinierter Forms-Task Standard** Wählen Sie das benutzerdefinierte Formular oder die Formulare aus, die Sie mit allen neuen Aufgaben verknüpfen möchten, wenn Sie sie zu einem Projekt hinzufügen, das mit dieser Vorlage erstellt wurde. Sie müssen die benutzerdefinierten Formulare erstellen, bevor sie in diesem Feld ausgewählt werden können. In der Liste werden nur aktive benutzerdefinierte Formulare angezeigt. Weitere Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Erstellen benutzerdefinierter Forms](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). Sie können bis zu zehn benutzerdefinierte Formulare mit einer Aufgabe verknüpfen.
1. (Optional) Wählen Sie **Verwenden Sie den Arbeitsaufwand, um die geplante Aufgabe automatisch zu berechnen.** , wenn Sie die Verwaltung des Aufgabenaufwands aktivieren möchten, indem Sie im Projekt, das anhand der Vorlage erstellt wurde, &quot;Arbeitsaufwand&quot;anstelle von &quot;Geplante Stunden&quot;verwenden.
1. (Bedingt und optional) Wenn Sie &quot;Arbeitsaufwand verwenden&quot;ausgewählt haben, um die geplante Aufgabe automatisch zu berechnen, klicken Sie auf das Dropdown-Menü, um den Prozentsatz für die einzelnen Stufen des Arbeitsaufwands zu aktualisieren. Die folgenden Prozentwerte sind die Standardwerte:

   | Arbeitsaufwand | Prozentwert |
   |---|---|
   | Klein | 25 % |
   | Mittel | 50 % |
   | Groß | 75 % |

   Informationen zur Verwendung von &quot;Work Effort&quot;zur Verwaltung von Aufgaben für Projekte finden Sie unter [Übersicht über den Arbeitsaufwand](../../../manage-work/tasks/task-information/work-effort.md).

1. (Optional) Fahren Sie je nach den zu ändernden Informationen mit der Bearbeitung des folgenden Abschnitts fort.

   Oder

   Klicken Sie auf **Speichern**.

### Problemeinstellungen {#issue-settings}

Durch Bearbeiten der Problemeinstellungen können Sie verhindern, dass Benutzer Probleme inline in das zukünftige Projekt einfügen, das aus der Vorlage erstellt wird.

1. Beginnen Sie mit der Bearbeitung Ihrer Vorlage wie oben beschrieben.
1. Im **Vorlage bearbeiten** Feld, klicken Sie auf **Problemeinstellungen**.

   ![](assets/edit-template-box-issue-settings-section.png)

1. (Optional) Deaktivieren Sie die **Benutzern erlauben, Probleme inline hinzuzufügen** -Option. Sie ist standardmäßig aktiviert.

   Wenn Sie diese Option deaktivieren, können Benutzer beim Erstellen des Projekts aus der Vorlage keine Probleme inline zum Projekt oder den Aufgaben im Abschnitt Probleme hinzufügen.

   >[!TIP]
   >
   >Deaktivieren Sie diese Option, wenn Sie Benutzer dazu zwingen möchten, die Felder für neue Probleme oder die benutzerdefinierten Formulare auszufüllen, die neuen Problemen zugeordnet sind.

   Wenn Sie diese Option deaktivieren, können Benutzer mit der Berechtigung, dem aus der Vorlage erstellten Projekt Probleme hinzuzufügen, dies über die Schaltfläche Neues Problem oder eine mit dem Projekt verknüpfte Anforderungswarteschlange tun.

   Weitere Informationen zum Konfigurieren von Problemeinstellungen für Projekte finden Sie unter [Problemeinstellungen](../../../manage-work/projects/manage-projects/edit-projects.md#issue) im Artikel [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

   Informationen zum Erstellen von Problemen bei Projekten finden Sie unter [Erstellen von Problemen](../../../manage-work/issues/manage-issues/create-issues.md).

1. (Optional) Fahren Sie je nach den zu ändernden Informationen mit der Bearbeitung des folgenden Abschnitts fort.

   Oder

   Klicken Sie auf **Speichern**.

### Zugriff {#access-preview}

1. Beginnen Sie mit der Bearbeitung Ihrer Vorlage wie oben beschrieben.
1. Im **Vorlage bearbeiten** Feld, klicken Sie auf **Zugriff**.

   ![](assets/edit-template-box-access-section.png)

   Der Zugriff, den Sie für Ihre Vorlage angeben, wird zum Zugriff der mit dem Projekt verknüpften Benutzer, wenn die Vorlage zum Erstellen eines Projekts verwendet wird.

   Geben Sie Folgendes an: **Zugriff** Informationen für die Vorlage:

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
       <tr> 
         <td role="rowheader"><strong>Wenn jemand einer Aufgabe zugewiesen ist</strong> </td> 
         <td> <p>Wählen Sie aus <strong>Ansicht</strong>, <strong>Beitragen,</strong> oder <strong>Verwalten</strong> Zugriff auf eine Aufgabe. Der einer Aufgabe zugewiesene Benutzer erhält automatisch diesen Zugriff auf die Aufgabe. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Gewähren Sie außerdem Zugriff auf das Projekt</strong> </td> 
         <td> <p> Wählen Sie aus <strong>Ansicht</strong>, <strong>Beitragen</strong>oder <strong>Verwalten</strong> Zugriff auf das Projekt. Der einer Aufgabe zugewiesene Benutzer erhält automatisch auch diesen Zugriff auf das Projekt. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Wenn jemand einem Problem zugewiesen ist</strong> </td> 
         <td> <p>Wählen Sie aus <strong>Ansicht</strong>, <strong>Beitragen,</strong> oder <strong>Verwalten</strong> Zugriff auf ein Problem. Dem einem Problem zugewiesenen Benutzer wird automatisch dieser Zugriff auf das Problem gewährt. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Gewähren Sie außerdem Zugriff auf das Projekt</strong> </td> 
         <td> <p> Wählen Sie aus <strong>Ansicht</strong>, <strong>Beitragen</strong>oder <strong>Verwalten</strong> Zugriff auf das Projekt. Der einem Problem zugewiesene Benutzer erhält automatisch auch diesen Zugriff auf das Projekt. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Wenn ein Benutzer eine Anforderung sendet: Gewähren Sie ihm Zugriff</strong> </td> 
         <td> <p> Wählen Sie aus <strong>Ansicht</strong>, <strong>Beitragen</strong>oder <strong>Verwalten</strong> Zugriff auf die Anfrage. Wenn sie eine Anfrage an das Projekt senden, erhalten sie diesen Zugriff auf die von ihnen gesendete Anfrage. Weitere Informationen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Problem freigeben </a>.</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Personen desselben Unternehmens erben dieselben Berechtigungen für alle Anforderungen</strong> </td> 
         <td> <p>Wählen Sie dieses Feld aus, wenn Sie möchten, dass Personen desselben Unternehmens denselben Zugriff auf alle Anforderungen des Projekts haben, unabhängig davon, ob sie sie gesendet haben oder nicht.</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Wenn jemand Zugriff auf dieses Projekt erhält: Gewähren Sie ihm Zugriff auf ...</strong> </td> 
         <td> <p>Wählen Sie die Zugriffsoptionen aus, die Benutzer für das Projekt haben sollen, wenn das Projekt für sie freigegeben ist. Wählen Sie die spezifischen Optionen für den Zugriff aus, sofern sie als <strong>Viewer</strong>, <strong>Mitarbeiter</strong>oder <strong>Führungskräfte</strong> wenn Sie das Projekt für sie freigeben. </p> </td> 
       </tr> 
       </tbody> 
      </table>

1. (Optional) Fahren Sie je nach den zu ändernden Informationen mit der Bearbeitung der folgenden Abschnitte fort.

   Oder

   Klicken Sie auf **Speichern**.

   Ihre Änderungen werden für diese Vorlage gesendet.

   Wenn Sie diese Vorlage zum Erstellen eines Projekts verwenden, werden alle diese Einstellungen an das neue Projekt übertragen.


## Stapelweises Bearbeiten von Vorlagen

Sie können Vorlagen stapelweise bearbeiten und alle zugehörigen Informationen gleichzeitig aktualisieren.

So bearbeiten Sie Vorlagen stapelweise:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront.

1. Klicks **Vorlagen**.
1. Wählen Sie mehrere Vorlagen in der Liste aus.
1. Klicks **Bearbeiten**.

   Die **Vorlagen bearbeiten** wird geöffnet.

   ![](assets/edit-templates-in-bulk-box-nwe-350x327.png)

1. Klicken Sie auf die Abschnitte auf der linken Seite, um alle ausgewählten Vorlagen zu bearbeiten.

   Weitere Informationen zum Bearbeiten von Informationen zu Vorlagen finden Sie im Abschnitt [Vorlagen bearbeiten](#edit-a-template) in diesem Artikel beschrieben.

1. Klicken Sie auf **Änderungen speichern**.

   Alle von Ihnen vorgenommenen Änderungen sind nun in allen ausgewählten Vorlagen sichtbar.

## Aufgaben zu einer Vorlage hinzufügen

Nachdem Sie Ihre Vorlage erstellt und die Vorlageninformationen bearbeitet haben, können Sie ihr Aufgaben hinzufügen.

Das Hinzufügen von Aufgaben zu einer Vorlage ähnelt dem Hinzufügen von Aufgaben zu einem Projekt.

Weitere Informationen zum Hinzufügen von Aufgaben zu einem Projekt finden Sie unter [Erstellen von Aufgaben in einem Projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Wenn Sie einer Vorlage Aufgaben hinzufügen, ändern sich die Dauer der Vorlage und die Start- und Endtage der Vorlage entsprechend. Informationen zu den Start- und Fertigungstagen der Vorlage und der Vorlagenaufgaben finden Sie unter [Übersicht über Start- und Endtage in einer Vorlage](../../../manage-work/projects/create-and-manage-templates/overview-of-start-completion-day-on-template.md).

## Hinzufügen zusätzlicher Elemente zu einer Vorlage

Nachdem Sie Ihre Vorlage erstellt und die Vorlageninformationen bearbeitet haben, können Sie ihr weitere Elemente hinzufügen. Die Elemente, die Sie hinzufügen, stehen für das Projekt zur Verfügung, wenn Sie es aus der Vorlage erstellen.

Das Hinzufügen der folgenden Elemente zu einer Vorlage entspricht dem Hinzufügen zu einem Projekt:

* Dokumente
* Risiken

  Weitere Informationen zum Erstellen von Risiken finden Sie unter [Erstellen und Bearbeiten von Risiken für Projekte](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md#create)  im Artikel [Erstellen und Bearbeiten von Risiken für Projekte](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

* Genehmigungsprozesse

  Informationen zum Verknüpfen von Genehmigungsprozessen mit der Arbeit finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

* Abrechnungssätze

  Weitere Informationen zum Außerkraftsetzen der Abrechnungsraten für ein Projekt finden Sie unter [Übersicht über die Außerkraftsetzung der Abrechnungsraten von Auftragsrollen und die Berechnung des Umsatzes eines Projekts](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* Ausgaben

  Weitere Informationen zur Hinzufügung von Ausgaben finden Sie unter [Verwalten von Projektausgaben](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* Themengruppen und Warteschlangenthemen

  Weitere Informationen zum Hinzufügen von Themengruppen und Warteschlangenthemen zu einem Projekt oder einer Vorlage finden Sie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Sie können die folgenden Elemente zu den Aufgaben in der Vorlage hinzufügen:

* Dokumente
* Ausgaben

  Weitere Informationen zur Hinzufügung von Ausgaben finden Sie unter [Verwalten von Projektausgaben](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* Genehmigungen

  Weitere Informationen zum Verknüpfen von Genehmigungen mit der Arbeit finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).


## Aktivieren oder Deaktivieren einer Vorlage

Sie können eine Vorlage deaktivieren, wenn Benutzer sie nicht finden und keine Projekte daraus erstellen können sollen. Sie können keine deaktivierte Vorlage an Projekte anhängen und sie auch nicht zum Erstellen eines Projekts verwenden.

Deaktivierte Vorlagen wirken sich nicht auf bestehende Projekte aus, die mit ihnen erstellt wurden.

So deaktivieren Sie eine Vorlage:

1. Gehen Sie zu einer aktiven Vorlage und klicken Sie auf die Schaltfläche **Mehr** ![](assets/qs-more-icon-on-an-object.png) Menü neben dem Vorlagennamen und klicken Sie auf **Deaktivieren**.

   ![](assets/deactivate-template-link-in-more-menu.png)

   Die Vorlage ist nicht mehr aktiv und Benutzer können sie nicht mehr finden, Projekte daraus zu erstellen.
1. (Optional) Um die Vorlage zu aktivieren, klicken Sie auf die Schaltfläche **Mehr** ![](assets/qs-more-icon-on-an-object.png) Menü neben dem Vorlagennamen und klicken Sie auf **Aktivieren**.

   Die Vorlage ist jetzt aktiv und kann an Projekte angehängt oder zum Erstellen von Projekten verwendet werden.

