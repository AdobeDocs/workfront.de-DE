---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Entfernen von Fortschrittsanzeigen aus Zielen in Adobe Workfront-Zielen
description: Sie können Ergebnisse, Aktivitäten und Projekte aus Zielen in Adobe Workfront-Zielen entfernen, wenn sie nicht mehr relevant sind.
author: Alina
feature: Workfront Goals
exl-id: 0e064dbd-6168-47b4-98ab-b5c0481e839e
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Entfernen von Fortschrittsanzeigen aus Zielen in Adobe Workfront-Zielen

<!-- for goal redesign PRODUCTION RELEASE: Should this article be called "Remove or disconnect progress indicators from goals" when this is available to ALL progress indicators (including "disconnect goals")-- if yes, updte the title everywhere else where this is linked?
-->

Sie können Ergebnisse, Aktivitäten und Projekte aus Zielen entfernen, wenn sie nicht mehr relevant sind.

Informationen zum Erstellen von Zielen und Hinzufügen von Ergebnissen und Aktivitäten zu Zielen finden Sie in den folgenden Artikeln:

* [Erstellen von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/create-goals.md)
* [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
* [Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Ergebnisse und Aktivitäten in Adobe Workfront Goals bearbeiten](../../workfront-goals/results-and-activities/edit-results-and-activities.md)

Ziele können auch an übergeordneten Zielen ausgerichtet werden, sodass sie zu untergeordneten Zielen werden. Untergeordnete Ziele sind ebenfalls Fortschrittsindikatoren für die übergeordneten Ziele.

Sie können die Zielausrichtung entfernen, indem Sie die Verbindung zwischen den Zielen entfernen. Weitere Informationen finden Sie unter [Zielausrichtung in Adobe Workfront Goals entfernen](../goal-alignment/remove-goal-alignment.md).

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
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
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

## Voraussetzungen

Ein Ziel muss mit Ergebnissen, Aktivitäten oder Projekten verknüpft sein.

## Überlegungen zum Entfernen von Ergebnissen und Aktivitäten und zum Trennen von Projekten von Zielen

* Ergebnisse und Aktivitäten können nur aus aktiven Zielen entfernt werden.
* Sie können Ergebnisse und Aktivitäten aus einem Ziel entfernen, indem Sie sie löschen. Gelöschte Ergebnisse und Aktivitäten können nicht wiederhergestellt werden.
* Wenn Sie das Ergebnis oder die Aktivität aus einem Ziel entfernen, wirkt sich der Fortschritt des entfernten Ergebnisses oder der Aktivität auf den Gesamtfortschritt des Ziels aus.
* Sie können ein Projekt nicht aus einem Ziel löschen, es jedoch vom Ziel trennen. Wenn Sie das Projekt vom Ziel trennen, wirkt sich der Prozentsatz der Fertigstellung des Projekts nicht mehr auf den Fortschritt des Ziels aus.

  Informationen darüber, wie sich Projekte auf den Zielfortschritt auswirken, finden Sie unter [Hinzufügen von Projekten zu Zielen in Adobe Workfront Goals](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

* Sie können kein Ergebnis oder eine Aktivität aus einem Ziel entfernen und kein untergeordnetes Ziel oder Projekt trennen, wenn es sich dabei um die letzte Fortschrittsanzeige für das Ziel handelt.
* Wenn ein Projekt aus dem Bereich Projekte gelöscht wird und es die letzte Fortschrittsanzeige eines Ziels ist, wird das Ziel inaktiv.

## Ergebnisse und Aktivitäten aus Zielen löschen

Sie entfernen Ergebnisse und Aktivitäten aus einem Ziel, indem Sie sie löschen. Das Löschen von Ergebnissen und Aktivitäten aus einem Ziel ist identisch.

<!--
How you delete results and activities differs depending on the environment you use.

### Delete results and activities in the Production environment


1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click **Results** to remove results or **Activities** to remove activities. 

1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the result or activity name, then click **Delete** > **Yes, delete**.

   ![Delete result](assets/delete-result-goal-details-350x108.png)

   The result or activity is deleted and cannot be recovered. The percent complete of the goal updates to exclude the deleted activity or result.

-->

1. Klicken Sie oben rechts auf **Hauptmenü**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) und dann auf **Ziele**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
   Dadurch wird der Bereich Workfront-Ziele geöffnet. Die Liste der Ziele wird standardmäßig angezeigt.

1. Klicken Sie auf den Namen eines Ziels, aus dem Sie Ergebnisse und Aktivitäten entfernen möchten.

   Dadurch wird die Zielseite geöffnet.

1. Klicken Sie **linken Bereich** Fortschrittsanzeigen“.

1. Wählen Sie ein Ergebnis oder eine Aktivität aus und klicken Sie dann oben in **Liste auf** Symbol ![Löschen](assets/delete-icon.png)Symbol „Löschen“.

1. Klicken Sie **Löschen**, um den Löschvorgang zu bestätigen. Das Ergebnis oder die Aktivität wurde gelöscht und kann nicht wiederhergestellt werden. Der Prozentsatz der Fertigstellung des Ziels wird aktualisiert, um die gelöschte Aktivität oder das gelöschte Ergebnis auszuschließen.


## Projekte aus Zielen entfernen

<!--
Dsconnecting projects from goals differs depending on the environment you use.

### Disconnect projects from goals in the Production environment


1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click the **right-pointing arrow** to the left of the Activities sections to expand it. 
1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the project name, then click **Disconnect**.

   ![Disconnect](assets/disconnect-project-goal-details-350x94.png)

   The project is disconnected from the goal. The percent complete of the goal updates to exclude the percent complete of the disconnected project.
-->


1. Klicken Sie oben rechts auf **Hauptmenü** und dann auf **Ziele**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Dadurch wird der Bereich Workfront-Ziele geöffnet. Die Liste der Ziele wird standardmäßig angezeigt.

1. Klicken Sie auf den Namen eines Ziels, aus dem Sie Ergebnisse und Aktivitäten entfernen möchten.

   Dadurch wird die Zielseite geöffnet.
1. Klicken Sie **linken Bereich** Fortschrittsanzeigen“.
1. Wählen Sie ein Projekt aus und klicken Sie dann oben in **Liste auf** Symbol ![Trennen](assets/disconnect-icon.png)Symbol „Verbindung trennen“.
1. Klicken Sie **Trennen** zur Bestätigung.

   Das Projekt ist nicht mehr mit dem Ziel verbunden. Der Prozentsatz der Fertigstellung des Ziels wird aktualisiert, um das getrennte Projekt auszuschließen.

