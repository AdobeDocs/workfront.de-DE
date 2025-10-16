---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Löschen und Deaktivieren von Zielen in Adobe Workfront Goals
description: Wenn Sie mit der Arbeit an einem Ziel beginnen und es in Ihrer Organisation irrelevant wird, empfehlen wir, es zu deaktivieren, anstatt es zu löschen. Wenn Sie ein Ziel deaktivieren, werden dessen historische Informationen beibehalten und Sie haben die Möglichkeit, das Ziel zu einem späteren Zeitpunkt erneut zu aktivieren. Es gibt jedoch Zeiten, in denen das Löschen eines Ziels sinnvoll sein kann, um die Zielliste korrekt zu halten.
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

# Löschen und Deaktivieren von Zielen in Adobe Workfront Goals

<!--Audited for P&P only: 10/2025-->

Wenn Sie mit der Arbeit an einem Ziel beginnen und es in Ihrer Organisation irrelevant wird, empfehlen wir, es zu deaktivieren, anstatt es zu löschen. Wenn Sie ein Ziel deaktivieren, werden dessen historische Informationen beibehalten und Sie haben die Möglichkeit, das Ziel zu einem späteren Zeitpunkt erneut zu aktivieren. Es gibt jedoch Zeiten, in denen das Löschen eines Ziels sinnvoll sein kann, um die Zielliste korrekt zu halten.

## Zugriffsanforderungen

>[!NOTE]
>
>Ihr Unternehmen könnte sich dafür entscheiden, weiterhin Adobe Workfront Goals zu verwenden, wenn es dieses Paket in der Vergangenheit gekauft hat. Weitere Informationen erhalten Sie von Ihrem Kundenbetreuer.
>
>Adobe Workfront Goals ist nicht mehr erhältlich.

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Adobe Workfront-Paket</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-Lizenz</td>
 <td>
 <p>Mitwirkender oder höher</p>
<p>Anfrage oder höher</p></td>
 </tr>
  <tr>
 <td role="rowheader">Konfiguration der Zugriffsebene</td>
 <td> <p>Zugriff auf Ziele bearbeiten</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objektberechtigungen</td>
 <td>
  <div>
  <p>Anzeigen von oder höheren Berechtigungen für das Ziel, um es anzuzeigen</p>
  <p>Verwalten von Berechtigungen für das Ziel, um es zu bearbeiten</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Systemadministratoren, muss eine Layout-Vorlage zugewiesen werden, die den Bereich Ziele im Hauptmenü enthält. </p>  
</td>
  </tr>
</tbody>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td>  
  </tr>
 <tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
  <p> New product requirement: Workfront</p>
 <p>Or</p>
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
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
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Ziele deaktivieren

Sie können ein Ziel deaktivieren, das nicht mehr relevant ist und das Sie in Zukunft möglicherweise erneut aktivieren möchten.

* [Überlegungen beim Deaktivieren von Zielen](#considerations-when-deactivating-goals)
* [Ziele deaktivieren](#deactivate-goals)

### Überlegungen zur Deaktivierung von Zielen

Beachten Sie beim Deaktivieren von Zielen Folgendes:

* Sie können Ziele nur in einem aktiven Status deaktivieren. Informationen zum Aktivieren eines Ziels finden Sie unter [Aktivieren von Zielen in Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).

  >[!TIP]
  >
  >Ziele mit dem Status Entwurf können nicht deaktiviert werden.

* Workfront stoppt die Berechnung des Fortschritts deaktivierter Ziele.
* Inaktive Ziele werden in den Workfront-Zielen im Abschnitt Diagramme nicht mehr angezeigt oder berücksichtigt. Weitere Informationen zu Workfront-Zieldiagrammen finden Sie unter [Überprüfen von Diagrammen zum Verständnis der Zielfortschrittstrends in Adobe Workfront-Zielen](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goal-graphs.md).

  <!--* The Check-in section. For information about the Check-in page, see [Update goal progress in Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md). -->

* Sie können keine Aktualisierungen mehr an deaktivierten Zielen vornehmen.
* Sie können Informationen über das Ziel und seine Ausrichtung bearbeiten.
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

1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Deactivate**.

   ![Deactivate goal](assets/deactivate-goal-highlighted.png)

   The goal status changes to Inactive. 

1. Click the **X** icon in the upper-right to close Goal Details.
-->

1. Klicken Sie oben rechts auf **Hauptmenü**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) und dann auf **Ziele**.

   Die Liste „Ziel“ wird angezeigt.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Optional) Ändern Sie Ihre Filter, um nur aktive Ziele anzuzeigen.

   Informationen zum Filtern von Informationen in Workfront Goals finden Sie unter [Filtern von Informationen in Adobe Workfront Goals](../goal-management/filter-information-wf-goals.md).

1. Klicken Sie auf ein aktives Ziel.

   Die Zielseite wird geöffnet.

   ![Zielseite](assets/goal-page-unshimmed.png)

1. Klicken Sie auf das **Mehr**-Menü ![Mehr-Symbol](assets/more-icon.png) rechts neben dem Zielnamen und klicken Sie dann auf **Deaktivieren**.

1. Das Ziel wird deaktiviert und sein Status wird zu Inaktiv.

## Ziele löschen

Sie können Ziele löschen, die nicht mehr relevant sind oder nie relevant sein werden.

* [Überlegungen beim Löschen von Zielen](#considerations-when-deleting-goals)
* [Ziele löschen](#delete-goals)

### Überlegungen beim Löschen von Zielen {#considerations-when-deleting-goals}

* Sie können Ziele in jedem Status löschen, einschließlich geschlossener Ziele.
* Gelöschte Ziele können nicht wiederhergestellt werden.
* Ergebnisse und manuelle Fortschrittsleistenaktivitäten, die mit dem Ziel verknüpft sind, werden ebenfalls gelöscht.
* Mit Zielen verknüpfte Projekte werden nicht gelöscht, aber ihre Verknüpfung mit dem Ziel wird entfernt.

### Ziele löschen

<!--
Deleting  goals differs depending on which environment you use.

#### Delete goals in the Production environment

1. Go to the goal that you want to delete.

   For example, go to the Goal List and click a goal.

   The Goal Details panel opens on the right. 

1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Delete**.

   ![Delete goal](assets/delete-goal-highlighted.png)

1. Click **Yes, delete**.

   The goal is removed from the Goal List and cannot be recovered.
-->

1. Klicken Sie oben rechts auf das Hauptmenüsymbol ![Hauptmenüsymbol](assets/main-menu-icon.png) und dann auf **Ziele**.

   Die Liste „Ziel“ wird angezeigt.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. Klicken Sie auf den Namen eines Ziels. Dadurch wird die Zielseite geöffnet.
1. Klicken Sie auf das **Mehr**-Menü ![Mehr-Symbol](assets/more-icon.png) rechts neben dem Zielnamen, klicken Sie dann auf **Ziel löschen** und dann auf **Löschen**.

   Das Ziel und seine Aktivitäten und Ergebnisse werden ebenfalls gelöscht und können nicht wiederhergestellt werden. Projekte, die mit dem Ziel oder den untergeordneten Zielen verknüpft waren, werden nicht gelöscht.


