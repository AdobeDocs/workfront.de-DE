---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Ergebnisse und Aktivitäten in Adobe Workfront Goals bearbeiten
description: Nachdem Ihnen der Adobe Workfront-Administrator den richtigen Zugriff auf Adobe Workfront-Ziele gewährt hat, können Sie Ziele, Ergebnisse und Aktivitäten erstellen und bearbeiten.
author: Alina
feature: Workfront Goals
exl-id: 922a05f9-2995-4401-a6d2-e5a331270fd3
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '763'
ht-degree: 1%

---

# Ergebnisse und Aktivitäten in Adobe Workfront Goals bearbeiten

Nachdem Ihnen der Adobe Workfront-Administrator den richtigen Zugriff auf Adobe Workfront-Ziele gewährt hat, können Sie Ziele, Ergebnisse und Aktivitäten erstellen und bearbeiten.

Informationen zum Erstellen von Zielen, Ergebnissen und Aktivitäten finden Sie in den folgenden Artikeln:

* [Erstellen von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/create-goals.md)
* [Erste Schritte mit Ergebnissen und Aktivitäten in Adobe Workfront Goals](../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md)
* [Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md)

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
   <p>Für die neue Plan- und Lizenzstruktur:
  <ul><li>Ein Ultimate-Plan </li></ul>
   </p>
<p>Für die aktuelle Plan- und Lizenzstruktur: 
<ul><li> Ein Profi oder höher </li>
  <li>Eine Adobe Workfront-Ziellizenz zusätzlich zu einer Workfront-Lizenz.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-Lizenz*</td>
 <td>
 <p>Neue Lizenz: Mitwirkende oder höher</p>
 Oder
 <p>Aktuelle Lizenz: Anfrage oder höher</p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe Workfront-Lizenzen</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produkt*</td>
 <td>
 <p> Neue Produktanforderung, eine der folgenden: </p>
<ul>
<li>Einen ausgewählten oder Prime Adobe Workfront-Plan und eine zusätzliche Adobe Workfront Goals-Lizenz.</li>
<li>Ein Ultimate Workfront-Plan, der standardmäßig Workfront-Ziele enthält. </li></ul>
 <p>Oder</p>
 <p>Aktuelle Produktanforderung: Ein Workfront-Plan und eine zusätzliche Lizenz für Adobe Workfront Goals. </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Voraussetzungen für die Verwendung von Workfront-Zielen</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Zugriffsebene</p></td>
 <td> <p>Zugriff auf Ziele bearbeiten</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objektberechtigungen</td>
 <td>
  <div>
  <p>Anzeigen von oder höheren Berechtigungen für das Ziel, um es anzuzeigen</p>
  <p>Verwalten von Berechtigungen für das Ziel, um es zu bearbeiten</p>
  <p>Informationen zum Freigeben von Zielen finden Sie <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Freigeben eines Ziels in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layoutvorlage</p></td>
   <td> <p>Allen Benutzenden, einschließlich Workfront-Administratoren, muss eine Layout-Vorlage zugewiesen werden, die den Bereich Ziele im Hauptmenü enthält. </p>  
</td>
  </tr>
</tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Überlegungen beim Bearbeiten von Ergebnissen und Aktivitäten

<!--
According to Vazgen, access levels will add more considerations.)
-->

