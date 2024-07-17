---
product-area: resource-management
navigation-topic: resource-pools
title: Benutzer aus Ressourcen-Pools entfernen
description: Es gibt zwar keine Beschränkung dafür, wie viele Benutzer Sie in einem Ressourcenpool haben können, aber die Liste der Benutzer zeigt nur die ersten 2000 Benutzer an, die alphabetisch aufgelistet sind.
author: Alina
feature: Resource Management
exl-id: b888aa95-8d42-4cc3-8a99-6842435c84d2
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 1%

---

# Benutzer aus Ressourcen-Pools entfernen

Es gibt zwar keine Beschränkung dafür, wie viele Benutzer Sie in einem Ressourcenpool haben können, aber die Liste der Benutzer zeigt nur die ersten 2000 Benutzer an, die alphabetisch aufgelistet sind.

Es wird empfohlen, deaktivierte oder verschobene Rollen oder Abteilungen zu entfernen, um sicherzustellen, dass Sie in allen Ressourcen-Pools stets über eine genaue Liste der Benutzer verfügen.

Weitere Informationen zu Ressourcen-Pools finden Sie unter [Überblick über Ressourcen-Pools](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

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
   <td> <p>Zugriff auf die Ressourcenverwaltung bearbeiten, einschließlich Zugriff auf Ressourcen-Pools verwalten</p> <p>Anzeigen oder höherer Zugriff auf Benutzer</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>(NOTE:&nbsp;I don't think this is needed for removing users from the pool)</p> <p>Manage permissions for the projects, templates, and users you associate the Resource Pools with</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Entfernen von Benutzern aus einem Ressourcen-Pool

Sie können Benutzer aus einem Ressourcen-Pool entfernen, wenn diese Benutzer in diesem Pool nicht mehr benötigt werden.

So entfernen Sie einen Benutzer aus einem Ressourcen-Pool:

1. Klicken Sie oben rechts in Adobe Workfront auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png).

1. Klicken Sie auf **Ressourcen**.
1. Klicken Sie im linken Bereich auf **Ressourcenpools** .
1. Wählen Sie einen Ressourcen-Pool aus und klicken Sie auf &quot;Bearbeiten&quot;.**Oder\
   Klicken Sie auf den Namen eines Ressourcen-Pools.

1. Beginnen Sie mit der Eingabe des Namens eines Benutzers, den Sie im Feld **Suche in diesem Ressourcen-Pool** entfernen möchten.\
   Oder\
   Beginnen Sie mit der Eingabe des Namens eines Unternehmens, einer Rolle im Job, eines Teams oder einer Gruppe, wenn Sie alle mit diesen Entitäten verknüpften Benutzer entfernen möchten.\
   ![search_inside_NEW_resource_pool.png](assets/search-inside-new-resource-pool-350x314.png)

1. Klicken Sie auf das Symbol &quot;x&quot;auf Benutzerebene, um einen Benutzer aus dem Ressourcen-Pool zu entfernen. Sie werden aus allen Listen entfernt, in denen sie angezeigt werden.\
   Oder\
   Um alle Benutzer zu entfernen, die mit einer Auftragsrolle, Gruppe, Gruppe oder Firma verbunden sind, klicken Sie auf der Auftrags-, Gruppen-, Team- oder Unternehmensebene auf **Entfernen** . Dadurch werden alle mit dieser Auftragsrolle, Gruppe, Gruppe oder Firma verknüpften Benutzer aus dem Ressourcen-Pool entfernt.

1. Klicken Sie auf **Speichern**.
