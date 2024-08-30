---
product-area: resource-management
navigation-topic: resource-pools
title: Verknüpfen von Ressourcenpools mit Projekten und Vorlagen
description: Ressourcen-Pools sind Sammlungen von Benutzern, die Ihnen bei der Verwaltung von Ressourcen in Adobe Workfront helfen.
author: Lisa
feature: Resource Management
exl-id: bbfe8257-ff02-4f06-9763-3f2ae4871c9d
source-git-commit: a9d507bfcc0a602e71bcdd3142d63cc40175ebf4
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 1%

---

# Verknüpfen von Ressourcen-Pools mit Projekten und Vorlagen


<!-- drafted for bulk editing projects: keep this in yellow till this releases to ALL customers - May 1, 2023

Also - take out all the references to Preview and Prod at prod final
-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->


<!--
<p>The sections about how to add resource pools to templates, projects are duplicated from the articles listed in those sections (Editing Projects, Creating a Template, etc).</p>
<p>***I decided to keep these steps here, though, because it's hard to parse through those much lunger articles for just updating this one field.)</p>
-->

Ressourcen-Pools sind Sammlungen von Benutzern, die Ihnen bei der Verwaltung von Ressourcen in Adobe Workfront helfen.

Nachdem Sie Ressourcen-Pools erstellt haben, können Sie diese mit Projekten oder Vorlagen verknüpfen, damit Sie Ihre Ressourcen später für die Projekte einsetzen können.

Es wird empfohlen, die Ressourcen-Pools im Voraus zu erstellen, sie mit Projekten zu verknüpfen und die Ressourcen vor dem Projektstart zu finanzieren.

Informationen zu Ressourcen-Pools finden Sie unter [Überblick über Ressourcen-Pools](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

Informationen zum Erstellen von Ressourcen-Pools finden Sie unter [Erstellen von Ressourcen-Pools](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

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
       <p>Aktuell: Pro und höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf die Ressourcenverwaltung bearbeiten, einschließlich Zugriff auf Ressourcen-Pools verwalten</p> <p>Zugriff auf Projekte, Vorlagen und Benutzer bearbeiten</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Verwalten von Berechtigungen für die Projekte, Vorlagen und Benutzer, mit denen Sie die Ressourcenpools verknüpfen möchten</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ressourcen-Pools mit einem Projekt oder einer Vorlage verknüpfen

Sie können Ressourcen-Pools mit einer Vorlage auf dieselbe Weise verknüpfen wie Ressourcen-Pools mit einem Projekt. In diesem Artikel wird beschrieben, wie Sie Ressourcenpools mit Projekten verknüpfen können.

1. Wechseln Sie zu einem Projekt, klicken Sie auf das Symbol **Mehr** ![](assets/more-icon.png) neben dem Projektnamen und klicken Sie dann auf **Bearbeiten**.

1. Klicken Sie auf **Projekteinstellungen**.

1. Geben Sie den Namen eines Ressourcenpools in das Feld **Ressourcenpools** ein und wählen Sie ihn dann aus der Liste aus, wenn er angezeigt wird.\
   Sie können mehrere Ressourcen-Pools mit einem Projekt oder einer Vorlage verknüpfen.

   ![](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. Klicken Sie auf **Speichern**.

Weitere Informationen zum Bearbeiten und Verknüpfen eines Projekts mit Ressourcen-Pools finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

Weitere Informationen zum Bearbeiten einer Vorlage und zum Verknüpfen mit Ressourcen-Pools finden Sie unter [Bearbeiten von Projektvorlagen](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Ressourcenpools mit mehreren Projekten oder Vorlagen stapelweise verknüpfen

Sie können mehrere Projekte oder Vorlagen stapelweise bearbeiten und dieselben Ressourcen-Pools mit allen gleichzeitig verknüpfen.

Sie können Ressourcenpools mit Vorlagen auf die gleiche Weise verknüpfen wie Ressourcenpools mit Projekten.

So verknüpfen Sie Ressourcenpools stapelweise mit mehreren Projekten:

1. Gehen Sie zu einer Projektliste.
1. Wählen Sie mehrere Projekte aus und klicken Sie dann oben in der Liste auf das Symbol **Bearbeiten** ![](assets/edit-icon.png) .

1. Klicken Sie auf **Einstellungen**.
1. Geben Sie den Namen eines Ressourcenpools in das Feld **Ressourcenpools** ein und wählen Sie ihn dann aus der Liste aus, wenn er angezeigt wird.\
   Sie können den Projekten oder Vorlagen mehrere Ressourcen-Pools zuweisen.

   >[!NOTE]
   >
   >* Wenn Sie Vorlagen stapelweise bearbeiten, werden in diesem Feld nur die Ressourcen-Pools angezeigt, die für alle ausgewählten Vorlagen gelten. Wenn die ausgewählten Vorlagen keine gemeinsamen Ressourcen-Pools aufweisen, ist dieses Feld leer. Die Ressourcen-Pools, die Sie hier angeben, überschreiben die einzelnen Ressourcen-Pools der Projekte oder Vorlagen.
   >
   >* Wenn Sie Projekte stapelweise bearbeiten, gibt es einen Indikator &quot;Mehrere Werte&quot;, wenn die ausgewählten Projekte unterschiedliche Ressourcen-Pools aufweisen. Wenn Sie Ressourcenpools stapelweise für Projekte hinzufügen, werden alle Pools zum ausgewählten Projekt hinzugefügt, wodurch die ursprünglichen Ressourcenpools überschrieben werden.

   ![add_resource_pools_to_multiple_projects.png](assets/add-resource-pools-to-multiple-projects-350x358.png)

1. Klicken Sie auf **Änderungen speichern**.\
   Wenn Ihre Ressourcen-Pools mit Ihren Projekten oder Vorlagen verknüpft sind, können Sie im Ressourcenplaner Benutzerzuweisungen für Ihre Projekte einplanen.\
   Weitere Informationen zum Ressourcenplaner finden Sie unter [Ressourcenplaner - Übersicht](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Weitere Informationen zum Bearbeiten von Projekten in großen Mengen finden Sie im Abschnitt &quot;Projekte stapelweise bearbeiten&quot;in [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

Weitere Informationen zum stapelweisen Bearbeiten von Vorlagen finden Sie im Abschnitt &quot;Vorlagen stapelweise bearbeiten&quot;in [Projektvorlagen bearbeiten](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
