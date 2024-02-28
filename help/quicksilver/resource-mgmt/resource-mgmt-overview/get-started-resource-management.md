---
content-type: overview
product-area: resource-management
navigation-topic: resource-management-overview
title: Erste Schritte mit der Ressourcenverwaltung
description: Mit Resource Management können Sie Ihr System so konfigurieren, dass die Verwendung Ihrer Ressourcen auf der Grundlage ihrer Verfügbarkeit genau vorhergesagt wird, sodass die erforderliche Arbeit rechtzeitig und im Budget abgeschlossen wird.
author: Alina
feature: Resource Management
exl-id: b10ef503-60ea-4450-b63e-b2918e9bcc11
source-git-commit: c80d9b0b7eb2a638af9e0a11ca3038ed99ecf1ee
workflow-type: tm+mt
source-wordcount: '1167'
ht-degree: 0%

---

# Erste Schritte mit der Ressourcenverwaltung

<!-- Audited: 12/2023 -->

<!--
<p>(NOTE: DO NOT DELETE THIS ARTICLE. MANY ARTICLES MENTIONING RES MANAGEMENT ARE AND STILL SHOULD / WILL BE LINKED TO IT.) </p>
<p>(NOTE: Alina: ***As functionality is removed from Legacy and added to Res Planning - this will be continually updated: remove the Legacy Res Planning when that functionality is removed from the system.) </p>
</div>
-->

Mit Resource Management können Sie Ihr System so konfigurieren, dass die Verwendung Ihrer Ressourcen auf der Grundlage ihrer Verfügbarkeit genau vorhergesagt wird, sodass die erforderliche Arbeit rechtzeitig und im Budget abgeschlossen wird.

## Überblick über die Ressourcenverwaltung in Adobe Workfront

&quot;Ressourcenverwaltung&quot;bezieht sich auf alle Aktivitäten, die vom Adobe Workfront-Administrator, vom Ressourcenmanager und vom Projekteigentümer zur Planung (Ressourcen- oder Szenario-Planung) und Planung (Workload Balancer) einer Organisation durchgeführt werden, und weist ihnen die benötigten Ressourcen unter Berücksichtigung ihrer Verfügbarkeit zu. Darüber hinaus bezieht sich die Ressourcenverwaltung auch auf die Anzeige von Informationen über die geplante und die tatsächliche Ressourcenzuweisung in einer Berichtsansicht (Nutzungsbericht).

Workfront verfügt über mehrere Tools zur Ressourcenverwaltung. Jedes Tool hat einen individuellen Umfang. Derzeit können Sie die folgenden Tools für die Ressourcenverwaltung in Workfront verwenden, je nachdem, in welcher Phase der Ressourcenverwaltung Sie sich befinden:

* Verwenden Sie die folgenden Tools, um zu planen, wie Ressourcen auf höherer Ebene zugewiesen werden, bevor die eigentliche Arbeit an Projekten beginnt:

   * **Der Ressourcen-Planer**: Sie können den Ressourcen-Planer in der ersten Phase des Ressourcenmanagements verwenden, um die Projektzeit Ihrer Ressourcen entsprechend der geplanten Verfügbarkeit zu planen. Während der Planung der Ressourcenphase können Sie Benutzer in Ressourcen-Pools organisieren und einem Projekt mehrere Ressourcen-Pools zuweisen.

     Weitere Informationen zur Ressourcenplanung finden Sie unter [Ressourcenplanung: Artikelindex](../../resource-mgmt/resource-planning/resource-planning-overview.md).

   * **Der Szenario-Planer**: Hierbei handelt es sich um eine übergeordnete Ressourcenplanung, mit der Sie sie über mehrere Initiativen hinweg verwalten können, die sich über einen Ein-, Drei- oder Fünfjahresplan erstrecken und mehrere Projekte umfassen können. Sie können das beste Szenario nutzen, um die Verfügbarkeit und Ihr Budget optimal zu nutzen.

     Für den Szenario-Planer ist zusätzlich zur Workfront-Lizenz eine separate Lizenz erforderlich. Weitere Informationen zum Workfront-Szenario-Planer finden Sie unter [Übersicht über den Szenario-Planer](../../scenario-planner/scenario-planner-overview.md).

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when more functionality is added, maybe we add that we recommend to start here if this is available for them?!) </p>   
     -->

