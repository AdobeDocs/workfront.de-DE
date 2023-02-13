---
title: Zugriff auf Resource Management gewähren
user-type: administrator
product-area: system-administration;resource-management
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-Administrator können Sie mithilfe einer Zugriffsebene den Zugriff eines Benutzers auf die Ressourcenverwaltung in Workfront definieren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 14948e33-3dd7-4ef3-9307-51628dedd1f5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 3%

---

# Zugriff auf Resource Management gewähren

Als Adobe Workfront-Administrator können Sie mithilfe einer Zugriffsebene den Zugriff eines Benutzers auf die Ressourcenverwaltung definieren, wie hier beschrieben: [Übersicht über Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Benutzerzugriff auf Ressourcen-Management-Tools mithilfe einer benutzerdefinierten Zugriffsebene konfigurieren

1. Erstellen oder bearbeiten Sie die Zugriffsebene, wie hier beschrieben: [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicken Sie auf das Zahnradsymbol ![](assets/gear-icon-settings.png) auf **Ansicht** oder **Bearbeiten** auf der rechten Seite von &quot;Ressourcenverwaltung&quot;und wählen Sie dann die Fähigkeiten aus, die Sie unter **Einstellungen anpassen**.

   ![](assets/resource-management-details-of-edit-in-the-access-level.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Prioritäten und Budgetstunden im Planer bearbeiten</td> 
      <td> <p>Ermöglicht Benutzern mit dieser Lizenz Folgendes:</p> <p>Priorisieren Sie Projekte im Ressourcenplaner.</p> <p>Budgetzuweisung für Ressourcen in den Tools für die Ressourcenplanung (im Abschnitt Ressourcenplaner und im Abschnitt Ressourcenbudgeting im Geschäftsszenario eines Projekts)</p> <p>Diese Option ist standardmäßig aktiviert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ressourcenpools verwalten</td> 
      <td> <p>Ermöglicht Benutzern mit dieser Lizenz das Erstellen, Bearbeiten und Löschen von Ressourcen-Pools. Diese Option ist standardmäßig deaktiviert.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>Geplante Stunden im Workload Balancer aktualisieren</span> </td> 
      <td> <p>Ermöglicht Benutzern mit dieser Lizenz, die geplanten Stunden von Arbeitselementen zu aktualisieren, wenn sie die Benutzerzuordnungen im Arbeitslastausgleich aktualisieren. Die Gesamtzahl der zugewiesenen Stunden wird zu den geplanten Stunden der Arbeitselemente.</p> <p>Diese Option ist standardmäßig deaktiviert.</p> <p> Weitere Informationen finden Sie unter <a href="../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Verwalten von Benutzerzuordnungen im Lastenausgleich</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Um die Zugriffseinstellungen für andere Objekte und Bereiche in der Zugriffsebene zu konfigurieren, an der Sie arbeiten, fahren Sie mit einem der Artikel fort, die unter [Zugriff auf Adobe Workfront konfigurieren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), z. B. [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) und [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Wenn Sie fertig sind, klicken Sie auf **Speichern**.

   Nachdem die Zugriffsebene erstellt wurde, können Sie sie einem Benutzer zuweisen. Weitere Informationen finden Sie unter [Benutzerprofil bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Zugriff auf die Ressourcenverwaltung nach Lizenztyp

Informationen dazu, was Benutzer in den einzelnen Zugriffsebenen mit Resource Management tun können, finden Sie im Abschnitt [Ressourcenverwaltung](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#resource) im Artikel [Für jeden Objekttyp verfügbare Funktionen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Zugriff auf freigegebene Probleme

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Wenn Sie ein Objekt für einen anderen Benutzer freigeben, werden die Rechte des Empfängers zum Budget oder zur Anzeige der Ressourcenzuweisung für dieses Objekt durch eine Kombination aus drei Faktoren bestimmt:

* Die Einstellung auf Zugriffsebene des Empfängers für Resource Management
* Der Zugriff des Benutzers auf Finanzdaten, wie unter [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* Alle Berechtigungen für Finanzdaten, die der Freigebende für das Objekt erteilt hat

Informationen zu Berechtigungen, die Benutzer bei der Freigabe des Objekts Finanzdaten für ein Objekt gewähren können, finden Sie unter [Freigeben von Finanzberechtigungen für ein Objekt](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).
