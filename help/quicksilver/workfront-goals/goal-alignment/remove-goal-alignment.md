---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Entfernen der Zielausrichtung in Adobe Workfront-Zielen
description: Sie können die Ausrichtung zwischen zwei Zielen entfernen, wenn es nicht mehr sinnvoll ist, sie miteinander zu verbinden.
author: Alina
feature: Workfront Goals
exl-id: a6196356-ca11-4759-9cff-64850a60208e
source-git-commit: 2f8a5b2d2183090029966a13c7af37f20eb44fd0
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 1%

---

# Entfernen der Zielausrichtung in Adobe Workfront-Zielen

Sie können die Ausrichtung zwischen zwei Zielen entfernen, wenn es nicht mehr sinnvoll ist, sie miteinander zu verbinden.

Informationen zum Ausrichten von Zielen finden Sie in den folgenden Artikeln:

* [Ziele durch Verbinden in Adobe Workfront-Zielen ausrichten](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)
* [Ziele durch Konvertieren von Ergebnissen und Aktivitäten in Ziele ausrichten](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md)

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
   <p>Neuer Plan: Auswählen oder höher</p>
   Oder
   <p>Aktueller Plan: Pro oder höher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront-Lizenz*</td>
   <td>
   <p>Neue Lizenz: Mitarbeiter oder höher</p>
   Oder
   <p>Aktuelle Lizenz: Anfrage oder höher</p> </td>
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
    <p>Anzeigen oder Anzeigen höherer Berechtigungen zum Ziel</p>
     <p>Berechtigungen für das Ziel verwalten</p>
     <p>Informationen zum Freigeben von Zielen finden Sie unter <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Freigeben eines Ziels in Workfront-Zielen</a>. </p>
    </td>
  </tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Ziele im Hauptmenü enthält. </p>  
</td>
  </tr>
 </tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

Sie müssen über Folgendes verfügen, bevor Sie beginnen können:

* Ein übergeordnetes Ziel, dem mindestens ein untergeordnetes Ziel zugeordnet ist. Kinderziele sind die Fortschrittsindikatoren des Ziels.

## Überlegungen zum Entfernen der Zielausrichtung

Beachten Sie Folgendes, wenn Sie die Ausrichtung zwischen zwei Zielen entfernen:

* Dem übergeordneten Ziel muss ein anderes Ziel, eine andere Aktivität oder ein anderes Ergebnis zugeordnet sein, damit es aktiv bleiben kann.
* Sie können ein ausgerichtetes untergeordnetes Ziel nicht aus einem übergeordneten Ziel entfernen, wenn es der einzige Fortschrittsindikator des übergeordneten Ziels ist.
* Das untergeordnete Ziel wird zum eigenständigen Ziel, wenn Sie die Ausrichtung zum übergeordneten Ziel entfernen.

## Entfernen der Zielausrichtung

<!--
Removing goal alignment differs depending on which environment you use.

### Remove goal alignment in the Production environment


1. Go to a child goal aligned to a parent goal. 
1. Click the goal name to open the **Goal Details** panel. 
1. Click the **gear icon** ![](assets/gear-icon-settings.png) next to the parent goal, then click **Remove alignment**.

   ![](assets/edit-remove-alignment-350x88.png)

   The goal becomes a standalone goal and its progress no longer influences the progress of the original parent goal. 

1. (Optional) Click **Undo** in the lower-left corner of the screen if you want to revert this change and keep the goals aligned. 
1. (Optional) Add activities and results to either goals to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)
-->

1. Zugriff auf **Ziele** und klicken Sie auf den Namen eines Ziels, um die Zielseite zu öffnen.
1. Klicken Sie auf der Seite des Ziels eines übergeordneten Ziels auf **Fortschrittsanzeigen** im linken Bereich.

   ![](assets/remove-goal-alignment-from-list-unshimmed.png)

1. Im **Typ: Ziel** Gruppierung, ein Ziel auswählen und auf die **Trennen** icon ![](assets/disconnect-goal-to-remove-alignment-icon-unshimmed.png) oben in der Liste.

   Das Feld Verbindung trennen wird angezeigt.

1. Klicks **Trennen** , um das ausgewählte Ziel von seinem übergeordneten Ziel zu trennen.

   Das Ziel wird zu einem eigenständigen Ziel und wird nicht mehr als Fortschrittsanzeige des ursprünglichen Ziels aufgeführt. Der Fortschritt des nicht verbundenen Ziels beeinflusst nicht mehr den Fortschritt des ursprünglichen Ziels.

   In der rechten oberen Ecke der Seite wird eine Erfolgsmeldung angezeigt, um zu bestätigen, dass die Verbindung zum Ziel getrennt wurde.