* Verwenden Sie das folgende Tool, um die tatsächliche Arbeit (Aufgaben und Probleme) zu planen oder Ressourcen zuzuweisen:

   * **Der Lastenausgleich**: Dies gehört zu einer Phase der Ressourcenverwaltung auf niedrigerer Ebene, in der Sie Ihre Ressourcen der eigentlichen Arbeit (Aufgaben und Probleme) zuweisen können, die sie ausführen müssen, basierend auf der Zeitdauer, die zum Abschließen der Ressourcen erforderlich ist, und deren Verfügbarkeit. Mithilfe des Workload Balancer können Sie Benutzern tatsächliche Aufgaben zuweisen, die derzeit nicht zugewiesen sind oder Auftragsrollen zugewiesen sind.

     Weitere Informationen zum Workfront Balancer finden Sie unter [Der Lastenausgleich: Artikelindex](../../resource-mgmt/workload-balancer/workload-balancer.md).

<!--

  * **Scheduling** (deprecated <span class="preview">and removed from the Preview environment</span>): Refers to assigning actual work to users by matching the job roles assigned to the tasks and issues with the job roles they can fulfill, or assigning actual work to users on tasks and issues which are currently unassigned. This happens at a lower-level in the process of managing resources, where you can assign your resources to the actual work (tasks and issues) that they must fulfill, according to the hours needed in the project plan to fulfill them.  

     For more information about resource scheduling, see the section [Resource Scheduling](../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md).

    >[!CAUTION]
    >
    >
    >We are no longer supporting the Resource Scheduling tools and they will be removed from Workfront in **January 2023**. We recommend that you use the Workload Balancer for scheduling your resources. 
    >
    >
    >* For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).
    >
    >
    >* For more information about the timeline for removing the Resource Scheduling tools and replacing them with the Workload Balancer, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

