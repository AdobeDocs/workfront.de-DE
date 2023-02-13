---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Aktualisieren des Zielfortschritts in Adobe Workfront-Zielen
description: Sie müssen Ihre Ziele regelmäßig überprüfen und ihren Fortschritt aktualisieren, um sicherzustellen, dass sie nicht zurückfallen oder Gefahr laufen, nicht erreicht zu werden.
author: Alina
feature: Workfront Goals
exl-id: 5092f508-e52c-4934-a8c1-d0be04ecce13
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 0%

---

# Aktualisieren des Zielfortschritts in Adobe Workfront-Zielen

Sie müssen Ihre Ziele regelmäßig überprüfen und ihren Fortschritt aktualisieren, um sicherzustellen, dass sie nicht zurückfallen oder Gefahr laufen, nicht erreicht zu werden.

<!--And: take this last sentence ^^ out when you update this for goal redesign production.-->

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
* Ein aktives Ziel. Sie können den Fortschritt bei Zielen, die Entwürfe, inaktiv oder geschlossen sind, nicht aktualisieren.

## Überlegungen zum Aktualisieren von Zielen

Beachten Sie bei der Aktualisierung des Fortschritts bei Zielen Folgendes:

* Workfront Goals berechnet automatisch den Fortschritt eines Ziels, wenn Sie den Fortschritt seiner Fortschrittsanzeigen aktualisieren.

   >[!TIP]
   >
   >Sie können den Fortschritt bei einem Ziel nicht direkt aktualisieren. Sie müssen den Fortschritt der Fortschrittsindikatoren des Ziels (Aktivitäten, Ergebnisse, verbundene Projekte) aktualisieren, die wiederum den Fortschritt des Ziels aktualisieren. Um den Projektfortschritt zu aktualisieren, müssen Sie die Aufgaben im Projekt aktualisieren.

   Siehe auch die folgenden Artikel:

   * Informationen zum Hinzufügen von Aktivitäten zu Zielen finden Sie unter [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/add-activities-to-goals.md).
   * Informationen zum Hinzufügen von Ergebnissen zu Zielen finden Sie unter [Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   * Informationen dazu, wie Workfront Goals den Fortschritt bei der Zielgruppenberechnung berechnet, finden Sie unter [Übersicht über den Zielfortschritt und die Bedingungen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/calculate-goal-progress.md).

* Sie müssen Ziele erstellen und aktivieren, bevor Sie ihren Fortschritt aktualisieren können.

   Siehe auch die folgenden Artikel:

   * Informationen zum Erstellen von Zielen finden Sie unter [Erstellen von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/create-goals.md).
   * Weitere Informationen zum Aktivieren von Zielen finden Sie unter [Aktivieren von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/activate-goals.md).

   >[!IMPORTANT]
   >
   >Sie können den Fortschritt von Zielen, die entworfen, geschlossen oder inaktiv sind, nicht aktualisieren.

* Wenn Sie oder eine andere Person zum ersten Mal den Fortschritt eines Ergebnisses oder einer Aktivität an einem Ziel aktualisiert, wird das Ziel Fortschritt ändert sich von Neu und Workfront-Ziele und es werden der Fortschritt und der Fortschritt des Ziels aktualisiert.

<!--

## Update goal progress by using Check-in in the Production environment

>[!IMPORTANT]
>
> <span class="preview"> The Check-in functionality has been removed from the Preview environment and will be removed from Workfront Goals with the 23.1 release. See the [Update goal progress in the Preview environment](#update-goal-progress-in-the-preview-environment) section in this article to update goal progress in Preview. </span>


You can check in on goals at the individual goal level, or you can check in on multiple goals from the Check-in section of Workfront Goals.

* [Update individual goals](#update-individual-goals) 
* [Update goals in the Check-in section](#update-goals-in-the-check-in-section)

### Update individual goals {#update-individual-goals}

When you check in on a goal at the goal level, you can update the progress of the results and activities that are assigned to you or other users.

For information about how to update additional information about results and activities, see [Edit results and activities in Adobe Workfront Goals](../../workfront-goals/results-and-activities/edit-results-and-activities.md).

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area.

   All goals display by default. 

1. (Optional) Click any of the following sections in the left panel to access a list of goals:

   * Goal Alignment 
   * Pulse 
   * Check-in

   Or

   From the Goal List, click the name of a goal to open the **Goal Details** panel on the right.

   >[!TIP]
   >
   >You must have Edit access to Goals in your Access Level to view the Check-in section or the Check in button.

1. Click **Check in**.

   ![](assets/check-in-link-inside-goal-details-highlighted-350x156.png)

   The progress of results and activities becomes editable.

1. Update the current progress on each of the results. Depending on what type of result you selected, you can do one of the following:

   * Update the quantity 
   * Update the currency amount
   * Update the percent complete

1. Update the percent complete on the Manual progress bar activity.

   >[!TIP]
   >
   >When you add projects as activities to your goals, you cannot manually update projects at the goal level. Workfront automatically updates project progress based on the project of their tasks. When the project percent complete updates in Workfront, the goal progress associated with the project also updates automatically.

1. Click **Back to Summary** to return to the Goal Details panel.

   Your goal progress updates as you update the results and activities of your goal. 

1. Click the **X icon** in the upper-right corner of the Goal Details panel to close it.

### Update goals in the Check-in section {#update-goals-in-the-check-in-section}

You can use the Check-in section to check in on goals when you want to quickly provide updates for several goals at the same time.

>[!TIP]
>
>You can access the Check-in section from any of the following sections:
>
>* Goal List 
>* Goal Alignment 
>* Pulse 
>

When you check in on a goal in the Check-in section, you can update the progress of the results and activities that are assigned only to you. You cannot update the progress of results and activities that are assigned to other users in this section.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List section displays by default. 

1. Click Check-in in the left panel.

   Or

   (Conditional) If you are in the Goal List, Goal Alignment, or Pulse sections, click the **Check in** button in the upper-right of the screen. This opens the Check-in section.

   ![](assets/check-in-button-highlighted-350x102.png)

   Goals display in a list and results and activities are listed under each goal.

   ![](assets/check-in-page-with-show-all-aligned-goals-link-350x178.png)

1. (Optional) Click **Show all results**, **Show all activities**, or **Show all aligned goals** to the far right of the goal name to display all results, activities, and aligned goals of a goal whose progress you want to update.

   >[!CAUTION]
   >
   >You cannot directly update aligned goals, but you can update their results and activities.

1. Update the current progress on each of the results assigned to you. Depending on what type of result you selected, you can do one of the following:

   * Update the quantity 
   * Update the currency amount
   * Update the percent complete

   The result and the goal progress updated automatically and you receive a confirmation of your changes.

1. Update the percent complete on your Manual progress bar activity.

   >[!TIP]
   >
   >When you add projects as activities to your goals, you cannot manually update projects at the goal level. Workfront automatically updates project progress based on the project of their tasks. When the project percent complete updates in Workfront, the goal progress associated with the project also updates automatically.

   The activity and the goal progress updated automatically and you receive a confirmation of your changes.

1. (Optional) Add a comment for your goal, then click **Post** to save your comment.

-->

So aktualisieren Sie den Fortschritt bei den Zielen:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) > **Ziele** in der oberen rechten Ecke.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Dadurch wird die Zielliste geöffnet. Alle Ziele, auf die Sie Zugriff haben, werden standardmäßig angezeigt.

   Alternativ können Sie im linken Bereich auf Zielausrichtung klicken.

1. Klicken Sie in der Zielliste auf den Namen eines Ziels, um die Zielseite zu öffnen.
1. Klicken **Fortschrittsanzeigen** im linken Bereich.

   In der Liste Fortschrittsanzeigen werden alle Fortschrittsanzeigen für das ausgewählte Ziel angezeigt.

   >[!NOTE]
   >
   >  * Sie können nur Ergebnisse und Aktivitäten aktualisieren.
   >  * Sie müssen die Fortschrittsindikatoren der Kinderziele aktualisieren, um Fortschritte bei den Kinderzielen zu zeigen.
   >  * Sie müssen die Aufgaben der verbundenen Projekte aktualisieren, um den Fortschritt der Projekte anzuzeigen.

      >   
      >    Der Fortschritt der Kinderziele und der Fortschritt der Projekte treiben wiederum den Fortschritt des ausgewählten Ziels.



1. Um den Fortschritt eines Ergebnisses oder einer Aktivität zu aktualisieren, klicken Sie auf den Wert in der **Tatsächlicher Fortschritt** Spalte des Ergebnisses oder der Aktivität, geben Sie eine Zahl ein, um den Wert zu aktualisieren, und drücken Sie dann die Eingabetaste.

   ![](assets/actual-progress-result-updating-highlighted-unshimmed.png)

   Die Fortschrittsleiste für die Fortschrittsanzeige in der Spalte Fortschritt und der Fortschritt des Ziels in der Zielkopfzeile werden sofort aktualisiert.

