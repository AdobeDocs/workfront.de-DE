---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Ziele durch Konvertieren von Ergebnissen und Aktivitäten in Ziele ausrichten
description: Sie können zwei Ziele manuell ausrichten oder die Ergebnisse und Aktivitäten eines vorhandenen Ziels in ein anderes umwandeln. Das konvertierte Ergebnis oder die konvertierte Aktivität wird zum untergeordneten Ziel des ursprünglichen Ziels. Informationen zum manuellen Ausrichten von zwei Zielen finden Sie unter Ausrichten von Zielen durch Verbinden in Adobe Workfront-Zielen.
author: Alina
feature: Workfront Goals
exl-id: 48371389-952c-4732-b519-9774cd4d1b93
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 0%

---

# Ziele durch Konvertieren von Ergebnissen und Aktivitäten in Ziele ausrichten

Sie können zwei Ziele manuell ausrichten oder die Ergebnisse und Aktivitäten eines vorhandenen Ziels in ein anderes umwandeln. Das konvertierte Ergebnis oder die konvertierte Aktivität wird zum untergeordneten Ziel des ursprünglichen Ziels.
Informationen zum manuellen Ausrichten von zwei Zielen finden Sie unter [Ziele durch Verbinden in Adobe Workfront-Zielen ausrichten](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

## Zugriffsanforderungen


<!--drafted for P&P release: 

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
* Ein vorhandenes Ziel mit vorhandenen Ergebnissen und Aktivitäten.

   Informationen zum Erstellen von Zielen finden Sie unter [Erstellen von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>Ein Ziel kann über bis zu 1000 Fortschrittsanzeigen verfügen.

<!--drafted for goal redesign: At PRODUCTION: update the sentence above to remove Production/ Preview references-->

## Überlegungen beim Konvertieren von Ergebnissen und Aktivitäten in Ziele

Manchmal kann ein Ergebnis oder eine Aktivität einen größeren Umfang haben als erwartet, und es wäre sinnvoller, dass sie zu Zielen werden. Sie können die Ergebnisse und Aktivitäten eines vorhandenen Ziels in ein neues Ziel konvertieren. Dies ist ein Bottom-up-Ansatz zur Ausrichtung von Zielen.

Beachten Sie beim Konvertieren von Ergebnissen und Aktivitäten in Ziele Folgendes:

* Das konvertierte Ergebnis oder die Aktivität wird zum untergeordneten Ziel des ursprünglichen Ziels und die beiden Ziele werden aufeinander abgestimmt.
* Das neu erstellte Ziel wird zum einzigen Fortschrittsindikator für das ursprüngliche Ziel, wenn keine zusätzlichen Ergebnisse oder Aktivitäten für das ursprüngliche Ziel vorhanden sind. Sie müssen dem untergeordneten Ziel Ergebnisse und Aktivitäten hinzufügen, um den Fortschritt verfolgen zu können.
* Das Konvertieren eines Ergebnisses oder einer Aktivität in ein Ziel ist unumkehrbar. Nach der Konvertierung kann das neue untergeordnete Ziel nie wieder ein Ergebnis oder eine Aktivität für das übergeordnete Ziel werden.

## Konvertieren eines Ergebnisses oder einer Aktivität in ein Ziel

<!--
<span class="preview">Converting results and activities differs depending on what environment you use. </span>

### Convert a result or activity to a goal in the Production environment

1. Go to a goal that has a result or an activity that you want to convert to a goal.
1. Click the name of the goal to open the **Goal Details** panel.
1. Expand the **Results** or **Activities** right-pointing arrows to see a list of results or activities for the goal. 

1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result or activity name that you want to convert, then click **Convert into a Goal**.

   ![](assets/convert-to-goal-link-highlighted-350x191.png)

1. (Optional) Remove the name of the original activity or result owner from the **Goal Owner** field and replace it with another user, team, group, or your organization's name. By default, Workfront selects the owner of the result or the activity as the goal owner. 
1. Click **Convert**. The activity or result displays as an aligned goal in the Goal Details panel of the original goal and the original activity or result is removed from the original goal and transferred to the second goal. By default, the new goal has the same name as the original converted result or activity. 
1. (Optional) Click the name of the new goal to open the **Goal Details** panel and edit the name of the goal. For information about editing any information for an existing goal, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
-->

1. Gehen Sie zu einem Ziel, das über ein Ergebnis oder eine Aktivität verfügt, die Sie in ein Ziel konvertieren möchten.
1. Klicken Sie auf der Zielseite auf **Fortschrittsanzeigen** im linken Bereich.
1. Wählen Sie ein Ergebnis oder eine Aktivität in der Liste der Fortschrittsanzeigen aus und klicken Sie auf die Schaltfläche **In Ziel konvertieren** icon ![](assets/convert-to-goal-icon-unshimmed.png) oben in der Fortschrittsanzeige. Das Feld In Ziel konvertieren wird geöffnet.

   ![](assets/convert-to-goal-box-unshimmed.png)
1. Aktualisieren Sie die folgenden Informationen:
   * **Zielname**: Standardmäßig hat das neue Ziel denselben Namen wie das ursprüngliche Ergebnis oder die ursprüngliche Aktivität.
   * **Zeitraum**: Standardmäßig ist der Zeitraum des neuen Ziels das aktuelle Quartal. Sie können die **Benutzerdefinierte Datumswerte aktivieren** -Einstellung, um einen benutzerdefinierten Zeitraum für das neue Ziel zu definieren.
   * **Zieleigentümer**: Standardmäßig ist der neue Zieleigentümer der Eigentümer des ursprünglichen Ergebnisses oder der Aktivität.
   * **Beschreibung**: Fügen Sie weitere Informationen zum neuen Ziel hinzu.
1. Klicken Sie auf **Speichern**

   Das Ergebnis oder die Aktivität wird jetzt in ein untergeordnetes Ziel des ursprünglichen Ziels konvertiert. Sie wird als Ziel in der Liste der Fortschrittsindikatoren des ursprünglichen Ziels aufgeführt.



