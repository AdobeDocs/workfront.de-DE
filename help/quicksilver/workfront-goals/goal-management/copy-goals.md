---
product-previous: workfront-goals
navigation-topic: goal-management
title: Kopieren von Zielen in Adobe Workfront-Zielen
description: Sie können Ziele in Adobe Workfront-Zielen kopieren, um ein Ziel zu erstellen. Einige der ursprünglichen Zielinformationen werden an das neue Ziel übertragen.
author: Alina
feature: Workfront Goals
exl-id: 690a6030-ee29-4e50-869f-cd014050b364
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Kopieren von Zielen in Adobe Workfront-Zielen

Sie können Ziele in Adobe Workfront-Zielen kopieren, um ein Ziel zu erstellen. Einige der ursprünglichen Zielinformationen werden an das neue Ziel übertragen.

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

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Sie müssen über Folgendes verfügen, bevor Sie beginnen können:

* Eine Layout-Vorlage, die den Bereich Ziele im Hauptmenü enthält.

## Überlegungen zum Kopieren von Zielen

Sie müssen Zugriff auf die Option Ziele bearbeiten in Ihrer Zugriffsebene haben, bevor Sie Ziele kopieren können. Informationen zur Gewährung des Zugriffs auf Ziele finden Sie unter [Zugriff auf Adobe Workfront-Ziele gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

Mögliche Gründe für das Kopieren eines vorhandenen Ziels sind:

* Wenn Sie am Ende eines Zeitraums (Quartal oder Jahr) dasselbe Ziel für den nächsten Zeitraum neu erstellen möchten.
* Wenn das Ziel am Ende eines Zeitraums nicht erreicht werden kann und Sie es für einen anderen Zeitraum bearbeiten möchten.
* Wenn mehrere Team-Mitglieder ähnliche Ziele haben und Sie möglicherweise eines für jede dieser Ziele erstellen müssen.

>[!TIP]
>
>Sie können ein Ziel in einen beliebigen Status kopieren. Weitere Informationen zum Zielstatus finden Sie unter [Zielstatusübersicht in Adobe Workfront-Zielen](../../workfront-goals/goal-management/goal-status-overview.md).

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


1. Gehen Sie zu einem Ziel und klicken Sie auf **Mehr** Menü ![](assets/more-icon.png)Klicken Sie auf **Ziel kopieren**.

   ![](assets/copy-goal-box-unshimmed.png)

1. Aktualisieren Sie die folgenden Informationen für das kopierte Ziel:
   * **Zielname**: Der Name des neuen Ziels. Der Standardname für das kopierte Ziel lautet &quot;Kopie von &lt;original goal=&quot;&quot;>&quot;.
   * **Zeitraum**: Der Zeitraum, in dem Sie das Ziel erreichen möchten. Wählen Sie einen Zeitraum aus dem Dropdown-Menü aus

      Oder

      Auswählen **Benutzerdefinierte Datumswerte aktivieren** zum Angeben benutzerdefinierter Datumswerte für das Ziel **Starten** und **Enddaten**. Die Einstellung Benutzerdefinierte Datumswerte aktivieren ist standardmäßig deaktiviert.

      >[!TIP]
      >
      >   Wenn Sie Benutzerdefinierte Datumswerte aktivieren deaktivieren, wird der Zeitraum des ursprünglichen Ziels zurückgesetzt.

      * **Zieleigentümer**: Der Eigentümer des Ziels. Dabei kann es sich um einen Benutzer, ein Team, eine Gruppe oder ein Unternehmen handeln. Die Standardeinstellung ist der Eigentümer des ursprünglichen Ziels.
      * **Beschreibung**: Zusätzliche Informationen zum Ziel.
      * **Ergebnisse kopieren**: Wählen Sie diese Option aus, wenn Sie die Ergebnisse vom aktuellen Ziel an das kopierte Ziel übertragen möchten. Dadurch werden die ursprünglichen Ergebnisse dupliziert und an das kopierte Ziel angehängt. Die Ergebnisse des kopierten Ziels haben denselben Eigentümer, dieselben Namen und die gemessenen Werte wie die Ergebnisse des ursprünglichen Ziels.

         >[!NOTE]
         >
         >* Der Fortschritt des ursprünglichen Ergebnisses wird nicht an das kopierte Ziel übertragen.
         >* Wenn der ursprüngliche Eigentümer aus Workfront gelöscht oder deaktiviert wurde, wird das neue Ergebnis dem angemeldeten Benutzer zugewiesen.


1. Klicken **Ziel kopieren**.

   Ein dem ursprünglichen Ziel ähnliches Ziel wird erstellt und erhält den Status Entwurf .

   >[!NOTE]
   >
   >Wenn Sie die Ergebnisse nicht aus dem ursprünglichen Ziel kopiert haben, müssen Sie zunächst das neue Ziel mit einem Fortschrittsanzeige verknüpfen, bevor Sie es aktivieren und anfangen, es zu erreichen.
   >Informationen zur Verknüpfung von Zielen mit Fortschrittsanzeigen finden Sie in den folgenden Artikeln:
   >* [Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront-Zielen](../results-and-activities/add-results-to-goals.md)
   >* [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront-Zielen](../results-and-activities/add-activities-to-goals.md)
   >* [Ziele durch Verbinden in Adobe Workfront-Zielen ausrichten](../goal-alignment/align-goals-by-connecting-them.md)

   >
   >Informationen zum Aktivieren von Zielen finden Sie unter [Ziele aktivieren](../goal-management/activate-goals.md).

