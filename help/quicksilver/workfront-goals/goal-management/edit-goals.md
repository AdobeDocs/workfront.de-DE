---
product-previous: workfront-goals
navigation-topic: goal-management
title: Ziele in Adobe Workfront bearbeiten
description: Sie können vorhandene Ziele von einem beliebigen Zeitraum bis zu einem beliebigen Status bearbeiten.
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 1%

---

# Ziele in Adobe Workfront bearbeiten

Sie können vorhandene Ziele von einem beliebigen Zeitraum bis zu einem beliebigen Status bearbeiten.

## Zugriffsanforderungen

<!--drafted - for P&P releases: 

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
* Sie haben die Ziele erstellt, die Sie bearbeiten möchten, oder Sie haben Verwaltungsberechtigungen für sie.

## Überlegungen zum Bearbeiten von Zielen

* Ziele mit dem Status Geschlossen können nicht bearbeitet werden.
* Sie können Ziele von einem beliebigen Zeitraum aus bearbeiten.

   Sie können die folgenden Informationen für ein vergangenes Ziel bearbeiten:

   * Name
   * Zeitraum
   * Status

      >[!TIP]
      >
      >Wenn das Ziel geschlossen ist, wird durch erneutes Öffnen der Prozentsatz für die Fertigstellung des Fortschritts neu berechnet. Ein geschlossenes Ziel kann nicht bearbeitet werden.

   * Beschreibung
   * Ergebnisse und Aktivitäten

## Ziele bearbeiten

<!--
Editing goals differs depending on what environment you use.

### Edit goals in the Production environment

1. Go to a goal that you want to edit and click the goal name to open the **Goal Details** panel. 
1. Click the **More icon** ![](assets/more-icon.png), then click **Edit**.

   ![](assets/edit-goal-highlighted.png)

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

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png)Klicken Sie auf **Ziele**.\
   Eine Liste der Ziele wird angezeigt.
1. Klicken Sie auf ein Ziel.\
   Die Zielseite wird angezeigt.

   ![](assets/goal-page-unshimmed.png)

1. Führen Sie einen der folgenden Schritte aus, um Informationen für das Ziel zu bearbeiten:
   * Klicken Sie auf Felder, die in der Zielkopfzeile angezeigt werden, um sie zu aktualisieren. Es können nicht alle Felder in der Kopfzeile bearbeitet werden.
   * Klicken Sie auf **Weitere Symbole** ![](assets/more-icon.png) rechts neben dem Zielnamen, und klicken Sie dann auf **Bearbeiten**.
   * Klicken **Zieldetails** im linken Bereich und klicken Sie auf die **Symbol Bearbeiten** ![](assets/edit-icon.png) in der oberen rechten Ecke und klicken Sie auf **Alle bearbeiten**. Aktualisieren Sie die Felder im Abschnitt Zieldetails .

      >[!IMPORTANT]
      >
      >Es können nicht alle Felder bearbeitet werden, die in den oben genannten Bereichen angezeigt werden. Workfront berechnet einige der Felder und ist schreibgeschützt.

1. (Bedingt) Aktualisieren Sie je nach Auswahl im vorherigen Schritt die folgenden Informationen zum Ziel:

   * Aktualisieren Sie die folgenden Informationen in der Ziel-Kopfzeile und drücken Sie dann die Eingabetaste , um Ihre Änderungen zu speichern:
      * **Zielname**: Klicken Sie auf den Namen des Ziels und geben Sie einen neuen Namen ein.
      * **Inhaber**: Klicken Sie auf den Namen des Eigentümers, geben Sie den Namen eines Benutzers, Teams, einer Gruppe oder Ihres Unternehmens ein und wählen Sie ihn aus, wenn er in der Liste angezeigt wird. Sie können nur einen Inhaber für ein Ziel haben.
   * Aktualisieren Sie die folgenden Informationen im Feld Ziel bearbeiten und klicken Sie auf **Speichern**:
      * **Name des Ziels**
      * **Zeitraum**: Klicken Sie auf , um den Zeitraum für das Ziel zu aktualisieren\
         Oder\
         Auswählen **Benutzerdefinierte Datumswerte aktivieren** zum Angeben von Daten für die **Starten** und **Enddaten**.

         >[!TIP]
         >
         >Auswahl aufheben **Benutzerdefinierte Datumswerte aktivieren** , um zum ursprünglichen Zeitraum für das Ziel zurückzukehren.

      * **Besitzer des Ziels**
      * **Beschreibung**: Hinzufügen oder Aktualisieren von Informationen zum Ziel.
   * Aktualisieren oder überprüfen Sie die Informationen im Abschnitt Zieldetails . Weitere Informationen finden Sie unter [Aktualisieren von Zielen im Abschnitt &quot;Zieldetails&quot;in Adobe Workfront-Zielen](../goal-management/update-goals-in-goal-details-panel.md).

   <!-- (should you update the title here after changing it at production??? - change it to Update goals in the goal Details section)-->

1. (Optional) Klicken Sie auf **Fortschrittsanzeigen** im linken Bereich, um dem Ziel Ergebnisse, Aktivitäten oder Projekte hinzuzufügen. Durch das Hinzufügen von Fortschrittsanzeigen können Sie sicherstellen, dass Sie den Fortschritt des Ziels verfolgen können.
Weitere Informationen finden Sie in den folgenden Artikeln:
   * [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront-Zielen](../results-and-activities/add-activities-to-goals.md)
   * [Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront-Zielen](../results-and-activities/add-results-to-goals.md).
   * [Hinzufügen von Projekten zu Zielen in Adobe Workfront-Zielen](../results-and-activities/connect-projects-to-goals-overview.md).

</div>
