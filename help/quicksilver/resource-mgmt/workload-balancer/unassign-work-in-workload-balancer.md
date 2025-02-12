---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Zuweisung von Arbeit im Workload Balancer aufheben
description: Sie können die Zuweisung von Benutzenden zu Arbeitselementen im Bereich Zugewiesene Arbeit im Adobe Workfront-Workload-Balancer aufheben oder sie anderen Benutzenden, Rollen oder Teams neu zuweisen.
author: Lisa
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 23c6d9335b0adcafc4e2ecdd8ef2d0ab09709fa8
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 2%

---

# Zuweisung von Arbeit im Workload Balancer aufheben

Sie können die Zuweisung von Benutzenden zu Arbeitselementen im Bereich Zugewiesene Arbeit im Adobe Workfront-Workload-Balancer aufheben oder sie anderen Benutzenden, Rollen oder Teams neu zuweisen.

Die Zuweisung von Benutzern zu Arbeitselementen kann manuell, durch Ziehen und Ablegen oder stapelweise aufgehoben werden. In diesem Artikel wird beschrieben, wie Sie die Zuweisung von Benutzern manuell aufheben können.

Informationen zum Aufheben der Zuweisung von Benutzern durch Ziehen und Ablegen finden Sie unter [Zuweisen von Arbeit im Workload Balancer durch Ziehen und Ablegen](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)

Informationen zum Aufheben der Zuweisung von Benutzern in großen Mengen finden Sie unter [Massenzuweisung von Arbeit mit dem Workload-Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

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
       <p>Aktuell: Plan, wenn der Workload Balancer im Bereich „Ressourcen“ verwendet wird</br>
       Arbeit bei Verwendung des Workload Balancer eines Teams oder Projekts</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Folgendes bearbeiten:</p> 
    <ul> 
     <li>Ressourcenverwaltung</li> 
     <li>Projekte</li> 
     <li>Aufgaben</li> 
     <li>Probleme</li> 
    </ul></td>
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Tragen Sie Berechtigungen oder höher zu den Projekten, Aufgaben und Problemen bei, die „Zuweisungen vornehmen“ enthalten</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Zuweisung von Arbeitselementen im Workload Balancer aufheben

Sie können die Zuweisung von Elementen zu Benutzern aufheben und sie in den Bereich Nicht zugewiesene Arbeit verschieben oder sie anderen Benutzern neu zuweisen.

So heben Sie die Zuweisung von Arbeitselementen zu Benutzenden auf:

1. Wechseln Sie im Workload Balancer zum Bereich **Zugewiesene Arbeit** und erweitern Sie einen Benutzer.
1. Führen Sie einen der folgenden Schritte aus:

   * Suchen Sie das Element, dessen Zuweisung Sie aufheben möchten, im Bereich „Nicht zugewiesen“ eines Benutzers, klicken Sie darauf und ziehen Sie es per Drag-and-Drop in den Bereich „Nicht zugewiesen“ oder in den Bereich eines anderen Benutzers.
   * Klicken Sie auf das **Mehr**-Symbol ![Mehr-Symbol](assets/more-icon-task-list.png) rechts neben dem Namen eines Arbeitselements, klicken Sie auf **Dies zuweisen zu**, entfernen Sie dann den Namen der dem Arbeitselement zugewiesenen Entitäten, oder geben Sie einen anderen Namen ein, und klicken Sie auf **Speichern**.

     ![Diese zuweisen zu](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   Das Element wird im Bereich Nicht zugewiesene Arbeit angezeigt, wenn es den Filterkriterien für diesen Bereich entspricht und keinem anderen Benutzer zugewiesen ist, oder es wird im Benutzerbereich angezeigt, wenn es einem anderen Benutzer zugewiesen ist.

   Informationen zum Filtern von Informationen im Workload Balancer finden Sie unter [Filtern von Informationen im Workload Balancer](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
