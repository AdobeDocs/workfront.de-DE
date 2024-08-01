---
product-area: resource-management
navigation-topic: resource-pools
title: Verknüpfen von Ressourcen-Pools mit Benutzern
description: Sie müssen einen Ressourcen-Pool erstellen, bevor Sie ihn mit Benutzern verknüpfen können. Sie können Benutzer bei der Erstellung Ihrer Ressourcen-Pools Ressourcen-Pools zuordnen.
author: Lisa
feature: Resource Management
exl-id: 0816a2d6-2a45-4e01-8ca2-6d0d190b2568
source-git-commit: 36599722aafadcbbc630650a94005fd73b3e517e
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 1%

---

# Verknüpfen von Ressourcen-Pools mit Benutzern

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: The info about how to add resource pools to users, are duplicated from the articles listed in those sections (Creating Users, etc). I decided to keep the steps here because those articles are too long to rummage through for updating just this one field.)</p>
-->

Ressourcen-Pools sind Sammlungen von Benutzern, die Ihnen bei der Verwaltung von Ressourcen in Adobe Workfront helfen.

Sie müssen einen Ressourcen-Pool erstellen, bevor Sie ihn mit Benutzern verknüpfen können.

Sie können Benutzer bei der Erstellung Ihrer Ressourcen-Pools Ressourcen-Pools zuordnen.

Wenn Sie Ressourcen-Pools erstellen, ohne sie mit Benutzern zu füllen, können Sie diese später beim Bearbeiten oder Erstellen neuer Benutzer Benutzern zuordnen.

Informationen zu Ressourcen-Pools finden Sie unter [Überblick über Ressourcen-Pools](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

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
   <td> <p>Zugriff auf die Ressourcenverwaltung bearbeiten, einschließlich Zugriff auf Ressourcen-Pools verwalten</p> <p>Zugriff auf Projekte, Vorlagen und Benutzer bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für die Projekte, Vorlagen und Benutzer, mit denen Sie die Ressourcenpools verknüpfen</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Verknüpfen von Ressourcen-Pools mit einem Benutzer

1. Klicken Sie oben rechts in Adobe Workfront auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png).

1. Klicken Sie auf **Benutzer**.
1. Aktivieren Sie das Kontrollkästchen neben dem Namen eines Benutzers aus der Liste und klicken Sie dann auf **Bearbeiten**.
1. Klicken Sie auf **Ressourcenplanung**.
1. Geben Sie den Namen eines Ressourcenpools, den Sie mit dem Benutzer verknüpfen möchten, im Feld **Ressourcenpools** ein und wählen Sie ihn dann aus der Liste aus, wenn er angezeigt wird.\
   Sie können mehrere Ressourcen-Pools mit einem Benutzer verknüpfen.\
   ![add_resource_pool_to_user.png](assets/add-resource-pool-to-user-350x307.png)

1. Klicken Sie auf **Änderungen speichern**.

Weitere Informationen zum Bearbeiten von Benutzern finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Weitere Informationen zum Erstellen neuer Benutzer finden Sie unter [Benutzer hinzufügen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Ressourcen-Pools mit mehreren Benutzern zuordnen

Sie können mehrere Benutzer stapelweise bearbeiten und dieselben Ressourcen-Pools mit allen gleichzeitig verknüpfen.

So verknüpfen Sie Ressourcenpools stapelweise mit mehreren Benutzern:

1. Klicken Sie oben rechts in Adobe Workfront auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png).

1. Klicken Sie auf **Benutzer**.
1. Wählen Sie mehrere Benutzer in der Liste aus und klicken Sie auf **Bearbeiten**.
1. Klicken Sie auf **Ressourcenplanung**.
1. Geben Sie im Feld **Ressourcen-Pools** den Namen eines Ressourcenpools ein, den Sie den Benutzern zuweisen möchten, und wählen Sie ihn dann aus der Liste aus, wenn er angezeigt wird.\
   Sie können mehrere Ressourcen-Pools mit mehreren Benutzern verknüpfen.

   >[!NOTE]
   >
   >In diesem Feld werden nur die Ressourcen-Pools angezeigt, die allen ausgewählten Benutzern gemeinsam sind. Wenn die ausgewählten Benutzer keine gemeinsamen Ressourcen-Pools haben, ist dieses Feld leer. Wenn dieses Feld leer ist, überschreiben die Ressourcen-Pools, die Sie hier angeben, ihre einzelnen Ressourcen-Pools.

1. Klicken Sie auf **Änderungen speichern**.

Weitere Informationen zum stapelweisen Bearbeiten von Benutzern finden Sie unter [Mehrere Benutzerprofile bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).
