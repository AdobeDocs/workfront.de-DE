---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Ziele durch Verbinden in Adobe Workfront-Zielen ausrichten
description: Wenn Sie ein einzelner Mitarbeiter sind, der ein persönliches Ziel verfolgt, können Sie es an die Ziele Ihres Teams anpassen, um den Fortschritt Ihres eigenen Ziels im größeren Kontext der Strategie Ihres Unternehmens effektiv darzustellen.
author: Alina
feature: Workfront Goals
exl-id: 4276f1c9-2ee9-4f74-b011-ae1e19fefe35
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# Ziele durch Verbinden in Adobe Workfront-Zielen ausrichten


Wenn Sie ein einzelner Mitarbeiter sind, der ein persönliches Ziel verfolgt, können Sie es an die Ziele Ihres Teams anpassen, um den Fortschritt Ihres eigenen Ziels im größeren Kontext der Strategie Ihres Unternehmens effektiv darzustellen.

Wenn alle Mitarbeiter in Ihrer Organisation ihre Ziele an die Ziele Ihrer Organisation anpassen, können sie deutlich erkennen, wie ihre individuellen Beiträge und Teambemühungen dazu beitragen, die Umsetzung größerer Prioritäten auf Unternehmensebene voranzutreiben. Weitere Informationen zu Best Practices für die Ausrichtung von Zielen finden Sie unter [Übersicht über die Zielausrichtung in Adobe Workfront-Zielen](../../workfront-goals/goal-alignment/goal-alignment-overview.md).

Es gibt zwei Ansätze zum Verbinden von Zielen in Adobe Workfront-Zielen:

* Sie können eine Ausrichtung zwischen Zielen erstellen, indem Sie Ziele miteinander verbinden.

* Sie können zwei Ziele manuell ausrichten oder die Ergebnisse und Aktivitäten eines vorhandenen Ziels in ein anderes Ziel konvertieren. Das konvertierte Ergebnis oder die konvertierte Aktivität wird zum untergeordneten Ziel des ursprünglichen Ziels.

>[!IMPORTANT]
>
>Ein Ziel kann über insgesamt 1000 Fortschrittsanzeigen verfügen.

In diesem Artikel wird beschrieben, wie Sie Ziele ausrichten können, indem Sie sie miteinander verbinden. Informationen zur Ausrichtung von Zielen durch Konvertieren von Ergebnissen und Aktivitäten in Ziele finden Sie unter [Ziele durch Konvertieren von Ergebnissen und Aktivitäten in Ziele ausrichten](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

## Zugriffsanforderungen

<!--drfated for the P&P release: 

You must have the following:

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
   <td> <p>Zugriff auf Ziele bearbeiten</p> <p><b>NOTIZ</b>

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

## Ziele ausrichten, indem sie miteinander verbunden werden

<!--
Aligning goals by connecting them differs depending on what environment you use. 

### Align goals by connecting them in the Production environment

1. Create two goals that you want to align. For information about creating goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).
1. (Optional) Activate the goals that you want to align. You can align goals that have a Draft, Active, or Inactive status. For information about activating goals, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).
1. Go to the goal that you want to align (child goal) to another goal (parent goal) and click its name to open the **Goal Details** panel.

   For example, if you want Goal 2 to influence the progress of Goal 1, you must go to Goal 2. 

1. Click **Align to another goal** in the upper-right corner of the right panel.

   ![](assets/align-to-another-goal-link-highlighted-350x128.png)

1. Start typing the name of an existing goal or the name of an owner in the **Align to another goal** field, then select it when it appears in the list. Only goals that are from the same or future periods display in the list. 
1. Click **Save**.

   The goal you started with (Goal 2) is now the child goal of the goal you aligned it with (Goal 1).   
   The aligned goals display connected in the Goal Alignment section with Goal 2 as secondary to Goal 1.

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Optional) To view the goals in the Goal Alignment section, do one of the following:

   * Click the Goal Alignment section in the left panel and find the goals by applying the correct filter. For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).
   * Click the Goal List, Check-in, or Pulse sections in the left panel and find one of the goals, then click the **Alignment icon** ![](assets/align-icon.png) next to the goal name to go directly to the goal in the Goal Alignment section.

   For information about the Goal Alignment section, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md). 

