---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Smart Assignments - Übersicht
description: Bei der Verwaltung von Aufgaben- und Problemzuweisungen können Sie mithilfe von Smart Assignments ermitteln, wer die Arbeit am besten erledigt. Smart-Zuweisungen sind Vorschläge, die Ihnen Adobe Workfront unterbreitet, wenn Sie Ressourcen Arbeitselemente auf der Grundlage eines Algorithmus zuweisen, der die am besten geeignete Ressource für den Auftrag bestimmt.
author: Lisa
feature: Work Management
exl-id: 8d17eff6-5ff0-4985-b575-4934a3bb7c0b
source-git-commit: 1211a441b542df49480d933d4c25b0c31ef0883d
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 0%

---

# Smart Assignments - Übersicht

<!--Audited: 07/2024-->

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die nur in der Vorschau-Umgebung verfügbar sind.</span>

<!--<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview"> This functionality will be removed from the Production environment for customers who enabled fast release with the 25.1 release in January 2025. For information about the 25.1 release, see [First Quarter 2025 release overview](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md). -->

Bei der Verwaltung von Aufgaben- und Problemzuweisungen können Sie mithilfe von Smart Assignments ermitteln, wer die beste Ressource ist, um die Arbeit abzuschließen.

Smart-Zuweisungen sind Vorschläge, die Ihnen Adobe Workfront unterbreitet, wenn Sie Ressourcen Arbeitselemente auf der Grundlage eines Algorithmus zuweisen, der die am besten geeignete Ressource für den Auftrag bestimmt. Smart-Zuweisungen können Benutzer, Aufgabengebiete oder Teams sein.

