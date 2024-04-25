---
product-previous: workfront-goals
navigation-topic: goal-management
title: Ziele in Adobe Workfront erstellen
description: Unabhängig davon, ob Sie CEO, Manager oder Einzelmitwirkender sind, können Sie in Adobe Workfront Goals Ziele festlegen, um Ihre Arbeit an Ihren Zielen und Zielen auszurichten, die die Strategie Ihres Unternehmens umreißen.
author: Alina
feature: Workfront Goals
exl-id: 14bf48b6-eb0c-4b00-a1a4-0d070ccc1392
source-git-commit: 09e34ecdfeec531ebbaaba4fb8682496c53d86bf
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 5%

---

# Ziele in Adobe Workfront erstellen

Unabhängig davon, ob Sie CEO, Manager oder Einzelmitwirkender sind, können Sie in Adobe Workfront Goals Ziele festlegen, um Ihre Arbeit an Ihren Zielen und Zielen auszurichten, die die Strategie Ihres Unternehmens umreißen.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">Adobe Workfront-Abo</td>
 <td>
 <p>Alle</p>

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
<p>Anzeigen oder Anzeigen höherer Berechtigungen zum Ziel</p>
<p>Berechtigungen für das Ziel verwalten</p>
<p>Informationen zum Freigeben von Zielen finden Sie unter <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Freigeben eines Ziels in Workfront-Zielen</a>. </p>
</td>
</tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Ziele im Hauptmenü enthält. </p>  
</td>
  </tr>
</tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Richtlinien für das Erstellen von Zielen

Bevor Sie mit Workfront-Zielen beginnen, empfehlen wir Ihnen, sich über unsere Best Practices-Empfehlungen und -Richtlinien für die wirksame Verwaltung von Zielen zu informieren. Weitere Informationen zu Richtlinien zum Erstellen und Verwalten von Zielen finden Sie unter [Übersicht über Adobe Workfront-Ziele](../../workfront-goals/goal-management/wf-goals-overview.md).

## Erstellen von Zielen

In diesem Artikel wird beschrieben, wie Sie ein strategisches Ziel in Workfront-Zielen erstellen. Informationen zum Erstellen eines Geschäftsfallziels finden Sie unter [Geschäftsfallziele erstellen](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

Sie können ein strategisches Ziel auf eine der folgenden Arten erstellen:

* [Neues Ziel erstellen](#create-a-goal-from-scratch)
* [Vorhandenes Ziel kopieren](#copy-an-existing-goal)
* [Konvertieren eines Ergebnisses oder einer Aktivität in ein Ziel](#convert-a-result-or-activity-to-a-goal)

### Ein Ziel von Grund auf neu erstellen {#create-a-goal-from-scratch}

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
1. Klicks **Neues Ziel**.

   Das Feld Neues Ziel wird angezeigt.

   ![](assets/new-goal-box-unshimmed.png)

1. Geben Sie Informationen in die folgenden Felder ein:
   * **Zielname**: Geben Sie einen Namen für das Ziel ein. Dies ist ein Pflichtfeld.
   * **Zeitraum**: Wählen Sie ein vordefiniertes Quartal oder Jahr aus dem **Zeitraum** Dropdown-Feld

     Oder

     Wählen Sie die **Benutzerdefinierte Datumswerte aktivieren** und wählen Sie eine **Starten** und **Enddatum** für das Ziel.

     Die vorherigen, aktuellen und nachfolgenden Jahre und ihre jeweiligen Quartale werden als vordefinierte Optionen im Dropdown-Feld Zeitraum aufgeführt.

     Der Zeitraum des Ziels gibt den Zeitraum an, in dem das Ziel voraussichtlich abgeschlossen sein wird.

   * **Goal Owner**: Beginnen Sie mit der Eingabe des Namens eines Benutzers, eines Teams, einer Gruppe oder Ihres Unternehmens, um anzugeben, wer Inhaber des Ziels ist. Sie werden standardmäßig als Eigentümer des Ziels ausgewählt.
   * **Beschreibung**: Geben Sie zusätzliche Informationen zum Ziel ein.
1. Klicks **Ziel erstellen**.

   Das neue Ziel wird in der Zielliste aufgeführt und hat den Status **Entwurf**.

   Sie müssen ein Ziel mit einer Fortschrittsanzeige verknüpfen, um es zu aktivieren und damit zu beginnen, daran zu arbeiten.

   Führen Sie mindestens einen der folgenden Schritte aus, um ein zu aktivierendes Ziel vorzubereiten:
   * Ergebnis hinzufügen

     Informationen zum Hinzufügen von Ergebnissen finden Sie unter [Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront-Zielen](../results-and-activities/add-results-to-goals.md).
   * Aktivität hinzufügen

     Informationen zum Hinzufügen von Aktivitäten finden Sie unter [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront-Zielen](../results-and-activities/add-activities-to-goals.md).
   * Ein anderes Ziel daran ausrichten

     Informationen zum Ausrichten von Zielen finden Sie unter [Ziele durch Verbinden in Adobe Workfront-Zielen ausrichten](../goal-alignment/align-goals-by-connecting-them.md).


### Ein vorhandenes Ziel kopieren {#copy-an-existing-goal}

Sie können ein Ziel durch Kopieren eines vorhandenen Ziels erstellen.

Informationen zum Kopieren von Zielen finden Sie unter [Kopieren von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/copy-goals.md).

### Konvertieren eines Ergebnisses oder einer Aktivität in ein Ziel {#convert-a-result-or-activity-to-a-goal}

Sie können ein Ziel erstellen, indem Sie das Ergebnis oder die Aktivität eines vorhandenen Ziels in ein Ziel konvertieren. Das neue Ziel wird an das ursprüngliche Ziel ausgerichtet.

Informationen zum Konvertieren von Ergebnissen und Aktivitäten in Ziele finden Sie unter [Ziele durch Konvertieren von Ergebnissen und Aktivitäten in Ziele ausrichten](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

