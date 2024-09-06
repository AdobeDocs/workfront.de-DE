---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Manuelles Zuweisen der Arbeit mithilfe des Lastenausgleichs
description: Mit dem Adobe Workfront Workload Balancer können Sie Benutzern Arbeitselemente manuell zuweisen.
author: Lisa
feature: Resource Management
role: User
exl-id: 445cb250-53a4-488b-911d-3afca3a02c23
source-git-commit: db0aab0e6e7e896a8e7c0afe2da709de7c3c2a4e
workflow-type: tm+mt
source-wordcount: '722'
ht-degree: 1%

---

# Manuelles Zuweisen von Arbeiten mithilfe des Lastenausgleichs

Mit dem Adobe Workfront Workload Balancer können Sie Benutzern Arbeitselemente manuell zuweisen.

Allgemeine Informationen zum Zuweisen von Arbeit zu Benutzern mithilfe des Workload-Balancers finden Sie unter [Übersicht über die Zuweisung von Arbeit im Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

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
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Contribute-Berechtigungen oder höher für die Projekte, Aufgaben und Probleme, die Zuweisungen beinhalten</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Manuelles Zuweisen von Arbeiten im Arbeitslastausgleich

Sie können Arbeitselemente zuweisen, die noch keinem Benutzer zugewiesen wurden, oder Elemente neu zuweisen, die Benutzern im Arbeitslastausgleich zugewiesen wurden.

1. Wechseln Sie zum Arbeitslast-Balancer, dem Sie Arbeit zuweisen möchten.

   Sie können Benutzern mithilfe des Lastenausgleichs im Bereich &quot;Ressourcen&quot;, auf Projekt- oder Teamebene Arbeit zuweisen. Weitere Informationen darüber, wo sich der Arbeitslast-Balancer in Workfront befindet, finden Sie unter [Suchen des Arbeitslast-Balancers](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Optional) Wechseln Sie zum Bereich **Nicht zugewiesene Arbeit** und wenden Sie einen Filter an, um Aufgaben oder Probleme anzuzeigen.

   Oder

   Wechseln Sie zum Bereich **Zugewiesene Arbeit** und erweitern Sie den Namen eines Benutzers, um die ihm zugewiesenen Arbeitselemente anzuzeigen, wenn Sie dessen Elemente neu zuweisen möchten.

1. Klicken Sie links neben dem Namen eines Arbeitselements auf das Menü &quot;**Mehr&quot;** ![](assets/qs-more-menu.png) und klicken Sie dann auf &quot;**Dieses Element zuweisen&quot;**.

   ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   >[!TIP]
   >
   >Sie können auch die folgenden Verknüpfungen verwenden, um Aufgaben oder Probleme zuzuweisen:
   >
   >* Unter Windows: Klicken Sie bei gedrückter Strg-Taste auf die Aufgaben- oder Problemleiste.
   >* In Mac: Klicken Sie bei gedrückter CMD-Taste auf die Aufgaben- oder Problemleiste.

1. Führen Sie einen der folgenden Schritte aus:

   * Beginnen Sie mit der Eingabe des Namens eines Benutzers, einer Rolle oder eines Teams, den bzw. das Sie dem Element im Feld **Personen, Rollen oder Teams suchen** zuweisen möchten, wählen Sie es aus, wenn es in der Liste angezeigt wird, und klicken Sie dann auf **Speichern**.

   >[!TIP]
   >
   >Beachten Sie beim Hinzufügen eines Benutzers den Avatar, die Primäre Rolle des Benutzers und seine E-Mail-Adresse, um zwischen Benutzern mit identischen Namen zu unterscheiden.
   >
   >Benutzer müssen mindestens einer Auftragsrolle zugeordnet sein, damit sie beim Hinzufügen angezeigt werden können.
   >
   > Sie müssen die Einstellung Kontaktinformationen anzeigen auf Ihrer Zugriffsebene aktivieren, damit Benutzer E-Mails von Benutzern anzeigen können. Weitere Informationen finden Sie unter [Gewähren des Zugriffs für Benutzer](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


   ![](assets/assignments-box-with-advanced-assignments-delegations-wb.png)

   >[!TIP]
   >
   > Wenn Ihr Workfront- oder Gruppenadministrator Delegationen in Ihrer Umgebung aktiviert hat, verwenden Sie die Registerkarte Zuweisungen , um Benutzer der Aufgabe oder dem Problem zuzuweisen. Verwenden Sie die Registerkarte &quot;Delegationen&quot;, um Benutzer anzuzeigen, die dem Arbeitselement zugewiesen sind. Informationen zum Delegieren von Aufgaben finden Sie unter [Verwalten von Aufgaben und Problemdelegationen](../../manage-work/delegate-work/how-to-delegate-work.md).


   Dadurch wird das Arbeitselement den angegebenen Bevollmächtigten zugewiesen oder neu zugewiesen.

   Wenn Sie ein Element nur einem Team oder einer Auftragsrolle zuweisen, wird das Element nur im Bereich Nicht zugewiesene Arbeit angezeigt. Sie müssen den Benutzern Arbeitselemente zuweisen, um sie im Bereich &quot;Zugewiesene Arbeit&quot;des Workload Balancer anzuzeigen.

   >[!TIP]
   >
   >Sie können mehrere Benutzer, Auftragsrollen oder Teams zuweisen. Sie können nur aktive Benutzer, Stellenrollen und Teams zuweisen.
   >
   >
   >Wenn ein Benutzer, eine Rolle oder ein Team zugewiesen wurde, bevor sie deaktiviert wurden, bleiben sie dem Arbeitselement zugewiesen. In diesem Fall empfehlen wir Folgendes:
   >
   >   
   >   
   >   * Weisen Sie das Arbeitselement aktiven Ressourcen erneut zu.
   >   * Verknüpfen Sie die Benutzer in einem deaktivierten Team mit einem aktiven Team und weisen Sie das Arbeitselement dem aktiven Team erneut zu.
   >   
   >

   * Klicken Sie auf **Erweitert** , um auf erweiterte Zuweisungen zuzugreifen.

     Weitere Informationen zum Erstellen erweiterter Zuweisungen finden Sie unter [Erstellen erweiterter Zuweisungen](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. (Optional) Klicken Sie auf das Symbol **Zuordnungen anzeigen** ![](assets/show-allocations-icon-small.png) und dann auf das Menü **Mehr** ![](assets/qs-more-menu.png) > **Zuordnungen bearbeiten**.

   Oder

   Doppelklicken Sie auf eine tägliche oder wöchentliche Zuordnung, um die Zeit zu ändern, die der Benutzer dem Arbeitselement zugewiesen ist.

   Informationen zum Ändern von Benutzerzuordnungen im Arbeitslastausgleich finden Sie im Abschnitt &quot;Ändern der Benutzerzuordnungen&quot;im Artikel [Verwalten von Benutzerzuordnungen im Arbeitslastausgleich](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Weitere Informationen zum Entfernen von Zuweisungen aus einem Arbeitselement mithilfe des Lastenausgleichs finden Sie unter [Zuweisung der Arbeit im Arbeitslastausgleich aufheben](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

    
