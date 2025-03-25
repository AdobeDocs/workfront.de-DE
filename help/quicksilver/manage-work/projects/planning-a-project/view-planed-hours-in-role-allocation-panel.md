---
product-area: projects
navigation-topic: plan-a-project
title: Geplante Projektstunden im Bedienfeld „Rollenzuweisung“ anzeigen
description: Sie können die Rollenzuweisung für alle Aufgabengebiete anzeigen, die Arbeitselementen in einem Projekt zugewiesen sind, und zwar im Bedienfeld „Rollenzuweisung“ des Projekts.
author: Alina
feature: Work Management
exl-id: 76f70cb6-f707-4a73-bc81-e755e2d0a33d
source-git-commit: 15ddf6b4d82ccc694ec7a6c60d8e2d5b6b3645d6
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 1%

---

# Geplante Projektstunden im Bedienfeld „Rollenzuweisung“ anzeigen

Sie können die Rollenzuweisung für alle Aufgabengebiete anzeigen, die Arbeitselementen in einem Projekt zugewiesen sind, und zwar im Bedienfeld „Rollenzuweisung“ des Projekts.

>[!NOTE]
>
>Dieser Artikel bezieht sich auf die Anzeige der Aufgabengebiete, die mit Aufgaben und Problemen in einem Projekt verknüpft sind, und der ihnen zugewiesenen geplanten Stunden im Bedienfeld „Rollenzuweisung“ eines Projekts. Informationen zur Abstimmung der geplanten Stunden mit den Stunden für Initiativen mithilfe des Bedienfelds „Rollenzuweisung“ bei Verwendung des Adobe Workfront-Szenarioplaners finden Sie unter:
>
>* [Funktionszuordnung für Projekte und Initiativen in der Aufgabenliste anzeigen](../../../scenario-planner/show-role-allocation-task-list-nwe.md)
>* [Funktionszuordnung für Projekte und Initiativen im Workload-Balancer anzeigen](../../../scenario-planner/show-role-allocation-workload-balancer.md)
>
>  Sie müssen über eine Lizenz für Szenario-Planer verfügen, um Initiativstunden im Bedienfeld „Rollenzuweisung“ anzeigen zu können. Weitere Informationen zum Szenario-Planer finden Sie unter [Erste Schritte mit dem Szenario-Planer](../../../scenario-planner/get-started-with-scenario-planning.md) .
>

## Zugriffsanforderungen

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Light or higher</p> 
   Or
   <p>Legacy license: Review or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

Sie müssen über Folgendes verfügen:

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
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte anzeigen oder höher</p> <p>Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für das Projekt</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Voraussetzungen

Sie müssen über Folgendes verfügen:

* Aufgaben oder Probleme, die Aufgabengebieten oder Benutzern zugewiesen wurden, die mit einem Aufgabengebiet verknüpft sind.

  >[!TIP]
  >
  >Wenn die Aufgaben oder Probleme nicht zugewiesen oder Teams bzw. Benutzern ohne Aufgabengebiet zugewiesen werden, sind die geplanten Stunden des Projekts im Bedienfeld „Rollenzuweisung“ auf null festgelegt.

* Aufgaben und Probleme mit einer Dauer größer als null.

## Geplante Projektstunden im Bedienfeld „Rollenzuweisung“ anzeigen

1. Klicken Sie auf **Hauptmenü**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront und dann auf **Projekte**.
1. Klicken Sie auf den Namen eines Projekts, um darauf zuzugreifen. Dadurch wird die Projektseite geöffnet.
1. Klicken Sie im linken Bedienfeld auf eine der folgenden Optionen:

   * **Aufgaben**
   * **Workload Balancer**

1. Klicken Sie auf das Symbol **Rollenzuweisung anzeigen** ![Symbol für die Rollenzuweisung anzeigen](assets/show-role-allocation-icon.png).

   Das Bedienfeld „Rollenzuweisung“ wird angezeigt.

   ![Bedienfeld „Rollenzuweisung“ nur mit „Geplante Stunden“](assets/role-allocation-panel-planned-hours-only-350x316.png)

1. Überprüfen Sie die folgenden Informationen im Bedienfeld **Rollenzuweisung**:

   | Feld | Beschreibung |
   |---|---|
   | **Aufgabengebiet** | Aufgabengebiete, die den Aufgaben und Problemen im Projekt zugewiesen sind Dabei kann es sich um Aufgabengebiete handeln, die direkt Aufgaben und Problemen zugewiesen sind, oder um Aufgabengebiete, die Benutzern zugewiesen sind, die Aufgaben und Problemen im Projekt zugewiesen sind. |
   | **Geplante Stunden** | Die Gesamtzahl der geplanten Stunden aus Aufgaben und Problemen, die Aufgabengebieten oder Benutzern zugewiesen wurden, die mit einem Aufgabengebiet im Projekt verknüpft sind. |

