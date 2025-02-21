---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Zielausrichtung in Adobe Workfront Goals entfernen
description: Sie können die Ausrichtung zwischen zwei Zielen entfernen, wenn es nicht mehr sinnvoll ist, sie miteinander zu verbinden.
author: Alina
feature: Workfront Goals
exl-id: a6196356-ca11-4759-9cff-64850a60208e
source-git-commit: 45c71a8106bdb8eeaa38f2fb83ff0312e48183d0
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 1%

---

# Zielausrichtung in Adobe Workfront Goals entfernen

Sie können die Ausrichtung zwischen zwei Zielen entfernen, wenn es nicht mehr sinnvoll ist, sie miteinander zu verbinden.

Informationen zum Ausrichten von Zielen finden Sie in den folgenden Artikeln:

* [Ziele ausrichten, indem Sie sie in Adobe Workfront Goals miteinander verbinden](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)
* [Ausrichten von Zielen durch Konvertieren von Ergebnissen und Aktivitäten in Ziele](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md)

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">Adobe Workfront-Plan</td>
 <td>
 <p>Beliebig</p>

</td>
 </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-Lizenz*</td>
 <td>
 <p>Neue Lizenz: Mitwirkende oder höher</p>
 Oder
 <p>Aktuelle Lizenz: Anfrage oder höher</p> </td>
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
 <td role="rowheader">Zugriffsebene</td>
 <td> <p>Zugriff auf Ziele bearbeiten</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objektberechtigungen</td>
 <td>
  <p>Anzeigen von oder höheren Berechtigungen für das Ziel, um es anzuzeigen</p>
  <p>Verwalten von Berechtigungen für das Ziel, um es zu bearbeiten</p>
  <p>Informationen zum Freigeben von Zielen finden Sie <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Freigeben eines Ziels in Workfront Goals</a>. </p>
  </td>
 </tr>
   <td role="rowheader"><p>Layoutvorlage</p></td>
   <td> <p>Allen Benutzenden, einschließlich Workfront-Administratoren, muss eine Layout-Vorlage zugewiesen werden, die den Bereich Ziele im Hauptmenü enthält. </p>  
</td>
  </tr>
</tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

Sie müssen über Folgendes verfügen, bevor Sie beginnen können:

* Ein übergeordnetes Ziel, dem mindestens ein untergeordnetes Ziel zugeordnet ist. Untergeordnete Ziele sind die Fortschrittsindikatoren des Ziels.

## Überlegungen zum Entfernen der Zielausrichtung

Beachten Sie Folgendes, wenn Sie die Ausrichtung zwischen zwei Zielen entfernen:

* Dem übergeordneten Ziel muss ein anderes Ziel, eine andere Aktivität oder ein anderes Ergebnis zugeordnet sein, damit es aktiv bleiben kann.
* Sie können ein angepasstes untergeordnetes Ziel nicht aus einem übergeordneten Ziel entfernen, wenn dies der einzige Fortschrittsindikator des übergeordneten Ziels ist.
* Das untergeordnete Ziel wird zu einem eigenständigen Ziel, wenn Sie dessen Ausrichtung am übergeordneten Ziel entfernen.

## Entfernen der Zielausrichtung

<!--
Removing goal alignment differs depending on which environment you use.

### Remove goal alignment in the Production environment


1. Go to a child goal aligned to a parent goal. 
1. Click the goal name to open the **Goal Details** panel. 
1. Click the **gear icon** ![Gear icon](assets/gear-icon-settings.png) next to the parent goal, then click **Remove alignment**.

   ![Reove alignment](assets/edit-remove-alignment-350x88.png)

   The goal becomes a standalone goal and its progress no longer influences the progress of the original parent goal. 

1. (Optional) Click **Undo** in the lower-left corner of the screen if you want to revert this change and keep the goals aligned. 
1. (Optional) Add activities and results to either goals to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)
-->

1. Rufen Sie den **Ziele** in Workfront auf und klicken Sie auf den Namen eines Ziels, um die Zielseite zu öffnen.
1. Klicken Sie auf der Zielseite eines übergeordneten Ziels im linken Bereich **Fortschrittsanzeigen**.

   ![Zielausrichtung erneut verschieben](assets/remove-goal-alignment-from-list-unshimmed.png)

1. Wählen **in der Gruppierung Typ: Ziel** ein Ziel aus und klicken Sie dann oben in der Liste auf das **Trennen**-Symbol ![Verbindung trennen](assets/disconnect-goal-to-remove-alignment-icon-unshimmed.png).

   Das Dialogfeld Trennen wird angezeigt.

1. Klicken Sie **Trennen**, um das ausgewählte Ziel vom übergeordneten Ziel zu trennen.

   Das Ziel wird zu einem eigenständigen Ziel und wird nicht mehr als Fortschrittsindikator für das ursprüngliche Ziel aufgeführt. Der Fortschritt des getrennten Ziels beeinflusst den Fortschritt des ursprünglichen Ziels nicht mehr.

   Eine Erfolgsmeldung wird oben rechts auf der Seite angezeigt, die bestätigt, dass die Verbindung zum Ziel getrennt wurde.