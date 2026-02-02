---
product-area: projects
navigation-topic: manage-tasks
title: Zuordnen von Meilensteinen zu Aufgaben
description: Sie können Meilensteine mit Aufgaben verknüpfen, um anzugeben, wann Sie wichtige Schritte während der Lebensdauer des Projekts erreichen. Sie müssen einem Projekt einen Meilensteinpfad zuordnen, bevor Sie dem Projekt Meilensteine zuordnen können.
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 6%

---

# Zuordnen von Meilensteinen zu Aufgaben

<!--Audited: 01/2024-->

Sie können Meilensteine mit Aufgaben verknüpfen, um anzugeben, wann Sie wichtige Schritte während der Lebensdauer des Projekts erreichen.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p> 
   <p>Work oder höher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten der Berechtigungen für die Aufgabe</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New license: Standard</p> 
   <p>Current license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Voraussetzungen

Bevor Sie einen Meilenstein mit einer Aufgabe verknüpfen können, muss Folgendes vorhanden sein:

* Der Workfront-Administrator muss einen Meilensteinpfad erstellen, wie beschrieben in [Erstellen eines Meilensteinpfads](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* Sie müssen einem Projekt einen Meilensteinpfad zuordnen.

  Weitere Informationen finden Sie unter [Projekte bearbeiten](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

* Um einen Meilensteinpfad mit einem Projekt verknüpfen zu können, muss das Projekt den Status Planung oder Aktuell aufweisen.

  >[!TIP]
  >
  >Um mithilfe der Meilenstein -Ansicht den besten Überblick über den Fortschritt der Meilensteine in Ihren Projekten zu erhalten, sollten Sie übergeordnete Aufgaben erstellen und sie mit jeder Hauptphase Ihres Projekts verknüpfen. Ordnen Sie dann diese übergeordneten Aufgaben jedem der Meilensteine Ihres Meilensteinpfads zu.

## Meilenstein mit einer Aufgabe verknüpfen

Nachdem einem Projekt ein Meilensteinpfad zugeordnet wurde, können Aufgaben einem Meilenstein zugewiesen werden.

1. Wechseln Sie zu einer Aufgabe und klicken Sie dann auf das **Mehr**-Symbol ![Mehr](assets/more-icon.png) rechts neben dem Aufgabennamen und dann **Bearbeiten**.

   Aufgaben und Meilensteine haben eine 1:1-Beziehung. Sie können denselben Meilenstein nicht mehreren Aufgaben zuordnen. Jede Aufgabe kann mit einem einzelnen Meilenstein verknüpft werden oder jeder Meilenstein kann einer Aufgabe zugeordnet werden.

1. Klicken Sie **Einstellungen** und wählen Sie dann im Feld **Meilenstein** einen Meilenstein für die Aufgabe aus.
1. Klicken Sie auf **Speichern**.
1. (Optional) Fügen Sie einer Aufgabenliste die Spalte **Statussymbole“ hinzu** um festzustellen, welche Aufgaben Meilensteine aufweisen. Die Diamantanzeige Meilenstein wird in der Spalte Statussymbole angezeigt.

   Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten von Ansichten in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

   ![Statussymbole](assets/amwt3.png)

1. (Optional) Um zu einer Liste von Projekten zu wechseln, wählen Sie die Ansicht **Meilenstein**, um den Fortschritt Ihrer Meilensteinaufgaben zu ermitteln.

   ![Meilenstein-Ansicht - Projektliste](assets/milestone-view-project-list.png)
