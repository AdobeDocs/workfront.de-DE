---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Entfernen von Fortschrittsindikatoren aus Zielen in Adobe Workfront-Zielen
description: Sie können Ergebnisse, Aktivitäten und Projekte aus Zielen in Adobe Workfront-Zielen entfernen, wenn sie nicht mehr relevant sind.
author: Alina
feature: Workfront Goals
exl-id: 0e064dbd-6168-47b4-98ab-b5c0481e839e
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---

# Entfernen von Fortschrittsindikatoren aus Zielen in Adobe Workfront-Zielen

<!-- for goal redesign PRODUCTION RELEASE: Should this article be called "Remove or disconnect progress indicators from goals" when this is available to ALL progress indicators (including "disconnect goals")-- if yes, updte the title everywhere else where this is linked?
-->

Sie können Ergebnisse, Aktivitäten und Projekte aus Zielen entfernen, wenn sie nicht mehr relevant sind.

Informationen zum Erstellen von Zielen sowie zum Hinzufügen von Ergebnissen und Aktivitäten zu diesen finden Sie in den folgenden Artikeln:

* [Erstellen von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/create-goals.md)
* [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
* [Ergebnisse zu Zielen in Adobe Workfront-Zielen hinzufügen](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Ergebnisse und Aktivitäten in Adobe Workfront-Zielen bearbeiten](../../workfront-goals/results-and-activities/edit-results-and-activities.md)

Ziele können auch auf übergeordnete Ziele ausgerichtet werden, sodass sie zu Kinderzielen werden. Kinderziele sind auch Fortschrittsindikatoren der übergeordneten Ziele.

Sie können die Ausrichtung zwischen Zielen entfernen, indem Sie die Verbindung zwischen ihnen entfernen. Weitere Informationen finden Sie unter [Entfernen der Zielausrichtung in Adobe Workfront-Zielen](../goal-alignment/remove-goal-alignment.md).

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
   <p>Für den neuen Plan und die Lizenzstruktur:
  <ul><li>Ein ultimativer Plan </li>
  Oder
  <li>Eine zusätzliche Lizenz für Adobe Workfront Goals für die Prime- oder Select Adobe Workfront-Pläne. </li></ul> </p>
<p>Für den aktuellen Plan und die Lizenzstruktur: 
<ul><li> A Pro oder höher </li>
  <li>Eine Adobe Workfront Goals-Lizenz zusätzlich zu einer Workfront-Lizenz.</li></ul></p>
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

Sie müssen ein Ziel mit Ergebnissen, Aktivitäten oder Projekten verknüpfen.

## Überlegungen zum Entfernen von Ergebnissen, Aktivitäten und Trennen von Projekten von Zielen

* Sie können Ergebnisse und Aktivitäten nur aus aktiven Zielen entfernen.
* Sie können Ergebnisse und Aktivitäten aus einem Ziel entfernen, indem Sie sie löschen. Gelöschte Ergebnisse und Aktivitäten können nicht wiederhergestellt werden.
* Wenn Sie das Ergebnis oder die Aktivität aus einem Ziel entfernen, wirkt sich der Fortschritt des entfernten Ergebnisses oder der Aktivität auf den Gesamtfortschritt des Ziels aus.
* Ein Projekt kann nicht aus einem Ziel gelöscht werden, es kann jedoch vom Ziel getrennt werden. Wenn Sie das Projekt vom Ziel trennen, wirkt sich der Prozentsatz des Projektabschlusses nicht mehr auf den Fortschritt des Ziels aus.

  Informationen dazu, wie Projekte den Zielfortschritt beeinflussen, finden Sie unter [Projekte zu Zielen in Adobe Workfront hinzufügen](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

* Sie können ein Ergebnis oder eine Aktivität nicht aus einem Ziel entfernen und die Verbindung zu einem untergeordneten Ziel bzw. Projekt nicht trennen, wenn es sich um die letzte Fortschrittsanzeige für das Ziel handelt.
* Wenn ein Projekt aus dem Bereich &quot;Projekte&quot;gelöscht wird und es der letzte Fortschrittsindikator eines Ziels ist, wird das Ziel inaktiv.

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

1. Klicken Sie oben rechts auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png) und dann auf **Ziele**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
   Dadurch wird der Workfront-Zielbereich geöffnet und die Zielliste wird standardmäßig angezeigt.

1. Klicken Sie auf den Namen eines Ziels, aus dem Sie Ergebnisse und Aktivitäten entfernen möchten.

   Dadurch wird die Zielseite geöffnet.

1. Klicken Sie im linken Bereich auf **Fortschrittsanzeigen** .

1. Wählen Sie ein Ergebnis oder eine Aktivität aus und klicken Sie dann oben in der Liste auf das Symbol **Löschen** ![](assets/delete-icon.png) .

1. Klicken Sie auf **Löschen** , um den Löschvorgang zu bestätigen. Das Ergebnis oder die Aktivität wird gelöscht und kann nicht wiederhergestellt werden. Der prozentuale Abschluss des Ziels wird aktualisiert, um die gelöschte Aktivität oder das gelöschte Ergebnis auszuschließen.


## Entfernen von Projekten aus Zielen

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


1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts und dann auf **Ziele**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Dadurch wird der Workfront-Zielbereich geöffnet und die Zielliste wird standardmäßig angezeigt.

1. Klicken Sie auf den Namen eines Ziels, aus dem Sie Ergebnisse und Aktivitäten entfernen möchten.

   Dadurch wird die Zielseite geöffnet.
1. Klicken Sie im linken Bereich auf **Fortschrittsanzeigen** .
1. Wählen Sie ein Projekt aus und klicken Sie dann oben in der Liste auf das Symbol **Trennen** ![](assets/disconnect-icon.png) .
1. Klicken Sie zur Bestätigung auf **Trennen** .

   Das Projekt ist nicht mehr mit dem Ziel verbunden. Der prozentuale Abschluss des Ziels wird aktualisiert, um das nicht verbundene Projekt auszuschließen.

