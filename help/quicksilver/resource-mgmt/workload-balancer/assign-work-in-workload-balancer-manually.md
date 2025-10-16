---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Manuelles Zuweisen von Arbeit über den Workload Balancer
description: Mit dem Adobe Workfront Workload Balancer können Sie Benutzenden manuell Arbeitselemente zuweisen.
author: Lisa
feature: Resource Management
role: User
exl-id: 445cb250-53a4-488b-911d-3afca3a02c23
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '747'
ht-degree: 1%

---

# Manuelles Zuweisen von Arbeit über den Workload Balancer

{{preview-fast-release-general}}

Mit dem Adobe Workfront Workload Balancer können Sie Benutzenden manuell Arbeitselemente zuweisen.

Allgemeine Informationen zum Zuweisen von Arbeit zu Benutzern mithilfe des Workload Balancer finden Sie unter [Übersicht über die Zuweisung von Arbeit im Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td>
  </tr>
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Planung, wenn der Workload Balancer im Bereich „Ressourcen“ verwendet wird; Arbeit, wenn der Workload Balancer eines Teams oder Projekts verwendet wird</p></td>
  </tr>
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
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
   <td>Objektberechtigungen</td> 
   <td>Tragen Sie Berechtigungen oder höher zu den Projekten, Aufgaben und Problemen bei, die „Zuweisungen vornehmen“ enthalten</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Arbeiten im Workload Balancer manuell zuweisen

Sie können Arbeitselemente, die noch keinem Benutzer zugewiesen wurden, oder Elemente, die Benutzern im Workload Balancer zugewiesen wurden, neu zuweisen.

1. Wechseln Sie zum Workload Balancer, dem Sie Arbeit zuweisen möchten.

   Sie können Benutzern mithilfe des Workload Balancer im Bereich Ressource, auf Projekt- oder auf Teamebene Arbeit zuweisen. Weitere Informationen dazu, wo sich der Workload-Balancer in Workfront befindet, finden Sie unter [Suchen des Workload-Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Optional) Wechseln Sie zum Bereich **Nicht zugewiesene Arbeit** und wenden Sie einen Filter an, um Aufgaben, Probleme <span class="preview"> Rollenzuweisungen anzuzeigen</span>.

   Oder

   Wechseln Sie zum Bereich **Zugewiesene Arbeit** und erweitern Sie den Namen eines Benutzers, um die ihm zugewiesenen Arbeitselemente anzuzeigen, wenn Sie seine Elemente neu zuweisen möchten.

   >[!NOTE]
   >
   ><span class="preview">Funktionszuweisungen werden unter Arbeitselementen im Bereich Nicht zugeordnete Arbeit angezeigt, wenn die Einstellung „Funktionszuweisungen anzeigen“ aktiviert ist. Weitere Informationen finden Sie unter [Anpassen der Ansicht](/help/quicksilver/resource-mgmt/workload-balancer/navigate-the-workload-balancer.md#customize-the-view) in [Navigieren im Workload Balancer](/help/quicksilver/resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).</span>

1. Klicken Sie auf das **Mehr** Menü ![Mehr](assets/qs-more-menu.png) links neben einem Arbeitselementnamen <span class="preview">oder einer </span>) und klicken Sie dann auf **Zuweisen zu**.

   ![Diese zuweisen zu](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   >[!TIP]
   >
   >Sie können auch die folgenden Tastaturbefehle verwenden, um Aufgaben oder Probleme zuzuweisen:
   >
   >* Unter Windows: STRG+Klicken auf die Aufgaben- oder Problemleiste.
   >* In Mac: Klicken Sie bei gedrückter Befehlstaste auf die Aufgaben- oder Problemleiste.

1. Führen Sie einen der folgenden Schritte aus:

   * Beginnen Sie mit der Eingabe des Namens eines Benutzers, eines Aufgabengebiets oder Teams, das Sie dem Element zuweisen möchten, in das Feld **Personen, Funktionen oder Teams suchen** wählen Sie es aus, wenn es in der Liste angezeigt wird, und klicken Sie dann auf **Speichern**.

   >[!TIP]
   >
   >Beachten Sie beim Hinzufügen eines Benutzers den Avatar, die Primäre Rolle des Benutzers und seine E-Mail-Adresse, um zwischen Benutzern mit identischen Namen zu unterscheiden.
   >
   >Benutzende müssen mindestens einem Aufgabengebiet zugeordnet sein, damit sie es beim Hinzufügen anzeigen können.
   >
   > Die Einstellung Kontaktinformationen anzeigen muss in Ihrer Zugriffsebene aktiviert sein, damit Benutzer die E-Mails von Benutzern anzeigen können. Weitere Informationen finden Sie unter [Gewähren des Benutzerzugriffs](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


   ![Erweiterte Zuweisungen](assets/assignments-box-with-advanced-assignments-delegations-wb.png)

   >[!TIP]
   >
   > Wenn der Workfront- oder Gruppenadministrator Delegierungen in Ihrer Umgebung aktiviert hat, verwenden Sie die Registerkarte Zuweisungen , um Benutzende der Aufgabe oder dem Problem zuzuweisen. Verwenden Sie die Registerkarte Delegierungen , um Benutzer anzuzeigen, die an das Arbeitselement delegiert wurden. Informationen zum Delegieren von Arbeit finden Sie unter [Delegieren von Aufgaben und Problemen](../../manage-work/delegate-work/how-to-delegate-work.md).


   Dadurch wird das Arbeitselement den angegebenen Beauftragten zugewiesen oder neu zugewiesen.

   Wenn Sie ein Element nur einem Team oder einem Aufgabengebiet zuweisen, wird das Element nur im Bereich Nicht zugewiesene Arbeit angezeigt. Sie müssen Benutzenden Arbeitselemente zuweisen, damit diese im Bereich Zugewiesene Arbeit des Workload-Balancer angezeigt werden.

   >[!TIP]
   >
   >Sie können mehrere Benutzer, Aufgabengebiete oder Teams zuweisen. Sie können nur aktive Benutzer, Aufgabengebiete und Teams zuweisen.
   >
   >
   >Wenn ein(e) Benutzende(r), ein Aufgabengebiet oder ein Team zugewiesen wurde, bevor sie/er deaktiviert wurden, bleiben sie/sie dem Arbeitselement zugewiesen. In diesem Fall empfehlen wir Folgendes:
   >
   >   
   >   
   >   * Weisen Sie das Arbeitselement den aktiven Ressourcen neu zu.
   >   * Verknüpfen Sie die Benutzer in einem deaktivierten Team mit einem aktiven Team und weisen Sie das Arbeitselement dem aktiven Team zu.
   >   
   >

   * Klicken Sie **Erweitert**, um auf Erweiterte Zuweisungen zuzugreifen.

     Weitere Informationen zu erweiterten Zuweisungen finden Sie unter [Erstellen erweiterter Zuweisungen](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. (Optional) Klicken Sie auf das **Zuordnungssymbol anzeigen** ![Zuordnungssymbol anzeigen](assets/show-allocations-icon-small.png) und klicken Sie dann auf das **Mehr Menü** ![Mehr Menü](assets/qs-more-menu.png) > **Zuordnungen bearbeiten**.

   Oder

   Doppelklicken Sie auf eine tägliche oder wöchentliche Zuordnung, um die Zeit zu ändern, die der Benutzer dem Arbeitselement zugewiesen ist.

   Informationen zum Ändern der Benutzerzuweisungen im Workload Balancer finden Sie im Abschnitt „Ändern von Benutzerzuweisungen“ im Artikel [Verwalten von Benutzerzuweisungen im Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Informationen zum Entfernen von Zuweisungen aus einem Arbeitselement mithilfe des Workload Balancer finden Sie unter [Zuweisung von Arbeit im Workload Balancer aufheben](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

    
