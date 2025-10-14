---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Ausrichten von Zielen durch Verbinden in Adobe Workfront-Zielen
description: Wenn Sie als Mitarbeiter ein persönliches Ziel haben, sollten Sie es an den Zielen Ihres Teams ausrichten, um den Fortschritt Ihres eigenen Ziels effektiv im größeren Kontext der Strategie Ihres Unternehmens darzustellen.
author: Alina
feature: Workfront Goals
exl-id: 4276f1c9-2ee9-4f74-b011-ae1e19fefe35
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 1%

---

# Ausrichten von Zielen durch Verbinden in Adobe Workfront-Zielen

<!--Audited P&P only: 04/2025-->

Wenn Sie als Mitarbeiter ein persönliches Ziel haben, sollten Sie es an den Zielen Ihres Teams ausrichten, um den Fortschritt Ihres eigenen Ziels effektiv im größeren Kontext der Strategie Ihres Unternehmens darzustellen.

Wenn alle Mitarbeiter in Ihrem Unternehmen ihre Ziele an den Zielen Ihres Unternehmens ausrichten, können sie klar erkennen, wie ihre individuellen Beiträge und Teamaktivitäten dazu beitragen, die Nadeln bei größeren Prioritäten auf Unternehmensebene nach vorne zu bringen. Weitere Informationen zu Best Practices für die Ausrichtung von Zielen finden Sie unter [Zielausrichtung - Übersicht in Adobe Workfront Goals](../../workfront-goals/goal-alignment/goal-alignment-overview.md).

Es gibt zwei Ansätze zum Verbinden von Zielen in Adobe Workfront:

* Sie können eine Ausrichtung zwischen Zielen erstellen, indem Sie Ziele miteinander verbinden.

* Sie können zwei Ziele manuell ausrichten oder die Ergebnisse und Aktivitäten eines vorhandenen Ziels in ein anderes Ziel konvertieren. Das konvertierte Ergebnis oder die konvertierte Aktivität wird zum untergeordneten Ziel des ursprünglichen Ziels.

>[!IMPORTANT]
>
>Ein Ziel kann insgesamt 1000 Fortschrittsindikatoren aufweisen.

In diesem Artikel wird beschrieben, wie Sie Ziele ausrichten können, indem Sie sie miteinander verbinden. Informationen zum Ausrichten von Zielen durch Konvertieren von Ergebnissen und Aktivitäten in Ziele finden Sie unter &quot;[&#x200B; durch Konvertieren von Ergebnissen und Aktivitäten in Ziele ausrichten](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
 <p>Aktuelle Lizenz: Anfrage oder höher</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produkt*</td>
 <td>
  <p> Neue Produktanforderung: Workfront</p>
  Oder
  <p>Aktuelle Produktanforderung: Zusätzlich zu einer Workfront-Lizenz müssen Sie eine Lizenz für Adobe Workfront Goals erwerben. </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Voraussetzungen für die Verwendung von Workfront-Zielen</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Zugriffsebene</td>
 <td> <p>Zugriff auf Ziele bearbeiten</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Objektberechtigungen</td>
 <td>

<p>Anzeigen von oder höheren Berechtigungen für das Ziel, um es anzuzeigen</p>
  <p>Verwalten von Berechtigungen für das Ziel, um es zu bearbeiten</p>
  <p>Informationen zum Freigeben von Zielen finden Sie <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Freigeben eines Ziels in Workfront Goals</a>. </p>
   </td>
 </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzenden, einschließlich Workfront-Administratoren, muss eine Layout-Vorlage zugewiesen werden, die den Bereich Ziele im Hauptmenü enthält. </p>  
</td>
  </tr>
</tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ziele ausrichten, indem sie miteinander verbunden werden

<!--
Aligning goals by connecting them differs depending on what environment you use. 

### Align goals by connecting them in the Production environment

1. Create two goals that you want to align. For information about creating goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).
1. (Optional) Activate the goals that you want to align. You can align goals that have a Draft, Active, or Inactive status. For information about activating goals, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).
1. Go to the goal that you want to align (child goal) to another goal (parent goal) and click its name to open the **Goal Details** panel.

   For example, if you want Goal 2 to influence the progress of Goal 1, you must go to Goal 2. 

1. Click **Align to another goal** in the upper-right corner of the right panel.

   ![Align to another goal](assets/align-to-another-goal-link-highlighted-350x128.png)

