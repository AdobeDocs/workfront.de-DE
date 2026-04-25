---
product-area: documents
navigation-topic: organize-documents
title: Erstellen von Dokumentordnern
description: Dokumente können in Ordnern organisiert werden. Sie können persönliche Ordner in Ihrem Bereich für persönliche Dokumente erstellen.
author: Courtney
feature: Digital Content and Documents
exl-id: 41974d6b-fb00-49b7-9db2-36519994e0fd
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 6%

---

# Erstellen von Dokumentordnern

Dokumente können in Ordnern organisiert werden. Workfront verfügt derzeit über zwei Versionen des Dokumentbereichs: den alten Dokumentbereich und den neuen Dokumentbereich. Welche Version Ihr Unternehmen verwendet, hängt davon ab, ob sich Ihr Unternehmen auf ältere Workfront-Speicher oder Unternehmensspeicher stützt. Weitere Informationen zu diesen Speichertypen finden Sie unter [Übersicht über Adobe Enterprise-Speicher](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Jedes Workfront-Paket zum Verwalten von Dokumenten unter Verwendung des alten Workfront-Speichers</p>
<p>Beliebiges Workflow-Paket zum Verwalten von Dokumenten mit Adobe Enterprise Storage</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Mitwirkende oder höher</p>
   <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriffrecht „Bearbeiten“ für Dokumente</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen von Dokumentordnern im Bereich für veraltete Dokumente

Wenn sich Ihr Unternehmen im alten Workfront-Speicher befindet, wird der Bereich für ältere Dokumente angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Weitere Informationen zum alten Workfront-Speicher finden Sie unter [Unterschiede zwischen Adobe Enterprise-Speicher und Legacy-Workfront-Speicher](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-enterprise-storage-and-legacy-workfront-storage).

>[!NOTE]
>
>Beim Organisieren von Dokumenten werden einfach Verknüpfungen zwischen den Dokumenten und den Objekten erstellt, mit denen Sie sie verknüpfen. Sie werden nicht im System verschoben.

### Ordner anzeigen

Sie können Ordner in der Miniatur-, Standard- oder Listenansicht anzeigen. Um die Ansicht zu ändern, verwenden Sie die Ansichtsoptionen in der oberen rechten Ecke.

{{step1-to-documents}}

ODER

Klicken Sie bei geöffnetem Workfront **Objekt** linken Bereich auf Dokumente .

1. Klicken Sie auf die Anzeigeoptionen über dem rechten Bedienfeld, um zu ändern, wie die Dokumente angezeigt werden.

   ![Optionen für die Dokumentansicht](assets/screenshot-2016-07-07-12.46.54.png)

### Ordner und Unterordner erstellen

Erstellen von Ordnern zur besseren Organisation Ihrer Dokumente. Sie können bis zu 2.000 Ordner für ein Objekt und bis zu 50 Unterordner in jedem Ordner erstellen. Die Anzahl der Unterordner beläuft sich auf maximal 2.000 Ordner.

{{step1-to-documents}}

ODER

Klicken Sie bei geöffnetem Workfront **Objekt** linken Bereich auf Dokumente .

1. Um einen Ordner der obersten Ebene zu erstellen, stellen Sie sicher, dass nichts ausgewählt ist, und klicken Sie dann auf **Neu hinzufügen** > **Ordner**.

   ODER

   Um einen Unterordner zu erstellen, wählen Sie den Ordner aus, in dem Sie den Unterordner erstellen möchten, und klicken Sie dann auf **Neu hinzufügen** > **Ordner**.

### Freigeben von Ordnern

Informationen zum Freigeben von Ordnern finden Sie unter [Freigeben eines Dokumentordners](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Erstellen von Dokumentordnern im Bereich „Neue Dokumente“

Wenn Ihr Unternehmen Enterprise-Speicher verwendet, wird der Bereich „Neue Dokumente“ angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Weitere Informationen zu Massenspeicher für Unternehmen finden Sie unter [Übersicht über Speicher für Unternehmen in Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

### Systemgenerierte Ordner

Wenn Sie ein Dokument in eine Aufgabe oder ein Problem hochladen, erstellt Workfront automatisch einen systemgenerierten Ordner mit dem Namen nach der Aufgabe oder dem Problem. Dieser Ordner ist mit der Aufgabe oder dem Problem verknüpft und übernimmt die Berechtigungen. Systemgenerierte Ordner sind im Dokumentbereich auf Projektebene sichtbar.

Weitere Informationen zu Ordnerberechtigungen finden Sie unter [ von Dokumentberechtigungen](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

### Unterordner erstellen

Sie können in einem systemgenerierten Ordner Unterordner erstellen, um Dokumente weiter zu organisieren. Alle Unterordner erben Berechtigungen vom übergeordneten Ordner.

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen **Dokumente** im linken Bereich aus.
1. Klicken Sie auf den Ordner, in dem Sie einen Unterordner erstellen möchten, und klicken Sie dann auf das Symbol **Ordner hinzufügen** ![Ordner hinzufügen](assets/add-folder-icon.png).
   ![Unterordner hinzufügen](assets/add-subfolder.png)
1. Geben Sie einen Namen für den Unterordner ein und klicken Sie dann auf **Erstellen**.

### Umbenennen eines Ordners

Systemgenerierte Ordner übernehmen automatisch den Namen der Aufgabe oder des Problems. Sie können umbenannt werden, indem Sie auf den Ordnernamen klicken und ihn bearbeiten.

So benennen Sie einen Ordner um:

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen **Dokumente** im linken Bereich aus.
1. Find the folder you want to rename, then click the **More** ![more icon](assets/more-icon.png) icon.
1. Click **Rename**, then enter a new name for the folder.

   ![rename folder](assets/rename-folder.png)

1. Click **Rename**.

### Move a folder

System-generated folders can be moved to another project, task, or issue. If a system-generated folder is moved to another location, its linked object is updated to the new object and permissions are inherited from the new parent object. You can also move subfolders to another project, task, or issue.

>[!NOTE]
>
>Only projects, tasks, and issues using the same storage type are available in the move dialog. For example, if you&#39;re moving a folder in an enterprise storage project, only projects, tasks, and issues using enterprise storage are available to move to.


To move a folder:

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen **Dokumente** im linken Bereich aus.
1. Find the folder you want to move, then click the **More** ![more icon](assets/more-icon.png) icon.
1. Click **Move**, then select the project, task, or issue you want to move the folder to.


   ![move folder](assets/rename-folder.png)

<!-- STEPS PLACEHOLDER: Add steps for moving a folder in the new documents area -->

### Delete a folder

To delete a folder:

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen **Dokumente** im linken Bereich aus.
1. Find the folder you want to delete, then click the **More** ![more icon](assets/more-icon.png) icon.
1. Klicken Sie auf **Löschen**.

   ![delete folder](assets/rename-folder.png)
