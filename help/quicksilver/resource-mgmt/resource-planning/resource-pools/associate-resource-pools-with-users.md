---
product-area: resource-management
navigation-topic: resource-pools
title: Zuordnen von Ressourcenpools zu Benutzern
description: Sie müssen einen Ressourcenpool erstellen, bevor Sie ihn mit Benutzern verknüpfen können. Sie können Benutzer mit Ressourcenpools verknüpfen, wenn Sie Ihre Ressourcenpools erstellen.
author: Lisa
feature: Resource Management
exl-id: 0816a2d6-2a45-4e01-8ca2-6d0d190b2568
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 2%

---

# Zuordnen von Ressourcenpools zu Benutzern

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: The info about how to add resource pools to users, are duplicated from the articles listed in those sections (Creating Users, etc). I decided to keep the steps here because those articles are too long to rummage through for updating just this one field.)</p>
-->

Ressourcenpools sind Sammlungen von Benutzern, die Ihnen bei der Verwaltung von Ressourcen in Adobe Workfront helfen.

Sie müssen einen Ressourcenpool erstellen, bevor Sie ihn mit Benutzern verknüpfen können.

Sie können Benutzer mit Ressourcenpools verknüpfen, wenn Sie Ihre Ressourcenpools erstellen.

Wenn Sie Ressourcenpools erstellen, ohne sie mit Benutzern zu füllen, können Sie sie später bei der Bearbeitung oder Erstellung neuer Benutzer mit Benutzern verknüpfen.

Informationen zu Ressourcenpools finden Sie unter [Ressourcenpools - Übersicht](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

Informationen zum Erstellen von Ressourcenpools finden Sie unter [Ressourcenpools erstellen](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

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
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Bearbeiten des Zugriffs auf das Ressourcen-Management, der den Zugriff auf die Verwaltung von Ressourcenpools umfasst</p> <p>Zugriff auf Projekte, Vorlagen und Benutzer bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td>Verwalten Sie Berechtigungen für die Projekte, Vorlagen und Benutzer, mit denen Sie die Ressourcenpools verknüpfen möchten</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Zuordnen von Ressourcenpools zu einem Benutzer

{{step-1-to-users}}

1. Aktivieren Sie das Kontrollkästchen neben dem Namen eines Benutzers aus der Liste und klicken Sie dann auf **Bearbeiten**.
1. Klicken Sie **Ressourcenplanung**.
1. Geben Sie den Namen eines Ressourcenpools, den Sie mit dem Benutzer verknüpfen möchten, in das Feld **Ressourcenpools** ein und wählen Sie ihn dann aus der Liste aus.\
   Sie können mehrere Ressourcenpools mit einem Benutzer verknüpfen.\
   ![add_resource_pool_to_user.png](assets/add-resource-pool-to-user-350x307.png)

1. Klicken Sie auf **Änderungen speichern**.

Weitere Informationen zum Bearbeiten von Benutzern finden Sie [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Weitere Informationen zum Erstellen neuer Benutzer finden Sie unter [Benutzer hinzufügen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Ressourcenpools stapelweise mit Benutzern verknüpfen

Sie können mehrere Benutzer gleichzeitig bearbeiten und denselben Ressourcenpool mit allen Benutzern gleichzeitig verknüpfen.

So verknüpfen Sie Ressourcenpools mit mehreren Benutzern in großen Mengen:

{{step-1-to-users}}

1. Wählen Sie mehrere Benutzer aus der Liste aus und klicken Sie auf **Bearbeiten**.
1. Klicken Sie **Ressourcenplanung**.
1. Geben Sie den Namen eines Ressourcenpools, den Sie mit den Benutzern verknüpfen möchten, in das Feld **Ressourcenpools** ein und wählen Sie ihn dann aus der Liste aus.\
   Sie können mehrere Ressourcenpools mit mehreren Benutzern verknüpfen.

   >[!NOTE]
   >
   >In diesem Feld werden nur die Ressourcenpools angezeigt, die für alle ausgewählten Benutzer gelten. Wenn die ausgewählten Benutzer keine freigegebenen Ressourcenpools haben, ist dieses Feld leer. Wenn dieses Feld leer ist, überschreiben die hier angegebenen Ressourcenpools ihre einzelnen Ressourcenpools.

1. Klicken Sie auf **Änderungen speichern**.

Weitere Informationen zum Massenbearbeiten von Benutzern finden Sie unter [Benutzerprofile stapelweise bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).
