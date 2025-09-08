---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Zuweisen von Arbeit im Workload Balancer durch Ziehen und Ablegen
description: Sie können Arbeitselemente mit dem Adobe Workfront Workload Balancer zuweisen, indem Sie Arbeitselemente per Drag-and-Drop an die richtigen Benutzenden ziehen.
author: Lisa
feature: Resource Management
exl-id: caffcde8-3953-44a4-b945-76f2de84f4c6
source-git-commit: bf1a8e4384360554c6245b455650f30976e82ce1
workflow-type: tm+mt
source-wordcount: '991'
ht-degree: 0%

---

# Zuweisen von Arbeit im Workload Balancer durch Ziehen und Ablegen

{{preview-fast-release-general}}

Sie können Arbeitselemente mit dem Adobe Workfront Workload Balancer zuweisen, indem Sie Arbeitselemente per Drag-and-Drop an die richtigen Benutzenden ziehen.

Allgemeine Informationen zum Zuweisen von Arbeit zu Benutzern mithilfe des Workload Balancer finden Sie unter [Übersicht über die Zuweisung von Arbeit im Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>oder</p>
       <p>Aktuell: Plan, um Arbeit im Workload Balancer im Bereich Ressourcen zuzuweisen;</br>
       Arbeit, um Arbeit im Workload Balancer eines Teams oder Projekts zuzuweisen</p></td>
  </tr>
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Folgendes bearbeiten:</p> 
    <ul> 
     <li>Ressourcenverwaltung</li> 
     <li>Projekte</li> 
     <li>Aufgaben</li> 
     <li>Probleme</li> 
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Tragen Sie Berechtigungen oder höher zu den Projekten, Aufgaben und Problemen bei, die „Zuweisungen vornehmen“ enthalten</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Element durch Ziehen und Ablegen zuweisen

Sie können einem Benutzer ein Element aus dem Bereich Nicht zugewiesene Arbeit zuweisen oder ein bereits zugewiesenes Element einem anderen Benutzer im Bereich Zugewiesene Arbeit neu zuweisen.

1. Wechseln Sie zum Workload Balancer, dem Sie Arbeit zuweisen möchten.

   Sie können Benutzern mithilfe des Workload Balancer im Bereich Ressource, auf Projekt- oder auf Teamebene Arbeit zuweisen. Weitere Informationen dazu, wo sich der Workload-Balancer in Workfront befindet, finden Sie unter [Suchen des Workload-Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Optional) Wechseln Sie zum Bereich **Nicht zugewiesene Arbeit** und wenden Sie einen Filter an, um Aufgaben, Probleme <span class="preview">und Rollenzuweisungen</span> anzuzeigen, die Benutzern nicht zugewiesen sind

   Oder

   Wechseln Sie zum Bereich **Zugewiesene Arbeit** und erweitern Sie den Namen eines Benutzers, um die ihm zugewiesenen Arbeitselemente anzuzeigen, wenn Sie seine Elemente neu zuweisen möchten.

   >[!NOTE]
   >
   ><span class="preview">Funktionszuweisungen werden unter Arbeitselementen im Bereich Nicht zugeordnete Arbeit angezeigt, wenn die Einstellung „Funktionszuweisungen anzeigen“ aktiviert ist. Weitere Informationen finden Sie unter [Anpassen der Ansicht](/help/quicksilver/resource-mgmt/workload-balancer/navigate-the-workload-balancer.md#customize-the-view) in [Navigieren im Workload Balancer](/help/quicksilver/resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).</span>

1. (Bedingt) Klicken Sie im Workload-Balancer eines Projekts auf das Symbol **Alle Benutzer anzeigen** ![Alle Benutzer anzeigen](assets/show-all-users-icon-project-workload-balancer.png), um alle Workfront-Benutzer anzuzeigen.

   Dadurch werden alle Benutzer angezeigt, auf die Sie Zugriff haben.

   Die Benutzer, die auch Teil des Projektteams sind und bereits Elementen im Projekt zugewiesen sind, haben das Projektsymbol rechts neben ihrem Namen im Bereich Zugewiesene Arbeit .

   ![Benutzer im Projekt](assets/user-on-the-project-indicator-highlighted-project-workload-balancer.png)

   >[!TIP]
   >
   >* Die Option Alle Benutzer anzeigen ist nur im Workload Balancer eines Projekts verfügbar.
   >* Verwenden Sie Filter, um nur die Benutzer anzuzeigen, die für Sie wichtig sind. Verwenden Sie beispielsweise einen Filter, um nur Benutzer aus Ihren Teams oder Gruppen anzuzeigen.

1. Klicken Sie auf den Balken eines Arbeitselements (<span class="preview"> Rollenzuweisung), </span> entweder die geplante oder die projizierte Zeitleiste anzeigt, und ziehen Sie sie über die Stunden für einen Benutzer in den Bereich **Zugewiesen**.

   Der Benutzer, über den Sie den Mauszeiger bewegen, um das Arbeitselement abzulegen, ist hervorgehoben.

   <span class="preview">Beim Ziehen und Ablegen von Rollenzuweisungen wird der Benutzer orange hervorgehoben, wenn seine aktuelle Rolle nicht mit der Rollenzuweisung übereinstimmt. Sie können die Arbeit dennoch dem Benutzer zuweisen, wenn die Rollen nicht übereinstimmen.</span>

   >[!TIP]
   >
   >Die „Geplanten Stunden“ für den Benutzer, auf den Sie den Mauszeiger bewegen, werden in Echtzeit mit der Anzahl der täglichen geplanten Stunden aus dem Arbeitselement aktualisiert, um anzugeben, wie sich das Hinzufügen eines neuen Elements auf seine Gesamtzuweisung auswirken könnte.

   <span class="preview">Beispielbild in der Vorschau-Umgebung:</span>
   ![Element ablegen, das einem Benutzer zugewiesen werden soll](assets/wb-drag-drop-role-or-task-to-user.png)

   Beispielbild in der Produktionsumgebung:
   ![Element ablegen, das einem Benutzer zugewiesen werden soll](assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png)

1. Wenn Sie bereit sind, legen Sie das ausgewählte Arbeitselement <span class="preview">oder die </span>) in derselben Zeile wie den Namen des Benutzers im Bereich Zugeordnet ab. Das Element wird zugewiesen und die zugewiesenen geplanten Stunden werden für den Benutzer mit den neuen Stunden aus dem Arbeitselement aktualisiert.

   <span class="preview">Wenn die Einstellung „Funktionszuweisungen anzeigen“ nicht aktiviert </span> und das Arbeitselement einem Aufgabengebiet zugewiesen wurde, das der Benutzer nicht erfüllen kann, wird das Element unter dem Namen des Benutzers im Bereich Zugewiesene Arbeit angezeigt. Sie verbleibt auch im Bereich Nicht zugewiesene Arbeit , um anzugeben, dass das mit ihr verknüpfte Aufgabengebiet noch nicht durch einen Benutzer ersetzt wurde.

   >[!TIP]
   >
   >* Wenn Sie im Bereich Einstellungen die Option Nach Projekt gruppieren aktiviert haben, wird die zugewiesene Aufgabe unter dem entsprechenden Projekt angezeigt. Wenn die Einstellung deaktiviert ist, wird die zugewiesene Aufgabe im Benutzerbereich angezeigt.
   >
   >
   >     Das Element wird gemäß den Workload-Balancer-Kriterien zum Sortieren von Arbeitselementen angezeigt. Weitere Informationen finden Sie unter [Navigieren im Workload Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).
   >
   >
   >* Wenn Sie im Workload-Balancer eines Projekts die Option Alle Benutzer anzeigen aktiviert und Benutzern Elemente zugewiesen haben, die zuvor keinen Elementen im Projekt zugewiesen waren, werden die Benutzer zum Projekt-Team hinzugefügt. Weitere Informationen finden Sie unter [Projektteam verwalten](../../manage-work/projects/planning-a-project/manage-project-team.md).


1. (Optional) Klicken Sie auf die Leiste eines Arbeitselements unter dem Namen eines Benutzers im Bereich Zugewiesene Arbeit und ziehen Sie es dann über den Bereich Nicht zugewiesene Arbeit , um die Zuweisung aufzuheben. Die Zuweisung des Elements für den Benutzer wurde aufgehoben, es kann jedoch weiterhin einem Aufgabengebiet zugewiesen sein. In diesem Fall wird es im Bereich Nicht zugewiesene Arbeit angezeigt. Wenn das Element einem anderen Benutzer zugewiesen wird, bleibt es im Bereich Zugewiesene Arbeit unter dem Namen des Benutzers, der noch zugewiesen ist.
1. (Optional) Klicken Sie auf das **Zuordnungssymbol anzeigen** ![Zuordnungssymbol anzeigen](assets/show-allocations-icon-small.png) und klicken Sie dann auf das **Mehr Menü** ![Mehr Menü](assets/qs-more-menu.png) > **Zuordnungen bearbeiten**.

   <!--
   (make sure these are still called this, and that the icon has not changed)
   -->
   Oder

   Doppelklicken Sie auf eine tägliche oder wöchentliche Zuordnung, um die Zeit zu ändern, die der Benutzer dem Arbeitselement zugewiesen ist.

   Informationen zum Ändern der Benutzerzuweisungen im Workload Balancer finden Sie im Abschnitt „Ändern von Benutzerzuweisungen“ im Artikel [Verwalten von Benutzerzuweisungen im Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Informationen zum Entfernen von Zuweisungen aus einem Arbeitselement mithilfe des Workload Balancer finden Sie unter [Zuweisung von Arbeit im Workload Balancer aufheben](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

