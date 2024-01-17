---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Aufheben der Zuweisung von Arbeit zum Arbeitslastausgleich
description: Sie können die Zuweisung von Benutzern zu Arbeitselementen im Bereich Zugewiesene Arbeit des Adobe Workfront Workload Balancer aufheben oder sie anderen Benutzern, Rollen oder Teams zuweisen.
author: Lisa
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 2%

---

# Aufheben der Zuweisung von Arbeit zum Arbeitslastausgleich

Sie können die Zuweisung von Benutzern zu Arbeitselementen im Bereich Zugewiesene Arbeit des Adobe Workfront Workload Balancer aufheben oder sie anderen Benutzern, Rollen oder Teams zuweisen.

Sie können die Zuweisung von Benutzern zu Arbeitselementen manuell aufheben, indem Sie sie per Drag-and-Drop oder stapelweise verschieben. In diesem Artikel wird beschrieben, wie Sie die Zuweisung von Benutzern manuell aufheben.

Informationen zum Aufheben der Zuweisung von Benutzern durch Ziehen und Ablegen finden Sie unter [Zuweisen von Arbeiten im Arbeitslastausgleich durch Ziehen und Ablegen](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)

Informationen zum Aufheben der Zuweisung von Benutzern in großen Mengen finden Sie unter [Stapelweises Zuweisen von Arbeiten mithilfe des Lastenausgleichs](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

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
   <td> <p>Planen Sie bei Verwendung des Lastenausgleichs im Ressourcenbereich</p>
   <p>Arbeiten bei Verwendung des Workload Balancers für ein Team oder Projekt</p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Bearbeiten Sie den Zugriff auf Folgendes:</p> 
    <ul> 
     <li> <p>Ressourcenverwaltung</p> </li> 
     <li> <p>Projekte</p> </li> 
     <li> <p>Aufgaben</p> </li> 
     <li> <p>Probleme</p> </li> 
    </ul> <p>Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Beitragen Sie Berechtigungen oder höher zu den Projekten, Aufgaben und Problemen, die Zuweisungen beinhalten.</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

 

## Aufheben der Zuweisung von Arbeitselementen im Arbeitslastausgleich

Sie können die Zuweisung von Elementen zu Benutzern aufheben und sie in den nicht zugewiesenen Arbeitsbereich verschieben oder sie anderen Benutzern neu zuweisen.

So heben Sie die Zuweisung von Arbeitselementen zu Benutzern auf:

1. Wechseln Sie im Lastenausgleich zum **Zugewiesene Arbeit** Benutzer einblenden und erweitern.
1. Führen Sie einen der folgenden Schritte aus:

   * Suchen Sie das Element, das Sie aufheben möchten, im Bereich eines Benutzers, klicken Sie darauf und ziehen Sie es in den Bereich Nicht zugewiesen oder in den Bereich eines anderen Benutzers.
   * Klicken Sie auf **Mehr** icon ![](assets/more-icon-task-list.png) rechts neben dem Namen eines Arbeitselements klicken Sie auf **Zuweisen**, entfernen Sie dann den Namen der dem Arbeitselement zugewiesenen Entitäten oder geben Sie einen anderen Namen ein und klicken Sie auf **Speichern**.

     ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   Das Element wird im Arbeitsbereich &quot;Nicht zugewiesen&quot;angezeigt, wenn es den Filterkriterien für diesen Bereich entspricht und keinem anderen Benutzer zugewiesen ist, oder im Benutzerbereich, wenn es einem anderen Benutzer zugewiesen ist.

   Informationen zum Filtern von Informationen im Arbeitslastausgleich finden Sie unter [Filtern von Informationen im Arbeitslastausgleich](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
