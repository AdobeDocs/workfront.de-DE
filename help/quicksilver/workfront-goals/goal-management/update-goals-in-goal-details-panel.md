---
product-previous: workfront-goals
navigation-topic: goal-management
title: Aktualisieren von Zielen im Bereich "Zieldetails"in Adobe Workfront-Zielen
description: Sie können Informationen zu einzelnen Zielen aktualisieren, indem Sie auf das Bedienfeld "Zieldetails"zugreifen.
author: Alina
feature: Workfront Goals
exl-id: e9df0d98-05a1-4977-b7f1-426b8f5b3eae
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 1%

---

# Aktualisieren von Zielen im Abschnitt &quot;Zieldetails&quot;in Adobe Workfront-Zielen

<!--drafted for the goal redesign:
- change the title for Production to Update goals in the Goal details section in Adobe Workfront Goals. 
- update the description in the metadata above
-->

Sie können Informationen zu einzelnen Zielen aktualisieren, indem Sie auf das Bedienfeld &quot;Zieldetails&quot;zugreifen.

>[!NOTE]
>
>Ziele mit dem Status Geschlossen können nicht aktualisiert werden.


## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

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
 <td role="rowheader">Zugriffsstufe*</td>
 <td> <p>Zugriff auf Ziele bearbeiten</p> </td>
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

## Aktualisieren von Zielen im Abschnitt &quot;Zieldetails&quot;

Sie können über eine Liste von Zielen auf ein einzelnes Ziel zugreifen.

<!--

Updating goals in the Goal Details panel differs depending on where you access the goal from. 

### Update goals in the Goal Details panel in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Goals area in Workfront. 

1. Click the name of a goal in the Goal List, then click the name of a goal.

   This opens the Goal Details panel on the right.
   ![](assets/goal-details-summary-tab-350x294.png)

   >[!TIP]
   >
   >You can also click the name of a goal in the Goal Alignment, Check-in, or Pulse sections. 
   >
   ><!-- drafted for goal redesign:
   >Add this to the TIP above with goal redesign: 
   >
   >The Check-in and Pulse sections have been removed from the Preview environment.
   >

1. On the Summary tab, click the **More icon** ![](assets/more-icon.png), then click any of the following options:

   1. **Edit**. For information about editing goals, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
   1. **Copy**. For information about copying goals, see [Copy goals in Adobe Workfront Goals](../../workfront-goals/goal-management/copy-goals.md).
   1. **Activate**. This option is available only for drafted and inactive goals.

      For information about activating goals, see [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md). 
   
   1. **Close**, then click**Close Goal**. This option is available only for active goals.

      For information about closing goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   
   1. **Deactivate**. This option is available only for active goals. This deactivates the goal immediately.

      For information about deactivating goals, see [Delete and deactivate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).
   
   1. **Delete**, then click **Yes, Delete**.

      For information about deleting goals, see [Delete and deactivate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

      >[!NOTE]
      >
      >Deleted goals cannot be recovered.

   1. **Reopen**, then click **Reopen**. This option is available only for closed goals that are from a current time period.

      For information about reopening goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   
   1. (Conditional) If you clicked any of the options between steps a-i above except Delete or Reopen, click **Save**.    
   
      (!--ensure this is accurate)--)

1. Click **Align to another goal** in the upper-right of the Summary tab, then specify the name of a goal in the **Align to** **another goal** field that you want to align the current goal to. The current goal becomes the child of the goal you align it to. For information about child and parent goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md). 
1. Click **Add results**. Results drive the progress of your goal. For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).

1. Click **Add activities**. Activities drive the progress of your goal. For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 

1. Click the **Updates** tab. Here, you can view goal comments and review the entire editing history of the goal, activities, and results, to understand who changed what and when.

   ![](assets/goal-details-updates-tab-350x280.png)

1. (Optional) Deselect any of the following options if you want to not display them in the Updates tab.&nbsp;They are selected by default: 

   | Option |Description  |
   |---|---|
   | Progress Updates |Displays information about the history of progress updates on results and activities.  |
   | Comments |Displays comments made by users on the goal.  |
   | Editing History |Displays information about creating and updating the goal, results, and activities.  |

