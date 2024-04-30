---
product-previous: workfront-goals
navigation-topic: goal-management
title: Ziele in Adobe Workfront bearbeiten
description: Sie können vorhandene Ziele von einem beliebigen Zeitraum bis zu einem beliebigen Status bearbeiten.
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 1%

---

# Ziele in Adobe Workfront bearbeiten

Sie können vorhandene Ziele von einem beliebigen Zeitraum bis zu einem beliebigen Status bearbeiten.

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

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   * Klicken Sie auf **Weitere Symbole** ![](assets/more-icon.png) rechts neben dem Zielnamen, klicken Sie auf **Bearbeiten**.
   * Klicks **Zieldetails** im linken Bereich und klicken Sie auf die **Symbol Bearbeiten** ![](assets/edit-icon.png) in der oberen rechten Ecke und klicken Sie auf **Alle bearbeiten**. Aktualisieren Sie die Felder im Abschnitt Zieldetails .

     >[!IMPORTANT]
     >
     >Es können nicht alle Felder bearbeitet werden, die in den oben genannten Bereichen angezeigt werden. Workfront berechnet einige der Felder und ist schreibgeschützt.

1. (Bedingt) Aktualisieren Sie je nach Auswahl im vorherigen Schritt die folgenden Informationen zum Ziel:

   * Aktualisieren Sie die folgenden Informationen in der Ziel-Kopfzeile und drücken Sie dann die Eingabetaste , um Ihre Änderungen zu speichern:
      * **Zielname**: Klicken Sie auf den Namen des Ziels und geben Sie einen neuen Namen ein.
      * **Inhaber**: Klicken Sie auf den Namen des Eigentümers, geben Sie den Namen eines Benutzers, Teams, einer Gruppe oder Ihres Unternehmens ein und wählen Sie ihn aus, wenn er in der Liste angezeigt wird. Sie können nur einen Inhaber für ein Ziel haben.
   * Aktualisieren Sie die folgenden Informationen im Feld Ziel bearbeiten und klicken Sie auf **Speichern**:
      * **Zielname**
      * **Zeitraum**: Klicken Sie auf , um den Zeitraum für das Ziel zu aktualisieren.\
        Oder\
        Auswählen **Benutzerdefinierte Datumswerte aktivieren** zum Angeben von Daten für die **Starten** und **Enddaten**.

        >[!TIP]
        >
        >Auswahl deaktivieren **Benutzerdefinierte Datumswerte aktivieren** , um zum ursprünglichen Zeitraum für das Ziel zurückzukehren.

      * **Goal Owner**
      * **Beschreibung**: Fügen Sie Informationen zum Ziel hinzu oder aktualisieren Sie diese.
   * Aktualisieren oder überprüfen Sie die Informationen im Abschnitt Zieldetails . Weitere Informationen finden Sie unter [Aktualisieren von Zielen im Abschnitt &quot;Zieldetails&quot;in Adobe Workfront-Zielen](../goal-management/update-goals-in-goal-details-panel.md).

   <!-- (should you update the title here after changing it at production??? - change it to Update goals in the goal Details section)-->

1. (Optional) Klicken Sie auf **Fortschrittsanzeigen** im linken Bereich, um dem Ziel Ergebnisse, Aktivitäten oder Projekte hinzuzufügen. Durch das Hinzufügen von Fortschrittsanzeigen können Sie sicherstellen, dass Sie den Fortschritt des Ziels verfolgen können.
Weitere Informationen finden Sie in den folgenden Artikeln:
   * [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront-Zielen](../results-and-activities/add-activities-to-goals.md)
   * [Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront-Zielen](../results-and-activities/add-results-to-goals.md).
   * [Hinzufügen von Projekten zu Zielen in Adobe Workfront-Zielen](../results-and-activities/connect-projects-to-goals-overview.md).

</div>
