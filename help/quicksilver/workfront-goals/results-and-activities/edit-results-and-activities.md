---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Ergebnisse und Aktivitäten in Adobe Workfront Goals bearbeiten
description: Nachdem Ihnen der Adobe Workfront-Administrator den richtigen Zugriff auf Adobe Workfront-Ziele gewährt hat, können Sie Ziele, Ergebnisse und Aktivitäten erstellen und bearbeiten.
author: Alina
feature: Workfront Goals
exl-id: 922a05f9-2995-4401-a6d2-e5a331270fd3
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '713'
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
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Access level</p></td>
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
  >   * Projektbesitzer bzw. -besitzerin
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
1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the result you want to edit.

   ![Results gear icon](assets/results-gear-icon-options-350x85.png)

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


1. Klicken Sie auf **Hauptmenü** ![Hauptmenüsymbol](assets/main-menu-icon.png) und dann auf **Ziele**.
1. Klicken Sie in der Liste Ziel auf den Namen eines Ziels, um die Seite Ziel zu öffnen.
1. Klicken Sie **linken Bereich** Fortschrittsanzeigen“.
1. Wählen Sie ein Ergebnis in der Liste der Fortschrittsanzeigen aus und klicken Sie auf das **Bearbeiten**-Symbol ![Bearbeiten](assets/edit-icon.png).

   Das Feld Ergebnis bearbeiten wird geöffnet.

   ![Ergebnisfeld bearbeiten](assets/edit-result-box-unshimmed.png)

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
1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the activity you want to edit .

   ![Activities gear icon](assets/activities-gear-icon-options-350x84.png)

1. Click **Edit** to edit the following information:

   | Field |Description |
   |---|---|
   | Name |The name of the activity. |
   | Owner |The owner of activity.  |

1. Click **Save**.
-->

1. Klicken Sie auf **Hauptmenü** ![Hauptmenüsymbol](assets/main-menu-icon.png) und dann auf **Ziele**.
1. Klicken Sie in der Liste Ziel auf den Namen eines Ziels, um die Seite Ziel zu öffnen.
1. Klicken Sie **linken Bereich** Fortschrittsanzeigen“.
1. Wählen Sie eine Aktivität in der Liste Fortschrittsanzeigen aus und klicken Sie auf das Symbol **Bearbeiten** ![Symbol Bearbeiten](assets/edit-icon.png).

   Das Feld Aktivität bearbeiten wird geöffnet.

   ![Aktivitätsfeld bearbeiten](assets/edit-activity-box-unshimmed.png)

1. Bearbeiten Sie die folgenden Informationen:
   * **Aktivitätsname**: Der Name der Aktivität. Verwenden Sie einen beschreibenden Namen, der veranschaulicht, welche Aktivität Sie durchführen sollten, um anzugeben, dass das Ziel abgeschlossen ist.
   * **Aktivitätsbesitzer:** Der Eigentümer der Aktivität. Der Besitzer muss ein aktiver Workfront-Benutzer sein.\
     Weitere Informationen zu Aktivitätsfeldern finden Sie unter [Hinzufügen von Aktivitäten zu Zielen](../results-and-activities/add-activities-to-goals.md).
1. Klicken Sie auf **Speichern**.


