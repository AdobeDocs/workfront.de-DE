---
user-type: administrator
product-area: system-administration;user-management
keywords: Gruppe,Projekte
navigation-topic: work-with-a-groups-objects
title: Erstellen und Ändern von Projekten einer Gruppe
description: Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie die Projekte der Gruppe erstellen, bearbeiten, exportieren, kopieren und löschen.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: db90cf52-7c8f-4972-b67f-401657ba9b13
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 1%

---

# Erstellen und Ändern von Projekten einer Gruppe

Wenn Sie eine Gruppe, die Sie im Bereich Gruppen verwalten, anzeigen, können Sie ihre Projekte wie folgt anzeigen und mit ihnen arbeiten:

* Erstellen eines neuen Projekts für die Gruppe
* Bearbeiten, Exportieren, Kopieren oder Löschen eines Projekts

Wenn es Gruppen oberhalb Ihrer Gruppe gibt, können deren Administratoren diese Dinge auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

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
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr>
  <tr> 
   <td>Objektberechtigungen</td>
   <td> 
    <ul> 
     <li> <p>Das Projekt muss mit der Gruppe oder einer ihrer Untergruppen verknüpft sein. </p> <p>Informationen zum Zuweisen einer Gruppe zu einem Projekt finden Sie unter <a href="../../../manage-work/projects/manage-projects/understand-project-overview-area.md" class="MCXref xref">Verwalten von Informationen im Projektübersichtsbereich</a>.</p> </li> 
     <li> <p>Außerdem müssen Sie über Berechtigungen zum Bearbeiten des Projekts verfügen, entweder weil Sie es erstellt haben oder weil es für Sie freigegeben wurde.</p></li> 
    </ul>
    <p><b>HINWEIS</b>: Wenn Sie ein Projekt auf der Seite einer Gruppe erstellen, weist das System das Projekt dieser Gruppe zu. Dies unterscheidet sich von der Erstellung eines Projekts in anderen Workfront-Bereichen, bei denen das System das Projekt der Hauptgruppe der Person zuweist, die es erstellt (der Projektbesitzerin bzw. dem Projektbesitzer).</p> </td>
  </tr>
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Im Bereich Gruppen können Sie Projekte für Ihre Gruppe anzeigen, damit arbeiten und erstellen

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** ![Gruppen](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe, für die Sie Projekte erstellen, anzeigen oder mit ihnen arbeiten möchten.
1. Klicken Sie im linken Bereich auf **Projekte** ![Projekte im Hauptmenü](assets/projects-in-main-menu.png) um eine Liste der mit der Gruppe verknüpften Projekte anzuzeigen.

1. Führen Sie einen der folgenden Schritte aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Arbeiten mit einem Projekt</p> </td> 
      <td> <p>Wählen Sie das Projekt aus und verwenden Sie dann die Schaltflächen der Symbolleiste, um <img src="assets/edit-icon.png"> zu bearbeiten, <img src="assets/share-icon.png"> freizugeben oder <img src="assets/delete.png"> zu löschen.</p> <p>Weitere Informationen zu diesen Aktivitäten finden Sie unter <a href="../../../manage-work/projects/manage-projects/manage-projects-overview.md" class="MCXref xref">Verwalten von Projekten: Artikelindex</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Erstellen eines neuen Projekts für die Gruppe</p> </td> 
      <td> 
       <ol> 
        <li value="1"> <p>Klicken Sie auf <strong>Neues Projekt</strong> und wählen Sie dann im Dropdown-Menü eine Option aus, um anzugeben, wie Sie es erstellen möchten. </p> <p>Weitere Informationen finden Sie im Abschnitt <a href="../../../manage-work/projects/create-projects/create-project.md#ways-to-create-projects" class="MCXref xref">Erstellen von Projekten</a> im Artikel <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Erstellen eines Projekts</a>.</p> </li> 
        <li value="2">Geben Sie einen Namen für das Projekt ein und konfigurieren Sie ihn, wie in <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Projekte bearbeiten</a> beschrieben.</li> 
       </ol> <p> Projektvoreinstellungen, die für die Gruppe festgelegt sind, wirken sich auf alle Projekte aus, die Sie im Bereich Gruppen erstellen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md" class="MCXref xref">Projektvoreinstellungen für eine Gruppe konfigurieren</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Liste der Projekte exportieren</td> 
      <td>Klicken Sie auf das Symbol Exportieren <img src="assets/export.png"> in der Symbolleiste oberhalb der Liste.</td> 
     </tr> 
    </tbody> 
   </table>