>[!NOTE]
>
>Bei der Empfehlung von Benutzern berücksichtigen Smart Assignments nicht die Verfügbarkeit der Benutzer. Ihre Verfügbarkeit entsprechend ihren Zeitplänen wirkt sich jedoch auf die geplanten und geplanten Termine von Aufgaben und Problemen aus, wenn diese zugewiesen werden. Weitere Informationen zu Zeitplänen finden Sie im Artikel [Erstellen eines Zeitplans](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Dieser Artikel enthält allgemeine Informationen zu Smart-Zuweisungen. Informationen zur Verwendung von Smart-Zuweisungen zum Zuweisen von Aufgaben und Problemen zu Benutzern finden Sie unter [Erstellen von Smart-Zuweisungen](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md).

## Smart Assignments - Übersicht

Beachten Sie beim Arbeiten mit Smart-Zuweisungen Folgendes:

<!--* <span class="preview">The algorithm works independently for tasks and issues. This means that the list of suggested users for issues might differ from the list of suggested users for a task because Workfront builds the lists according to criteria pertaining to issues and tasks separately. </span>-->
<!--not sure this is accurate: * Smart assignments do not recommend job roles or teams. Instead, they are suggestions of users who are best fit to complete a task or an issue. -->
* Die vorgeschlagenen Arbeitsaufträge sind immer aktive Benutzer, Aufgabengebiete oder Teams.
* Die zuerst aufgeführte Ressource sollte der Aufgabe am besten entsprechen.

## Suchen von Smart-Zuweisungsvorschlägen

Smart Assignments können in den folgenden Bereichen angezeigt werden, in denen Sie Aufgaben oder Probleme zuweisen können:

* Eine Problemliste oder ein Bericht in der Spalte „Zuweisungen“

  ![Spalte „Problemlistenzuweisungen“](assets/smart-assignments-issue-list.png)

* Aufgabenliste oder Bericht in der Spalte „Zuweisungen“

  ![Aufgabenlistenzuweisungen-Spalte](assets/smart-assignments-task-list.png)

* Eine Aufgabenkopfzeile im Feld Arbeitsaufträge

  ![Feld für Aufgabenkopfzeilenzuweisungen](assets/smart-assignments-task-header-nwe-350x302.png)

* Eine Anfragekopfzeile im Feld „Zuweisungen“

  ![Feld „Kopfzeilenzuweisungen für Probleme“](assets/smart-assignments-issue-header.png)

* Das Bedienfeld „Aufgaben- oder Problemzusammenfassung“ im Bereich „Zuweisungen“

  ![Bereich „Zusammenfassungsfeldzuweisungen“](assets/issue-assignments-summary-panel.png)

<!--* The Assignments field in the New Task box, when adding a task to a project

  ![](assets/smart-assignments-new-task-modal.png)-->

<!--this is not possible in the new home  - we have Summary there: 
* The Assignments field for an item listed in the Home area, when you open a task or issue

  ![](assets/smart-assignments-in-home-nwe-350x216.png)
-->

* Lastenausgleich im Bereich Diesem Bereich zugewiesen bei der Zuweisung einer Aufgabe oder eines Problems

  ![Bereich „Workload Balancer-Zuweisungen“](assets/smart-assignments-workload-balancer-bulk-assignments.png)

## Kriterien für intelligente Zuweisungen

<!--Smart assignments work differently for tasks than for issues.  -->

<!--### Smart assignments criteria for tasks

The task smart assignments calculation works in <span class="preview">two phases which use two different algorithms.</span>

<span class="preview">Depending on which algorithm finds the smart assignment, the assignments are listed under two separate sections in the Assignments field.</span> For information, see [Make smart assignments](/help/quicksilver/manage-work/tasks/assign-tasks/make-smart-assignments.md). 

![](assets/smart-assignments-task-list.png)

<div class="preview">

#### First phase of smart assignment calculation for tasks 

In the first phase of calculating smart assignments, Workfront calculates a similarity score for every assignment. 

>[!NOTE]
>
>The first phase of the smart assignments calculation does not apply to the following task areas:
>
>* Bulk Assignments in the Workload Balancer.
>* Connected cards on boards.


The calculation for the similarity score and the order in which the assignments are listed take into account the following:  

* A score of 100% is given to an existing assignment where the task, project, and portfolio names are identical to the task you're trying to assign. The project and portfolio names of the task of an existing assignment must also match the project and portfolio of the task you are trying to assign.   

* If only some of this information from other assignments matches on the existing tasks, the score might be lower than 100%.  

  For example, if you are assigning a task called "My second task" on a project called "My project" in a portfolio called "My portfolio" and you have an existing task called "My task" in another project called "My project" in a portfolio called "My portfolio", the user assigned to "My task" might get a score of 95% because the name of the existing task and the task you're trying to assign now are similar, but not identical.  
 
    >[!TIP]
    >
    >  Workfront looks for matches only in the Name fields of tasks, projects, and portfolios and not in any other fields. 

* An assignment could get a higher score when they are assigned to a lot of tasks in the system that have similar names. For example, if a team called "Development" is assigned to 50% of the tasks in the system containing "AI" in the name and you are now assigning another task with "AI" in the name, the score of the "Development" team is higher. In this case, the names of  projects and portfolios are not as important.  

* Taking into account this scoring system, the first 7 suggestions are listed as smart assignments, in the descending order of their scores. Assignments with scores lower than 40% do not display.  

* If several assignments have identical scores, they display in order of the date on which the assignments were made, starting from the most recent date.  

  For example, if Rick was assigned to a similar task earlier today and Jennifer was assigned to a similar task two days ago, Rick displays first.  

* Assignments identified in this phase are listed in the    **Suggested assignments**  section of the Assignments field for tasks. 

* If there are no matches using this calculation, the second phase of smart assignments starts which is calculated using a different algorithm.  

</div>

#### Second phase of smart assignment calculation for tasks-->

<!--If the first step of task smart assignments has found no matches,-->

Workfront berechnet Smart Assignments für Aufgaben auf die gleiche Weise wie für Probleme.

<!--For more information, see the section [Smart assignments criteria for tasks and issues](#smart-assignments-criteria-for-tasks-and-issues) in this article. -->

Die identifizierten Zuweisungen werden in den Abschnitten **Benutzer und Teams**, **Aufgabenrollenzuweisungen** und <span class="preview">**Tarifkartenrollen**</span> des Felds Zuweisungen aufgeführt. <span class="preview">Weitere Informationen zu Tarifkarten finden Sie unter [Tarifkarten verwalten](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md)</span>. <!--keep the rate cards roles in yellow after the release of assignments to Prod-->

<!--
### Smart assignments criteria for tasks and issues 

>[!NOTE]
>
>The following criteria applies for tasks only when the first phase of the task smart assignment calculation did not find any matches. For information, see the section [First phase of smart assignment calculation for tasks](#first-phase-of-smart-assignment-calculation-for-tasks) in this article. The following criteria always applies for issues, by default. -->

![Beispiel für intelligente Zuweisung](assets/smart-assignments-issue-header.png)

Benutzer werden in der Dropdown-Liste Smart Assignments empfohlen, basierend auf einer Kombination der folgenden Kriterien (aufgeführt in der Reihenfolge von Wichtig bis Unwichtig):

1. Benutzer, die in den letzten 30 Tagen von dem Benutzer, der die Zuweisung vorgenommen hat, anderen Arbeitselementen zugewiesen wurden. Die ersten 50 Benutzer, die diesen Kriterien entsprechen, werden angezeigt. Der Benutzer, der am häufigsten zugewiesen wird, wird zuerst angezeigt.

2. Wenn das Arbeitselement einem Team oder einer Funktion zugewiesen ist, wird die Liste der vorgeschlagenen Benutzer unter Berücksichtigung der vorhandenen Zuweisungen unten weiter gefiltert. In diesem Fall werden in der Liste der Vorschläge nur die folgenden Benutzer angezeigt:

   * Benutzer, deren Home-Team das Team ist, das dem Arbeitselement zugewiesen ist.
   * Benutzende, deren Primäre Funktion die dem Arbeitselement zugewiesene Funktion ist.

>[!TIP]
>
>* Wenn der Aufgabe oder dem Problem keine Rolle oder kein Team zugewiesen wurde, zeigt Workfront alle Benutzenden an, die in den letzten 30 Tagen zugewiesen wurden, bis zu 50.
>
>* Wenn Sie in den letzten 30 Tagen keine Zuweisungen vorgenommen haben, werden in der Liste „Smart-Zuweisungen“ nur Benutzer angezeigt, die entweder dem zugewiesenen Team oder dem Arbeitselement die Rolle zugewiesen haben.



<!--the commented out piece in the tip above was live before but I am not totally sure that smart assignments look at your team. I think they look JUST at the team/ role assigned to the work item; see this help site request for more info: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/62fd222200037eb87572c5b6ad6bf53e/overview -->
<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h3>Smart assignments criteria for the Production environment</h3>
<p>(NOTE: drafted,this was the case BEFORE we updated the logic in the WB - with the 21.4 release)</p>
</div>
<p>Smart assignments display on tasks and issues when the following conditions are met:</p>
<ul>
<li>The task or issue is subordinate to a parent task or issue that has a user, team, or job role currently assigned. </li>
</ul>
<p>Smart assignments display the top twenty recommendations based on a proprietary algorithm that uses your own team information.</p>
<p>Users are recommended in the smart assignments drop-down list based on a combination of the following criteria (listed in order from most important to least important):</p>
<ul>
<li>The user has the team assigned to the task or issue designated as their Home Team</li>
<li>The user is also assigned to the parent task</li>
<li>The user has the same primary job role as is currently assigned to the task or issue</li>
<li>The user has the team assigned to the parent task or issue designated as their Home Team</li>
<li>The user is associated with the same primary job role currently assigned to the parent task</li>
<li>The user is a member of the same team as the user who assigned the task or issue and the team is designated as their Home Team</li>
<li>The user is a member of the same Home Group as the user who is assigning the task or issue</li>
<li>The user has the same primary job role as the user who is assigning the task or issue.</li>
</ul>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Make smart assignments</h2>
<p>(NOTE:&nbsp;this was moved to its own article: make-smart-assignments.) </p>
<p>Smart assignments are available in most locations where you can make assignments in Workfront.</p>
<p>You can use smart assignments on tasks and issues that have previously been assigned to a job role or a team.</p> <note type="note">
You must have a Plan or a Work license and have at least Contribute permissions to a task or an issue to be able to make assignments to the task or the issue. You must have the Make Assignments option enabled in your permission level to make assignments.
</note>
<p>To use smart assignments:</p>
<ol>
<li value="1">Navigate to an issue or a task and click one of the following fields to edit them: <br>
<ul>
<li><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">The <strong>Assignments</strong> field in the task or issue header</p></li>
<li>The <strong>Assignments</strong> field of a task or issue list using in-line editing in a task or issue list. </li>
<li>The <strong>Assignee</strong> field after you have clicked <strong>Advanced</strong> from a task or an issue. </li>
</ul></li>
<li value="2"> <p>Place your cursor in the assignment field, and wait for two seconds, then the <strong>Suggestions</strong> list is displayed.</p> <p>Users displayed in this list are the smart assignment suggestions for the task or the issue.<br></p> <p> <img src="assets/nwe-smart-assignment-suggestions-350x160.png" style="width: 350;height: 160;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3"> <p>Select the user in the recommendations list by clicking their name. </p> <p>If there are no suggestions, the suggestion list does not open.</p> </li>
<li value="4">(Optional) If you do not want to use one of the recommended users from the smart assignments list, start typing the name of the desired user and select the name when it appears in the list.</li>
<li value="5">Click <strong>Enter</strong> to make the assignment. </li>
</ol>
</div>
-->
