---
title: Zugriff auf Ressourcenverwaltung gewähren
user-type: administrator
product-area: system-administration;resource-management
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-Administrator können Sie eine Zugriffsebene verwenden, um den Zugriff eines Benutzers auf die Ressourcenverwaltung in Workfront zu definieren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 14948e33-3dd7-4ef3-9307-51628dedd1f5
TQID: https://experienceleague.adobe.com/K-SveIsDCsH7eskte0y96MwUlPoQ2FANImBY3RxshKo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
  - id: d3382524-5489-431b-bde9-271ab257bc37
  - id: fceb5125-bb41-419a-b0db-31958cb42f6c
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 488
ht-degree: 15%

---

# Gewähren von Zugriff auf das Ressourcen-Management

Als Adobe Workfront-Administrator können Sie eine Zugriffsebene verwenden, um den Zugriff eines Benutzers auf die Ressourcenverwaltung zu definieren, wie in [Übersicht über Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md) beschrieben.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
   <p>Abo</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurieren des Benutzerzugriffs auf Ressourcen-Management-Tools mithilfe einer benutzerdefinierten Zugriffsebene

1. Erstellen oder bearbeiten Sie die Zugriffsebene, wie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen“ &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicken Sie auf das Zahnradsymbol ![](assets/gear-icon-settings.png) der Schaltfläche **Anzeigen** oder **Bearbeiten** rechts neben Resource Management und wählen Sie dann die Funktionen aus, die Sie unter **Einstellungen optimieren** gewähren möchten.

   ![](assets/resource-management-details-of-edit-in-the-access-level.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Prioritäten und Budgetstunden im Planer bearbeiten</td> 
      <td> <p>Ermöglicht Benutzern mit dieser Lizenz, Folgendes auszuführen:</p> <p>Priorisieren Sie Projekte im Ressourcenplaner.</p> <p>Budgetzuweisung für Ressourcen in den Ressourcenplanungs-Tools (Ressourcenplaner und Ressourcenbudgetierung im Business Case eines Projekts).</p> <p>Standardmäßig ist diese Option aktiviert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ressourcenpools verwalten</td> 
      <td> <p>Ermöglicht Benutzern mit dieser Lizenz das Erstellen, Bearbeiten und Löschen von Ressourcenpools. Standardmäßig ist diese Option deaktiviert.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>Geplante Stunden im Workload Balancer aktualisieren</span> </td> 
      <td> <p>Ermöglicht es Benutzenden mit dieser Lizenz, die geplanten Stunden von Arbeitselementen zu aktualisieren, wenn sie die Benutzerzuweisungen im Workload Balancer aktualisieren. Die Gesamtzahl der zugewiesenen Stunden wird zu den geplanten Stunden der Arbeitselemente.</p> <p>Standardmäßig ist diese Option deaktiviert.</p> <p> Weitere Informationen finden Sie unter <a href="../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Verwalten von Benutzerzuweisungen im Workload-Balancer</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Um Zugriffseinstellungen für andere Objekte und Bereiche in der Zugriffsebene, an der Sie arbeiten, zu konfigurieren, fahren Sie mit einem der in [Zugriff auf Adobe Workfront konfigurieren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md) aufgelisteten Artikel fort, z. B. [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) und [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Wenn Sie fertig sind, klicken Sie auf **Speichern**.

   Nachdem die Zugriffsebene erstellt wurde, können Sie sie einem Benutzer zuweisen. Weitere Informationen finden Sie [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Zugriff auf die Ressourcenverwaltung nach Lizenztyp

Informationen dazu, was Benutzer in den einzelnen Zugriffsebenen mit der Ressourcenverwaltung tun können, finden Sie im Abschnitt [Ressourcenverwaltung](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#resource) im Artikel [Für jeden Objekttyp verfügbare Funktionen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Zugriff auf freigegebene Anfragen

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Wenn Sie ein Objekt für einen anderen Benutzer freigeben, werden die Rechte des Empfängers, die Ressourcenzuteilung darauf anzuzeigen oder zu budgetieren, durch eine Kombination aus drei Elementen bestimmt:

* Zugriffsebenen-Einstellung des Empfängers für das Ressourcen-Management
* den Zugriff des Benutzers auf Finanzdaten, wie unter [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* Alle Berechtigungen für Finanzdaten, die der Teilhaber für das Objekt gewährt hat

Informationen zu den Berechtigungen, die Benutzer bei der Freigabe eines Objekts für Finanzdaten erteilen können, finden Sie unter [Freigeben von Finanzberechtigungen für ein Objekt](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).
