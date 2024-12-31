---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Entfernen von Fortschrittsanzeigen aus Zielen in Adobe Workfront-Zielen
description: Sie können Ergebnisse, Aktivitäten und Projekte aus Zielen in Adobe Workfront-Zielen entfernen, wenn sie nicht mehr relevant sind.
author: Alina
feature: Workfront Goals
exl-id: 0e064dbd-6168-47b4-98ab-b5c0481e839e
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 0%

---

# Entfernen von Fortschrittsanzeigen aus Zielen in Adobe Workfront-Zielen

<!-- for goal redesign PRODUCTION RELEASE: Should this article be called "Remove or disconnect progress indicators from goals" when this is available to ALL progress indicators (including "disconnect goals")-- if yes, updte the title everywhere else where this is linked?
-->

Sie können Ergebnisse, Aktivitäten und Projekte aus Zielen entfernen, wenn sie nicht mehr relevant sind.

Informationen zum Erstellen von Zielen und Hinzufügen von Ergebnissen und Aktivitäten zu Zielen finden Sie in den folgenden Artikeln:

* [Erstellen von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/create-goals.md)
* [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
* [Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Ergebnisse und Aktivitäten in Adobe Workfront Goals bearbeiten](../../workfront-goals/results-and-activities/edit-results-and-activities.md)

Ziele können auch an übergeordneten Zielen ausgerichtet werden, sodass sie zu untergeordneten Zielen werden. Untergeordnete Ziele sind ebenfalls Fortschrittsindikatoren für die übergeordneten Ziele.

Sie können die Zielausrichtung entfernen, indem Sie die Verbindung zwischen den Zielen entfernen. Weitere Informationen finden Sie unter [Zielausrichtung in Adobe Workfront Goals entfernen](../goal-alignment/remove-goal-alignment.md).

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
 <p>Aktuelle Lizenz: Anfrage oder höher</p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe Workfront-Lizenzen</a>.</p> </td>
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
  <div>
  <p>Anzeigen von oder höheren Berechtigungen für das Ziel, um es anzuzeigen</p>
  <p>Verwalten von Berechtigungen für das Ziel, um es zu bearbeiten</p>
  <p>Informationen zum Freigeben von Zielen finden Sie <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Freigeben eines Ziels in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layoutvorlage</p></td>
   <td> <p>Allen Benutzenden, einschließlich Workfront-Administratoren, muss eine Layout-Vorlage zugewiesen werden, die den Bereich Ziele im Hauptmenü enthält. </p>  
</td>
  </tr>
</tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

Ein Ziel muss mit Ergebnissen, Aktivitäten oder Projekten verknüpft sein.

## Überlegungen zum Entfernen von Ergebnissen und Aktivitäten und zum Trennen von Projekten von Zielen

* Ergebnisse und Aktivitäten können nur aus aktiven Zielen entfernt werden.
* Sie können Ergebnisse und Aktivitäten aus einem Ziel entfernen, indem Sie sie löschen. Gelöschte Ergebnisse und Aktivitäten können nicht wiederhergestellt werden.
* Wenn Sie das Ergebnis oder die Aktivität aus einem Ziel entfernen, wirkt sich der Fortschritt des entfernten Ergebnisses oder der Aktivität auf den Gesamtfortschritt des Ziels aus.
* Sie können ein Projekt nicht aus einem Ziel löschen, es jedoch vom Ziel trennen. Wenn Sie das Projekt vom Ziel trennen, wirkt sich der Prozentsatz der Fertigstellung des Projekts nicht mehr auf den Fortschritt des Ziels aus.

  Informationen darüber, wie sich Projekte auf den Zielfortschritt auswirken, finden Sie unter [Hinzufügen von Projekten zu Zielen in Adobe Workfront Goals](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

* Sie können kein Ergebnis oder eine Aktivität aus einem Ziel entfernen und kein untergeordnetes Ziel oder Projekt trennen, wenn es sich dabei um die letzte Fortschrittsanzeige für das Ziel handelt.
* Wenn ein Projekt aus dem Bereich Projekte gelöscht wird und es die letzte Fortschrittsanzeige eines Ziels ist, wird das Ziel inaktiv.

## Ergebnisse und Aktivitäten aus Zielen löschen

Sie entfernen Ergebnisse und Aktivitäten aus einem Ziel, indem Sie sie löschen. Das Löschen von Ergebnissen und Aktivitäten aus einem Ziel ist identisch.

<!--
How you delete results and activities differs depending on the environment you use.

### Delete results and activities in the Production environment


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click **Results** to remove results or **Activities** to remove activities. 

1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result or activity name, then click **Delete** > **Yes, delete**.

   ![](assets/delete-result-goal-details-350x108.png)

   The result or activity is deleted and cannot be recovered. The percent complete of the goal updates to exclude the deleted activity or result.

-->

1. Klicken Sie oben rechts auf **Hauptmenü**-Symbol ![](assets/main-menu-icon.png) und dann auf **Ziele**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
   Dadurch wird der Bereich Workfront-Ziele geöffnet. Die Liste der Ziele wird standardmäßig angezeigt.

1. Klicken Sie auf den Namen eines Ziels, aus dem Sie Ergebnisse und Aktivitäten entfernen möchten.

   Dadurch wird die Zielseite geöffnet.

1. Klicken Sie **linken Bereich** Fortschrittsanzeigen“.

1. Wählen Sie ein Ergebnis oder eine Aktivität aus und klicken Sie dann oben in **Liste auf** Symbol „Löschen![](assets/delete-icon.png) .

1. Klicken Sie **Löschen**, um den Löschvorgang zu bestätigen. Das Ergebnis oder die Aktivität wurde gelöscht und kann nicht wiederhergestellt werden. Der Prozentsatz der Fertigstellung des Ziels wird aktualisiert, um die gelöschte Aktivität oder das gelöschte Ergebnis auszuschließen.


## Projekte aus Zielen entfernen

<!--
Dsconnecting projects from goals differs depending on the environment you use.

### Disconnect projects from goals in the Production environment


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click the **right-pointing arrow** to the left of the Activities sections to expand it. 
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the project name, then click **Disconnect**.

   ![](assets/disconnect-project-goal-details-350x94.png)

   The project is disconnected from the goal. The percent complete of the goal updates to exclude the percent complete of the disconnected project.
-->


1. Klicken Sie oben rechts auf **Hauptmenü** und dann auf **Ziele**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Dadurch wird der Bereich Workfront-Ziele geöffnet. Die Liste der Ziele wird standardmäßig angezeigt.

1. Klicken Sie auf den Namen eines Ziels, aus dem Sie Ergebnisse und Aktivitäten entfernen möchten.

   Dadurch wird die Zielseite geöffnet.
1. Klicken Sie **linken Bereich** Fortschrittsanzeigen“.
1. Wählen Sie ein Projekt aus und klicken Sie dann oben in **Liste auf** Symbol „Trennen![](assets/disconnect-icon.png) .
1. Klicken Sie **Trennen** zur Bestätigung.

   Das Projekt ist nicht mehr mit dem Ziel verbunden. Der Prozentsatz der Fertigstellung des Ziels wird aktualisiert, um das getrennte Projekt auszuschließen.

