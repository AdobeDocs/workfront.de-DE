---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Zuweisen von Arbeiten im Arbeitslastausgleich durch Ziehen und Ablegen
description: Sie können Arbeitselemente mithilfe des Adobe Workfront Workload Balancer zuweisen, indem Sie Arbeitselemente an die richtigen Benutzer ziehen und dort ablegen.
author: Lisa
feature: Resource Management
exl-id: caffcde8-3953-44a4-b945-76f2de84f4c6
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Zuweisen von Arbeiten im Arbeitslastausgleich durch Ziehen und Ablegen

<!--remove production and preview preferences at release-->

Sie können Arbeitselemente mithilfe des Adobe Workfront Workload Balancer zuweisen, indem Sie Arbeitselemente an die richtigen Benutzer ziehen und dort ablegen.

Allgemeine Informationen zum Zuweisen von Arbeit zu Benutzern mithilfe des Workload-Balancers finden Sie unter [Übersicht über die Zuweisung von Arbeit im Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Planen, um Arbeit im Arbeitslastausgleich im Ressourcenbereich zuzuweisen</p>
   <p>Arbeit, um Arbeit im Arbeitslastausgleich eines Teams oder Projekts zuzuweisen</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsstufe*</td> 
   <td> <p>Bearbeiten Sie den Zugriff auf Folgendes:</p> 
    <ul> 
     <li> <p>Ressourcenverwaltung</p> </li> 
     <li> <p>Projekte</p> </li> 
     <li> <p>Aufgaben</p> </li> 
     <li> <p>Probleme</p> </li> 
    </ul> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Contribute-Berechtigungen oder höher für die Projekte, Aufgaben und Probleme, die Zuweisungen beinhalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Zuweisen eines Elements durch Ziehen und Ablegen

Sie können einem Benutzer ein Element aus dem Bereich &quot;Nicht zugewiesene Arbeit&quot;zuweisen oder ein bereits zugewiesenes Element einem anderen Benutzer im Bereich &quot;Zugewiesene Arbeit&quot;neu zuweisen.

1. Wechseln Sie zum Arbeitslast-Balancer, dem Sie Arbeit zuweisen möchten.

   Sie können Benutzern mithilfe des Lastenausgleichs im Bereich &quot;Ressourcen&quot;, auf Projekt- oder Teamebene Arbeit zuweisen. Weitere Informationen darüber, wo sich der Arbeitslast-Balancer in Workfront befindet, finden Sie unter [Suchen des Arbeitslast-Balancers](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Optional) Wechseln Sie zum Bereich **Nicht zugewiesene Arbeit** und wenden Sie einen Filter an, um Aufgaben und Probleme anzuzeigen, die Benutzern nicht zugewiesen sind.

   Oder

   Wechseln Sie zum Bereich **Zugewiesene Arbeit** und erweitern Sie den Namen eines Benutzers, um die ihm zugewiesenen Arbeitselemente anzuzeigen, wenn Sie dessen Elemente neu zuweisen möchten.

1. (Bedingt) Klicken Sie im Arbeitslast-Balancer eines Projekts auf das Symbol **Alle Benutzer anzeigen** ![](assets/show-all-users-icon-project-workload-balancer.png) , um alle Workfront-Benutzer anzuzeigen.

   Dadurch werden alle Benutzer angezeigt, auf die Sie Zugriff haben.

   Benutzer, die ebenfalls Teil des Projektteams sind und bereits Elementen im Projekt zugewiesen sind, haben im Bereich &quot;Zugewiesene Arbeit&quot;das Projektsymbol rechts neben ihrem Namen.

   ![](assets/user-on-the-project-indicator-highlighted-project-workload-balancer.png)


   >[!TIP]
   >
   >* Die Option Alle Benutzer anzeigen ist nur im Lastenausgleich eines Projekts verfügbar.
   >* Verwenden Sie Filter, um nur die für Sie wichtigen Benutzer anzuzeigen. Verwenden Sie beispielsweise einen Filter, um nur Benutzer aus Ihren Teams oder Gruppen anzuzeigen.



1. Klicken Sie auf die Leiste eines Arbeitselements, das die geplante oder die geplante Timeline anzeigt, und ziehen Sie sie über den Namen eines Benutzers im Bereich **Zugeordneter Benutzer** .

   Der Benutzer, über den Sie den Mauszeiger bewegen, um das Arbeitselement in abzulegen, wird hervorgehoben.

   >[!TIP]
   >
   >Die geplanten Stunden für den Benutzer, über den Sie den Mauszeiger bewegen, werden in Echtzeit mit der Anzahl der täglichen geplanten Stunden ab dem Arbeitselement aktualisiert, um anzugeben, welche Auswirkungen das Hinzufügen eines neuen Elements auf die Gesamtzuordnung haben könnte.

   ![](assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png)

1. Wenn Sie bereit sind, legen Sie das ausgewählte Arbeitselement in derselben Zeile wie den Benutzernamen im zugewiesenen Bereich ab. Das Element wird zugewiesen und die zugewiesenen geplanten Stunden werden für den Benutzer mit den neuen Stunden aus dem Arbeitselement aktualisiert.

   Wenn das Element einer Auftragsrolle zugewiesen wurde, die der Benutzer nicht erfüllen kann, wird das Element unter dem Namen des Benutzers im Bereich Zugewiesene Arbeit angezeigt und es bleibt auch im Bereich Nicht zugewiesene Arbeit , um anzugeben, dass die damit verknüpfte Auftragsrolle noch nicht durch einen Benutzer ersetzt wurde.

   >[!TIP]
   >
   >* Wenn Sie Gruppe nach Projekt im Bereich Einstellungen aktiviert haben, wird die zugewiesene Aufgabe unter dem entsprechenden Projekt angezeigt. Wenn die Einstellung deaktiviert ist, wird die zugewiesene Aufgabe im Benutzerbereich angezeigt.
   >
   >
   >     Das Element wird gemäß den Kriterien für den Lastenausgleich zum Sortieren von Arbeitselementen angezeigt. Weitere Informationen finden Sie unter [Navigieren im Arbeitslastausgleich](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).
   >
   >
   >* Wenn Sie die Option Anzeigen aller Benutzer im Arbeitslastausgleich eines Projekts aktiviert und Benutzern Elemente zugewiesen haben, die zuvor nicht Elementen im Projekt zugewiesen waren, werden die Benutzer zum Projektteam hinzugefügt. Weitere Informationen finden Sie unter [Verwalten des Projektteams](../../manage-work/projects/planning-a-project/manage-project-team.md).


1. (Optional) Klicken Sie auf die Leiste eines Arbeitselements unter dem Namen eines Benutzers im Bereich &quot;Zugewiesene Arbeit&quot;und ziehen Sie es dann über den Bereich &quot;Nicht zugewiesene Arbeit&quot;, um die Zuweisung aufzuheben. Das Element wird vom Benutzer nicht zugewiesen, kann jedoch dennoch einer Auftragsrolle zugewiesen sein. In diesem Fall wird es im Arbeitsbereich &quot;Nicht zugewiesen&quot;angezeigt. Wenn das Element einem anderen Benutzer zugewiesen ist, bleibt es im Bereich Zugewiesene Arbeit unter dem Namen des Benutzers, der noch zugewiesen ist.
1. (Optional) Klicken Sie auf das Symbol **Zuordnungen anzeigen** ![](assets/show-allocations-icon-small.png) und dann auf das Menü **Mehr** ![](assets/qs-more-menu.png) > **Zuordnungen bearbeiten**.

   <!--
   (make sure these are still called this, and that the icon has not changed)
   -->
   Oder

   Doppelklicken Sie auf eine tägliche oder wöchentliche Zuordnung, um die Zeit zu ändern, die der Benutzer dem Arbeitselement zugewiesen ist.

   Informationen zum Ändern von Benutzerzuordnungen im Arbeitslastausgleich finden Sie im Abschnitt &quot;Ändern der Benutzerzuordnungen&quot;im Artikel [Verwalten von Benutzerzuordnungen im Arbeitslastausgleich](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Weitere Informationen zum Entfernen von Zuweisungen aus einem Arbeitselement mithilfe des Lastenausgleichs finden Sie unter [Zuweisung der Arbeit im Arbeitslastausgleich aufheben](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

