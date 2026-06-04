---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Anzeigen und Verwalten der kürzlich gelöschten Elemente einer Gruppe
description: Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie ihre kürzlich gelöschten Arbeitselemente, Dokumente und Vorlagen anzeigen, filtern, wiederherstellen und exportieren.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: d5fbc71b-3b22-48d1-a056-f2c4b32c220c
TQID: https://experienceleague.adobe.com/PnEW-05sHiDCOS-Kua4w8eeO6CXxiUo3toU1yZ77HOw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 415
ht-degree: 10%

---

# Anzeigen und Verwalten der kürzlich gelöschten Elemente einer Gruppe

Wenn Sie eine Gruppe, die Sie im Bereich Gruppen verwalten, anzeigen, können Sie ihre kürzlich gelöschten Projekte, Aufgaben, Probleme, Dokumente und Vorlagen wie folgt anzeigen und damit arbeiten:

* Anzeigen, Filtern und Gruppieren einer Liste kürzlich gelöschter Elemente
* Zuletzt gelöschte Elemente wiederherstellen, die Sie auswählen
* Exportiert eine Liste der kürzlich gelöschten Elemente

Wenn es Gruppen oberhalb Ihrer Gruppe gibt, können deren Administratoren diese Dinge auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

Weitere Informationen zu gelöschten Elementen finden Sie unter [Verwalten gelöschter Elemente](../../../administration-and-setup/manage-workfront/manage-deleted-items/manage-deleted-items.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

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
       <p>Abo</p></td>
  </tr> 
  <tr>
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr>
  <tr> 
   <td>Objektberechtigungen</td>
   <td>Die gelöschten Elemente müssen mit der Gruppe oder einer ihrer Untergruppen verknüpft sein.</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Anzeigen und Verwalten der kürzlich gelöschten Elemente einer Gruppe

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** ![Gruppen](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe.
1. Klicken Sie im linken Bedienfeld auf **Zuletzt gelöscht**.
1. Öffnen Sie eine der folgenden Registerkarten, auf denen Sie die kürzlich gelöschten Elemente der Gruppe anzeigen und verwalten möchten:

   * Projekte
   * Aufgaben
   * Probleme
   * Dokumente
   * Vorlagen

   Jede Registerkarte listet Elemente des entsprechenden Objekttyps auf, die zur aktuellen Gruppe oder zu ihren Untergruppen gehören und in den letzten 30 Tagen gelöscht wurden.

   >[!NOTE]
   >
   >Wenn jemand ein Projekt gelöscht hat, wurden alle Einzelaufgaben, Probleme und Dokumente gleichzeitig gelöscht. Diese werden nicht einzeln auf den Registerkarten Aufgaben, Probleme, Dokumente oder Vorlagen angezeigt. Beim Wiederherstellen des Projekts werden jedoch auch alle diese untergeordneten Objekte im Projekt wiederhergestellt.
   >
   >
   >Wenn jemand eine Aufgabe, ein Problem, ein Dokument oder eine Vorlage einzeln gelöscht hat, können Sie diese auf der entsprechenden Registerkarte anzeigen und verwalten.

1. Führen Sie eine der folgenden Aktionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Objekte wiederherstellen</p> </td> 
      <td> <p>Wählen Sie bis zu 10 Objekte aus und klicken Sie dann auf <strong>Wiederherstellen</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Gesamte Objektliste auf der Registerkarte exportieren</p> </td> 
      <td> <p>Klicken Sie auf <strong>Exportieren</strong>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"> <p>Ändern der Anzeige von Informationen in der Liste</p> </td> 
      <td> <p>Verwenden Sie in der oberen rechten Ecke über der Liste <strong>Filter</strong>, um festzulegen, was basierend auf den von Ihnen angegebenen Kriterien angezeigt werden soll. Mit <strong>Ansicht</strong> können Sie festlegen, welche Felder als Spalten angezeigt werden. Verwenden Sie <strong>Gruppierung</strong>, um die Elemente in Kategorien zu gruppieren.</p> </td> 
     </tr> 
    </tbody> 
   </table>
