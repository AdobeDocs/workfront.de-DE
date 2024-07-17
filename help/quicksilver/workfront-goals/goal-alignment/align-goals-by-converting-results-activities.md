---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Ziele durch Konvertieren von Ergebnissen und Aktivitäten in Ziele ausrichten
description: Sie können zwei Ziele manuell ausrichten oder die Ergebnisse und Aktivitäten eines vorhandenen Ziels in ein anderes umwandeln. Das konvertierte Ergebnis oder die konvertierte Aktivität wird zum untergeordneten Ziel des ursprünglichen Ziels. Informationen zum manuellen Ausrichten von zwei Zielen finden Sie unter Ausrichten von Zielen durch Verbinden in Adobe Workfront-Zielen.
author: Alina
feature: Workfront Goals
exl-id: 48371389-952c-4732-b519-9774cd4d1b93
source-git-commit: 330ee20ad14ea7409db1c6f627ed6aa0e0c5c014
workflow-type: tm+mt
source-wordcount: '642'
ht-degree: 16%

---

# Ziele durch Konvertieren von Ergebnissen und Aktivitäten in Ziele ausrichten

Sie können zwei Ziele manuell ausrichten oder die Ergebnisse und Aktivitäten eines vorhandenen Ziels in ein anderes umwandeln. Das konvertierte Ergebnis oder die konvertierte Aktivität wird zum untergeordneten Ziel des ursprünglichen Ziels.
Informationen zum manuellen Ausrichten von zwei Zielen finden Sie unter [Ziele durch Verbinden in Adobe Workfront-Zielen ausrichten](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

## Zugriffsanforderungen


<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">Adobe Workfront-Abo</td>
 <td>
 <p>Alle</p>

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

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

Sie müssen über Folgendes verfügen, bevor Sie beginnen können:

* Ein vorhandenes Ziel mit vorhandenen Ergebnissen und Aktivitäten.

  Weitere Informationen zum Erstellen von Zielen finden Sie unter [Ziele in Adobe Workfront erstellen](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>Ein Ziel kann über bis zu 1000 Fortschrittsanzeigen verfügen.

<!--drafted for goal redesign: At PRODUCTION: update the sentence above to remove Production/ Preview references-->

## Überlegungen beim Konvertieren von Ergebnissen und Aktivitäten in Ziele

Manchmal kann ein Ergebnis oder eine Aktivität einen größeren Umfang haben als erwartet, und es wäre sinnvoller, dass sie zu Zielen werden. Sie können die Ergebnisse und Aktivitäten eines vorhandenen Ziels in ein neues Ziel konvertieren. Dies ist ein Bottom-up-Ansatz zur Ausrichtung von Zielen.

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

1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result or activity name that you want to convert, then click **Convert into a Goal**.

   ![](assets/convert-to-goal-link-highlighted-350x191.png)

1. (Optional) Remove the name of the original activity or result owner from the **Goal Owner** field and replace it with another user, team, group, or your organization's name. By default, Workfront selects the owner of the result or the activity as the goal owner. 
1. Click **Convert**. The activity or result displays as an aligned goal in the Goal Details panel of the original goal and the original activity or result is removed from the original goal and transferred to the second goal. By default, the new goal has the same name as the original converted result or activity. 
1. (Optional) Click the name of the new goal to open the **Goal Details** panel and edit the name of the goal. For information about editing any information for an existing goal, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
-->

1. Gehen Sie zu einem Ziel, das über ein Ergebnis oder eine Aktivität verfügt, die Sie in ein Ziel konvertieren möchten.
1. Klicken Sie auf der Zielseite im linken Bereich auf **Fortschrittsanzeigen** .
1. Wählen Sie ein Ergebnis oder eine Aktivität in der Liste der Fortschrittsanzeigen aus und klicken Sie dann oben in der Fortschrittsanzeige-Liste auf das Symbol **In Ziel konvertieren** ![](assets/convert-to-goal-icon-unshimmed.png). Das Feld In Ziel konvertieren wird geöffnet.

   ![](assets/convert-to-goal-box-unshimmed.png)
1. Aktualisieren Sie die folgenden Informationen:
   * **Zielname**: Standardmäßig hat das neue Ziel denselben Namen wie das ursprüngliche Ergebnis oder die ursprüngliche Aktivität.
   * **Zeitraum**: Standardmäßig ist der Zeitraum des neuen Ziels der aktuelle Quartal. Sie können die Einstellung **Benutzerdefinierte Datumswerte aktivieren** auswählen, um einen benutzerdefinierten Zeitraum für das neue Ziel festzulegen.
   * **Zieleigentümer**: Standardmäßig ist der neue Zieleigentümer der Eigentümer des ursprünglichen Ergebnisses oder der Aktivität.
   * **Beschreibung**: Fügen Sie weitere Informationen zum neuen Ziel hinzu.
1. Klicken Sie auf **Speichern**

   Das Ergebnis oder die Aktivität wird jetzt in ein untergeordnetes Ziel des ursprünglichen Ziels konvertiert. Sie wird als Ziel in der Liste der Fortschrittsindikatoren des ursprünglichen Ziels aufgeführt.



