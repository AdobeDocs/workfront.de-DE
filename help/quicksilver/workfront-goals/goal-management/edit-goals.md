---
product-previous: workfront-goals
navigation-topic: goal-management
title: Ziele in Adobe Workfront Goals bearbeiten
description: Sie können vorhandene Ziele aus jedem Zeitraum und in jedem Status bearbeiten.
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 1%

---

# Bearbeiten von Zielen in Adobe Workfront Goals

<!--Audited for P&P only: 10/2025-->

Sie können vorhandene Ziele aus jedem Zeitraum und in jedem Status bearbeiten.

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

## Überlegungen zum Bearbeiten von Zielen

* Ziele mit dem Status Geschlossen können nicht bearbeitet werden.
* Sie können Ziele aus jedem beliebigen Zeitraum bearbeiten.

  Sie können die folgenden Informationen für ein früheres Ziel bearbeiten:

   * Name
   * Zeitraum
   * Status

     >[!TIP]
     >
     >Wenn das Ziel geschlossen ist, wird beim erneuten Öffnen der Fortschritt in Prozent abgeschlossen neu berechnet. Ein geschlossenes Ziel kann nicht bearbeitet werden.

   * Beschreibung
   * Ergebnisse und Aktivitäten

## Ziele bearbeiten

<!--
Editing goals differs depending on what environment you use.

### Edit goals in the Production environment

1. Go to a goal that you want to edit and click the goal name to open the **Goal Details** panel. 
1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Edit**.

   ![Edit goal](assets/edit-goal-highlighted.png)

1. Update the name of the goal in the **Goal** field. 
1. Select a time period when the goal should be completed.

   Select from the following predefined options:

   * The current year
   * The quarters of the current year
   * The next two years
   * The quarters of the next two years

   Or

   Click **Define custom dates** to select a custom time frame. 

1. (Conditional) Select a start and an end date for your goal, if you clicked **Define custom dates**.

   
   <p>(NOTE: these fields don't yet have a name) </p>
   

   >[!CAUTION]
   >
   >You cannot create a goal with custom dates in the past.

1. (Optional) Click **Reset custom dates** to return to the predefined options.

   >[!TIP]
   >
   >We recommend that everyone in your organization selects the same time frames for similar goals or goals that are aligned. This provides better alignment between goals and ensures that everyone's work supports your larger organization-wide strategy.

1. Click the **Owner** field and select a new owner for the goal, if you want to indicate someone else as the owner of the goal. 
1. (Conditional) Start typing the name of a user, team, group, or the name of your organization in the **Owner** field, then select it when it displays in the list. You can have only one owner for a goal. 
1. Update the **Description** of the goal, then click **Save**.

-->

1. Klicken Sie auf das **Hauptmenü**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) und dann auf **Ziele**.\
   Eine Liste der Ziele wird angezeigt.
1. Klicken Sie auf ein Ziel.\
   Die Zielseite wird angezeigt.

   ![Zielseite](assets/goal-page-unshimmed.png)

1. Führen Sie einen der folgenden Schritte aus, um Informationen für das Ziel zu bearbeiten:
   * Klicken Sie auf Felder, die in der Zielkopfzeile angezeigt werden, um sie zu aktualisieren. Nicht alle Felder in der Kopfzeile können bearbeitet werden.
   * Klicken Sie auf **Mehr**![Mehr](assets/more-icon.png) rechts neben dem Zielnamen und dann auf **Bearbeiten**.
   * Klicken Sie **linken** auf „Zieldetails“ und klicken Sie oben rechts auf **Bearbeiten** ![Bearbeiten](assets/edit-icon.png) und dann auf **Alle bearbeiten**. Beginnen Sie mit der Aktualisierung der Felder im Abschnitt Zieldetails .

     >[!IMPORTANT]
     >
     >Nicht alle Felder, die in den oben genannten Bereichen angezeigt werden, können bearbeitet werden. Workfront berechnet einige der Felder und ist schreibgeschützt.

1. (Bedingt) Aktualisieren Sie je nach Auswahl im vorherigen Schritt die folgenden Informationen zum Ziel:

   * Aktualisieren Sie die folgenden Informationen in der Kopfzeile des Ziels und drücken Sie dann die Eingabetaste , um Ihre Änderungen zu speichern:
      * **Zielname**: Klicken Sie auf den Namen des Ziels und geben Sie einen neuen Namen ein.
      * **Verantwortlicher**: Klicken Sie auf den Namen des Verantwortlichen, und geben Sie den Namen eines Benutzers, Teams, einer Gruppe oder Ihrer Firma ein. Wählen Sie den Namen aus, wenn er in der Liste angezeigt wird. Für ein Ziel kann nur ein Besitzer vorhanden sein.
   * Aktualisieren Sie die folgenden Informationen im Feld Ziel bearbeiten und klicken Sie dann auf **Speichern**:
      * **Name des Ziels**
      * **Zeitraum**: Klicken Sie darauf, um den Zeitraum für das Ziel zu aktualisieren\
        Oder\
        Wählen Sie **Benutzerdefinierte Datumswerte aktivieren** **aus, um ein Datum für die Start-** Enddaten **Ziels**.

        >[!TIP]
        >
        >Deaktivieren Sie **Benutzerdefinierte Datumswerte aktivieren**, um zum ursprünglichen Zeitraum für das Ziel zurückzukehren.

      * **Zielbesitzer**
      * **Beschreibung**: Informationen zum Ziel hinzufügen oder aktualisieren.
   * Aktualisieren oder überprüfen Sie die Informationen im Abschnitt mit den Zieldetails. Weitere Informationen finden Sie unter [Aktualisieren von Zielen im Abschnitt „Zieldetails“ in Adobe Workfront-](../goal-management/update-goals-in-goal-details-panel.md).

   <!-- (should you update the title here after changing it at production??? - change it to Update goals in the goal Details section)-->

1. (Optional) Klicken Sie **linken Bereich auf**Fortschrittsanzeigen“, um Ergebnisse, Aktivitäten oder Projekte zum Ziel hinzuzufügen. Durch Hinzufügen von Fortschrittsanzeigen können Sie sicherstellen, dass Sie den Fortschritt des Ziels verfolgen können.
Weitere Informationen finden Sie in den folgenden Artikeln:
   * [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront Goals](../results-and-activities/add-activities-to-goals.md)
   * [Fügen Sie Ergebnisse zu Zielen in Adobe Workfront-Zielen hinzu](../results-and-activities/add-results-to-goals.md).
   * [Projekte zu Zielen in Adobe Workfront-Zielen hinzufügen](../results-and-activities/connect-projects-to-goals-overview.md).

</div>
