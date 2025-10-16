---
product-previous: workfront-goals
navigation-topic: goal-management
title: Erstellen von Zielen in Adobe Workfront Goals
description: Unabhängig davon, ob Sie CEO, Manager oder ein einzelner Mitwirkender sind, können Sie in Adobe Workfront Goals Ziele erstellen, um Ihre Arbeit an Ihren Zielen und den Zielen auszurichten, die die Strategie Ihres Unternehmens darstellen.
author: Alina
feature: Workfront Goals
exl-id: 14bf48b6-eb0c-4b00-a1a4-0d070ccc1392
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 5%

---

# Erstellen von Zielen in Adobe Workfront Goals

<!--Audited for P&P only: 4/2025-->

Unabhängig davon, ob Sie CEO, Manager oder ein einzelner Mitwirkender sind, können Sie in Adobe Workfront Goals Ziele erstellen, um Ihre Arbeit an Ihren Zielen und den Zielen auszurichten, die die Strategie Ihres Unternehmens darstellen.

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

## Richtlinien für die Zielerstellung

Bevor Sie mit der Umsetzung der Workfront-Produktziele beginnen, sollten Sie sich über unsere Empfehlungen zu Best Practices und Richtlinien für die effektive Verwaltung von Produktzielen informieren. Weitere Informationen zu Richtlinien zum Erstellen und Verwalten von Zielen finden Sie unter [Adobe Workfront-Ziele - Übersicht](../../workfront-goals/goal-management/wf-goals-overview.md).

## Erstellen von Zielen

In diesem Artikel wird beschrieben, wie Sie ein strategisches Ziel in Workfront Goals erstellen. Informationen zum Erstellen eines Business-Case-Ziels finden Sie [Erstellen von Business-Case-Zielen](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

Sie können ein strategisches Ziel auf eine der folgenden Arten erstellen:

* [Ziel von Grund auf neu erstellen](#create-a-goal-from-scratch)
* [Kopieren eines vorhandenen Ziels](#copy-an-existing-goal)
* [Konvertieren eines Ergebnisses oder einer Aktivität in ein Ziel](#convert-a-result-or-activity-to-a-goal)

### Ein Ziel von Grund auf neu erstellen {#create-a-goal-from-scratch}

<!--
Creating goals differs depending on what environment you use.

#### Create a goal from scratch in the Production environment 


1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) in the upper right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -)

   The Goal List displays.

1. (Conditional) Click **Goal List**, **Graphs**, **Pulse**, or **Check-in** in the left pane, then click **Add Goal** in the upper-right corner of the page. The Add Goal box displays.

   ![Add goal box](assets/add-goal-box-350x235.png)

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

1. Klicken Sie oben rechts auf **Hauptmenü**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) und dann auf **Ziele**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Die Liste „Ziel“ wird angezeigt.
1. Klicken Sie auf **Neues Ziel**.

   Das Feld Neues Ziel wird angezeigt.

   ![Neues Zielfeld](assets/new-goal-box-unshimmed.png)

1. Geben Sie Informationen in die folgenden Felder ein:
   * **Zielname**: Geben Sie einen Namen für das Ziel ein. Dies ist ein Pflichtfeld.
   * **Zeitraum**: Wählen Sie ein vordefiniertes Quartal oder Jahr aus der Dropdown **Liste &quot;**&quot;

     Oder

     Wählen Sie die Option **Benutzerdefinierte Datumswerte aktivieren** und wählen Sie dann ein **Start** und **Enddatum** für das Ziel aus.

     Das vorherige, aktuelle und das folgende Jahr sowie die entsprechenden Quartale werden als vordefinierte Optionen im Dropdown-Feld Zeitraum aufgeführt.

     Der Zeitraum des Ziels gibt den Zeitrahmen an, in dem das Ziel erwartungsgemäß abgeschlossen wird.

   * **Zielinhaber**: Beginnen Sie mit der Eingabe des Namens eines Benutzers, eines Teams, einer Gruppe oder Ihrer Organisation, um anzugeben, wer der Besitzer des Ziels ist. Sie werden standardmäßig als Eigentümer des Ziels ausgewählt.
   * **Beschreibung**: Geben Sie zusätzliche Informationen zum Ziel ein.
1. Klicken Sie **Ziel erstellen**.

   Das neue Ziel wird in der Liste Ziel aufgeführt und hat den Status **Entwurf**.

   Sie müssen ein Ziel mit einer Fortschrittsanzeige verknüpfen, um es zu aktivieren und mit der Bearbeitung zu beginnen.

   Führen Sie mindestens einen der folgenden Schritte aus, um ein Ziel für die Aktivierung vorzubereiten:
   * Ergebnis hinzufügen

     Informationen zum Hinzufügen von Ergebnissen finden Sie unter [Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront Goals](../results-and-activities/add-results-to-goals.md).
   * Aktivität hinzufügen

     Informationen zum Hinzufügen von Aktivitäten finden Sie unter [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront Goals](../results-and-activities/add-activities-to-goals.md).
   * Ein weiteres Ziel daran ausrichten

     Informationen zum Ausrichten von Zielen finden Sie unter [Ausrichten von Zielen durch Verbinden in Adobe Workfront-Zielen](../goal-alignment/align-goals-by-connecting-them.md).


### Ein vorhandenes Ziel kopieren {#copy-an-existing-goal}

Sie können ein Ziel erstellen, indem Sie ein vorhandenes kopieren.

Informationen zum Kopieren von Zielen finden Sie unter [Kopieren von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/copy-goals.md).

### Konvertieren eines Ergebnisses oder einer Aktivität in ein Ziel {#convert-a-result-or-activity-to-a-goal}

Sie können ein Ziel erstellen, indem Sie das Ergebnis oder die Aktivität eines vorhandenen Ziels in ein Ziel konvertieren. Das neue Ziel wird am ursprünglichen Ziel ausgerichtet.

Informationen zur Konvertierung von Ergebnissen und Aktivitäten in Ziele finden Sie unter [Ausrichten von Zielen durch Konvertieren von Ergebnissen und Aktivitäten in Ziele](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

