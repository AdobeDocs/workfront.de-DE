---
product-area: resource-management
navigation-topic: resource-pools
title: Benutzer aus Ressourcen-Pools entfernen
description: Es gibt zwar keine Beschränkung dafür, wie viele Benutzer Sie in einem Ressourcenpool haben können, aber die Liste der Benutzer zeigt nur die ersten 2000 Benutzer an, die alphabetisch aufgelistet sind.
author: Lisa
feature: Resource Management
exl-id: b888aa95-8d42-4cc3-8a99-6842435c84d2
source-git-commit: a9d507bfcc0a602e71bcdd3142d63cc40175ebf4
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 1%

---

# Benutzer aus Ressourcen-Pools entfernen

{{preview-and-fast-release-Q424}}

Es gibt zwar keine Beschränkung dafür, wie viele Benutzer Sie in einem Ressourcenpool haben können, aber die Liste der Benutzer zeigt nur die ersten 2000 Benutzer an, die alphabetisch aufgelistet sind.

Es wird empfohlen, deaktivierte oder verschobene Rollen oder Abteilungen zu entfernen, um sicherzustellen, dass Sie in allen Ressourcen-Pools stets über eine genaue Liste der Benutzer verfügen.

Weitere Informationen zu Ressourcen-Pools finden Sie unter [Überblick über Ressourcen-Pools](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td><p>Neu: Beliebig</p>
       <p>oder</p>
       <p>Aktuell: Pro und höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf die Ressourcenverwaltung bearbeiten, einschließlich Zugriff auf Ressourcen-Pools verwalten</p> <p>Anzeigen oder höherer Zugriff auf Benutzer</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Entfernen von Benutzern aus einem Ressourcen-Pool

Sie können Benutzer aus einem Ressourcen-Pool entfernen, wenn diese Benutzer in diesem Pool nicht mehr benötigt werden.

So entfernen Sie einen Benutzer aus einem Ressourcen-Pool:

{{step1-to-resourcing}}

1. Klicken Sie im linken Bereich auf **Ressourcenpools** .
1. Wählen Sie einen Ressourcen-Pool aus und klicken Sie auf **Bearbeiten**.
Oder\
   Klicken Sie auf den Namen eines Ressourcen-Pools.

1. Beginnen Sie mit der Eingabe des Namens eines Benutzers, den Sie im Feld **Suche in diesem Ressourcen-Pool** entfernen möchten.\
   Oder\
   Beginnen Sie mit der Eingabe des Namens eines Unternehmens, einer Rolle im Job, eines Teams oder einer Gruppe, wenn Sie alle mit diesen Entitäten verknüpften Benutzer entfernen möchten.

   <span class="preview">Beispielbild in der Vorschauumgebung:<span>

   ![Entfernen von Benutzern aus Resource Pool](assets/remove-users-from-resource-pool.png)

   Beispielbild in der Produktionsumgebung:
   ![Suchen im Ressourcen-Pool](assets/search-inside-new-resource-pool-350x314.png)

1. Klicken Sie auf das Symbol &quot;x&quot;auf Benutzerebene, um einen Benutzer aus dem Ressourcen-Pool zu entfernen. Sie werden aus allen Listen entfernt, in denen sie angezeigt werden.\
   Oder\
   Um alle Benutzer zu entfernen, die mit einer Auftragsrolle, Gruppe, Gruppe oder Firma verbunden sind, klicken Sie auf der Auftrags-, Gruppen-, Team- oder Unternehmensebene auf **Entfernen** . Dadurch werden alle mit dieser Auftragsrolle, Gruppe, Gruppe oder Firma verknüpften Benutzer aus dem Ressourcen-Pool entfernt.

1. Klicken Sie auf **Speichern**.
