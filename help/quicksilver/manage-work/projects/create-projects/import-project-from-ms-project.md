---
product-area: projects
navigation-topic: create-projects
title: Importieren eines Projekts aus einem Microsoft-Projekt
description: Sie können Projekte aus Microsoft Project in Adobe Workfront importieren und alle Ihre Projekte in einer Anwendung verwalten. Jedes Mal, wenn Sie ein Projekt aus einem Microsoft-Projekt importieren, wird in Workfront ein neues Projekt erstellt.
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 1%

---

# Importieren eines Projekts aus einem Microsoft-Projekt

Sie können Projekte aus Microsoft Project in Adobe Workfront importieren und alle Ihre Projekte in einer Anwendung verwalten. Jedes Mal, wenn Sie ein Projekt aus einem Microsoft-Projekt importieren, wird in Workfront ein neues Projekt erstellt.

>[!IMPORTANT]
>
>Nicht alle Microsoft-Projektfelder werden in Workfront übertragen.
>
>Weitere Informationen zur Kompatibilität von Feldern zwischen Workfront und Microsoft Project finden Sie unter [Zuordnen von Microsoft-Projektfeldern zu Adobe Workfront-Projekten](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

## Zugriffsanforderungen

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neue Lizenz: Standard </p> 
   Oder
   <p>Aktuelle Lizenz: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsstufe*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen zum Zugriff auf Projekte finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Projektzugriff gewähren</a>. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Beim Erstellen eines Projekts erhalten Sie automatisch Verwaltungsberechtigungen für das Projekt </p> <p> Weitere Informationen zu Projektberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Freigeben eines Projekts in Adobe Workfront</a>.</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

<!--old permissions model: 

You must have the following access to perform the steps in this article:

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
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

## Erstellen eines Projekts aus einem MS-Projekt

Sie können ein Projekt aus dem Bereich Projekte im Hauptmenü oder aus dem Bereich Projekte eines Portfolios oder eines Programms erstellen.

1. Wechseln Sie zu Microsoft Project und öffnen Sie ein Projekt, aus dem Sie in Workfront importieren möchten.
1. Klicks **Datei**, dann **Speichern unter** , um das Projekt als XML-Datei zu speichern.

1. Melden Sie sich bei Workfront an.
1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf **Hauptmenü** ![](assets/main-menu-icon.png)klicken **Projekte**, dann erweitern **Neues Projekt**.
   * Wechseln Sie zu einem Portfolio und erweitern Sie **Neues Projekt**.
   * Öffnen Sie ein Programm und erweitern Sie **Neues Projekt**.
   * Als Gruppenadministrator können Sie auch ein Projekt im Abschnitt &quot;Projekte&quot;einer von Ihnen verwalteten Gruppe erstellen. Weitere Informationen finden Sie unter [Erstellen und Ändern von Gruppenprojekten](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. Wählen Sie die **Importieren von MS-Projekten** -Option.

   ![](assets/new-project-dropdown-nwe-350x358.png)

1. Klicks **Datei auswählen** und suchen Sie dann auf Ihrem Computer nach der .xml-Datei, die Sie aus dem Microsoft-Projekt exportiert haben.
1. Importieren Sie die ausgewählte Datei.

   Workfront startet den Importvorgang und erstellt ein neues Projekt basierend auf der aus dem Microsoft-Projekt exportierten Datei.

   Nachdem der Importvorgang abgeschlossen ist, werden Sie zur neuen Projektseite geleitet, auf der eine Bestätigung angezeigt wird, dass der Import erfolgreich abgeschlossen wurde.

   >[!NOTE]
   >
   >Workfront hat eine 15-minütige Zeitbeschränkung für Datei-Uploads. Wenn der Datei-Upload länger dauert, wird empfohlen, Ihr Projekt in kleinere Projekte zu unterteilen und separat zu importieren. Verschieben Sie nach dem Import in Workfront die Aufgaben von einem Projekt in das andere, um sie in einem Projekt zu kombinieren. Informationen zum Verschieben von Aufgaben finden Sie unter [Aufgaben verschieben](../../../manage-work/tasks/manage-tasks/move-tasks.md).

1. (Optional) Fahren Sie mit der Bearbeitung des Projekts in Workfront fort. Weitere Informationen zum Bearbeiten von Projekten finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

   Der Status eines neuen Projekts, das anhand einer Vorlage erstellt wurde, entspricht dem Status, den der Workfront-Administrator im Bereich &quot;Projekteinstellungen&quot;oder ein Gruppenadministrator im Bereich &quot;Gruppenprojekteinstellungen&quot;definiert hat. Informationen zum Konfigurieren von Projektvoreinstellungen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
