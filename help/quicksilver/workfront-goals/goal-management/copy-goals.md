---
product-previous: workfront-goals
navigation-topic: goal-management
title: Kopieren von Zielen in Adobe Workfront-Zielen
description: Sie können Ziele in Adobe Workfront-Zielen kopieren, um ein Ziel zu erstellen. Einige der ursprünglichen Zielinformationen werden an das neue Ziel übertragen.
author: Alina
feature: Workfront Goals
exl-id: 690a6030-ee29-4e50-869f-cd014050b364
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 4%

---

# Kopieren von Zielen in Adobe Workfront-Zielen

Sie können Ziele in Adobe Workfront-Zielen kopieren, um ein Ziel zu erstellen. Einige der ursprünglichen Zielinformationen werden an das neue Ziel übertragen.

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

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Überlegungen zum Kopieren von Zielen

Sie müssen auf der Zugriffsebene Zugriff auf Ziele bearbeiten haben, bevor Sie Ziele kopieren können. Informationen zur Gewährung des Zugriffs auf Ziele finden Sie unter [Gewähren des Zugriffs auf Adobe Workfront-Ziele](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

Mögliche Gründe für das Kopieren eines vorhandenen Ziels sind:

* Wenn Sie am Ende eines Zeitraums (Quartal oder Jahr) dasselbe Ziel für den nächsten Zeitraum neu erstellen möchten.
* Wenn das Ziel am Ende eines Zeitraums nicht erreicht werden kann und Sie es für einen anderen Zeitraum bearbeiten möchten.
* Wenn mehrere Team-Mitglieder ähnliche Ziele haben und Sie möglicherweise eines für jede dieser Ziele erstellen müssen.

>[!TIP]
>
>Sie können ein Ziel in einen beliebigen Status kopieren. Informationen zu den Zielstatus finden Sie unter [Zielstatusübersicht in Adobe Workfront-Zielen](../../workfront-goals/goal-management/goal-status-overview.md).

Beachten Sie beim Kopieren von Zielen Folgendes:

* Alle Informationen über das Ziel werden ebenfalls in das neue Ziel kopiert.
* Sie können auswählen, ob die Ergebnisse eines vorhandenen Ziels kopiert werden sollen. Der Name der Ergebnisse wird auf das neue Ziel übertragen, der aktuelle Fortschritt der Ergebnisse auf dem vorhandenen Ziel wird jedoch nicht in das neue Ziel kopiert. Die kopierten Ergebnisse werden standardmäßig demselben Eigentümer zugewiesen.

  >[!NOTE]
  >
  >Wenn der ursprüngliche Eigentümer aus Workfront gelöscht oder deaktiviert wurde, wird das neue Ergebnis dem angemeldeten Benutzer zugewiesen.

* Sie können die Aktivitäten eines Ziels nicht kopieren, wenn Sie das Ziel kopieren.

## Ziele kopieren

<!--
Copying goals differs depending on what environment you use. 

To copy goals in the Production environment:

1. Go to a goal and click it to open the Goal Details panel.

   For information about accessing an individual goal, see the "Access individual goals" section in [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md).

   This opens the Goal Details panel.

1. Click the **More icon** ![](assets/more-icon.png), then click **Copy**. 

1. Update any of the following information for the copied goal:

   | Field |Description  |
   |---|---|
   | New Goal |The name of the new goal. The default is the name of the original goal.  |
   | Period |The time period during which you want to achieve the goal. Select a time period from the drop-down menu or click **Define custom dates** to indicate a custom time period. By default, the Period is always the current quarter. |
   | Owner |The owner of the goal. It can be a user, team, group, or a company. The default is the owner of the original goal.  |
   | Description |Additional information about the goal.  |

1. (Conditional) Select **Copy results** if the original goal had results added to it and you want to copy them to the new goal. This duplicates the original results to the new goal. The results of the copied goal have the same owner, names and measured values as the results of the original goal.

   >[!TIP]
   >
   >* The progress of the original result does not transfer to the copied goal. 
   >* If the original owner was deleted or deactivated from Workfront, the new result is assigned to the logged in user.

1. Click **Save**.

   The copied goal is saved with a status of Draft and displays in the Goal Details panel.

   >[!IMPORTANT]
   >
   >If you have not copied the results from the original goal, you must first associate the new goal with a progress indicator before you can activate it and start working towards achieving it. 
   >
   >Do at least one of the following to be able to activate a goal: 
   >   
   >* Add a Result
   >   
   >  For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   >   
   >* Add an Activity
   >   
   >  For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 
   >   
   >* Align another goal to it
   >   
   >  For information about aligning goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).
   >
   > For information about activating a goal, see [Activate goals in Adobe Workfront Goals](../goal-management/activate-goals.md). 

