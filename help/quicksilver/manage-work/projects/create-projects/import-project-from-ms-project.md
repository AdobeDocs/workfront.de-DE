---
product-area: projects
navigation-topic: create-projects
title: Importieren eines Projekts aus dem Microsoft-Projekt
description: Sie können Projekte aus Microsoft Project in Adobe Workfront importieren und alle Ihre Projekte in einer Anwendung verwalten. Jedes Mal, wenn Sie ein Projekt aus Microsoft Project importieren, wird in Workfront ein neues Projekt erstellt.
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 1%

---

# Importieren eines Projekts aus dem Microsoft-Projekt

<!-- Audited: 10/2025 -->

Sie können Projekte aus Microsoft Project in Adobe Workfront importieren und alle Ihre Projekte in einer Anwendung verwalten. Jedes Mal, wenn Sie ein Projekt aus Microsoft Project importieren, wird in Workfront ein neues Projekt erstellt.

>[!IMPORTANT]
>
>Nicht alle Microsoft Project-Felder werden an Workfront übertragen.
>
>Weitere Informationen zur Kompatibilität von Feldern zwischen Workfront und Microsoft Project finden Sie unter [Zuordnen von Microsoft-Projektfeldern zu Adobe Workfront-Projekten](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

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
    <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfiguration der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> 
   <p>Wenn Sie ein Projekt zu einem Portfolio oder einem Programm hinzufügen, benötigen Sie Bearbeitungszugriff auf Portfolios und Programme.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Wenn Sie ein Projekt erstellen, erhalten Sie automatisch Verwaltungsberechtigungen für das Projekt</p>
   <p>Wenn Sie ein Projekt zu einem Portfolio oder einem Programm hinzufügen, müssen Sie über Verwaltungsberechtigungen für das Portfolio und das Programm verfügen.</p>
   </td> 
    </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--old permissions model: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p> 
   Or
   <p>Current: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> </td> 
  </tr> 
 </tbody> 
</table>

-->

## Erstellen eines Projekts aus einem MS Project

Sie können ein Projekt im Bereich **Projekte** im **Hauptmenü** oder im Bereich **Projekte** eines Portfolios oder Programms erstellen.

1. Melden Sie sich beim Microsoft-Projekt an und öffnen Sie ein Projekt, aus dem Sie in Workfront importieren möchten.
1. Klicken Sie auf **Datei** und dann auf **Speichern unter**, um das Projekt als XML-Datei zu speichern.

1. Melden Sie sich bei Workfront an.
1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke oder auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront, falls verfügbar, klicken Sie dann auf **Projekte** und erweitern Sie **Neues Projekt**.
   * Gehen Sie zu einem Portfolio und erweitern Sie dann **Neues Projekt**.
   * Wechseln Sie zu einem Programm und erweitern Sie dann **Neues Projekt**.
   * Wenn Sie Gruppenadministrator sind, können Sie ein Projekt im Abschnitt **Projekte** einer Gruppe erstellen, die Sie verwalten. Weitere Informationen finden Sie unter [Erstellen und Ändern der Projekte einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. Klicken Sie **MS Project importieren**.

   ![Dropdown-Liste „Neues Projekt“](assets/import-ms-project-option.png)

   Das **MS-Datei importieren**-Feld wird geöffnet.

1. Klicken Sie **Datei auswählen** und suchen Sie auf Ihrem Computer nach der XML-Datei, die Sie aus Microsoft Project exportiert haben.
1. Importiert die ausgewählte Datei. Workfront beginnt den Importvorgang und erstellt ein neues Projekt basierend auf der aus Microsoft Project exportierten Datei.

   Nach Abschluss des Importvorgangs werden Sie zur Seite Neues Projekt weitergeleitet, auf der eine Bestätigung des erfolgreichen Imports angezeigt wird.

   >[!NOTE]
   >
   >Workfront unterliegt einer Zeitbeschränkung von 15 Minuten für Datei-Uploads. Wenn der Datei-Upload länger dauert, empfehlen wir, das Projekt in kleinere Projekte aufzuteilen und sie separat zu importieren. Nachdem sie in Workfront importiert wurden, verschieben Sie die Aufgaben von einem Projekt in das andere Projekt, um sie in einem Projekt zu kombinieren. Informationen zum Verschieben von Aufgaben finden Sie unter [Verschieben von Aufgaben](../../../manage-work/tasks/manage-tasks/move-tasks.md).

1. (Optional) Fahren Sie mit der Bearbeitung des Projekts in Workfront fort. Informationen zum Bearbeiten von Projekten finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).


   >[!NOTE]
   >
   >Der Status eines über eine Vorlage erstellten neuen Projekts entspricht dem Status, den Ihr Workfront-Administrator im Bereich **Projektvoreinstellungen** oder ein Gruppenadministrator im Bereich **Gruppenprojektvoreinstellungen** definiert hat. Informationen zum Konfigurieren von Projektvoreinstellungen finden Sie [Konfigurieren von systemweiten Projektvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
