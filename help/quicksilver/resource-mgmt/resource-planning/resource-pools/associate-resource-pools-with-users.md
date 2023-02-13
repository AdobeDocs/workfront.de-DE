---
product-area: resource-management
navigation-topic: resource-pools
title: Verknüpfen von Ressourcen-Pools mit Benutzern
description: Verknüpfen von Ressourcen-Pools mit Benutzern
author: Alina
feature: Resource Management
exl-id: 0816a2d6-2a45-4e01-8ca2-6d0d190b2568
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# Verknüpfen von Ressourcen-Pools mit Benutzern

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: The info about how to add resource pools to users, are duplicated from the articles listed in those sections (Creating Users, etc). I decided to keep the steps here because those articles are too long to rummage through for updating just this one field.)</p>
-->

Ressourcen-Pools sind Sammlungen von Benutzern, die Ihnen bei der Verwaltung von Ressourcen in Adobe Workfront helfen.

Sie müssen einen Ressourcen-Pool erstellen, bevor Sie ihn mit Benutzern verknüpfen können.

Sie können Benutzer bei der Erstellung Ihrer Ressourcen-Pools Ressourcen-Pools zuordnen.

Wenn Sie Ressourcen-Pools erstellen, ohne sie mit Benutzern zu füllen, können Sie diese später beim Bearbeiten oder Erstellen neuer Benutzer Benutzern zuordnen.

Informationen zu Ressourcen-Pools finden Sie unter [Ressourcen-Pools - Übersicht](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

Informationen zum Erstellen von Ressourcen-Pools finden Sie unter [Erstellen von Ressourcen-Pools](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Pro und höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf die Ressourcenverwaltung bearbeiten, einschließlich Zugriff auf Ressourcen-Pools verwalten</p> <p>Zugriff auf Projekte, Vorlagen und Benutzer bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für die Projekte, Vorlagen und Benutzer, mit denen Sie die Ressourcenpools verknüpfen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Verknüpfen von Ressourcen-Pools mit einem Benutzer

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.

1. Klicken **Benutzer**.
1. Markieren Sie in der Liste das Kästchen neben dem Namen eines Benutzers und klicken Sie auf **Bearbeiten**.
1. Klicken **Ressourcenplanung**.
1. Beginnen Sie mit der Eingabe des Namens eines Ressourcenpools, den Sie mit dem Benutzer in der **Ressourcen-Pools** und wählen Sie es aus der Liste aus, sobald es erscheint.\
   Sie können mehrere Ressourcen-Pools mit einem Benutzer verknüpfen.\
   ![add_resource_pool_to_user.png](assets/add-resource-pool-to-user-350x307.png)

1. Klicken **Änderungen speichern**.

Weitere Informationen zum Bearbeiten von Benutzern finden Sie unter [Benutzerprofil bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Weitere Informationen zum Erstellen neuer Benutzer finden Sie unter [Benutzer hinzufügen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Ressourcen-Pools mit mehreren Benutzern zuordnen

Sie können mehrere Benutzer stapelweise bearbeiten und dieselben Ressourcen-Pools mit allen gleichzeitig verknüpfen.

So verknüpfen Sie Ressourcenpools stapelweise mit mehreren Benutzern:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.

1. Klicken **Benutzer**.
1. Wählen Sie mehrere Benutzer in der Liste aus und klicken Sie auf **Bearbeiten**.
1. Klicken **Ressourcenplanung**.
1. Beginnen Sie mit der Eingabe des Namens eines Ressourcenpools, den Sie mit den Benutzern in der **Ressourcen-Pools** und wählen Sie es aus der Liste aus, sobald es erscheint.\
   Sie können mehrere Ressourcen-Pools mit mehreren Benutzern verknüpfen.

   >[!NOTE]
   >
   >In diesem Feld werden nur die Ressourcen-Pools angezeigt, die allen ausgewählten Benutzern gemeinsam sind. Wenn die ausgewählten Benutzer keine gemeinsamen Ressourcen-Pools haben, ist dieses Feld leer. Wenn dieses Feld leer ist, überschreiben die Ressourcen-Pools, die Sie hier angeben, ihre einzelnen Ressourcen-Pools.

1. Klicken **Änderungen speichern**.

Weitere Informationen zum Massenbearbeitung von Benutzern finden Sie unter [Massenbearbeitung von Benutzerprofilen](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).
