---
product-area: resource-management
navigation-topic: resource-pools
title: Erstellen von Ressourcen-Pools
description: Ressourcen-Pools sind Sammlungen von Benutzern, mit denen Sie Ressourcen in Adobe Workfront einfacher verwalten können. Weitere Informationen zu Ressourcen-Pools finden Sie unter Überblick über Ressourcen-Pools .
author: Alina
feature: Resource Management
exl-id: 4991634c-e400-466e-bcee-3b461b6662d8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 1%

---

# Erstellen von Ressourcen-Pools

Ressourcen-Pools sind Sammlungen von Benutzern, mit denen Sie Ressourcen in Adobe Workfront einfacher verwalten können. Weitere Informationen zu Ressourcen-Pools finden Sie unter [Ressourcen-Pools - Übersicht](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

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
   <td> <p>Zugriff auf die Ressourcenverwaltung bearbeiten, einschließlich Zugriff auf Ressourcen-Pools verwalten</p> <p>Zugriff auf Benutzer, Projekte und Vorlagen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für die Projekte und Vorlagen, mit denen Sie die Ressourcenpools verknüpfen möchten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Erstellen eines Ressourcen-Pools {#create-a-resource-pool}

1. Melden Sie sich als Benutzer an, der Zugriff auf die Bearbeitung von Ressourcen-Pools hat.\
   Weitere Informationen finden Sie unter [Erstellen eines Ressourcen-Pools](#create-a-resource-pool).

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.

1. Klicken **Ressourcen**.
1. Klicken **Ressourcen-Pools** im linken Bereich.\
   ![resource_pools_tab.png](assets/resource-pools-tab-350x198.png)

1. Klicken **Neuer Ressourcen-Pool**.
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
         <li><strong>Teams</strong>: Alle Mitglieder des Teams werden dem Ressourcenpool hinzugefügt.</li>
         <li><strong>Gruppen</strong>: Alle Mitglieder der Gruppe werden dem Ressourcenpool hinzugefügt.</li>
         <li><strong>Rollen</strong>: Alle mit dieser Rolle verknüpften Benutzer werden zum Ressourcenpool hinzugefügt.</li>
         <li><strong>Unternehmen</strong>: Alle Benutzer im Unternehmen werden dem Ressourcenpool hinzugefügt.</li>
        </ul><p>Tipp: Sie können nur aktive Benutzer, Teams, <span>Rollen,</span> oder Unternehmen.</p><p>Hinweis: Wenn ein Benutzer Mitglied einer Gruppe, eines Teams, eines Unternehmens oder einer Rolle als Job wird, nachdem die Gruppe, das Team, das Unternehmen oder die Rolle als Job zum Resource Pool hinzugefügt wurden, wird das neue Mitglied nicht automatisch zum Resource Pool hinzugefügt. <br>Wenn ein Benutzer zu dem Team, der Gruppe, dem Unternehmen und der Auftragrolle gehört, die Sie hinzufügen, wird der Benutzer gleichzeitig nur einmal zum Ressourcenpool hinzugefügt.<br>Benutzer, die deaktiviert werden, nachdem sie zum Ressourcenpool hinzugefügt wurden, erscheinen in der Liste der Benutzer abgeblendet und werden als deaktiviert markiert.</p></p></td>
     </tr>
    </tbody>
   </table>

1. (Optional) Verwenden Sie die **Rückgängig** -Link, um die Benutzer zu entfernen, die über eine Gruppe, ein Team, ein Unternehmen oder eine Rolle hinzugefügt wurden.

   >[!NOTE]
   >
   >Es gibt keine Beschränkung dafür, wie viele Benutzer Sie in einem Ressourcen-Pool haben können. Es wird jedoch empfohlen, nicht zu viele Benutzer zu einem Ressourcen-Pool hinzuzufügen, da das Ressourcen-Management andernfalls zu einer Herausforderung werden könnte. Die Liste der Benutzer zeigt nur die ersten 2.000 Benutzer im Ressourcen-Pool an und sie werden alphabetisch aufgelistet.

   ![Resource_pools_NEW__UNDO_button_for_teams_groups_etc.png](assets/resource-pools-new---undo-button-for-teams-groups-etc-350x113.png)

1. (Optional) Klicken Sie auf das X-Symbol rechts neben dem Namen eines Benutzers, um einen Benutzer zu entfernen. Weitere Informationen zum Entfernen von Benutzern aus einem Ressourcenpool finden Sie unter [Benutzer aus Ressourcen-Pools entfernen](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md).
1. (Optional) Verwenden Sie die **Suche** -Option, um einen Benutzer im Ressourcen-Pool zu finden.
1. Klicken Sie auf **Erstellen**.
