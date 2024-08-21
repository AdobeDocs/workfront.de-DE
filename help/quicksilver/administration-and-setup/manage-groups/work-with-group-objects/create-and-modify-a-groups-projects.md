---
user-type: administrator
product-area: system-administration;user-management
keywords: group,projects
navigation-topic: work-with-a-groups-objects
title: Erstellen und Ändern von Gruppenprojekten
description: Wenn Sie eine Gruppe anzeigen, die Sie im Bereich "Gruppen"verwalten, können Sie die Projekte der Gruppe erstellen, bearbeiten, exportieren, kopieren und löschen.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: db90cf52-7c8f-4972-b67f-401657ba9b13
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# Erstellen und Ändern von Gruppenprojekten

Wenn Sie eine Gruppe anzeigen, die Sie im Bereich &quot;Gruppen&quot;verwalten, können Sie ihre Projekte wie folgt anzeigen und bearbeiten:

* Neues Projekt für die Gruppe erstellen
* Bearbeiten, Exportieren, Kopieren oder Löschen eines Projekts

Wenn es Gruppen über Ihrer Gruppe gibt, können ihre Administratoren diese Dinge auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td >Workfront-Plan</a>*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</a>*</td> 
   <td> <p>Plan </p> <p>Sie müssen Gruppenadministrator der Gruppe oder Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadministratoren</a> und <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs für Benutzer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> 
    <ul> 
     <li> <p>Das Projekt muss mit der Gruppe oder einer ihrer Untergruppen verknüpft sein. </p> <p>Weitere Informationen zum Zuweisen einer Gruppe zu einem Projekt finden Sie unter <a href="../../../manage-work/projects/manage-projects/understand-project-overview-area.md" class="MCXref xref">Verwalten von Informationen im Bereich "Projektübersicht"</a>.</p> </li> 
     <li> <p>Außerdem müssen Sie über Berechtigungen zum Bearbeiten des Projekts verfügen, entweder weil Sie es erstellt haben oder es für Sie freigegeben wurde.</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </li> 
    </ul> <p><b>HINWEIS</b>: Wenn Sie ein Projekt auf der Seite einer Gruppe erstellen, weist das System das Projekt dieser Gruppe zu. Dies unterscheidet sich vom Erstellen eines Projekts in anderen Workfront-Bereichen, in denen das Projekt der Startseite des Benutzers zugeordnet wird, der es erstellt hat (dem Projekteigentümer).</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, wenn Sie herausfinden möchten, welchen Plan oder welchen Lizenztyp Sie haben.

+++

## Projekte für Ihre Gruppe über den Bereich &quot;Gruppen&quot;anzeigen, bearbeiten und erstellen

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** ![](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe, für die Sie Projekte erstellen, anzeigen oder bearbeiten möchten.
1. Klicken Sie im linken Bereich auf **Projekte** ![](assets/projects-in-main-menu.png) , um eine Liste der mit der Gruppe verknüpften Projekte anzuzeigen.

1. Führen Sie einen der folgenden Schritte aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Arbeiten mit einem Projekt</p> </td> 
      <td> <p>Wählen Sie das Projekt aus und verwenden Sie dann die Symbolleistenschaltflächen, um <img src="assets/edit-icon.png"> zu bearbeiten, <img src="assets/share-icon.png"> freizugeben oder es zu löschen <img src="assets/delete.png">.</p> <p>Weitere Informationen zu diesen Aktivitäten finden Sie unter <a href="../../../manage-work/projects/manage-projects/manage-projects-overview.md" class="MCXref xref">Projekte verwalten: Artikelindex</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Neues Projekt für die Gruppe erstellen</p> </td> 
      <td> 
       <ol> 
        <li value="1"> <p>Klicken Sie auf <strong>Neues Projekt</strong> und wählen Sie dann eine Option im Dropdown-Menü aus, um anzugeben, wie Sie es erstellen möchten. </p> <p>Weitere Informationen finden Sie im Abschnitt <a href="../../../manage-work/projects/create-projects/create-project.md#ways-to-create-projects" class="MCXref xref">Möglichkeiten zum Erstellen von Projekten</a> im Artikel <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Erstellen eines Projekts</a>.</p> </li> 
        <li value="2">Geben Sie einen Namen für das Projekt ein und konfigurieren Sie es wie unter <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Projekte bearbeiten</a> beschrieben.</li> 
       </ol> <p> Die für die Gruppe festgelegten Projektvoreinstellungen wirken sich auf alle Projekte aus, die Sie im Bereich "Gruppen"erstellen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md" class="MCXref xref">Konfigurieren von Projekteigenschaften für eine Gruppe</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Projektliste exportieren</td> 
      <td>Klicken Sie in der Symbolleiste oberhalb der Liste auf das Symbol Exportieren <img src="assets/export.png"> .</td> 
     </tr> 
    </tbody> 
   </table>
