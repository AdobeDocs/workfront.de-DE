---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Aufheben der Zuweisung von Arbeit im Arbeitslastausgleich
description: Sie können die Zuweisung von Benutzern zu Arbeitselementen im Bereich Zugewiesene Arbeit des Adobe Workfront Workload Balancer aufheben oder sie anderen Benutzern, Rollen oder Teams zuweisen.
author: Lisa
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 196d0aa4ed67cf564c823625515ef49d811e0e06
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 2%

---

# Aufheben der Zuweisung von Arbeit zum Arbeitslastausgleich

Sie können die Zuweisung von Benutzern zu Arbeitselementen im Bereich Zugewiesene Arbeit des Adobe Workfront Workload Balancer aufheben oder sie anderen Benutzern, Rollen oder Teams zuweisen.

Sie können die Zuweisung von Benutzern zu Arbeitselementen manuell aufheben, indem Sie sie per Drag-and-Drop oder stapelweise verschieben. In diesem Artikel wird beschrieben, wie Sie die Zuweisung von Benutzern manuell aufheben.

Weitere Informationen zum Aufheben der Zuweisung von Benutzern durch Ziehen und Ablegen finden Sie unter [Zuweisen von Arbeiten im Arbeitslastausgleich durch Ziehen und Ablegen](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)

Informationen zum Aufheben der Zuweisung von Benutzern in großen Mengen finden Sie unter [Zuweisen von Aufgaben in großen Mengen mithilfe des Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle </p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>oder</p>
       <p>Aktuell: Planen Sie bei Verwendung des Workload-Balancers im Ressourcenbereich;</br>
       Arbeiten bei Verwendung des Workload Balancers für ein Team oder Projekt</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Bearbeiten Sie den Zugriff auf Folgendes:</p> 
    <ul> 
     <li>Ressourcenverwaltung</li> 
     <li>Projekte</li> 
     <li>Aufgaben</li> 
     <li>Probleme</li> 
    </ul></td>
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Contribute-Berechtigungen oder höher für die Projekte, Aufgaben und Probleme, die Zuweisungen beinhalten</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aufheben der Zuweisung von Arbeitselementen im Arbeitslastausgleich

Sie können die Zuweisung von Elementen zu Benutzern aufheben und sie in den nicht zugewiesenen Arbeitsbereich verschieben oder sie anderen Benutzern neu zuweisen.

So heben Sie die Zuweisung von Arbeitselementen zu Benutzern auf:

1. Wechseln Sie im Arbeitslastausgleich zum Bereich **Zugewiesene Arbeit** und erweitern Sie einen Benutzer.
1. Führen Sie einen der folgenden Schritte aus:

   * Suchen Sie das Element, das Sie aufheben möchten, im Bereich eines Benutzers, klicken Sie darauf und ziehen Sie es in den Bereich Nicht zugewiesen oder in den Bereich eines anderen Benutzers.
   * Klicken Sie auf das Symbol **Mehr** ![](assets/more-icon-task-list.png) rechts neben dem Namen eines Arbeitselements, klicken Sie auf **Zuweisen zu**, entfernen Sie dann den Namen der dem Arbeitselement zugewiesenen Entitäten oder geben Sie einen anderen Namen ein und klicken Sie auf **Speichern**.

     ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   Das Element wird im Arbeitsbereich &quot;Nicht zugewiesen&quot;angezeigt, wenn es den Filterkriterien für diesen Bereich entspricht und keinem anderen Benutzer zugewiesen ist, oder im Benutzerbereich, wenn es einem anderen Benutzer zugewiesen ist.

   Informationen zum Filtern von Informationen im Arbeitslastausgleich finden Sie unter [Informationen im Arbeitslastausgleich filtern](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