1. (Optional) Add activities and results to either goal to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Optional) Remove the alignment between two goals, when you consider that no longer is relevant to your organization's overall strategy For information about removing alignment between goals, see [Remove goal alignment in Adobe Workfront Goals](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

-->
1. Erstellen Sie zwei Ziele, die Sie ausrichten möchten. Informationen zum Erstellen von Zielen finden Sie unter [Erstellen von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/create-goals.md).
1. (Optional) Aktivieren Sie die Ziele, die Sie ausrichten möchten. Sie können Ziele mit dem Status Entwurf, Aktiv oder Inaktiv ausrichten. Informationen zum Aktivieren von Zielen finden Sie unter [Aktivieren von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/activate-goals.md).
1. Wechseln Sie zum Ziel, das Sie ausrichten möchten (untergeordnetes Ziel), zu einem anderen Ziel (übergeordnetes Ziel) und klicken Sie auf dessen Namen, um die Zielseite zu öffnen.

   >[!INFO]
   >
   >Wenn Sie beispielsweise Ziel 2 auf den Fortschritt von Ziel 1 auswirken möchten, müssen Sie zu Ziel 2 gehen.

1. Klicken **Zieldetails** im linken Bereich.

1. Im **Übergeordnete Zielinformationen** Bereich, klicken Sie **Hinzufügen** im **Übergeordnetes Ziel** Feld, wenn kein übergeordnetes Ziel vorhanden ist,

   Oder

   Klicken Sie auf den Namen des übergeordneten Ziels, um ein anderes auszuwählen.

1. Beginnen Sie mit der Eingabe des Namens eines vorhandenen Ziels im **Übergeordnetes Ziel** und wählen Sie es aus, wenn es in der Liste angezeigt wird. In der Liste werden nur Ziele angezeigt, die aus denselben oder künftigen Zeiträumen stammen.

1. Klicken **Änderungen speichern**.

   Das Ziel, mit dem Sie begonnen haben (Ziel 2), ist jetzt das untergeordnete Ziel des übergeordneten Ziels, mit dem Sie es ausgerichtet haben (Ziel 1).\
   Die ausgerichteten Ziele werden im Abschnitt Zielausrichtung mit Ziel 2 als sekundär zu Ziel 1 angezeigt.
Das untergeordnete Ziel wird im Abschnitt Fortschrittsindikatoren des übergeordneten Ziels angezeigt, wenn der Fortschritt den Fortschritt des übergeordneten Ziels aktualisiert.

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Optional) Um die Ziele im Abschnitt &quot;Zielausrichtung&quot;anzuzeigen, gehen Sie zum Bereich &quot;Ziele&quot;von Workfront und klicken Sie dann auf das **Zielausrichtung** im linken Bereich. Weitere Informationen zur Zielausrichtung finden Sie unter [Navigieren Sie im Abschnitt Zielausrichtung in Adobe Workfront-Zielen.](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).

1. (Optional) Fügen Sie Aktivitäten und Ergebnisse zu beiden Zielen hinzu, um deren Fortschritt anzuzeigen. Weitere Informationen zum Hinzufügen von Aktivitäten und Ergebnissen finden Sie in den folgenden Artikeln:

   * [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
   * [Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Optional) Entfernen Sie die Ausrichtung zwischen zwei Zielen, wenn Sie der Ansicht sind, dass dies nicht mehr für die Gesamtstrategie Ihres Unternehmens relevant ist. Informationen zum Entfernen der Ausrichtung zwischen Zielen finden Sie unter [Entfernen der Zielausrichtung in Adobe Workfront-Zielen](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

