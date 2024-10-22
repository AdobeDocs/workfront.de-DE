---
product-area: resource-management
navigation-topic: resource-pools
title: Erstellen von Ressourcen-Pools
description: Ressourcen-Pools sind Sammlungen von Benutzern, mit denen Sie Ressourcen in Adobe Workfront einfacher verwalten können.
author: Lisa
feature: Resource Management
exl-id: 4991634c-e400-466e-bcee-3b461b6662d8
source-git-commit: 854197fcb8c4d3a87e4d93fe2ae9e968a3254027
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 8%

---

# Erstellen von Ressourcen-Pools {#create-resource-pools}

>[!CONTEXTUALHELP]
>id="wf_resource_pools"
>title="Ressourcenpools"
>abstract="Ein Ressourcenpool-Pool ist eine Sammlung von Benutzenden, die gleichzeitig für die Fertigstellung eines Projekts benötigt werden. Nachdem Sie einen Ressourcen-Pool erstellt haben, können Sie ihn mit Projekten und Vorlagen verknüpfen."

Ressourcen-Pools sind Sammlungen von Benutzern, mit denen Sie Ressourcen in Adobe Workfront einfacher verwalten können. Weitere Informationen zu Ressourcen-Pools finden Sie unter [Überblick über Ressourcen-Pools](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

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
       <p>Aktuell: Pro oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf die Ressourcenverwaltung bearbeiten, einschließlich Zugriff auf Ressourcen-Pools verwalten</p> <p>Zugriff auf Projekte, Vorlagen und Benutzer bearbeiten</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Verwalten von Berechtigungen für die Projekte, Vorlagen und Benutzer, mit denen Sie die Ressourcenpools verknüpfen möchten</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen eines Ressourcen-Pools {#create-a-resource-pool}

{{step1-to-resourcing}}

1. Klicken Sie im linken Bereich auf **Ressourcenpools** .
1. Klicken Sie auf **New Resource Pool**.

   ![Ressourcenpools](assets/list-of-resource-pools.png)

1. Geben Sie Folgendes an:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Name</strong></td>
      <td>Dies ist der Name des Ressourcen-Pools.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Beschreibung</strong></td>
      <td>Dies ist eine kurze Beschreibung zu diesem Ressourcen-Pool. Sie können beispielsweise angeben, zu welchem Zweck sie verwendet werden soll.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Pool-Mitglieder</strong></td>
      <td><p> Fügen Sie Benutzer einzeln zum Ressourcen-Pool hinzu.<br>Oder <br>So fügen Sie eine große Anzahl von Benutzern gleichzeitig zum Ressourcen-Pool hinzu. Sie können eine der folgenden Entitäten hinzufügen, die mit Benutzern oder der Sammlung von Benutzern verknüpft sind:
        <ul>
         <li><strong>Teams</strong>: Alle Mitglieder des Teams werden zum Ressourcen-Pool hinzugefügt.</li>
         <li><strong>Gruppen</strong>: Alle Mitglieder der Gruppe werden zum Ressourcenpool hinzugefügt.</li>
         <li><strong>Rollen</strong>: Alle Benutzer, die dieser Rolle zugeordnet sind, werden zum Ressourcen-Pool hinzugefügt.</li>
         <li><strong>Unternehmen</strong>: Alle Benutzer im Unternehmen werden zum Ressourcenpool hinzugefügt.</li>
        </ul><p>Tipp: Sie können nur aktive Benutzer, Teams, <span>Rollen,</span> oder Unternehmen hinzufügen.</p><br>Möglicherweise müssen Sie im Dialogfeld nach unten scrollen, um alle Benutzer im Ressourcen-Pool anzuzeigen.
        <p>Hinweis: Wenn ein Benutzer Mitglied einer Gruppe, eines Teams, eines Unternehmens oder einer Rolle als Job wird, nachdem die Gruppe, das Team, die Firma oder die Rolle für den Job zum Resource Pool hinzugefügt wurden, wird das neue Mitglied nicht automatisch zum Resource Pool hinzugefügt. <br>Wenn ein Benutzer zum Team, zur Gruppe, zum Unternehmen und zur Auftragrolle gehört, die Sie hinzufügen, wird der Benutzer gleichzeitig nur einmal zum Ressourcenpool hinzugefügt.<br>Benutzer, die deaktiviert werden, nachdem sie zum Ressourcen-Pool hinzugefügt wurden, erscheinen in der Liste der Benutzer abgeblendet und werden als deaktiviert markiert.</p></p></td>
     </tr>
    </tbody>
   </table>

1. (Optional) Verwenden Sie den Link &quot;**Rückgängig**&quot;, um die Benutzer zu entfernen, die über eine Gruppe, ein Team, ein Unternehmen oder eine Jobrolle hinzugefügt wurden.

   >[!NOTE]
   >
   >Es gibt keine Beschränkung dafür, wie viele Benutzer Sie in einem Ressourcen-Pool haben können. Es wird jedoch empfohlen, nicht zu viele Benutzer zu einem Ressourcen-Pool hinzuzufügen, da das Ressourcen-Management andernfalls zu einer Herausforderung werden könnte. Die Liste der Benutzer zeigt nur die ersten 2.000 Benutzer im Ressourcen-Pool an und sie werden alphabetisch aufgelistet.

   ![Benutzer, die zum Ressourcen-Pool hinzugefügt wurden](assets/users-in-resource-pool2.png)

1. (Optional) Klicken Sie auf das X-Symbol rechts neben dem Namen eines Benutzers, um einen Benutzer zu entfernen. Weitere Informationen zum Entfernen von Benutzern aus einem Ressourcen-Pool finden Sie unter [Entfernen von Benutzern aus Ressourcen-Pools](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md).
1. (Optional) Verwenden Sie die Option **Suchen** , um einen Benutzer im Ressourcen-Pool zu finden.
1. Klicken Sie auf **Erstellen**.
