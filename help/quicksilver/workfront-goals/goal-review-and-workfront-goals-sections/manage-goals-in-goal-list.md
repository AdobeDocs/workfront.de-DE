---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Ziele in der Zielliste von Adobe Workfront verwalten
description: Nachdem Sie oder andere Benutzer Ziele erstellt haben, können Sie deren Fortschritt und Informationen in der Zielliste überprüfen. Informationen zum Erstellen von Zielen finden Sie unter Ziele in Adobe Workfront erstellen .
author: Alina
feature: Workfront Goals
exl-id: 2a2c1240-f796-4cb8-b8a6-2ad5853916b9
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 2%

---

# Ziele in der Zielliste von Adobe Workfront verwalten

<!-- printing or exporting goals is no longer possible, but see if they add it later-->

Nachdem Sie oder andere Benutzer Ziele erstellt haben, können Sie deren Fortschritt und Informationen in der Zielliste überprüfen. Informationen zum Erstellen von Zielen finden Sie unter [Ziele in Adobe Workfront erstellen](../../workfront-goals/goal-management/create-goals.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die in diesem Artikel beschriebenen Aktionen durchzuführen:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> 
   <p>Für den neuen Plan und die Lizenzstruktur:
  <ul><li>Ein ultimativer Plan </li>
  Oder
  <li>Eine zusätzliche Lizenz für Adobe Workfront Goals für die Prime- oder Select Adobe Workfront-Pläne. </li></ul> </p>
<p>Für den aktuellen Plan und die Lizenzstruktur: 
<ul><li> A Pro oder höher </li>
  <li>Eine Adobe Workfront Goals-Lizenz zusätzlich zu einer Workfront-Lizenz.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-Lizenz*</td>
 <td>
 <p>Neue Lizenz: Mitarbeiter oder höher</p>
 Oder
 <p>Aktuelle Lizenz: Anfrage oder höher</p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe Workfront-Lizenzen</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produkt*</td>
 <td>
 <p> Neue Produktanforderungen, eine der folgenden: </p>
<ul>
<li>Ein Select- oder Prime-Adobe Workfront-Plan und eine zusätzliche Adobe Workfront Goals-Lizenz.</li>
<li>Ein Ultimate Workfront-Plan, der standardmäßig Workfront-Ziele enthält. </li></ul>
 <p>Oder</p>
 <p>Aktuelle Produktanforderungen: Ein Workfront-Plan und eine zusätzliche Lizenz für Adobe Workfront Goals. </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Voraussetzungen für die Verwendung von Workfront-Zielen</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Zugriffsebene</td>
 <td> <p>Zugriff auf Ziele bearbeiten</p>  </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objektberechtigungen</td>
 <td>
  <div>
  <p>Anzeigen oder Anzeigen höherer Berechtigungen zum Ziel</p>
  <p>Berechtigungen für das Ziel verwalten</p>
  <p>Informationen zum Freigeben von Zielen finden Sie unter <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Freigeben eines Ziels in Workfront-Zielen</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Ziele im Hauptmenü enthält. </p>  
</td>
  </tr>
</tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   * **Inhaber**: Der Name des Ziel-Eigentümers.
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

     Weitere Informationen zu Zielbedingungen finden Sie unter [Übersicht über den Zielfortschritt und die Bedingungen in den Adobe Workfront-Zielen](../goal-management/calculate-goal-progress.md).

   * **Fortschritt**: Die Fortschrittsanzeige für das Ziel als Prozentwert. Die Farbe der Fortschrittsanzeige entspricht der Farbe der Bedingung des Ziels.

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





