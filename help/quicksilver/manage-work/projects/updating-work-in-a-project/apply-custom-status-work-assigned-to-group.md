---
product-area: projects
navigation-topic: update-work-in-a-project
title: Anwenden von Status auf Arbeiten, die einer Gruppe zugeordnet sind
description: Wenn ein Projekt mit einer Gruppe verknüpft ist, können Sie sowohl den Status auf Systemebene als auch einen mit dieser Gruppe verknüpften benutzerdefinierten Status auf das Projekt, die Aufgabe oder Probleme in diesem Projekt anwenden.
author: Alina
feature: Work Management
exl-id: 7564ab6a-8ddf-4e76-8e45-d59f9cf8d38b
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---

# Anwenden von Status auf Arbeiten, die einer Gruppe zugeordnet sind

<!--
Alina, I moved this out of an admin article about statuses (Create and customize statuses)
-->

Wenn ein Projekt mit einer Gruppe verknüpft ist, können Sie sowohl den Status auf Systemebene als auch einen benutzerdefinierten Status, der mit dieser Gruppe verknüpft ist, auf das Projekt oder Aufgaben und Probleme in diesem Projekt anwenden. Informationen zum Gruppenstatus in Adobe Workfront finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

>[!TIP]
>
>Sie können nur Projekte mit Gruppen verknüpfen. Probleme und Aufgaben übernehmen die Gruppe von dem Projekt, zu dem sie gehören.

## Zugriffsanforderungen

<!--drafted for P&P:

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> 
   </td> 
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

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Projekt verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Aktualisieren der Projektgruppe und des Status

Wenn Sie die Gruppe für ein Projekt aktualisieren, ändern sich die für den Status der Aufgaben, Probleme oder das Projekt verfügbaren Optionen entsprechend der Gruppe.

1. Wechseln Sie zu einem Projekt oder erstellen Sie ein neues Projekt, wie unter [Projekt erstellen](../../../manage-work/projects/create-projects/create-project.md).
1. Klicken Sie auf **Mehr** icon ![](assets/more-icon.png)Klicken Sie auf **Bearbeiten**.

1. Im **Projekt bearbeiten** unten im **Übersicht** Wählen Sie die Gruppe im **Gruppe** Dropdown-Menü.

1. Im **Status** Dropdown-Menü den benutzerdefinierten Status aus.

   >[!NOTE]
   >
   >Wenn Sie eine andere Gruppe im **Gruppe** Dropdown-Menü die benutzerdefinierten Status im **Status** automatisch mit der neuen Gruppe korrelieren.
   >
   >
   >![](assets/status-drop-down-expanded-with-custom-statuses-for-project-nwe.png)   >

1. Wählen Sie den Status des Projekts aus. Die benutzerdefinierten Status, die Sie erstellt und auf diese Gruppe angewendet haben, werden in der Liste angezeigt.
