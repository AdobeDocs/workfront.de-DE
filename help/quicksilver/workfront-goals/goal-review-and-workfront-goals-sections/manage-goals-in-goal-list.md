---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Ziele in der Zielliste von Adobe Workfront verwalten
description: Nachdem Sie oder andere Benutzer Ziele erstellt haben, können Sie deren Fortschritt und Informationen in der Zielliste überprüfen. Informationen zum Erstellen von Zielen finden Sie unter Ziele in Adobe Workfront erstellen .
author: Alina
feature: Workfront Goals
exl-id: 2a2c1240-f796-4cb8-b8a6-2ad5853916b9
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 2%

---

# Ziele in der Zielliste von Adobe Workfront verwalten

<!-- printing or exporting goals is no longer possible, but see if they add it later-->

Nachdem Sie oder andere Benutzer Ziele erstellt haben, können Sie deren Fortschritt und Informationen in der Zielliste überprüfen. Informationen zum Erstellen von Zielen finden Sie unter [Erstellen von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/create-goals.md).

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

Sie müssen über folgenden Zugriff verfügen, um die in diesem Artikel beschriebenen Aktionen durchzuführen:

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
   <td role="rowheader">Zugriffsebene*</td> 
   <td> <p>Zugriff auf Ziele anzeigen oder höher</p> <p><b>NOTIZ</b><p>Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Zugriff auf Adobe Workfront-Ziele gewähren</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> 
    <div> 
     <p>Anzeigen oder Höhere Berechtigungen für Ziele</p> 
     <p>Informationen zum Freigeben von Zielen finden Sie unter <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Freigeben eines Ziels in Workfront-Zielen</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Sie müssen über Folgendes verfügen, bevor Sie beginnen können:

* Eine Layout-Vorlage, die den Bereich Ziele im Hauptmenü enthält.

## Ziele in der Zielliste verwalten

Sie können Ziele in den folgenden Abschnitten von Workfront-Zielen anzeigen und verwalten:

* Liste der Ziele
* Ziel-Ausrichtung

In jedem Abschnitt werden Ziele in etwas unterschiedlichen Formaten angezeigt. Welchen Abschnitt Sie verwenden, hängt vom Zweck ab, den Sie beim Arbeiten mit Zielen erreichen möchten.

Weitere Informationen finden Sie unter [Überblick über die Adobe Workfront-Ziele - Abschnitte](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

In diesem Artikel wird beschrieben, wie Sie Ziele in der Zielliste überprüfen.

Beachten Sie bei der Überprüfung der Zielliste Folgendes:

* Sie können Ziele anzeigen, die Sie oder andere in Ihrer Organisation in der Zielliste erstellt haben. Sie müssen über Verwaltungsberechtigungen für Ziele verfügen, um diese bearbeiten zu können.

<!--

### Manage the Goal List in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List section displays by default. You can view goals regardless of their status, period, or owner, by default.

   The list of goals contains the following columns with information about each goal, result, or activity: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> 
       <div> 
        <p role="rowheader">Name </p> 
       </div> </td> 
      <td>The name of the goal, result, or activity.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Owner</td> 
      <td>The name of the goal, result, or activity owner. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Period</td> 
      <td>The time period for which the goal is scheduled.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progress </td> 
      <td> <p>The progress indicator for the goal includes the following:</p> 
       <ul> 
      <li> <p>The progress label. </p> <p>For information, see <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Overview of goal progress and condition in Adobe Workfront Goals</a>. </p> </li> 
      <li> <p>The percent complete of the goal, activity, or result. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Status (includes alignment icon)</p> <p> <img src="assets/alignment-icon-large.png"> </p> </td> 
      <td> <p>The status of the goal which can be one of the following:</p> 
       <ul> 
        <li>Active</li> 
        <li>Draft</li> 
        <li>Inactive</li> 
        <li>Closed</li> 
       </ul> <p>For information about goal status, see <a href="../../workfront-goals/goal-management/goal-status-overview.md" class="MCXref xref">Goal status overview in Adobe Workfront Goals</a>. </p> <p>The alignment icon appears on goals that are aligned to other goals. For information about aligning goals, see <a href="../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md" class="MCXref xref">Align goals by connecting them in Adobe Workfront Goals</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Use the filters in the upper-right corner of the goal list to select only goals that are important to you. For information about using filters in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md)
1. Click any of the fields in the column headers to sort it by that field.

   An arrow displays to the right of the field by which the list is sorted.

   ![](assets/goal-list-with-goal-expanded-+-result-+-activity-350x117.png)

1. (Optional) Click the field in the column again to sort the same column in a descending order. 
1. Click the right-pointing arrow to the left of the goal name to expand a goal

   Or

   Click the right-pointing arrow ![](assets/right-pointing-arrow.png) in the header of the list to expand all the goals in the list and view additional information about each goal, including any of the following:

   * Results names, owners, and progress

     For information about results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   
   * Activity names, owners, and progress

     For information about activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

1. Click the name of a goal to open the **Goal Details** panel on the right and review more information about the goal as well as manage it. For information about reviewing individual goals, see [Update goals in the Goal details section in Adobe Workfront Goals](../../workfront-goals/goal-management/update-goals-in-goal-details-panel.md).
1. (Optional) Expand the **Goals per page** drop-down menu and select from the following options to display additional goals:

   * 20  
      
      This is the default selection. 
   * 50
   * 100

