---
product-previous: workfront-goals
navigation-topic: goal-management
title: Erstellen von Zielen in Adobe Workfront-Zielen
description: Unabhängig davon, ob Sie CEO, Manager oder Einzelmitwirkender sind, können Sie in Adobe Workfront Goals Ziele festlegen, um Ihre Arbeit an Ihren Zielen und Zielen auszurichten, die die Strategie Ihres Unternehmens umreißen.
author: Alina
feature: Workfront Goals
exl-id: 14bf48b6-eb0c-4b00-a1a4-0d070ccc1392
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 1%

---

# Erstellen von Zielen in Adobe Workfront-Zielen

Unabhängig davon, ob Sie CEO, Manager oder Einzelmitwirkender sind, können Sie in Adobe Workfront Goals Ziele festlegen, um Ihre Arbeit an Ihren Zielen und Zielen auszurichten, die die Strategie Ihres Unternehmens umreißen.

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

## Richtlinien für das Erstellen von Zielen

Bevor Sie mit Workfront-Zielen beginnen, empfehlen wir Ihnen, sich über unsere Best Practices-Empfehlungen und -Richtlinien für die wirksame Verwaltung von Zielen zu informieren. Weitere Informationen zu Richtlinien zum Erstellen und Verwalten von Zielen finden Sie unter [Übersicht über Adobe Workfront-Ziele](../../workfront-goals/goal-management/wf-goals-overview.md).

## Ziele erstellen

In diesem Artikel wird beschrieben, wie Sie ein strategisches Ziel in Workfront-Zielen erstellen. Informationen zum Erstellen eines Geschäftsfallziels finden Sie unter [Geschäftsfallziele erstellen](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

Sie können ein strategisches Ziel auf eine der folgenden Arten erstellen:

* [Neues Ziel erstellen](#create-a-goal-from-scratch)
* [Vorhandenes Ziel kopieren](#copy-an-existing-goal)
* [Konvertieren eines Ergebnisses oder einer Aktivität in ein Ziel](#convert-a-result-or-activity-to-a-goal)

### Neues Ziel erstellen {#create-a-goal-from-scratch}

<!--
Creating goals differs depending on what environment you use.

#### Create a goal from scratch in the Production environment 


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -)

   The Goal List displays.

1. (Conditional) Click **Goal List**, **Graphs**, **Pulse**, or **Check-in** in the left pane, then click **Add Goal** in the upper-right corner of the page. The Add Goal box displays.

   ![](assets/add-goal-box-350x235.png)

   >[!TIP]
   >
   >You can add a goal from any section in Workfront Goals. The process for creating a goal is identical regardless of the section you choose to add the goal from.

1. Start typing what you want to achieve in the **Goal** field. This is the name of the goal and a required field. 
1. Select a time period when the goal should be executed in the **Period** drop-down menu. This is a pre-filled field. The default is the current quarter.

   Select from the following predefined options:

   * The current year
   * The quarters of the current year
   * The next two years
   * The quarters of the next two years

   Or

   Click **Define custom dates** to select a custom time frame. 

1. (Conditional) Select a **Start date** and an **End date** for your goal, if you clicked **Define custom dates**.

   >[!TIP]
   >
   >* You can create a goal with dates in any time period, including up to 2 years in the past. 
   >* When defining custom dates, they are constrained by the initial date you selected. So if you select quarter and then custom dates, you can't go beyond that quarter.

1. (Optional) Click **Reset custom dates** to return to the predefined options.

   >[!TIP]
   >
   >We recommend that everyone in your organization selects the same timeframes for similar goals or goals that are aligned. This provides better alignment between goals and ensures that everyone's work supports your over-arching strategy.

1. (Optional) Click your name in the **Owner** field, if you want to indicate someone else as the owner of the goal. By default, you are the owner of goals you create. 
1. Start typing the name of a user, team, group, or the name of your organization in the **Owner** field, then select it when it displays in the list. You can have only one owner for a goal. 
1. (Optional) Enter a **Description** for the goal. This field is optional. 
1. Click **Save**.

   The status of the new goal is Draft.

   >[!IMPORTANT]
   >
   >You must associate a goal with a progress indicator to activate it and start working on it. 
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

1. Click the **X** icon in the upper-right of the Goal Details panel to close it.

-->

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts auf **Ziele**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Die Zielliste wird angezeigt.
1. Klicken **Neues Ziel**.

   Das Feld Neues Ziel wird angezeigt.

   ![](assets/new-goal-box-unshimmed.png)

1. Geben Sie Informationen in die folgenden Felder ein:
   * **Zielname**: Geben Sie einen Namen für das Ziel ein. Dies ist ein Pflichtfeld.
   * **Zeitraum**: Wählen Sie ein vordefiniertes Quartal oder Jahr aus dem **Zeitraum** Dropdown-Feld

      Oder

      Wählen Sie die **Benutzerdefinierte Datumswerte aktivieren** und wählen Sie eine **Starten** und **Enddatum** für das Ziel.

      Die vorherigen, aktuellen und nachfolgenden Jahre und ihre jeweiligen Quartale werden als vordefinierte Optionen im Dropdown-Feld Zeitraum aufgeführt.

      Der Zeitraum des Ziels gibt den Zeitraum an, in dem das Ziel voraussichtlich abgeschlossen sein wird.

   * **Zieleigentümer**: Beginnen Sie mit der Eingabe des Namens eines Benutzers, eines Teams, einer Gruppe oder Ihres Unternehmens, um anzugeben, wer Inhaber des Ziels ist. Sie werden standardmäßig als Eigentümer des Ziels ausgewählt.
   * **Beschreibung**: Geben Sie zusätzliche Informationen zum Ziel ein.
1. Klicken **Ziel erstellen**.

   Das neue Ziel wird in der Zielliste aufgeführt und hat den Status **Entwurf**.

   Sie müssen ein Ziel mit einer Fortschrittsanzeige verknüpfen, um es zu aktivieren und damit zu beginnen, daran zu arbeiten.

   Führen Sie mindestens einen der folgenden Schritte aus, um ein zu aktivierendes Ziel vorzubereiten:
   * Ergebnis hinzufügen

      Informationen zum Hinzufügen von Ergebnissen finden Sie unter [Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront-Zielen](../results-and-activities/add-results-to-goals.md).
   * Aktivität hinzufügen

      Informationen zum Hinzufügen von Aktivitäten finden Sie unter [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront-Zielen](../results-and-activities/add-activities-to-goals.md).
   * Ein anderes Ziel ausrichten

      Informationen zum Ausrichten von Zielen finden Sie unter [Ziele durch Verbinden in Adobe Workfront-Zielen ausrichten](../goal-alignment/align-goals-by-connecting-them.md).


### Vorhandenes Ziel kopieren {#copy-an-existing-goal}

Sie können ein Ziel durch Kopieren eines vorhandenen Ziels erstellen.

Informationen zum Kopieren von Zielen finden Sie unter [Kopieren von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/copy-goals.md).

### Konvertieren eines Ergebnisses oder einer Aktivität in ein Ziel {#convert-a-result-or-activity-to-a-goal}

Sie können ein Ziel erstellen, indem Sie das Ergebnis oder die Aktivität eines vorhandenen Ziels in ein Ziel konvertieren. Das neue Ziel wird an das ursprüngliche Ziel ausgerichtet.

Informationen zum Konvertieren von Ergebnissen und Aktivitäten in Ziele finden Sie unter [Ziele durch Konvertieren von Ergebnissen und Aktivitäten in Ziele ausrichten](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