1. Start typing the name of an existing goal or the name of an owner in the **Align to another goal** field, then select it when it appears in the list. Only goals that are from the same or future periods display in the list. 
1. Click **Save**.

   The goal you started with (Goal 2) is now the child goal of the goal you aligned it with (Goal 1).   
   The aligned goals display connected in the Goal Alignment section with Goal 2 as secondary to Goal 1.

   ![Aligned cards](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Optional) To view the goals in the Goal Alignment section, do one of the following:

   * Click the Goal Alignment section in the left panel and find the goals by applying the correct filter. For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).
   * Click the Goal List, Check-in, or Pulse sections in the left panel and find one of the goals, then click the **Alignment icon** ![Align icon](assets/align-icon.png) next to the goal name to go directly to the goal in the Goal Alignment section.

   For information about the Goal Alignment section, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md). 

1. (Optional) Add activities and results to either goal to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Optional) Remove the alignment between two goals, when you consider that no longer is relevant to your organization's overall strategy For information about removing alignment between goals, see [Remove goal alignment in Adobe Workfront Goals](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

-->
1. Erstellen Sie zwei Ziele, die Sie ausrichten möchten. Informationen zum Erstellen von Zielen finden Sie unter [Erstellen von Zielen in Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).
1. (Optional) Aktivieren Sie die Ziele, die Sie ausrichten möchten. Sie können Ziele mit dem Status Entwurf, Aktiv oder Inaktiv ausrichten. Informationen zum Aktivieren von Zielen finden Sie unter [Aktivieren von Zielen in Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).
1. Wechseln Sie zu dem Ziel, das Sie (untergeordnetes Ziel) an einem anderen Ziel (übergeordnetes Ziel) ausrichten möchten, und klicken Sie auf den Namen, um die Zielseite zu öffnen.

   >[!INFO]
   >
   >Wenn Sie beispielsweise möchten, dass Ziel 2 den Fortschritt von Ziel 1 beeinflusst, müssen Sie zu Ziel 2 wechseln.

1. Klicken Sie **linken** auf „Zieldetails“.

1. Klicken Sie im Bereich **Informationen zum übergeordneten Ziel** im Feld **Übergeordnetes Ziel** auf **Hinzufügen**, wenn kein übergeordnetes Ziel vorhanden ist,

   Oder

   Klicken Sie auf den Namen des übergeordneten Ziels, um ein anderes Ziel auszuwählen.

1. Geben Sie den Namen eines vorhandenen Ziels in das Feld **Übergeordnetes Ziel** ein und wählen Sie es aus, wenn es in der Liste angezeigt wird. In der Liste werden nur Ziele angezeigt, die aus derselben oder künftigen Perioden stammen.

1. Klicken Sie auf **Änderungen speichern**.

   Das Ziel, mit dem Sie begonnen haben (Ziel 2), ist jetzt das untergeordnete Ziel des übergeordneten Ziels, mit dem Sie es abgestimmt haben (Ziel 1).\
   Die abgestimmten Ziele werden im Abschnitt „Zielausrichtung“ mit Ziel 2 als sekundärer Ziel 1 verbunden angezeigt.
Das untergeordnete Ziel wird im Abschnitt Fortschrittsanzeigen des übergeordneten Ziels angezeigt, da sein Fortschritt den Fortschritt des übergeordneten Ziels aktualisiert.

   ![Abgestimmte Karten](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Optional) Um die Ziele im Abschnitt „Zielausrichtung“ anzuzeigen, gehen Sie zum Bereich „Ziele“ von Workfront und klicken Sie dann **Abschnitt &quot;**&quot; im linken Bedienfeld. Informationen zum Abschnitt „Zielausrichtung“ finden Sie unter [Navigieren im Abschnitt „Zielausrichtung“ in Adobe Workfront-](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).

1. (Optional) Fügen Sie Aktivitäten und Ergebnisse zu einem der Ziele hinzu, um deren Fortschritt anzuzeigen. Informationen zum Hinzufügen von Aktivitäten und Ergebnissen finden Sie in den folgenden Artikeln:

   * [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
   * [Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Optional) Entfernen Sie die Ausrichtung zwischen zwei Zielen, wenn Sie der Ansicht sind, dass dies für die Gesamtstrategie Ihres Unternehmens nicht mehr relevant ist. Informationen zum Entfernen der Zielausrichtung finden Sie unter [Zielausrichtung in Adobe Workfront-Zielen entfernen](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

