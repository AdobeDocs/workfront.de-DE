---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Löschen und Deaktivieren von Zielen in Adobe Workfront-Zielen
description: Wenn Sie mit der Arbeit an einem Ziel beginnen und es in Ihrer Organisation irrelevant wird, empfehlen wir, es zu deaktivieren, anstatt es zu löschen. Durch das Deaktivieren eines Ziels werden seine historischen Informationen beibehalten und Sie können es zu einem späteren Zeitpunkt reaktivieren. Es kann jedoch manchmal sinnvoll sein, ein Ziel zu löschen, um die Zielliste genau zu halten.
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# Löschen und Deaktivieren von Zielen in Adobe Workfront-Zielen

Wenn Sie mit der Arbeit an einem Ziel beginnen und es in Ihrer Organisation irrelevant wird, empfehlen wir, es zu deaktivieren, anstatt es zu löschen. Durch das Deaktivieren eines Ziels werden seine historischen Informationen beibehalten und Sie können es zu einem späteren Zeitpunkt reaktivieren. Es kann jedoch manchmal sinnvoll sein, ein Ziel zu löschen, um die Zielliste genau zu halten.

## Zugriffsanforderungen

<!--drafted for P&P release: 

You must have the following:

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
   <td> <p>Zugriff auf Ziele oder höher bearbeiten</p> <p><b>NOTIZ</b>

<p>Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter:</p> 
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

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Sie müssen über Folgendes verfügen, bevor Sie beginnen können:

* Eine Layout-Vorlage, die den Bereich Ziele im Hauptmenü enthält.

## Ziele deaktivieren

Sie können ein Ziel deaktivieren, das nicht mehr relevant ist und in Zukunft möglicherweise reaktiviert werden soll.

* [Überlegungen zum Deaktivieren von Zielen](#considerations-when-deactivating-goals)
* [Ziele deaktivieren](#deactivate-goals)

### Überlegungen zum Deaktivieren von Zielen

Beachten Sie beim Deaktivieren von Zielen Folgendes:

* Sie können Ziele nur im Status Aktiv deaktivieren. Informationen zum Aktivieren eines Ziels finden Sie unter [Aktivieren von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/activate-goals.md).

   >[!TIP]
   >
   >Ziele können im Status Entwurf nicht deaktiviert werden.

* Workfront unterbricht die Berechnung des Fortschritts deaktivierter Ziele.
* Inaktive Ziele werden im Abschnitt &quot;Diagramme&quot;von Workfront-Zielen nicht mehr angezeigt oder werden nicht mehr berücksichtigt. Weitere Informationen zu Workfront-Zieldiagrammen finden Sie unter [Überprüfen Sie Diagramme, um die Trends beim Zielfortschritt in Adobe Workfront-Zielen zu verstehen.](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goal-graphs.md).

   <!--* The Check-in section. For information about the Check-in page, see [Update goal progress in Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md). -->

* Sie können keine Aktualisierungen zu deaktivierten Zielen mehr vornehmen.
* Sie können Informationen zum Ziel und seiner Ausrichtung bearbeiten.
* Sie können ein zuvor deaktiviertes Ziel reaktivieren.

### Ziele deaktivieren

<!--
Deactivating goals differs depending on which environment you use.

### Deactivate goals in the Production environment


1. Go to the goal that you want to deactivate.

   For example, go to the Goal List and click the name of a goal.

   The Goal Details panel opens on the right.

   >[!TIP]
   >
   >You can open goals from any sections of Workfront Goals.

1. Click the **More icon** ![](assets/more-icon.png), then click **Deactivate**.

   ![](assets/deactivate-goal-highlighted.png)

   The goal status changes to Inactive. 

1. Click the **X** icon in the upper-right to close Goal Details.
-->

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts auf **Ziele**.

   Die Zielliste wird angezeigt.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Optional) Ändern Sie Ihre Filter so, dass nur aktive Ziele angezeigt werden.

   Informationen zum Filtern von Informationen in Workfront-Zielen finden Sie unter [Informationen in Adobe Workfront-Zielen filtern](../goal-management/filter-information-wf-goals.md).

1. Klicken Sie auf ein aktives Ziel.

   Die Zielseite wird geöffnet.

   ![](assets/goal-page-unshimmed.png)

1. Klicken Sie auf **Mehr** Menü ![](assets/more-icon.png) rechts neben dem Zielnamen, und klicken Sie dann auf **Deaktivieren**.

1. Das Ziel wird deaktiviert und sein Status wird inaktiv.

## Löschen von Zielen

Sie können Ziele löschen, die nicht mehr oder möglicherweise nie relevant sind.

* [Überlegungen zum Löschen von Zielen](#considerations-when-deleting-goals)
* [Löschen von Zielen](#delete-goals)

### Überlegungen zum Löschen von Zielen {#considerations-when-deleting-goals}

* Sie können Ziele in jedem Status löschen, einschließlich geschlossener Ziele.
* Gelöschte Ziele können nicht wiederhergestellt werden.
* Die mit dem Ziel verknüpften Aktivitäten &quot;Ergebnisse&quot;und &quot;Manueller Fortschritt&quot;werden ebenfalls gelöscht.
* Projekte, die mit Zielen verknüpft sind, werden nicht gelöscht, aber ihre Verknüpfung mit dem Ziel wird entfernt.

### Löschen von Zielen

<!--
Deleting  goals differs depending on which environment you use.

#### Delete goals in the Production environment

1. Go to the goal that you want to delete.

   For example, go to the Goal List and click a goal.

   The Goal Details panel opens on the right. 

1. Click the **More icon** ![](assets/more-icon.png), then click **Delete**.

   ![](assets/delete-goal-highlighted.png)

1. Click **Yes, delete**.

   The goal is removed from the Goal List and cannot be recovered.
-->

1. Klicken Sie auf das Symbol Hauptmenü . ![](assets/main-menu-icon.png) Klicken Sie oben rechts auf **Ziele**.

   Die Zielliste wird angezeigt.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. Klicken Sie auf den Namen eines Ziels. Dadurch wird die Zielseite geöffnet.
1. Klicken Sie auf **Mehr** Menü ![](assets/more-icon.png) rechts neben dem Zielnamen, und klicken Sie dann auf **Löschziel**, dann **Löschen**.

   Das Ziel sowie seine Aktivitäten und Ergebnisse werden ebenfalls gelöscht und können nicht wiederhergestellt werden. Projekte, die mit dem Ziel oder den untergeordneten Zielen verknüpft waren, werden nicht gelöscht.


