---
product-area: projects;templates
navigation-topic: plan-a-project
title: Ressourcen-Manager für ein Projekt oder eine Vorlage bestimmen
description: Sie können Ressourcen-Manager für ein Projekt bestimmen, um anzugeben, wer für die Verwaltung der Ressourcen für das Projekt verantwortlich ist.
author: Alina
feature: Work Management
exl-id: ae2a89e7-8049-4ee6-9b28-ce247d3f2a6f
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 0%

---

# Ressourcen-Manager für ein Projekt oder eine Vorlage bestimmen

<!--
<p This article might have to be deleted when the Resource Manager field/ requirement will be forever removed from the system; right now it's still a requirement for Scheduler - January 2023/p>
-->

<!-- remove Prod and Prev references with Prod release - Jan 2023-->

Sie können Ressourcen-Manager für ein Projekt bestimmen, um anzugeben, wer für die Verwaltung der Ressourcen für das Projekt verantwortlich ist. Es handelt sich um ein Informationsfeld, das keinerlei Verbindung zu Ressourcen-Management-Tools aufweist.

<!-- drafted for res scheduling deprecation blurb for preview release
Designating Resource Managers for a project is a prerequisite for using the Scheduling tools in Adobe Workfront, in the Production environment.
  
>[!CAUTION]  
>  
>  
> <span class="preview">Some of the information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span>  
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span>  
>  
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../../resource-mgmt/workload-balancer/workload-balancer.md).</span>  
>  
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

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
   <td> <p>Edit access to Projects and Templates</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project or template</p> 
   
   <p><b>NOTE</b>
   
   Users who are added as Resource Managers to a project or a template immediately gain Manage permissions on the project or the template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte und Vorlagen bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für ein Projekt oder eine Vorlage verwalten</p>

<p><b>NOTIZ</b>

Benutzer, die einem Projekt oder einer Vorlage als Ressourcen-Manager hinzugefügt werden, erhalten sofort Verwaltungsberechtigungen für das Projekt oder die Vorlage</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td>
</tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Überlegungen zu Ressourcen-Managern

>[!NOTE]
>
>Resource Manager ist keine Auftragsrolle. Es handelt sich um ein Feld, das für ein Projekt oder eine Vorlage verfügbar ist und das/die Sie manuell aktualisieren können.

* Sie können bis zu 30 Benutzer als Ressourcen-Manager für ein einzelnes Projekt oder eine einzelne Vorlage festlegen.

<!--
* In the Production environment,designating Resource Managers on projects is a prerequisite to allowing users to schedule resources for work on the project when using the Scheduling tools.

  For information about resource scheduling, see [Resource Scheduling](../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md). 

  <span class="preview">Scheduling tools have been removed from the Preview environment.</span>

* Designating Resource Managers on projects is not a prerequisite to allowing users to schedule resources for work using the Workload Balancer.

  For information about the Workload Balancer, see [Workload Balancer overview](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md). 

 -->

* Sie können Teams oder Gruppen nicht als Ressourcen-Manager festlegen. Sie können Benutzer nur als Ressourcen-Manager festlegen.

* Die Benutzer, die Sie für ein Projekt oder eine Vorlage als Ressourcen-Manager festlegen, werden nicht automatisch Teil des Projektteams.

  Weitere Informationen zu Projektteams finden Sie unter [Verwalten des Projektteams](../../../manage-work/projects/planning-a-project/manage-project-team.md).

