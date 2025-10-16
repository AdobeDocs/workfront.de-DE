---
product-area: projects;templates
navigation-topic: plan-a-project
title: Ressourcenmanager für ein Projekt oder eine Vorlage bestimmen
description: Sie können Ressourcenmanager für ein Projekt bestimmen, um anzugeben, wer für die Verwaltung der Ressourcen im Projekt zuständig ist.
author: Alina
feature: Work Management
exl-id: ae2a89e7-8049-4ee6-9b28-ce247d3f2a6f
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 1%

---

# Ressourcenmanager für ein Projekt oder eine Vorlage bestimmen

<!--
<p This article might have to be deleted when the Resource Manager field/ requirement will be forever removed from the system; right now it's still a requirement for Scheduler - January 2023/p>
-->

<!-- remove Prod and Prev references with Prod release - Jan 2023-->

Sie können Ressourcenmanager für ein Projekt bestimmen, um anzugeben, wer für die Verwaltung der Ressourcen im Projekt zuständig ist. Dies ist ein Informationsfeld, das nicht mit Ressourcenverwaltungstools verbunden ist.

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

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte und Vorlagen bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für das Projekt oder die Vorlage</p>

</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

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
   <td> <p>Plan </p> </td> 
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
</table>-->

## Überlegungen zu Ressourcen-Managern

>[!NOTE]
>
>Ressourcenmanager ist kein Aufgabengebiet. Es ist ein Feld, das für ein Projekt oder eine Vorlage verfügbar ist und das Sie manuell aktualisieren können.

* Sie können bis zu 30 Benutzer als Ressourcenmanager für ein einzelnes Projekt oder eine Vorlage festlegen.

<!--
* In the Production environment,designating Resource Managers on projects is a prerequisite to allowing users to schedule resources for work on the project when using the Scheduling tools.

  For information about resource scheduling, see [Resource Scheduling](../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md). 

  <span class="preview">Scheduling tools have been removed from the Preview environment.</span>

* Designating Resource Managers on projects is not a prerequisite to allowing users to schedule resources for work using the Workload Balancer.

  For information about the Workload Balancer, see [Workload Balancer overview](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md). 

 -->

* Es ist nicht möglich, Teams oder Gruppen als Ressourcenmanager zu bestimmen. Sie können nur Benutzer als Ressourcenmanager festlegen.

* Die Benutzer, die Sie als Ressourcenmanager für ein Projekt oder eine Vorlage festlegen, werden nicht automatisch Teil des Projektteams.

  Informationen zu Projektteams finden Sie unter [Verwalten des Projektteams](../../../manage-work/projects/planning-a-project/manage-project-team.md).