1. (Optional) Click **Details** under a progress or an editing history update to display additional information about the update.

   ![](assets/update-details-in-updates-tab-expanded-highlighted-350x139.png)

-->



1. Klicken Sie auf den Namen eines Ziels in der Zielliste und dann auf den Namen eines Ziels.

   Dadurch wird die **Zieldetails** auf der linken Seite.

   ![](assets/goal-page-unshimmed.png)

1. Klicken Sie auf **Symbol Bearbeiten** ![](assets/edit-icon.png) in der oberen rechten Ecke und klicken Sie auf **Alle bearbeiten** oder **Übersicht**

   Oder

   Geben Sie Informationen in eines der bearbeitbaren Felder im Abschnitt Zieldetails ein. Der Abschnitt kann bearbeitet werden.

   >[!IMPORTANT]
   >
   >Es können nicht alle Felder bearbeitet werden, die im Abschnitt Zieldetails angezeigt werden. Workfront berechnet einige der Felder und ist schreibgeschützt.

1. Aktualisieren oder überprüfen Sie die folgenden Felder:

   * **Beschreibung**: Fügen Sie Informationen zum Ziel hinzu oder aktualisieren Sie diese.
   * **Fortschritt**: Gibt an, welcher Prozentsatz des Ziels bisher abgeschlossen wurde. Sie können den Fortschritt eines Ziels nicht manuell aktualisieren. Ziel des Fortschritts ist die Berechnung aller Fortschrittsindikatoren.
   * **Bedingung**: Gibt an, ob das Ziel neu ist und noch nicht aktualisiert wurde, ob es sich um ein Ziel handelt, das rechtzeitig abgeschlossen werden soll oder zurückliegt. Die Bedingung eines Ziels kann nicht aktualisiert werden. Die Bedingung des Ziels wird automatisch von Worfront berechnet.\
     Weitere Informationen zu Zielbedingungen und Fortschritt finden Sie unter
     [Übersicht über den Zielfortschritt und die Bedingungen in den Adobe Workfront-Zielen](../goal-management/calculate-goal-progress.md).
   * **Status**: Der Status eines Ziels kann nicht manuell aktualisiert werden. Weitere Informationen finden Sie unter [Zielstatusübersicht in Adobe Workfront-Zielen](../goal-management/goal-status-overview.md).
   * **Goal Owner**: Klicken Sie auf , um den Namen des Eigentümers des Ziels zu aktualisieren. Geben Sie den Namen eines Benutzers, Teams, einer Gruppe oder Ihres Unternehmens ein und wählen Sie ihn aus, wenn er in der Liste angezeigt wird. Sie können nur einen Inhaber für ein Ziel haben.
   * **Übergeordnetes Ziel**: Beginnen Sie mit der Eingabe des Namens eines Ziels, das Sie als übergeordnetes Ziel des ausgewählten Ziels festlegen möchten. Der Fortschritt des ausgewählten Ziels aktualisiert automatisch den Fortschritt des übergeordneten Ziels.

     >[!TIP]
     >
     >Sie können die folgenden Informationen zu einem übergeordneten Ziel nicht aktualisieren:
     >    * Zeitraum des übergeordneten Ziels
     >    * Fortschritt des übergeordneten Ziels
     >    * Übergeordneter Zieleigentümer.
     >      
     >Sie müssen diese Informationen über das übergeordnete Ziel selbst aktualisieren.

   * **Zeitraum**: Klicken Sie auf , um den Zeitraum für das Ziel zu aktualisieren.\
     Oder\
     Auswählen **Benutzerdefinierte Datumswerte aktivieren** zum Angeben von Daten für die **Starten** und **Enddaten**.
   * **Notizen schließen**: Dieses Feld ist nur für Ziele mit dem Status Geschlossen sichtbar. Geschlossene Ziele können nicht bearbeitet werden. Beim erneuten Öffnen eines geschlossenen Ziels werden die schließenden Notizen dauerhaft gelöscht.


