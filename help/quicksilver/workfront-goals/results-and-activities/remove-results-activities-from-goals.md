---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Entfernen von Ergebnissen, Aktivitäten und Projekten aus Zielen in Adobe Workfront Goals
description: Sie können Ergebnisse, Aktivitäten und Projekte aus Zielen in Adobe Workfront-Zielen entfernen, wenn sie nicht mehr relevant sind.
author: Alina
feature: Workfront Goals
exl-id: 0e064dbd-6168-47b4-98ab-b5c0481e839e
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 0%

---

# Entfernen von Ergebnissen, Aktivitäten und Projekten aus Zielen in Adobe Workfront Goals

<!-- for goal redesign PRODUCTION RELEASE: Should this article be called "Remove or disconnect progress indicators from goals" when this is available to ALL progress indicators (including "disconnect goals")-- if yes, updte the title everywhere else where this is linked?
-->

Sie können Ergebnisse, Aktivitäten und Projekte aus Zielen entfernen, wenn sie nicht mehr relevant sind.

Informationen zum Erstellen von Zielen sowie zum Hinzufügen von Ergebnissen und Aktivitäten zu diesen finden Sie in den folgenden Artikeln:

* [Erstellen von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/create-goals.md)
* [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
* [Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Ergebnisse und Aktivitäten in Adobe Workfront-Zielen bearbeiten](../../workfront-goals/results-and-activities/edit-results-and-activities.md)

Ziele können auch auf übergeordnete Ziele ausgerichtet werden, sodass sie zu Kinderzielen werden. Kinderziele sind auch Fortschrittsindikatoren der übergeordneten Ziele.

Sie können die Ausrichtung zwischen Zielen entfernen, indem Sie die Verbindung zwischen ihnen entfernen. Weitere Informationen finden Sie unter [Entfernen der Zielausrichtung in Adobe Workfront-Zielen](../goal-alignment/remove-goal-alignment.md).

## Zugriffsanforderungen

<!--drafted - replace the table below with this one when P&P releases: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>
-->

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Pro oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Anforderung oder höher</p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe Workfront-Lizenzen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td> <p>Sie müssen eine zusätzliche Lizenz für die Adobe Workfront Goals erwerben, um auf die in diesem Artikel beschriebene Funktion zugreifen zu können. </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Voraussetzungen für die Verwendung von Workfront-Zielen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Ziele oder höher bearbeiten</p> <p><b>NOTIZ</b><p>Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Zugriff auf Adobe Workfront-Ziele gewähren</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> 
    <div> 
     <p>Berechtigungen für das Ziel verwalten</p> 
     <p>Informationen zum Freigeben von Zielen finden Sie unter <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Freigeben eines Ziels in Workfront-Zielen</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Sie müssen über Folgendes verfügen, bevor Sie beginnen können:

* Eine Layout-Vorlage, die den Bereich Ziele im Hauptmenü enthält.
* Ein Ziel mit Ergebnissen, Aktivitäten oder Projekten.

## Überlegungen zum Entfernen von Ergebnissen, Aktivitäten und Trennen von Projekten von Zielen

* Sie können Ergebnisse und Aktivitäten nur aus aktiven Zielen entfernen.
* Sie können Ergebnisse und Aktivitäten aus einem Ziel entfernen, indem Sie sie löschen. Gelöschte Ergebnisse und Aktivitäten können nicht wiederhergestellt werden.
* Wenn Sie das Ergebnis oder die Aktivität aus einem Ziel entfernen, wirkt sich der Fortschritt des entfernten Ergebnisses oder der Aktivität auf den Gesamtfortschritt des Ziels aus.
* Ein Projekt kann nicht aus einem Ziel gelöscht werden, es kann jedoch vom Ziel getrennt werden. Wenn Sie das Projekt vom Ziel trennen, wirkt sich der Prozentsatz des Projektabschlusses nicht mehr auf den Fortschritt des Ziels aus.

   Informationen darüber, wie Projekte den Zielfortschritt beeinflussen, finden Sie unter [Hinzufügen von Projekten zu Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

* Sie können ein Ergebnis oder eine Aktivität nicht aus einem Ziel entfernen und die Verbindung zu einem untergeordneten Ziel bzw. Projekt nicht trennen, wenn es sich um die letzte Fortschrittsanzeige für das Ziel handelt.
* Wenn ein Projekt aus dem Bereich &quot;Projekte&quot;gelöscht wird und es der letzte Fortschrittsindikator eines Ziels ist, wird das Ziel inaktiv.

## Ergebnisse und Aktivitäten aus Zielen löschen

Sie entfernen Ergebnisse und Aktivitäten aus einem Ziel, indem Sie sie löschen. Das Löschen von Ergebnissen und Aktivitäten aus einem Ziel ist identisch.

<!--
How you delete results and activities differs depending on the environment you use.

### Delete results and activities in the Production environment


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click **Results** to remove results or **Activities** to remove activities. 

1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result or activity name, then click **Delete** > **Yes, delete**.

   ![](assets/delete-result-goal-details-350x108.png)

   The result or activity is deleted and cannot be recovered. The percent complete of the goal updates to exclude the deleted activity or result.

-->

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke und klicken Sie auf **Ziele**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
   Dadurch wird der Workfront-Zielbereich geöffnet und die Zielliste wird standardmäßig angezeigt.

1. Klicken Sie auf den Namen eines Ziels, aus dem Sie Ergebnisse und Aktivitäten entfernen möchten.

   Dadurch wird die Zielseite geöffnet.

1. Klicken **Fortschrittsanzeigen** im linken Bereich.

1. Wählen Sie ein Ergebnis oder eine Aktivität aus und klicken Sie auf die Schaltfläche **Löschen** icon ![](assets/delete-icon.png) oben in der Liste.

1. Klicken **Löschen** , um den Löschvorgang zu bestätigen. Das Ergebnis oder die Aktivität wird gelöscht und kann nicht wiederhergestellt werden. Der prozentuale Abschluss des Ziels wird aktualisiert, um die gelöschte Aktivität oder das gelöschte Ergebnis auszuschließen.


## Entfernen von Projekten aus Zielen

<!--
Dsconnecting projects from goals differs depending on the environment you use.

### Disconnect projects from goals in the Production environment


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click the **right-pointing arrow** to the left of the Activities sections to expand it. 
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the project name, then click **Disconnect**.

   ![](assets/disconnect-project-goal-details-350x94.png)

   The project is disconnected from the goal. The percent complete of the goal updates to exclude the percent complete of the disconnected project.
-->


1. Klicken Sie auf **Hauptmenü** Symbol oben rechts und klicken Sie dann auf **Ziele**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Dadurch wird der Workfront-Zielbereich geöffnet und die Zielliste wird standardmäßig angezeigt.

1. Klicken Sie auf den Namen eines Ziels, aus dem Sie Ergebnisse und Aktivitäten entfernen möchten.

   Dadurch wird die Zielseite geöffnet.
1. Klicken **Fortschrittsanzeigen** im linken Bereich.
1. Wählen Sie ein Projekt aus und klicken Sie dann auf das **Trennen** icon ![](assets/disconnect-icon.png) oben in der Liste.
1. Klicken **Trennen** zur Bestätigung.

   Das Projekt ist nicht mehr mit dem Ziel verbunden. Der prozentuale Abschluss des Ziels wird aktualisiert, um das nicht verbundene Projekt auszuschließen.