* Sie können Ergebnisse und Aktivitäten bearbeiten, die zu von Ihnen erstellten Zielen oder zu Zielen gehören, für die Sie über Berechtigungen zum Verwalten verfügen.
* Sie können den Fortschritt von Projekten, die mit Zielen als Aktivitäten verbunden sind, nicht über Workfront Goals bearbeiten. Der Projektfortschritt wird aktualisiert, wenn Aufgaben im Projekt abgeschlossen sind. Sie können Projekte aus dem Ziel entfernen, indem Sie sie trennen. Weitere Informationen finden Sie im Abschnitt „Trennen von Projekten“ im Artikel [Entfernen von Ergebnissen, Aktivitäten und Projekten aus Zielen in Adobe Workfront Goals](../../workfront-goals/results-and-activities/remove-results-activities-from-goals.md).

  >[!NOTE]
  >
  >Wenn die folgenden Projektinformationen auf Projektebene aktualisiert werden, werden sie von Workfront Goals automatisch auf Zielebene aktualisiert:
  >
  >   
  >   
  >   * Projektbesitzer
  >   * Projektname
  >   * Projekt Prozent abgeschlossen
  >   
  >   
  >Informationen zum Verbinden von Projekten mit Zielen finden Sie unter [Hinzufügen von Projekten zu Zielen in Adobe Workfront Goals](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

* Sie können Ergebnisse und Aktivitäten aus Zielen löschen, wenn sie für den Zielfortschritt nicht mehr relevant sind. Gelöschte Ergebnisse und Aktivitäten können nicht wiederhergestellt werden. Informationen zum Löschen von Ergebnissen und Aktivitäten finden Sie unter [Entfernen von Ergebnissen, Aktivitäten und Projekten aus Zielen in Adobe Workfront Goals](../../workfront-goals/results-and-activities/remove-results-activities-from-goals.md).
* Sie können Ergebnisse und Aktivitäten bearbeiten, die mit Zielen aus einem beliebigen Zeitraum in Verbindung stehen, auch aus der Vergangenheit.
* Durch die Bearbeitung von Ergebnissen und Aktivitäten werden deren Einstellungen aktualisiert, ohne dass der Fortschritt aktualisiert wird. Sie müssen den Fortschritt der Ergebnisse und Aktivitäten aktualisieren. Informationen zum Aktualisieren des Fortschritts bei Zielen, Ergebnissen und Aktivitäten finden Sie unter [Aktualisieren des Zielfortschritts in Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).

## Ergebnisse bearbeiten

<!--
Editing results differs depending on which environment you use.

### Edit results in the Production environment

1. Go to the goal for which you want to edit a result and click the goal name to open the **Goal Details** panel.
1. Click **Results**.
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result you want to edit.

   ![](assets/results-gear-icon-options-350x85.png)

1. Click **Edit** to edit the following information:

   | Field |Description|
   |---|---|
   | Name |The name of the result. |
   | Owner |The owner of result.  |
   | Value |How you measure the progress of the result. |
   | Initial |The original value of the result. |
   | Target |The desired value when the result is completed. |

1. Click **Save**.
-->


1. Klicken Sie auf **Hauptmenü** ![](assets/main-menu-icon.png) dann auf **Ziele**.
1. Klicken Sie in der Liste Ziel auf den Namen eines Ziels, um die Seite Ziel zu öffnen.
1. Klicken Sie **linken Bereich** Fortschrittsanzeigen“.
1. Wählen Sie ein Ergebnis in der Liste der Fortschrittsanzeigen aus und klicken Sie auf das Symbol **Bearbeiten** ![](assets/edit-icon.png).

   Das Feld Ergebnis bearbeiten wird geöffnet.

   ![](assets/edit-result-box-unshimmed.png)

1. Bearbeiten Sie die folgenden Informationen:
   * **Ergebnisname**: Der Name des Ergebnisses. Verwenden Sie einen beschreibenden Namen, der veranschaulicht, welches Ergebnis Sie erreichen müssen, um das Ziel abzuschließen.
   * **Ergebnisbesitzer**: Der Besitzer des Ergebnisses. Der Besitzer muss ein aktiver Workfront-Benutzer sein.
   * **Werttyp**: Wie Sie den Fortschritt des Ergebnisses messen.
   * **Anfangswert**: Der ursprüngliche Wert des Ergebnisses.
   * **Zielwert**: Der gewünschte Wert, wenn das Ergebnis abgeschlossen ist.
Weitere Informationen zu Ergebnisfeldern finden Sie unter [Hinzufügen von Ergebnissen zu Zielen](../results-and-activities/add-results-to-goals.md).
1. Klicken Sie auf **Speichern**.

## Aktivitäten bearbeiten

<!--
Editing activities differs depending on which environment you use.

### Edit activities in the Production environment

>[!TIP]
>
>You cannot edit the Activity Type after you saved an activity on a goal.

1. Go to the goal for which you want to edit an activity and click the goal name to open the **Goal Details** panel.
1. Click **Activities**.
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the activity you want to edit .

   ![](assets/activities-gear-icon-options-350x84.png)

1. Click **Edit** to edit the following information:

   | Field |Description |
   |---|---|
   | Name |The name of the activity. |
   | Owner |The owner of activity.  |

1. Click **Save**.
-->

1. Klicken Sie auf **Hauptmenü** ![](assets/main-menu-icon.png) dann auf **Ziele**.
1. Klicken Sie in der Liste Ziel auf den Namen eines Ziels, um die Seite Ziel zu öffnen.
1. Klicken Sie **linken Bereich** Fortschrittsanzeigen“.
1. Wählen Sie eine Aktivität in der Liste Fortschrittsanzeigen aus und klicken Sie auf das Symbol **Bearbeiten** ![](assets/edit-icon.png).

   Das Feld Aktivität bearbeiten wird geöffnet.

   ![](assets/edit-activity-box-unshimmed.png)

1. Bearbeiten Sie die folgenden Informationen:
   * **Aktivitätsname**: Der Name der Aktivität. Verwenden Sie einen beschreibenden Namen, der veranschaulicht, welche Aktivität Sie durchführen sollten, um anzugeben, dass das Ziel abgeschlossen ist.
   * **Aktivitätsbesitzer:** Der Eigentümer der Aktivität. Der Besitzer muss ein aktiver Workfront-Benutzer sein.\
     Weitere Informationen zu Aktivitätsfeldern finden Sie unter [Hinzufügen von Aktivitäten zu Zielen](../results-and-activities/add-activities-to-goals.md).
1. Klicken Sie auf **Speichern**.