* Sie können Ressourcen-Manager für Projekte oder für Projektvorlagen bestimmen. Wenn Sie Ressourcenmanager für eine Projektvorlage festlegen, werden alle Benutzer, die Sie als Ressourcenmanager für die Vorlage festlegen, automatisch Ressourcenmanager für alle Projekte, die mithilfe dieser Vorlage erstellt werden.
* Sie können das Feld Ressourcen-Manager in den folgenden Bereichen anzeigen:

   * Beim Bearbeiten eines Projekts, wie in diesem Artikel beschrieben.
   * Beim Bearbeiten einer Vorlage, wie in diesem Artikel beschrieben.
   * Beim Erstellen von Projekt- oder Vorlagenberichten. Informationen zum Erstellen von Berichten finden Sie [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
   * Beim Erstellen oder Anpassen eines Projekts oder einer Vorlagenansicht für eine Liste. Weitere Informationen finden Sie unter [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* Sie können Ressourcenmanager für mehrere Projekte oder Vorlagen schnell hinzufügen oder entfernen, indem Sie das Feld Ressourcenmanager zu einer Ansicht einer Liste oder eines Projekts hinzufügen und dieses Feld mithilfe der Inline-Bearbeitung bearbeiten.

## Ressourcenmanager für ein Projekt bestimmen

1. Führen Sie einen der folgenden Schritte aus:

   * Um Ressourcenmanager zu einem Projekt hinzuzufügen, gehen Sie zu dem Projekt, in dem Sie einen oder mehrere Ressourcenmanager bestimmen möchten, klicken Sie dann auf das **Mehr** neben dem Projektnamen und dann **Bearbeiten .**

   * Um Ressourcenmanager mehreren Projekten gleichzeitig hinzuzufügen, navigieren Sie zu einer Projektliste, wählen Sie die Projekte aus, für die Sie einen oder mehrere Ressourcenmanager festlegen möchten, und klicken Sie dann auf **Bearbeiten**.

     Vorhandene Ressourcenmanager werden nicht aus den Projekten entfernt, die Sie bearbeiten. Alle Benutzer, die Sie auf diese Weise hinzufügen, werden zusätzlich zu vorhandenen Ressourcenmanagern als Ressourcenmanager zum Projekt hinzugefügt.

   * Um Ressourcenmanager zu einem neuen Projekt hinzuzufügen, beginnen Sie mit der Erstellung eines neuen Projekts.

     Informationen zum Erstellen eines Projekts finden Sie unter [Erstellen eines Projekts](../../../manage-work/projects/create-projects/create-project.md).

1. Klicken Sie **Abschnitt**&#x200B;Übersicht“ im Dialogfeld Projekt bearbeiten in das Feld **Ressourcen-Manager**.
1. Geben Sie zunächst den Namen des Benutzers ein, den Sie als Ressourcen-Manager für das Projekt hinzufügen möchten, und klicken Sie dann auf den Namen, wenn er in der Liste angezeigt wird.

   Wiederholen Sie diesen Schritt, um mehrere Ressourcen-Manager für das Projekt hinzuzufügen.

1. Klicken Sie auf **Änderungen speichern**.

## Ressourcenmanager für eine Vorlage bestimmen

1. Klicken Sie auf **Hauptmenü**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.

1. Klicken Sie auf **Vorlagen**.

1. Führen Sie einen der folgenden Schritte aus:

   * Um Ressourcenmanager zu einer Vorlage hinzuzufügen, gehen Sie zu der Vorlage, in der Sie einen oder mehrere Ressourcenmanager festlegen möchten, klicken Sie dann auf das **Mehr Menü** neben dem Vorlagennamen und **Bearbeiten .**

   * Um Ressourcenmanager mehreren Vorlagen gleichzeitig hinzuzufügen, gehen Sie zu einer Liste von Vorlagen und wählen Sie die Vorlagen aus, in denen Sie einen oder mehrere Ressourcenmanager bestimmen möchten. Klicken Sie dann auf **Bearbeiten**.

     Vorhandene Ressourcen-Manager werden nicht aus den Vorlagen entfernt, die Sie bearbeiten. Alle Benutzer, die Sie auf diese Weise hinzufügen, werden zusätzlich zu den vorhandenen Ressourcen-Managern als Ressourcen-Manager zur Vorlage hinzugefügt.

   * Um Ressourcen-Manager zu einer neuen Vorlage hinzuzufügen, klicken Sie auf **Neue Vorlage** und klicken Sie dann auf das **Mehr** neben dem Vorlagennamen und anschließend **Bearbeiten .**

1. Klicken Sie **Abschnitt**&#x200B;Übersicht“ in das Feld **Ressourcen-Manager**.
1. Geben Sie zunächst den Namen des Benutzers ein, den Sie als Ressourcen-Manager für die Vorlage hinzufügen möchten, und klicken Sie dann auf den Namen, wenn er in der Liste angezeigt wird.

   Wiederholen Sie diesen Schritt, um der Vorlage mehrere Ressourcen-Manager hinzuzufügen.

1. Klicken Sie auf **Änderungen speichern**.