* Sie können Ressourcen-Manager für Projekte oder Projektvorlagen bestimmen. Wenn Sie Resource Manager für eine Projektvorlage bestimmen, werden alle Benutzer, die Sie auf der Vorlage als Ressourcen-Manager festlegen, automatisch zu Resource Manager für alle Projekte, die mit dieser Vorlage erstellt werden.
* Sie können das Feld Ressourcen-Manager in den folgenden Bereichen anzeigen:

   * Beim Bearbeiten eines Projekts, wie in diesem Artikel beschrieben.
   * Beim Bearbeiten einer Vorlage, wie in diesem Artikel beschrieben.
   * Beim Erstellen von Projekt- oder Vorlagenberichten. Informationen zum Erstellen von Berichten finden Sie unter [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
   * Beim Erstellen oder Anpassen einer Projekt- oder Vorlagenansicht für eine Liste. Weitere Informationen finden Sie unter [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* Sie können Ressourcen-Manager schnell zu mehreren Projekten oder Vorlagen hinzufügen oder daraus entfernen, indem Sie das Feld Ressourcen-Manager zu einer Liste oder einem Projekt hinzufügen und dieses Feld mithilfe der Inline-Bearbeitung bearbeiten.

## Ressourcen-Manager für ein Projekt bestimmen

1. Führen Sie einen der folgenden Schritte aus:

   * Um Ressourcen-Manager zu einem einzelnen Projekt hinzuzufügen, gehen Sie zu dem Projekt, für das Sie einen oder mehrere Ressourcen-Manager bestimmen möchten, und klicken Sie dann auf die Schaltfläche **Mehr Menü** neben dem Projektnamen und **Bearbeiten .**

   * Um Ressourcen-Manager mehreren Projekten gleichzeitig hinzuzufügen, navigieren Sie zu einer Liste von Projekten, wählen Sie die Projekte aus, für die Sie einen oder mehrere Ressourcen-Manager bestimmen möchten, und klicken Sie dann auf **Bearbeiten**.

     Vorhandene Ressourcen-Manager werden nicht aus den Projekten entfernt, die Sie bearbeiten. Alle Benutzer, die Sie auf diese Weise hinzufügen, werden zusätzlich zu vorhandenen Ressourcen-Managern als Ressourcen-Manager für das Projekt hinzugefügt.

   * Um Ressourcen-Manager zu einem neuen Projekt hinzuzufügen, beginnen Sie mit der Erstellung eines neuen Projekts.

     Weitere Informationen zum Erstellen eines Projekts finden Sie unter [Projekt erstellen](../../../manage-work/projects/create-projects/create-project.md).

1. Im **Übersicht** im Dialogfeld &quot;Projekt bearbeiten&quot;auf die Schaltfläche **Ressourcen-Manager** -Feld.
1. Geben Sie den Namen des Benutzers ein, den Sie als Ressourcen-Manager für das Projekt hinzufügen möchten, und klicken Sie dann auf den Namen, wenn er in der Liste angezeigt wird.

   Wiederholen Sie diesen Schritt, um mehrere Ressourcen-Manager für das Projekt hinzuzufügen.

1. Klicks **Änderungen speichern**.

## Ressourcen-Manager für eine Vorlage bestimmen

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront.

1. Klicks **Vorlagen**.

1. Führen Sie einen der folgenden Schritte aus:

   * Um Ressourcen-Manager zu einer Vorlage hinzuzufügen, wechseln Sie zur Vorlage, in der Sie einen oder mehrere Ressourcen-Manager bestimmen möchten, und klicken Sie auf die Schaltfläche **Mehr Menü** neben dem Vorlagennamen und **Bearbeiten .**

   * Um Ressourcen-Manager mehreren Vorlagen gleichzeitig hinzuzufügen, wählen Sie aus einer Liste von Vorlagen die Vorlagen aus, für die Sie einen oder mehrere Ressourcen-Manager bestimmen möchten, und klicken Sie auf **Bearbeiten**.

     Vorhandene Ressourcen-Manager werden nicht aus den Vorlagen entfernt, die Sie bearbeiten. Alle Benutzer, die Sie auf diese Weise hinzufügen, werden zusätzlich zu vorhandenen Ressourcen-Managern als Ressourcen-Manager in der Vorlage hinzugefügt.

   * Um Resource Manager zu einer neuen Vorlage hinzuzufügen, klicken Sie auf **Neue Vorlage** und klicken Sie dann auf **Mehr Menü** neben dem Vorlagennamen und **Bearbeiten .**

1. Im **Übersicht** klicken Sie in der **Ressourcen-Manager** -Feld.
1. Geben Sie den Namen des Benutzers ein, den Sie als Ressourcen-Manager für die Vorlage hinzufügen möchten, und klicken Sie dann auf den Namen, wenn er in der Liste angezeigt wird.

   Wiederholen Sie diesen Schritt, um der Vorlage mehrere Ressourcen-Manager hinzuzufügen.

1. Klicks **Änderungen speichern**.
