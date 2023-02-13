---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Entfernen der Zielausrichtung in Adobe Workfront-Zielen
description: Sie können die Ausrichtung zwischen zwei Zielen entfernen, wenn es nicht mehr sinnvoll ist, sie miteinander zu verbinden.
author: Alina
feature: Workfront Goals
exl-id: a6196356-ca11-4759-9cff-64850a60208e
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---

# Entfernen der Zielausrichtung in Adobe Workfront-Zielen

Sie können die Ausrichtung zwischen zwei Zielen entfernen, wenn es nicht mehr sinnvoll ist, sie miteinander zu verbinden.

Informationen zum Ausrichten von Zielen finden Sie in den folgenden Artikeln:

* [Ziele durch Verbinden in Adobe Workfront-Zielen ausrichten](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)
* [Ziele durch Konvertieren von Ergebnissen und Aktivitäten in Ziele ausrichten](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md)

## Zugriffsanforderungen

<!--drafted - replace the table below with this one when P&P releases: 

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
* Ein übergeordnetes Ziel, dem mindestens ein untergeordnetes Ziel zugeordnet ist. Kinderziele sind die Fortschrittsindikatoren des Ziels.

## Überlegungen zum Entfernen der Zielausrichtung

Beachten Sie beim Entfernen der Ausrichtung zwischen zwei Zielen Folgendes:

* Dem übergeordneten Ziel muss ein anderes Ziel, eine andere Aktivität oder ein anderes Ergebnis zugeordnet sein, damit es aktiv bleiben kann.
* Sie können ein ausgerichtetes untergeordnetes Ziel nicht aus einem übergeordneten Ziel entfernen, wenn es der einzige Fortschrittsindikator des übergeordneten Ziels ist.
* Das untergeordnete Ziel wird zum eigenständigen Ziel, wenn Sie die Ausrichtung zum übergeordneten Ziel entfernen.

## Zielausrichtung entfernen

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

1. Klicken **Trennen** , um das ausgewählte Ziel von seinem übergeordneten Ziel zu trennen.

   Das Ziel wird zu einem eigenständigen Ziel und wird nicht mehr als Fortschrittsanzeige des ursprünglichen Ziels aufgeführt. Der Fortschritt des nicht verbundenen Ziels beeinflusst nicht mehr den Fortschritt des ursprünglichen Ziels.

   In der rechten oberen Ecke der Seite wird eine Erfolgsmeldung angezeigt, um zu bestätigen, dass die Verbindung zum Ziel getrennt wurde.