-->
* Verwenden Sie das folgende Tool, um die veranschlagten, geplanten und tatsächlichen Zuweisungen für mehrere Projekte zu analysieren:

   * **Nutzungsbericht**: Verwenden Sie diesen Bericht, um die Nutzung der Ressourcen für Projekte anzuzeigen. Sie können die geplanten, geplanten und tatsächlichen Zuweisungen für Ihre Projekte und deren Auswirkungen auf die Kosten und Einnahmen der Projekte vergleichen.

     Weitere Informationen zum Nutzungsbericht finden Sie unter [Informationen zur Ressourcenauslastung anzeigen](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Die Komponenten des Resource Management-Prozesses

>[!NOTE]
>
>Die Ressourcenverwaltung ist in Workfront nie ein stagnierender Prozess. Wenn sich der Zeitplan Ihrer Projekte, die Verfügbarkeit Ihrer Benutzer oder ihre Rollen ändern, müssen Sie die Informationen über Ihre Ressourcen, deren Zuweisung und deren Zuordnung zu Projekten, Aufgaben und Problemen kontinuierlich anpassen.

Die Ressourcenverwaltung in Workfront umfasst die folgenden Etappen:

* **Konfiguration**: Als Systemadministrator, Ressourcenmanager oder Projekteigentümer müssen Sie bestimmte Felder und Objekte in Ihrer Workfront-Instanz konfigurieren, bevor Sie Ihre Ressourcen verwalten. Weitere Informationen zu den Voraussetzungen für die Ressourcenverwaltung in Workfront finden Sie im Abschnitt [Voraussetzungen für eine genaue Ressourcenverwaltung](#prerequisites-for-accurate-resource-management) in diesem Artikel beschrieben.\
  Zusätzlich zu Projekten mit Arbeitselementen müssen Sie die folgenden Elemente in Workfront konfigurieren:

   * Benutzende\
     Weitere Informationen zum Erstellen von Benutzern finden Sie im Artikel [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   * Aufgabengebiete\
     Weitere Informationen zum Erstellen von Aufgabenrollen finden Sie im Artikel [Erstellen und Verwalten von Vorgangsrollen](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

   * Zeitpläne\
     Weitere Informationen zum Erstellen von Zeitplänen finden Sie im Artikel [Zeitplan erstellen](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   * Projektpräferenzen

     >[!TIP]
     >
     >Nur ein System- oder Gruppenadministrator kann die Projekteinstellungen für Ihr System oder Ihre Gruppe ändern.

     Weitere Informationen zum Definieren von Projekteinstellungen finden Sie im Artikel [Systemweite Projektvoreinstellungen konfigurieren](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * Ressourcenpools

     Weitere Informationen zum Erstellen von Ressourcen-Pools finden Sie unter [Erstellen von Ressourcen-Pools](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

   * Voreinstellungen für die Ressourcenverwaltung

     Als System müssen Sie entscheiden, wie Workfront die Benutzerverfügbarkeit auf Systemebene berechnet, unabhängig davon, ob der Benutzerzeitplan oder der Standardzeitplan Ihres Systems verwendet wird.

     Weitere Informationen finden Sie unter [Voreinstellungen für die Ressourcenverwaltung konfigurieren](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **Ressourcenzuweisung**: Als Ressourcen-Manager oder Projekteigentümer können Sie die Ressourcenzuordnung für Ihre Projekte definieren und Arbeiten zuweisen. Für diesen Schritt können Sie die geschätzte Zuordnung Ihrer Ressourcen mithilfe des Ressourcen-Planers oder des Szenario-Planers verwalten und den Benutzern im Lastenausgleich die tatsächliche Arbeit zuweisen.

  Weitere Informationen zur Ressourcenplanung und -zuweisung finden Sie in den folgenden Abschnitten:

   * [Ressourcenplanung: Artikelindex](../../resource-mgmt/resource-planning/resource-planning-overview.md)
   * [Adobe Workfront-Szenario-Planer](../../scenario-planner/scenario-planning.md)
   * [Der Lastenausgleich: Artikelindex](../../resource-mgmt/workload-balancer/workload-balancer.md)

<!--
* **Resource scheduling**: After generally planning for resources to use on your projects at a high level, you can start assigning work items (tasks and issues) to users based on their job roles using the Workload Balancer.

  For more information, see [Workload Balancer overview](../workload-balancer/overview-workload-balancer.md). 
-->

* **Analyse**: Als Ressourcen-Manager, Projekt-Eigentümer oder Personen-Manager überprüfen Sie den Nutzungsbericht, um zu verstehen, wie die budgetierten und geplanten Zuweisungen Ihrer Ressourcen mit den tatsächlichen vergleichen. Überprüfen Sie die Informationen nach Stunden, Kosten oder Umsatz. Weitere Informationen zum Bericht &quot;Nutzung&quot;finden Sie unter [Informationen zur Ressourcenauslastung anzeigen](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Zugriff auf Ressourcen, die mithilfe der Ressourcen-Management-Tools in Workfront angezeigt und verwaltet werden müssen

Die folgenden Benutzer haben Zugriff auf die Tools für die Ressourcenverwaltung in Workfront:

Sie müssen einer der folgenden Benutzer sein und über die folgenden Zugriffsberechtigungen und Zugriffsberechtigungen für Ressourcen-Management-Tools verfügen:

* Der Systemadministrator.
* Ein Benutzer mit einer Planungslizenz.

  Ein Benutzer mit einer Work-Lizenz kann den Workload-Balancer eines Projekts verwenden und Zuweisungen und Zuordnungen verwalten.

  Zusätzlich zur Lizenz für Work oder höher müssen Sie über Folgendes verfügen, um spezifische Tools für die Ressourcenverwaltung zu verwenden:

   * Zugriff auf die Ressourcenverwaltung bearbeiten (nicht erforderlich für Zuweisungen im Arbeitslastausgleich)
   * Zugriff auf Finanzdaten bearbeiten, um Kosteninformationen im Ressourcenplaner anzuzeigen
   * Zugriff auf Finanzdaten anzeigen, um Kosten- und Umsatzinformationen im Nutzungsbericht anzuzeigen (nur Benutzer mit einer Planungslizenz)

* Tragen Sie zu oder höheren Berechtigungen bei, die Zuweisungen für die Projekte enthalten, für die Sie Ressourcen verwalten möchten.

<!--
* Designated as a Resource Manager for projects to use the Scheduling tool (the Scheduling tool is deprecated).

  >[!TIP]
  >
  >You do not have to be a Resource Manager to use the Resource Planner, Scenario Planner, or the Workload Balancer. 
-->

Informationen zum benötigten Zugriff auf Budgetressourcen finden Sie im Artikel [Erforderlicher Zugriff auf Budgetmittel](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

Informationen zum Zugriff, der für die Verwaltung von Ressourcen im Workload Balancer erforderlich ist, finden Sie unter [Zugriff erforderlich für die Verwaltung von Ressourcen im Workload Balancer](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

## Voraussetzungen für eine genaue Ressourcenverwaltung  {#prerequisites-for-accurate-resource-management}

Sie müssen eine Reihe von Anforderungen erfüllen, bevor Sie die Tools zur Ressourcenverwaltung in Workfront effizient verwenden können.

Informationen zu den Anforderungen für die einzelnen Ressourcenverwaltungstools in Workfront finden Sie unter folgenden Themen:

* Der Abschnitt [Voraussetzungen für die Arbeit im Ressourcenplaner](../../resource-mgmt/resource-planning/get-started-resource-planner.md#prerequisites-for-working-in-the-resource-planner) im Artikel [Übersicht über den Ressourcenplaner](../../resource-mgmt/resource-planning/get-started-resource-planner.md).
  <!--remove this at production: * The section "Prerequisites" in the article [Get started with Resource Scheduling](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).-->
* Der Abschnitt [Best Practices für die Verwendung des Lastenausgleichs](../../resource-mgmt/workload-balancer/overview-workload-balancer.md#best-practices-for-using-the-workload-balancer) im Artikel [Übersicht über den Lastenausgleich](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
* [Erforderlicher Zugriff auf Budgetressourcen in Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).
* [Zugriff erforderlich für die Verwaltung von Ressourcen im Workload Balancer](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted and replaced with the links to each prerequisites instead) </p>
<p> We recommend that the following settings exist before starting to manage resources for your organization: </p>
<ul>
<li> You must have users in the system who have active accounts. </li>
<li> You must assign a Plan or a Worker license to the users whose work allocation you want to manage. <note type="note">
Although you can assign work to a Reviewer or a Requestor, they cannot complete it.
<br>We recommend against assigning work to Reviewers or Requestors. For information about access levels in Workfront, see
<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref" xrefformat="{para}">Access levels overview</a>.
</note></li>
<li> You must have job roles configured in the system.<br>For information about adding job roles to Workfront, see the article <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" xrefformat="{para}">Create and manage job roles</a>.</li>
<li> (Optional) If you want to budget cost for your work, your job roles and your users must also have rates associated with them.<br></li>
<li> You must associate at least one job role with your users. </li>
<li> You must specify a valid value for the FTE field of all users when you use the User's Schedule instead of The Default Schedule in your Resource Management system preferences. <br>For information about editing users to ensure they have a job role, FTE, or cost associated with them, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" xrefformat="{para}">Edit a user's profile</a>. For information about editing the Resource Management preferences in your system, see <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref" xrefformat="{para}">Configure Resource Management preferences</a>.</li>
<li>You must associate accurate schedules with your users and they should include schedule exceptions.<br>For information about creating and editing schedules, see the article <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" xrefformat="{para}">Create a schedule</a>.</li>
<li>The Time Off calendar of the users must be up to date. </li>
<li> <p>The following is recommended for the Resource Planner when applying the Project and Role views: </p>
<ul>
<li> <p>You must associate projects with Resource Pools.<br>For information about associating projects with Resource Pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md" class="MCXref xref" xrefformat="{para}">Associate resource pools with projects and templates</a>.</p> </li>
</ul> </li>
<li> <p>Your must designate a Resource Manager on your projects and they must have the correct access to budget resources when using the Scheduling tools. </p> <p>For information about the access needed to budget resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref" xrefformat="{para}">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> </li>
<li> <p>You must assign the tasks and issues in your system to job roles, teams, or users.</p> </li>
<li>You must specify a valid value for Planned Hours and Duration for all tasks in your system.<br>For information about Planned Hours, see the article <a href="../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref" xrefformat="{para}">Planned Hours overview</a>.<br>For information about Duration, see the article <a href="../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref" xrefformat="{para}">Overview of Task Duration and Duration Type</a>.</li>
</ul>
</div>
-->