1. Click the **X** icon in the upper-right of the Goal Details panel to close it.

   The copied goal displays in the following sections:

   * Goal List 
   * Check-in (after it is activated)
   * Goal Alignment section (after it is activated) 
   * Pulse
(!--drafted - this was important when we could not update the goal timeframe in the past but we can do that now - not needed
1. (Optional and conditional) If you have copied a goal that was not achieved in a previous time period to continue working on it in the following time period, do the following:

   1. Go to the original goal in the Goal List, Check-in page, or Pulse section and comment on the goal, to indicate that this goal was copied to another, more current goal. For information about commenting on a goal, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md).
   1. Close the original goal, to preserve the progress in its original time period. For information about closing goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   1. Update the the **Initial** value of the new Result to match the **End At** value of the previous result, so that your new goal progress will start calculating from the point you achieved in the previous period.
   
-->


1. Gehen Sie zu einem Ziel, klicken Sie auf das Menü **Mehr** ![](assets/more-icon.png) und dann auf **Ziel kopieren**.

   ![](assets/copy-goal-box-unshimmed.png)

1. Aktualisieren Sie die folgenden Informationen für das kopierte Ziel:
   * **Zielname**: Der Name des neuen Ziels. Der Standardname für das kopierte Ziel ist &quot;Kopie von &lt;ursprüngliches Ziel>&quot;.
   * **Zeitraum**: Der Zeitraum, in dem Sie das Ziel erreichen möchten. Wählen Sie einen Zeitraum aus dem Dropdownmenü aus

     Oder

     Wählen Sie **Benutzerdefinierte Datumswerte aktivieren** aus, um benutzerdefinierte Datumswerte für das Ziel **Start** und das Enddatum **5} festzulegen.** Die Einstellung Benutzerdefinierte Datumswerte aktivieren ist standardmäßig deaktiviert.

     >[!TIP]
     >
     >   Wenn Sie Benutzerdefinierte Datumswerte aktivieren deaktivieren, wird der Zeitraum des ursprünglichen Ziels zurückgesetzt.

      * **Zieleigentümer**: Der Eigentümer des Ziels. Dabei kann es sich um einen Benutzer, ein Team, eine Gruppe oder ein Unternehmen handeln. Standardmäßig ist es der Eigentümer des ursprünglichen Ziels.
      * **Beschreibung**: Zusätzliche Informationen zum Ziel.
      * **Ergebnisse kopieren**: Wählen Sie diese Option, wenn Sie die Ergebnisse vom aktuellen Ziel an das kopierte Ziel übertragen möchten. Dadurch werden die ursprünglichen Ergebnisse dupliziert und an das kopierte Ziel angehängt. Die Ergebnisse des kopierten Ziels haben dieselben Eigentümer, Namen und Messwerte wie die Ergebnisse des ursprünglichen Ziels.

        >[!NOTE]
        >
        >* Der Fortschritt des ursprünglichen Ergebnisses wird nicht an das kopierte Ziel übertragen.
        >* Wenn der ursprüngliche Eigentümer aus Workfront gelöscht oder deaktiviert wurde, wird das neue Ergebnis dem angemeldeten Benutzer zugewiesen.

1. Klicken Sie auf **Ziel kopieren**.

   Ein dem ursprünglichen Ziel ähnliches Ziel wird erstellt und erhält den Status Entwurf .

   >[!NOTE]
   >
   >Wenn Sie die Ergebnisse nicht aus dem ursprünglichen Ziel kopiert haben, müssen Sie zunächst das neue Ziel mit einem Fortschrittsanzeige verknüpfen, bevor Sie es aktivieren und anfangen, es zu erreichen.
   >Informationen zur Verknüpfung von Zielen mit Fortschrittsanzeigen finden Sie in den folgenden Artikeln:
   >* [Ergebnisse zu Zielen in Adobe Workfront-Zielen hinzufügen](../results-and-activities/add-results-to-goals.md)
   >* [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront-Zielen](../results-and-activities/add-activities-to-goals.md)
   >* [Ziele durch Verbinden in Adobe Workfront-Zielen ausrichten](../goal-alignment/align-goals-by-connecting-them.md)
   >
   >Informationen zum Aktivieren von Zielen finden Sie unter [Ziele aktivieren](../goal-management/activate-goals.md).

