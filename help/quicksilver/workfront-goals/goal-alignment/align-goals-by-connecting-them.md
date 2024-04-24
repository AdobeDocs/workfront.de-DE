---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Ziele durch Verbinden in Adobe Workfront-Zielen ausrichten
description: Wenn Sie ein einzelner Mitarbeiter sind, der ein persönliches Ziel verfolgt, können Sie es an die Ziele Ihres Teams anpassen, um den Fortschritt Ihres eigenen Ziels im größeren Kontext der Strategie Ihres Unternehmens effektiv darzustellen.
author: Alina
feature: Workfront Goals
exl-id: 4276f1c9-2ee9-4f74-b011-ae1e19fefe35
source-git-commit: 2f8a5b2d2183090029966a13c7af37f20eb44fd0
workflow-type: tm+mt
source-wordcount: '775'
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
   <p>Aktuelle Lizenz: Mitarbeiter oder höher</p>
   Oder
   <p>Ältere Lizenz: Anfrage oder höher</p> </td>
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
  <tr>
   <td role="rowheader">Objektberechtigungen</td>
   <td>
    
     <p>Anzeigen oder Anzeigen höherer Berechtigungen zum Ziel</p>
     <p>Berechtigungen für das Ziel verwalten</p>
     <p>Informationen zum Freigeben von Zielen finden Sie unter <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Freigeben eines Ziels in Workfront-Zielen</a>. </p>
     </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Ziele im Hauptmenü enthält. </p>  
</td>
  </tr>
 </tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
1. Erstellen Sie zwei Ziele, die Sie ausrichten möchten. Informationen zum Erstellen von Zielen finden Sie unter [Ziele in Adobe Workfront erstellen](../../workfront-goals/goal-management/create-goals.md).
1. (Optional) Aktivieren Sie die Ziele, die Sie ausrichten möchten. Sie können Ziele mit dem Status Entwurf, Aktiv oder Inaktiv ausrichten. Informationen zum Aktivieren von Zielen finden Sie unter [Ziele in Adobe Workfront aktivieren](../../workfront-goals/goal-management/activate-goals.md).
1. Wechseln Sie zum Ziel, das Sie ausrichten möchten (untergeordnetes Ziel), zu einem anderen Ziel (übergeordnetes Ziel) und klicken Sie auf dessen Namen, um die Zielseite zu öffnen.

   >[!INFO]
   >
   >Wenn Sie beispielsweise Ziel 2 auf den Fortschritt von Ziel 1 auswirken möchten, müssen Sie zu Ziel 2 gehen.

1. Klicks **Zieldetails** im linken Bereich.

1. Im **Übergeordnete Zielinformationen** Bereich, klicken Sie **Hinzufügen** im **Übergeordnetes Ziel** Feld, wenn kein übergeordnetes Ziel vorhanden ist,

   Oder

   Klicken Sie auf den Namen des übergeordneten Ziels, um ein anderes auszuwählen.

1. Beginnen Sie mit der Eingabe des Namens eines vorhandenen Ziels im **Übergeordnetes Ziel** und wählen Sie es aus, wenn es in der Liste angezeigt wird. In der Liste werden nur Ziele angezeigt, die aus denselben oder künftigen Zeiträumen stammen.

1. Klicken Sie auf **Änderungen speichern**.

   Das Ziel, mit dem Sie begonnen haben (Ziel 2), ist jetzt das untergeordnete Ziel des übergeordneten Ziels, mit dem Sie es ausgerichtet haben (Ziel 1).\
   Die ausgerichteten Ziele werden im Abschnitt Zielausrichtung mit Ziel 2 als sekundär zu Ziel 1 angezeigt.
Das untergeordnete Ziel wird im Abschnitt Fortschrittsindikatoren des übergeordneten Ziels angezeigt, wenn der Fortschritt den Fortschritt des übergeordneten Ziels aktualisiert.

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Optional) Um die Ziele im Abschnitt &quot;Zielausrichtung&quot;anzuzeigen, gehen Sie zum Bereich &quot;Ziele&quot;von Workfront und klicken Sie dann auf das **Zielausrichtung** im linken Bereich. Weitere Informationen zur Zielausrichtung finden Sie unter [Navigieren Sie im Abschnitt Zielausrichtung in Adobe Workfront-Zielen.](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).

1. (Optional) Fügen Sie Aktivitäten und Ergebnisse zu beiden Zielen hinzu, um deren Fortschritt anzuzeigen. Weitere Informationen zum Hinzufügen von Aktivitäten und Ergebnissen finden Sie in den folgenden Artikeln:

   * [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
   * [Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Optional) Entfernen Sie die Ausrichtung zwischen zwei Zielen, wenn Sie der Ansicht sind, dass dies nicht mehr für die Gesamtstrategie Ihres Unternehmens relevant ist. Informationen zum Entfernen der Ausrichtung zwischen Zielen finden Sie unter [Entfernen der Zielausrichtung in Adobe Workfront-Zielen](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

