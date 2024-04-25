---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Löschen und Deaktivieren von Zielen in Adobe Workfront-Zielen
description: Wenn Sie mit der Arbeit an einem Ziel beginnen und es in Ihrer Organisation irrelevant wird, empfehlen wir, es zu deaktivieren, anstatt es zu löschen. Durch das Deaktivieren eines Ziels werden seine historischen Informationen beibehalten und Sie können es zu einem späteren Zeitpunkt reaktivieren. Es kann jedoch manchmal sinnvoll sein, ein Ziel zu löschen, um die Zielliste genau zu halten.
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: 09e34ecdfeec531ebbaaba4fb8682496c53d86bf
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 0%

---

# Löschen und Deaktivieren von Zielen in Adobe Workfront-Zielen

Wenn Sie mit der Arbeit an einem Ziel beginnen und es in Ihrer Organisation irrelevant wird, empfehlen wir, es zu deaktivieren, anstatt es zu löschen. Durch das Deaktivieren eines Ziels werden seine historischen Informationen beibehalten und Sie können es zu einem späteren Zeitpunkt reaktivieren. Es kann jedoch manchmal sinnvoll sein, ein Ziel zu löschen, um die Zielliste genau zu halten.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

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
 <td role="rowheader"><p>Zugriffsebene</p></td>
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

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Deaktivieren von Zielen

Sie können ein Ziel deaktivieren, das nicht mehr relevant ist und in Zukunft möglicherweise reaktiviert werden soll.

* [Überlegungen zum Deaktivieren von Zielen](#considerations-when-deactivating-goals)
* [Deaktivieren von Zielen](#deactivate-goals)

### Überlegungen zum Deaktivieren von Zielen

Beachten Sie beim Deaktivieren von Zielen Folgendes:

* Sie können Ziele nur im Status Aktiv deaktivieren. Informationen zum Aktivieren eines Ziels finden Sie unter [Ziele in Adobe Workfront aktivieren](../../workfront-goals/goal-management/activate-goals.md).

  >[!TIP]
  >
  >Ziele können im Status Entwurf nicht deaktiviert werden.

* Workfront unterbricht die Berechnung des Fortschritts deaktivierter Ziele.
* Inaktive Ziele werden im Abschnitt &quot;Diagramme&quot;von Workfront-Zielen nicht mehr angezeigt oder werden nicht mehr berücksichtigt. Weitere Informationen zu Workfront-Zieldiagrammen finden Sie unter [Überprüfen Sie Diagramme, um die Trends beim Zielfortschritt in Adobe Workfront-Zielen zu verstehen.](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goal-graphs.md).

  <!--* The Check-in section. For information about the Check-in page, see [Update goal progress in Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md). -->

* Sie können keine Aktualisierungen zu deaktivierten Zielen mehr vornehmen.
* Sie können Informationen zum Ziel und seiner Ausrichtung bearbeiten.
* Sie können ein zuvor deaktiviertes Ziel reaktivieren.

### Deaktivieren von Zielen

<!--
Deactivating goals differs depending on which environment you use.

### Deactivate goals in the Production environment


1. Go to the goal that you want to deactivate.

   For example, go to the Goal List and click the name of a goal.

   The Goal Details panel opens on the right.

   >[!TIP]
   >
   >You can open goals from any sections of Workfront Goals.

1. Click the **More icon** ![](assets/more-icon.png), then click **Deactivate**.

   ![](assets/deactivate-goal-highlighted.png)

   The goal status changes to Inactive. 

1. Click the **X** icon in the upper-right to close Goal Details.
-->

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts auf **Ziele**.

   Die Zielliste wird angezeigt.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Optional) Ändern Sie Ihre Filter so, dass nur aktive Ziele angezeigt werden.

   Informationen zum Filtern von Informationen in Workfront-Zielen finden Sie unter [Informationen in Adobe Workfront-Zielen filtern](../goal-management/filter-information-wf-goals.md).

1. Klicken Sie auf ein aktives Ziel.

   Die Zielseite wird geöffnet.

   ![](assets/goal-page-unshimmed.png)

1. Klicken Sie auf **Mehr** Menü ![](assets/more-icon.png) rechts neben dem Zielnamen, klicken Sie auf **Deaktivieren**.

1. Das Ziel wird deaktiviert und sein Status wird inaktiv.

## Löschen von Zielen

Sie können Ziele löschen, die nicht mehr oder möglicherweise nie relevant sind.

* [Überlegungen zum Löschen von Zielen](#considerations-when-deleting-goals)
* [Löschen von Zielen](#delete-goals)

### Überlegungen zum Löschen von Zielen {#considerations-when-deleting-goals}

* Sie können Ziele in jedem Status löschen, einschließlich geschlossener Ziele.
* Gelöschte Ziele können nicht wiederhergestellt werden.
* Die mit dem Ziel verknüpften Aktivitäten &quot;Ergebnisse&quot;und &quot;Manueller Fortschritt&quot;werden ebenfalls gelöscht.
* Projekte, die mit Zielen verknüpft sind, werden nicht gelöscht, aber ihre Verknüpfung mit dem Ziel wird entfernt.

### Löschen von Zielen

<!--
Deleting  goals differs depending on which environment you use.

#### Delete goals in the Production environment

1. Go to the goal that you want to delete.

   For example, go to the Goal List and click a goal.

   The Goal Details panel opens on the right. 

1. Click the **More icon** ![](assets/more-icon.png), then click **Delete**.

   ![](assets/delete-goal-highlighted.png)

1. Click **Yes, delete**.

   The goal is removed from the Goal List and cannot be recovered.
-->

1. Klicken Sie auf das Symbol Hauptmenü . ![](assets/main-menu-icon.png) Klicken Sie oben rechts auf **Ziele**.

   Die Zielliste wird angezeigt.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. Klicken Sie auf den Namen eines Ziels. Dadurch wird die Zielseite geöffnet.
1. Klicken Sie auf **Mehr** Menü ![](assets/more-icon.png) rechts neben dem Zielnamen, klicken Sie auf **Löschziel**, dann **Löschen**.

   Das Ziel sowie seine Aktivitäten und Ergebnisse werden ebenfalls gelöscht und können nicht wiederhergestellt werden. Projekte, die mit dem Ziel oder den untergeordneten Zielen verknüpft waren, werden nicht gelöscht.


