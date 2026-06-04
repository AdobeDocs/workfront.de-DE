---
product-area: projects
navigation-topic: update-work-in-a-project
title: Anwenden von Status auf Arbeiten, die einer Gruppe zugeordnet sind
description: Wenn ein Projekt mit einer Gruppe verknüpft ist, können Sie sowohl den Status auf Systemebene als auch einen benutzerdefinierten Status, der mit dieser Gruppe verknüpft ist, auf das Projekt, die Aufgabe oder die Probleme in diesem Projekt anwenden.
author: Alina
feature: Work Management
exl-id: 7564ab6a-8ddf-4e76-8e45-d59f9cf8d38b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/D6IbseeEu-prRZcdJNLvHvW-wSaclUAreufre9Fkyjo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 309
ht-degree: 14%

---

# Anwenden von Status auf Arbeit, die einer Gruppe zugeordnet ist

<!--
Alina, I moved this out of an admin article about statuses (Create and customize statuses)
-->

Wenn ein Projekt mit einer Gruppe verknüpft ist, können Sie sowohl den Status auf Systemebene als auch einen benutzerdefinierten Status, der mit dieser Gruppe verknüpft ist, auf das Projekt bzw. auf die Aufgaben und Probleme in diesem Projekt anwenden. Informationen zum Gruppenstatus in Adobe Workfront finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

>[!TIP]
>
>Sie können nur Projekte mit Gruppen verknüpfen. Probleme und Aufgaben übernehmen die Gruppe aus dem Projekt, dem sie angehören.

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
   <p>Abo</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für das Projekt</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:
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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Projektgruppe und -status aktualisieren

Wenn Sie die Gruppe für ein Projekt aktualisieren, ändern sich die verfügbaren Optionen für den Status von Aufgaben, Problemen oder das Projekt, sodass sie mit der Gruppe übereinstimmen.

1. Gehen Sie zu einem Projekt oder erstellen Sie ein neues Projekt, wie in [Erstellen eines Projekts](../../../manage-work/projects/create-projects/create-project.md) beschrieben.
1. Klicken Sie auf das **Mehr**-Symbol ![Mehr-Symbol](assets/more-icon.png) und dann auf **Bearbeiten**.

1. Wählen Sie in dem **Projekt bearbeiten** unten im Abschnitt **Übersicht** die Gruppe im Dropdownmenü **Gruppe** aus.

1. Wählen **im Dropdown** Menü „Status“ den benutzerdefinierten Status aus.

   >[!NOTE]
   >
   >Wenn Sie im Dropdown-Menü **Gruppe** eine andere Gruppe auswählen, ändern sich die benutzerdefinierten Status im Menü **Status** automatisch, um sie mit der neuen Gruppe zu korrelieren.
   >
   >
   >![Status-Dropdown mit benutzerdefinierten Status für das Projekt erweitert](assets/status-drop-down-expanded-with-custom-statuses-for-project-nwe.png)
   >

1. Wählen Sie den Status des Projekts aus. Die benutzerdefinierten Status, die Sie erstellt und auf diese Gruppe angewendet haben, werden in der Liste angezeigt.