1. Click **Print** to export a list of goals, results, and activities to a .pdf file.

   >[!TIP]
   >
   >* When printing a list of goals, the file produced contains only the information displayed on the screen. Items eliminated by filtering a list of goals do not display in the .pdf file.
   >* When you do not expand the goals in the list before printing the list, the .pdf file displays only goals without their results and activities.

   For more information, see [Print the Goal List in Adobe Workfront Goals](../../workfront-goals/goal-management/print-the-goal-list.md). 

1. Click the **Alignment icon** ![](assets/align-icon.png) next to an aligned to open the goal's card in the Goal Alignment section. For more information, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).
-->

So verwalten Sie Ziele in der Zielliste:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png)  in der oberen rechten Ecke und klicken Sie auf **Ziele**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Der Abschnitt &quot;Zielliste&quot;wird standardmäßig angezeigt. Sie können Ziele standardmäßig unabhängig von ihrem Status, Zeitraum oder Eigentümer anzeigen.

   Die Liste der Ziele enthält die folgenden Felder mit Informationen zu den einzelnen Zielen:

   * **Name**: Der Name des Ziels.
   * **Inhaber**: Der Name des Zieleigentümers.
   * **Zeitraum**: Der Zeitraum, für den das Ziel geplant ist.
   * **Status**: Der Status des Ziels kann einer der folgenden sein:
      * Aktiv
      * Entwurf
      * Inaktiv
      * Geschlossen

      Weitere Informationen zum Zielstatus finden Sie unter [Zielstatusübersicht in Adobe Workfront-Zielen](../goal-management/goal-status-overview.md).

      Das Ausrichtungssymbol wird für Ziele angezeigt, die an anderen Zielen ausgerichtet sind. Informationen zum Ausrichten von Zielen finden Sie unter [Ziele durch Verbinden in Adobe Workfront-Zielen ausrichten](../goal-alignment/align-goals-by-connecting-them.md).

   * **Bedingung**: Eine visuelle Darstellung des Fortschritts des Ziels innerhalb des Zeitraums, der für den Abschluss des Ziels zugewiesen ist.

      Die Bedingung eines Ziels kann eine der folgenden sein:

      * Neu
      * Im Zielbereich
      * Gefährdet
      * In Schwierigkeiten

      Weitere Informationen zu Zielbedingungen finden Sie unter [Übersicht über den Zielfortschritt und die Bedingungen in Adobe Workfront-Zielen](../goal-management/calculate-goal-progress.md).

   * **Fortschritt**: Der Fortschrittsindikator für das Ziel als Prozentwert. Die Farbe der Fortschrittsanzeige entspricht der Farbe der Bedingung des Ziels.

      Weitere Informationen finden Sie unter [Berechnung des Zielfortschritts in Adobe Workfront-Zielen](../goal-management/calculate-goal-progress.md).



1. Klicken Sie auf das Filtersymbol ![](assets/filter-icon.png) in der oberen rechten Ecke der Zielliste ein und wenden Filter an, um nur für Sie wichtige Ziele anzuzeigen.

   Informationen zur Verwendung von Filtern in Workfront-Zielen finden Sie unter [Informationen in Adobe Workfront-Zielen filtern](../goal-management/filter-information-wf-goals.md).

1. Klicken Sie auf eines der Felder in den Spaltenüberschriften, um die Liste nach diesem Feld zu sortieren.
Rechts neben dem Feld, nach dem die Liste sortiert ist, wird ein Pfeil angezeigt.

1. (Optional) Klicken Sie erneut auf das Feld in der Spalte , um dieselbe Spalte in absteigender Reihenfolge zu sortieren.
1. Klicken Sie auf den Namen eines Ziels, um die Seite des Ziels zu öffnen.
1. Wählen Sie ein Ziel in der Liste aus und klicken Sie dann oben in der Liste auf eine der folgenden Optionen:
   * **Bearbeiten** icon ![](assets/edit-icon.png) , um Informationen zum Ziel zu bearbeiten. Weitere Informationen finden Sie unter [Ziele in Adobe Workfront bearbeiten](../goal-management/edit-goals.md).
   * **Freigeben** icon ![](assets/share-icon.png) , um das Ziel mit anderen Menschen zu teilen. Weitere Informationen finden Sie unter [Freigeben eines Ziels in Adobe Workfront-Zielen](../workfront-goals-settings/share-a-goal.md).
   * **Offene Ausrichtung** icon ![](assets/align-icon-unshimmed.png) , um den Bereich &quot;Zielausrichtung&quot;zu öffnen. Diese Option wird nur angezeigt, wenn das ausgewählte Ziel an einem anderen Ziel ausgerichtet ist.
   * **Löschen** icon ![](assets/delete-icon.png) , um das Ziel zu löschen, klicken Sie auf **Löschen** zur Bestätigung.  Weitere Informationen finden Sie unter [Löschen und Deaktivieren von Zielen in Adobe Workfront-Zielen](../goal-management/delete-and-deactivate-goals.md).





