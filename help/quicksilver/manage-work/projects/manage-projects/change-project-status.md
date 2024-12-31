---
product-area: projects
navigation-topic: manage-projects
title: Ändern des Status eines Projekts
description: Sie können den Status eines Projekts bei Bedarf manuell in einen anderen Status ändern. Sie können den Status eines Projekts manuell in einen Status ändern, der nur dann Abgeschlossen entspricht, wenn der Fertigstellungsmodus des Projekts auf Manuell festgelegt ist.
author: Alina
feature: Work Management
exl-id: 80098514-fd44-436d-836b-bd9c1b52b3a9
source-git-commit: 7363e86f5c507e40955e16843c6776777c7ad823
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Ändern des Status eines Projekts

<!--Audited: 02/2024-->

Sie können den Status eines Projekts bei Bedarf manuell in einen anderen Status ändern.

Sie können den Status eines Projekts manuell in einen Status ändern, der nur dann Abgeschlossen entspricht, wenn der Fertigstellungsmodus des Projekts auf Manuell festgelegt ist.

Andernfalls markiert Adobe Workfront das Projekt automatisch als abgeschlossen, wenn alle Aufgaben und Probleme des Projekts abgeschlossen und genehmigt sind.

Weitere Informationen zum Fertigstellungsmodus des Projekts finden Sie unter [Projekte bearbeiten](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neu: Standard </p> 
   Oder
   <p>Aktuell: Plan </p>
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

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen. Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Überlegungen zur Aktualisierung auf bestimmte Status

* **Beim Aktualisieren eines Projekts auf „Abgeschlossen“** Stellen Sie sicher, dass alle Aufgaben und Probleme im Projekt abgeschlossen sind. Sie können nicht den Status Abgeschlossen für ein Projekt oder einen anderen Status auswählen, der Abgeschlossen entspricht, wenn es Aufgaben oder Probleme gibt, die im Projekt nicht abgeschlossen wurden. Dazu gehört die Genehmigung von Aufgaben oder Problemen, die den Status „Ausstehende Genehmigung abschließen“ aufweisen.
* **Beim Aktualisieren eines Projekts von „Abgeschlossen“ auf „Aktuell“:** Wenn alle Aufgaben und Probleme im Projekt abgeschlossen sind, stellen Sie sicher, dass der Abschlussmodus des Projekts auf „Manuell“ festgelegt ist. Wenn der Fertigstellungsmodus des Projekts auf Automatisch festgelegt ist, bleibt der Status des Projekts „Abgeschlossen“.

## Projektstatus ändern

1. Wechseln Sie zu dem Projekt, dessen Status Sie aktualisieren möchten.
1. Klicken Sie in der Projekt-Kopfzeile im Feld **Status** auf den Namen des Status und wählen Sie dann einen neuen Status aus.

   ![](assets/change-project-status-in-header-drop-down-nwe-350x371.png)

   Oder

   Klicken Sie auf den **Mehr**-![](assets/qs-more-menu.png) neben dem Namen des Projekts, klicken Sie auf **Bearbeiten** und wählen Sie einen neuen Status im Feld **Status** aus. Klicken Sie dann auf **Speichern**.

   Der Projektstatus wird auf den ausgewählten Status aktualisiert.
