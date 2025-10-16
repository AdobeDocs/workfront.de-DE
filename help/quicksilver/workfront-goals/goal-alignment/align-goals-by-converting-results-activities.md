---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Ausrichten von Zielen durch Konvertieren von Ergebnissen und Aktivitäten in Ziele
description: Sie können zwei Ziele manuell ausrichten oder die Ergebnisse und Aktivitäten eines vorhandenen Ziels in ein anderes Ziel konvertieren. Das konvertierte Ergebnis oder die konvertierte Aktivität wird zum untergeordneten Ziel des ursprünglichen Ziels. Informationen zum manuellen Ausrichten von zwei Zielen finden Sie unter Ausrichten von Zielen durch Verbinden in Adobe Workfront-Zielen.
author: Alina
feature: Workfront Goals
exl-id: 48371389-952c-4732-b519-9774cd4d1b93
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 17%

---

# Ausrichten von Zielen durch Konvertieren von Ergebnissen und Aktivitäten in Ziele

<!--Audited P&P only: 4/2025-->

Sie können zwei Ziele manuell ausrichten oder die Ergebnisse und Aktivitäten eines vorhandenen Ziels in ein anderes Ziel konvertieren. Das konvertierte Ergebnis oder die konvertierte Aktivität wird zum untergeordneten Ziel des ursprünglichen Ziels.
Informationen zum manuellen Ausrichten von zwei Zielen finden Sie unter [Ausrichten von Zielen durch Verbinden in Adobe Workfront-Zielen](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

## Zugriffsanforderungen

>[!NOTE]
>
>Ihr Unternehmen könnte sich dafür entscheiden, weiterhin Adobe Workfront Goals zu verwenden, wenn es dieses Paket in der Vergangenheit gekauft hat. Weitere Informationen erhalten Sie von Ihrem Kundenbetreuer.
>
>Adobe Workfront Goals ist nicht mehr erhältlich.

+++Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<td> <p>Adobe Workfront-Paket</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-Lizenz</p> </td> 
   <td> <p>Mitwirkender oder höher</p> 
     <p>Antragsteller oder höher</p> </td> 
  </tr>

<td><p>Konfigurationen der Zugriffsebene</p> </td> 
   <td> <p>Zugriff auf Ziele bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Objektberechtigungen </p> </td> 
   <td> <p>Verwalten von Berechtigungen für ein Ziel</p>  </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Systemadministratoren, muss eine Layout-Vorlage zugewiesen werden, die den Bereich Ziele im Hauptmenü enthält. </p>  
</td>
  </tr>
 </tbody> 
</table>

Weitere Informationen finden Sie [Dokumentation zu Zugriffsanforderungen für Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <p> New product requirement: Workfront</p>
   Or
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

## Voraussetzungen

Sie müssen über Folgendes verfügen, bevor Sie beginnen können:

* Ein vorhandenes Ziel mit vorhandenen Ergebnissen und Aktivitäten.

  Informationen zum Erstellen von Zielen finden Sie unter [Erstellen von Zielen in Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>Ein Ziel kann über bis zu 1000 Fortschrittsindikatoren verfügen.

<!--drafted for goal redesign: At PRODUCTION: update the sentence above to remove Production/ Preview references-->

## Überlegungen zur Konvertierung von Ergebnissen und Aktivitäten in Ziele

Manchmal haben Ergebnisse oder Aktivitäten einen größeren Umfang als erwartet, und es wäre sinnvoller, sie zu Zielen zu machen. Sie können die Ergebnisse und Aktivitäten eines vorhandenen Ziels in ein neues Ziel konvertieren. Dies ist ein Bottom-up-Ansatz zur Ausrichtung der Ziele.

Beachten Sie beim Konvertieren von Ergebnissen und Aktivitäten in Ziele Folgendes:

* Das konvertierte Ergebnis oder die Aktivität wird zum untergeordneten Ziel des ursprünglichen Ziels und die beiden Ziele werden aufeinander abgestimmt.
* Das neu erstellte Ziel wird zur einzigen Fortschrittsanzeige für das ursprüngliche Ziel, wenn es keine zusätzlichen Ergebnisse oder Aktivitäten für das ursprüngliche Ziel gibt. Sie müssen zum untergeordneten Ziel Ergebnisse und Aktivitäten hinzufügen, um den Fortschritt verfolgen zu können.
* Die Konvertierung eines Ergebnisses oder einer Tätigkeit in ein Ziel kann nicht rückgängig gemacht werden. Nach der Konvertierung kann das neue untergeordnete Ziel nie wieder zu einem Ergebnis oder einer Aktivität für das übergeordnete Ziel werden.

## Konvertieren eines Ergebnisses oder einer Aktivität in ein Ziel

<!--
<span class="preview">Converting results and activities differs depending on what environment you use. </span>

### Convert a result or activity to a goal in the Production environment

1. Go to a goal that has a result or an activity that you want to convert to a goal.
1. Click the name of the goal to open the **Goal Details** panel.
1. Expand the **Results** or **Activities** right-pointing arrows to see a list of results or activities for the goal. 

1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the result or activity name that you want to convert, then click **Convert into a Goal**.

   ![Convert to goal](assets/convert-to-goal-link-highlighted-350x191.png)

1. (Optional) Remove the name of the original activity or result owner from the **Goal Owner** field and replace it with another user, team, group, or your organization's name. By default, Workfront selects the owner of the result or the activity as the goal owner. 
1. Click **Convert**. The activity or result displays as an aligned goal in the Goal Details panel of the original goal and the original activity or result is removed from the original goal and transferred to the second goal. By default, the new goal has the same name as the original converted result or activity. 
1. (Optional) Click the name of the new goal to open the **Goal Details** panel and edit the name of the goal. For information about editing any information for an existing goal, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
-->

1. Navigieren Sie zu einem Ziel mit einem Ergebnis oder einer Aktivität, die Sie in ein Ziel konvertieren möchten.
1. Klicken Sie auf der Zielseite im linken Bereich **Fortschrittsanzeigen**.
1. Wählen Sie ein Ergebnis oder eine Aktivität in der Liste der Fortschrittsindikatoren aus und klicken Sie dann oben in der Fortschrittsindikatorliste auf **In Ziel** Konvertieren![-Symbol ](assets/convert-to-goal-icon-unshimmed.png)In Ziel konvertieren . Das Feld In Ziel konvertieren wird geöffnet.

   ![In Zielfeld konvertieren](assets/convert-to-goal-box-unshimmed.png)
1. Aktualisieren Sie die folgenden Informationen:
   * **Zielname**: Standardmäßig hat das neue Ziel denselben Namen wie das ursprüngliche Ergebnis oder die ursprüngliche Aktivität.
   * **Zeitraum**: Standardmäßig ist der Zeitraum des neuen Ziels das aktuelle Quartal. Sie können die Einstellung **Benutzerdefinierte Datumswerte aktivieren** auswählen, um einen benutzerdefinierten Zeitraum für das neue Ziel zu definieren.
   * **Zieleigentümer**: Standardmäßig ist der neue Zieleigentümer der Eigentümer des ursprünglichen Ergebnisses oder der ursprünglichen Aktivität.
   * **Beschreibung**: Fügen Sie weitere Informationen über das neue Ziel hinzu.
1. Klicken Sie auf **Speichern**.

   Das Ergebnis oder die Aktivität wird jetzt in ein untergeordnetes Ziel des ursprünglichen Ziels konvertiert. Es wird als Ziel in der Liste der Fortschrittsindikatoren des ursprünglichen Ziels aufgeführt.



