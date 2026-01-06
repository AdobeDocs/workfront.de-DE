---
product-area: projects
navigation-topic: manage-projects
title: Ändern des Status eines Projekts
description: Sie können den Status eines Projekts bei Bedarf manuell in einen anderen Status ändern. Sie können den Status eines Projekts manuell in einen Status ändern, der nur dann Abgeschlossen entspricht, wenn der Fertigstellungsmodus des Projekts auf Manuell festgelegt ist.
author: Alina
feature: Work Management
exl-id: 80098514-fd44-436d-836b-bd9c1b52b3a9
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 5%

---

# Ändern des Status eines Projekts

<!--Audited: 02/2024-->

Sie können den Status eines Projekts bei Bedarf manuell in einen anderen Status ändern.

Sie können den Status eines Projekts manuell in einen Status ändern, der nur dann Abgeschlossen entspricht, wenn der Fertigstellungsmodus des Projekts auf Manuell festgelegt ist.

Andernfalls markiert Adobe Workfront das Projekt automatisch als abgeschlossen, wenn alle Aufgaben und Probleme des Projekts abgeschlossen und genehmigt sind.

Weitere Informationen zum Fertigstellungsmodus des Projekts finden Sie unter [Projekte bearbeiten](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

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
   <p>Plan</p>
   </td> 
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


<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard </p> 
   Or
   <p>Current: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Überlegungen zur Aktualisierung auf bestimmte Status

* **Beim Aktualisieren eines Projekts auf „Abgeschlossen“** Stellen Sie sicher, dass alle Aufgaben und Probleme im Projekt abgeschlossen sind. Sie können nicht den Status Abgeschlossen für ein Projekt oder einen anderen Status auswählen, der Abgeschlossen entspricht, wenn es Aufgaben oder Probleme gibt, die im Projekt nicht abgeschlossen wurden. Dazu gehört die Genehmigung von Aufgaben oder Problemen, die den Status „Ausstehende Genehmigung abschließen“ aufweisen.
* **Beim Aktualisieren eines Projekts von „Abgeschlossen“ auf „Aktuell“:** Wenn alle Aufgaben und Probleme im Projekt abgeschlossen sind, stellen Sie sicher, dass der Abschlussmodus des Projekts auf „Manuell“ festgelegt ist. Wenn der Fertigstellungsmodus des Projekts auf Automatisch festgelegt ist, bleibt der Status des Projekts „Abgeschlossen“.

## Projektstatus ändern

1. Wechseln Sie zu dem Projekt, dessen Status Sie aktualisieren möchten.
1. Klicken Sie in der Projekt-Kopfzeile im Feld **Status** auf den Namen des Status und wählen Sie dann einen neuen Status aus.

   ![Projektstatus ändern](assets/change-project-status-in-header-drop-down-nwe-350x371.png)

   ODER

   Klicken Sie auf das **Mehr** Menü ![Mehr](assets/qs-more-menu.png) neben dem Namen des Projekts und klicken Sie auf **Bearbeiten** und wählen Sie einen neuen Status im Feld **Status** aus und klicken Sie dann auf **Speichern**.

   Der Projektstatus wird auf den ausgewählten Status aktualisiert.
