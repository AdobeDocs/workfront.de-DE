---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Zuweisen von Arbeiten im Arbeitslastausgleich durch Ziehen und Ablegen
description: Sie können Arbeitselemente mithilfe des Adobe Workfront Workload Balancer zuweisen, indem Sie Arbeitselemente an die richtigen Benutzer ziehen und dort ablegen.
author: Alina
feature: Resource Management
exl-id: caffcde8-3953-44a4-b945-76f2de84f4c6
source-git-commit: bbd99435bb07d68bf9058bcd3e8c6ef5d9df75a9
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 1%

---

# Zuweisen von Arbeiten im Arbeitslastausgleich durch Ziehen und Ablegen

<!--remove production and preview preferences at release-->

Sie können Arbeitselemente mithilfe des Adobe Workfront Workload Balancer zuweisen, indem Sie Arbeitselemente an die richtigen Benutzer ziehen und dort ablegen.

Allgemeine Informationen zum Zuweisen von Arbeit zu Benutzern mithilfe des Workload Balancer finden Sie unter [Übersicht über die Zuweisung von Aufgaben im Arbeitslastausgleich](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Planen, um Arbeit im Arbeitslastausgleich im Ressourcenbereich zuzuweisen</p>
   <p>Arbeit, um Arbeit im Arbeitslastausgleich eines Teams oder Projekts zuzuweisen</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene*</td> 
   <td> <p>Bearbeiten Sie den Zugriff auf Folgendes:</p> 
    <ul> 
     <li> <p>Ressourcenverwaltung</p> </li> 
     <li> <p>Projekte</p> </li> 
     <li> <p>Aufgaben</p> </li> 
     <li> <p>Probleme</p> </li> 
    </ul> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Beitragen Sie Berechtigungen oder höher zu den Projekten, Aufgaben und Problemen, die Zuweisungen beinhalten.</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Zuweisen eines Elements durch Ziehen und Ablegen

Sie können einem Benutzer ein Element aus dem Bereich &quot;Nicht zugewiesene Arbeit&quot;zuweisen oder ein bereits zugewiesenes Element einem anderen Benutzer im Bereich &quot;Zugewiesene Arbeit&quot;neu zuweisen.

1. Wechseln Sie zum Arbeitslast-Balancer, dem Sie Arbeit zuweisen möchten.

   Sie können Benutzern mithilfe des Lastenausgleichs im Bereich &quot;Ressourcen&quot;, auf Projekt- oder Teamebene Arbeit zuweisen. Weitere Informationen darüber, wo sich der Arbeitslast-Balancer in Workfront befindet, finden Sie unter [Suchen Sie den Lastenausgleich .](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Optional) Navigieren Sie zum **Nicht zugewiesene Arbeit** und einen Filter anwenden, um Aufgaben und Probleme anzuzeigen, die Benutzern nicht zugewiesen sind

   Oder

   Navigieren Sie zu **Zugewiesene Arbeit** den Namen eines Benutzers ein und erweitern Sie ihn, um die ihm zugewiesenen Arbeitselemente anzuzeigen, wenn Sie dessen Elemente neu zuweisen möchten.

1. (Bedingt) Klicken Sie im Lastenausgleich eines Projekts auf die **Alle Benutzer anzeigen** icon ![](assets/show-all-users-icon-project-workload-balancer.png) , um alle Workfront-Benutzer anzuzeigen.

   Dadurch werden alle Benutzer angezeigt, auf die Sie Zugriff haben.

   Benutzer, die ebenfalls Teil des Projektteams sind und bereits Elementen im Projekt zugewiesen sind, haben im Bereich &quot;Zugewiesene Arbeit&quot;das Projektsymbol rechts neben ihrem Namen.

   ![](assets/user-on-the-project-indicator-highlighted-project-workload-balancer.png)


   >[!TIP]
   >
   >* Die Option Alle Benutzer anzeigen ist nur im Lastenausgleich eines Projekts verfügbar.
   >* Verwenden Sie Filter, um nur die für Sie wichtigen Benutzer anzuzeigen. Verwenden Sie beispielsweise einen Filter, um nur Benutzer aus Ihren Teams oder Gruppen anzuzeigen.




1. Klicken Sie auf die Leiste eines Arbeitselements, das entweder die geplante oder die geplante Timeline anzeigt, und ziehen Sie sie auf den Namen eines Benutzers im **Zugeordnet** Bereich.

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
      >     Das Element wird gemäß den Kriterien für den Lastenausgleich zum Sortieren von Arbeitselementen angezeigt. Weitere Informationen finden Sie unter [Navigieren Sie zum Lastenausgleich .](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).
   >
   >
   >* Wenn Sie die Option Anzeigen aller Benutzer im Arbeitslastausgleich eines Projekts aktiviert und Benutzern Elemente zugewiesen haben, die zuvor nicht Elementen im Projekt zugewiesen waren, werden die Benutzer zum Projektteam hinzugefügt. Weitere Informationen finden Sie unter [Verwalten des Projektteams](../../manage-work/projects/planning-a-project/manage-project-team.md).



1. (Optional) Klicken Sie auf die Leiste eines Arbeitselements unter dem Namen eines Benutzers im Bereich &quot;Zugewiesene Arbeit&quot;und ziehen Sie es dann über den Bereich &quot;Nicht zugewiesene Arbeit&quot;, um die Zuweisung aufzuheben. Das Element wird vom Benutzer nicht zugewiesen, kann jedoch dennoch einer Auftragsrolle zugewiesen sein. In diesem Fall wird es im Arbeitsbereich &quot;Nicht zugewiesen&quot;angezeigt. Wenn das Element einem anderen Benutzer zugewiesen ist, bleibt es im Bereich Zugewiesene Arbeit unter dem Namen des Benutzers, der noch zugewiesen ist.
1. (Optional) Klicken Sie auf die **Symbol &quot;Zuordnungen anzeigen&quot;** ![](assets/show-allocations-icon-small.png)und klicken Sie dann auf **Mehr Menü** ![](assets/qs-more-menu.png) > **Zuordnungen bearbeiten**.

   <!--
   (make sure these are still called this, and that the icon has not changed)
   -->
   Oder

   Doppelklicken Sie auf eine tägliche oder wöchentliche Zuordnung, um die Zeit zu ändern, die der Benutzer dem Arbeitselement zugewiesen ist.

   Informationen zum Ändern der Benutzerzuordnungen im Arbeitslastausgleich finden Sie im Abschnitt &quot;Ändern der Benutzerzuordnungen&quot;im Artikel [Verwalten von Benutzerzuordnungen im Lastenausgleich](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Informationen zum Entfernen von Zuweisungen aus einem Arbeitselement mithilfe des Lastenausgleichs finden Sie unter [Aufheben der Zuweisung von Arbeit zum Arbeitslastausgleich](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

