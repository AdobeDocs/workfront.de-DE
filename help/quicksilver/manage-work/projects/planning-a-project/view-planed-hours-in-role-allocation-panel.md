---
product-area: projects
navigation-topic: plan-a-project
title: Anzeigen von geplanten Projektstunden im Bereich "Rollenzuweisung"
description: Sie können die Rollenzuordnung für alle Arbeitsrollen anzeigen, die Arbeitselementen in einem Projekt zugewiesen sind, im Bereich Rollenzuweisung des Projekts.
author: Alina
feature: Work Management
exl-id: 76f70cb6-f707-4a73-bc81-e755e2d0a33d
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# Anzeigen von geplanten Projektstunden im Bereich &quot;Rollenzuweisung&quot;

Sie können die Rollenzuordnung für alle Arbeitsrollen anzeigen, die Arbeitselementen in einem Projekt zugewiesen sind, im Bereich Rollenzuweisung des Projekts.

>[!NOTE]
>
>Dieser Artikel bezieht sich auf das Anzeigen der mit Aufgaben und Problemen in einem Projekt verknüpften Vorgangsrollen und der ihnen zugewiesenen geplanten Stunden im Bereich Rollenzuweisung eines Projekts. Informationen zur Abstimmung von geplanten Stunden mit Initiativzeiten über das Bedienfeld &quot;Rollenzuweisung&quot;bei Verwendung des Adobe Workfront-Szenario-Players finden Sie unter folgenden Themen:
>
>* [Rollenzuweisung für Projekte und Initiativen in der Aufgabenliste anzeigen](../../../scenario-planner/show-role-allocation-task-list-nwe.md)
>* [Rollenzuweisung für Projekte und Initiativen im Arbeitslastausgleich anzeigen](../../../scenario-planner/show-role-allocation-workload-balancer.md)
>
>  Sie müssen über eine Scenario Planer-Lizenz verfügen, um die Startzeiten im Bereich Rollenzuweisung anzuzeigen. Weitere Informationen zum Szenario-Planer finden Sie unter [Erste Schritte mit dem Szenario-Planer](../../../scenario-planner/get-started-with-scenario-planning.md) .
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
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Anzeigen oder höherer Zugriff auf Projekte</p> <p>Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für das Projekt</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Sie müssen über Folgendes verfügen:

* Aufgaben oder Probleme, die Auftragsrollen oder Benutzern zugewiesen sind, die mit einer Auftragsrolle verknüpft sind.

  >[!TIP]
  >
  >Wenn die Aufgaben oder Probleme nicht zugewiesen, Teams zugewiesen oder Benutzern ohne Auftragsrolle zugewiesen sind, sind die geplanten Stunden des Projekts im Bereich Rollenzuweisung null.

* Aufgaben und Probleme mit einer Dauer größer als null.

## Anzeigen von geplanten Projektstunden im Bereich &quot;Rollenzuweisung&quot;

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Projekte**.![](assets/main-menu-icon.png)
1. Klicken Sie auf den Namen eines Projekts, um darauf zuzugreifen. Dadurch wird die Seite Projekt geöffnet.
1. Klicken Sie im linken Bereich auf einen der folgenden Elemente:

   * **Aufgaben**
   * **Workload Balancer**

1. Klicken Sie auf das Symbol **Rollenzuweisung anzeigen** ![](assets/show-role-allocation-icon.png).

   Das Bedienfeld Rollenzuordnung wird angezeigt.

   ![](assets/role-allocation-panel-planned-hours-only-350x316.png)

1. Überprüfen Sie die folgenden Informationen im Bereich **Rollenzuweisung** :
|Feld | Beschreibung|
|—|—|
| **Auftragsrolle** |Auftragsrollen, die Aufgaben und Problemen im Projekt zugewiesen sind. Dabei kann es sich um direkt den Aufgaben und Problemen zugewiesene Aufgabenrollen oder Aufgabenrollen handeln, die mit Benutzern verknüpft sind, die Aufgaben und Problemen im Projekt zugewiesen sind.  |
| **Geplante Stunden** |Die Gesamtanzahl der geplanten Stunden aus Aufgaben und Problemen, die Stellenrollen oder Benutzern zugewiesen sind, die mit einer Auftragsrolle im Projekt verknüpft sind.  |



