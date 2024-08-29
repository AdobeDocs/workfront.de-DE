---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Ergebnisse und Aktivitäten in Adobe Workfront-Zielen bearbeiten
description: Nachdem Ihnen Ihr Adobe Workfront-Administrator den richtigen Zugriff auf Adobe Workfront-Ziele gewährt hat, können Sie Ziele, Ergebnisse und Aktivitäten erstellen und bearbeiten.
author: Alina
feature: Workfront Goals
exl-id: 922a05f9-2995-4401-a6d2-e5a331270fd3
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '763'
ht-degree: 1%

---

# Ergebnisse und Aktivitäten in Adobe Workfront-Zielen bearbeiten

Nachdem Ihnen Ihr Adobe Workfront-Administrator den richtigen Zugriff auf Adobe Workfront-Ziele gewährt hat, können Sie Ziele, Ergebnisse und Aktivitäten erstellen und bearbeiten.

Informationen zum Erstellen von Zielen, Ergebnissen und Aktivitäten finden Sie in den folgenden Artikeln:

* [Erstellen von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/create-goals.md)
* [Erste Schritte mit Ergebnissen und Aktivitäten in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md)
* [Ergebnisse zu Zielen in Adobe Workfront-Zielen hinzufügen](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/add-activities-to-goals.md)

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
  <ul><li>Ein ultimativer Plan </li></ul>
   </p>
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
 <td role="rowheader"><p>Zugriffsebene</p></td>
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

## Überlegungen beim Bearbeiten von Ergebnissen und Aktivitäten

<!--
According to Vazgen, access levels will add more considerations.)
-->

* Sie können Ergebnisse und Aktivitäten bearbeiten, die zu von Ihnen erstellten Zielen oder Zielen gehören, für die Sie über die Berechtigung zum Verwalten verfügen.
* Sie können den Fortschritt von Projekten, die mit Zielen verknüpft sind, nicht als Aktivitäten aus Workfront-Zielen bearbeiten. Der Projektfortschritt wird aktualisiert, sobald die Aufgaben im Projekt abgeschlossen sind. Sie können Projekte aus dem Ziel entfernen, indem Sie sie trennen. Weitere Informationen finden Sie im Abschnitt &quot;Trennen von Projekten&quot;im Artikel [Entfernen von Ergebnissen, Aktivitäten und Projekten aus Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/remove-results-activities-from-goals.md).

  >[!NOTE]
  >
  >Wenn die folgenden Projektinformationen auf Projektebene aktualisiert werden, aktualisiert Workfront Goals sie automatisch auf der Zielebene:
  >
  >   
  >   
  >   * Projektbesitzer
  >   * Projektname
  >   * Abschluss des Projekts in Prozent
  >   
  >   
  >Informationen zum Verbinden von Projekten mit Zielen finden Sie unter [Projekte zu Zielen in Adobe Workfront-Zielen hinzufügen](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

* Sie können Ergebnisse und Aktivitäten aus Zielen löschen, wenn sie für den Zielfortschritt nicht mehr relevant sind. Gelöschte Ergebnisse und Aktivitäten können nicht wiederhergestellt werden. Informationen zum Löschen von Ergebnissen und Aktivitäten finden Sie unter [Entfernen von Ergebnissen, Aktivitäten und Projekten aus Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/remove-results-activities-from-goals.md).
* Sie können Ergebnisse und Aktivitäten bearbeiten, die mit Zielen verknüpft sind - auch in der Vergangenheit.
* Bei der Bearbeitung von Ergebnissen und Aktivitäten werden deren Einstellungen aktualisiert und der Fortschritt nicht aktualisiert. Sie müssen den Fortschritt der Ergebnisse und Aktivitäten aktualisieren. Informationen zum Aktualisieren des Fortschritts bei Zielen, Ergebnissen und Aktivitäten finden Sie unter [Aktualisieren des Zielfortschritts in Adobe Workfront-Zielen](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).

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


1. Klicken Sie auf das **Hauptmenü** ![](assets/main-menu-icon.png) und dann auf **Ziele**.
1. Klicken Sie in der Zielliste auf den Namen eines Ziels, um die Zielseite zu öffnen.
1. Klicken Sie im linken Bereich auf **Fortschrittsanzeigen** .
1. Wählen Sie in der Liste Fortschrittsanzeigen ein Ergebnis aus und klicken Sie auf das Symbol **Bearbeiten** ![](assets/edit-icon.png).

   Das Feld &quot;Ergebnis bearbeiten&quot;wird geöffnet.

   ![](assets/edit-result-box-unshimmed.png)

1. Bearbeiten Sie die folgenden Informationen:
   * **Ergebnisname**: Der Name des Ergebnisses. Verwenden Sie einen beschreibenden Namen, der zeigt, welches Ergebnis Sie benötigen, um das Ziel zu erreichen.
   * **Result owner**: Der Eigentümer des Ergebnisses. Der Inhaber muss ein aktiver Workfront-Benutzer sein.
   * **Werttyp**: Wie Sie den Fortschritt des Ergebnisses messen.
   * **Anfangswert**: Der Originalwert des Ergebnisses.
   * **Zielwert**: Der gewünschte Wert, wenn das Ergebnis abgeschlossen ist.
Weitere Informationen zu Ergebnisfeldern finden Sie unter [Ergebnisse zu Zielen hinzufügen](../results-and-activities/add-results-to-goals.md).
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

1. Klicken Sie auf das **Hauptmenü** ![](assets/main-menu-icon.png) und dann auf **Ziele**.
1. Klicken Sie in der Zielliste auf den Namen eines Ziels, um die Zielseite zu öffnen.
1. Klicken Sie im linken Bereich auf **Fortschrittsanzeigen** .
1. Wählen Sie eine Aktivität in der Liste Fortschrittsanzeigen aus und klicken Sie auf das Symbol **Bearbeiten** ![](assets/edit-icon.png).

   Das Feld Aktivität bearbeiten wird geöffnet.

   ![](assets/edit-activity-box-unshimmed.png)

1. Bearbeiten Sie die folgenden Informationen:
   * **Aktivitätsname**: Der Name der Aktivität. Verwenden Sie einen beschreibenden Namen, der zeigt, welche Aktivität Sie durchführen sollten, um anzugeben, dass das Ziel abgeschlossen ist.
   * **Aktivitätsinhaber:** Der Eigentümer der Aktivität. Der Inhaber muss ein aktiver Workfront-Benutzer sein.\
     Weitere Informationen zu Aktivitätsfeldern finden Sie unter [Aktivitäten zu Zielen hinzufügen](../results-and-activities/add-activities-to-goals.md).
1. Klicken Sie auf **Speichern**.


