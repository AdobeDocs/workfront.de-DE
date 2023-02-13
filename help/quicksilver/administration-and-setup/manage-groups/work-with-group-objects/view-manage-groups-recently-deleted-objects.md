---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Anzeigen und Verwalten der kürzlich gelöschten Elemente einer Gruppe
description: Wenn Sie eine Gruppe anzeigen, die Sie im Bereich "Gruppen"verwalten, können Sie die kürzlich gelöschten Arbeitselemente, Dokumente und Vorlagen anzeigen, filtern, wiederherstellen und exportieren.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: d5fbc71b-3b22-48d1-a056-f2c4b32c220c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 1%

---

# Anzeigen und Verwalten der kürzlich gelöschten Elemente einer Gruppe

Wenn Sie eine Gruppe anzeigen, die Sie im Bereich &quot;Gruppen&quot;verwalten, können Sie die kürzlich gelöschten Projekte, Aufgaben, Probleme, Dokumente und Vorlagen wie folgt anzeigen und damit arbeiten:

* Liste der zuletzt gelöschten Elemente anzeigen, filtern und gruppieren
* Kürzlich gelöschte Elemente wiederherstellen, die Sie auswählen
* Liste der zuletzt gelöschten Elemente exportieren

Wenn es Gruppen über Ihrer Gruppe gibt, können ihre Administratoren diese Dinge auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

Weitere Informationen zu gelöschten Elementen finden Sie unter [Gelöschte Elemente verwalten](../../../administration-and-setup/manage-workfront/manage-deleted-items/manage-deleted-items.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-Plan*</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> <p>Sie müssen Gruppenadministrator der Gruppe oder Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadministratoren</a> und <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Die gelöschten Elemente müssen der Gruppe oder einer ihrer Untergruppen zugeordnet sein. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenn Sie herausfinden möchten, welchen Plan oder welchen Lizenztyp Sie haben, wenden Sie sich an Ihren Workfront-Administrator.

## Anzeigen und Verwalten der kürzlich gelöschten Elemente einer Gruppe

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **Gruppen** ![](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe.
1. Klicken Sie im linken Bereich auf **Kürzlich gelöscht**.
1. Öffnen Sie eine der folgenden Registerkarten, auf denen Sie die kürzlich gelöschten Elemente der Gruppe anzeigen und verwalten möchten:

   * Projekte
   * Aufgaben
   * Probleme
   * Dokumente
   * Vorlagen

   Jede Registerkarte listet Elemente des entsprechenden Objekttyps auf, die zur aktuellen Gruppe oder ihren Untergruppen gehören und innerhalb der letzten 30 Tage gelöscht wurden.

   >[!NOTE]
   >
   >Wenn jemand ein Projekt gelöscht hat, wurden alle darin enthaltenen Aufgaben, Probleme und Dokumente gelöscht. Diese werden nicht einzeln auf den Registerkarten Aufgaben, Probleme, Dokumente oder Vorlagen angezeigt. Beim Wiederherstellen des Projekts werden jedoch auch alle diese untergeordneten Objekte zum Projekt zurückgegeben.
   >
   >
   >Wenn eine Aufgabe, ein Problem, ein Dokument oder eine Vorlage einzeln gelöscht wurde, können Sie sie auf der entsprechenden Registerkarte anzeigen und verwalten.

1. Führen Sie einen der folgenden Schritte aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Objekte wiederherstellen</p> </td> 
      <td> <p>Wählen Sie bis zu 10 Objekte aus und klicken Sie auf <strong>Wiederherstellen</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Gesamte Liste der Objekte auf der Registerkarte exportieren</p> </td> 
      <td> <p>Klicken <strong>Export</strong>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"> <p>Anzeige von Informationen in der Liste ändern</p> </td> 
      <td> <p>Verwenden Sie in der rechten oberen Ecke der Liste <strong>Filter</strong> , um festzulegen, was basierend auf den von Ihnen angegebenen Kriterien angezeigt wird. Verwendung <strong>Ansicht</strong> , um festzulegen, welche Felder als Spalten angezeigt werden. Verwendung <strong>Gruppierung</strong> um die Elemente in Kategorien zu gruppieren.</p> </td> 
     </tr> 
    </tbody> 
   </table>
