---
product-area: projects
navigation-topic: manage-projects
title: Ändern des Status eines Projekts
description: Sie können den Status eines Projekts bei Bedarf manuell auf einen anderen Status aktualisieren. Sie können den Status eines Projekts nur dann manuell auf einen Status aktualisieren, der "Fertig stellen"entspricht, wenn für den Abschlussmodus des Projekts "Manuell"eingestellt ist.
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

Sie können den Status eines Projekts bei Bedarf manuell auf einen anderen Status aktualisieren.

Sie können den Status eines Projekts nur dann manuell auf einen Status aktualisieren, der &quot;Fertig stellen&quot;entspricht, wenn für den Abschlussmodus des Projekts &quot;Manuell&quot;eingestellt ist.

Andernfalls markiert Adobe Workfront das Projekt automatisch als abgeschlossen, wenn alle Aufgaben und Probleme des Projekts abgeschlossen und genehmigt sind.

Weitere Informationen zum Abschlussmodus des Projekts finden Sie unter [Projekte bearbeiten](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neu: Standard </p> 
   Oder
   <p>Aktuell: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Projekt verwalten</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben. Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Überlegungen zum Aktualisieren auf bestimmte Status

* **Beim Aktualisieren eines Projekts auf &quot;Abgeschlossen&quot;:** Stellen Sie sicher, dass alle Aufgaben und Probleme im Projekt abgeschlossen sind. Sie können den Status Fertig stellen für ein Projekt oder einen anderen Status, der Abgeschlossen entspricht, nicht auswählen, wenn Aufgaben oder Probleme im Projekt noch nicht abgeschlossen sind. Dazu gehört die Genehmigung von Aufgaben oder Problemen, die sich im Status &quot;Abgeschlossen - Ausstehende Genehmigung&quot;befinden.
* **Beim Aktualisieren eines Projekts von &quot;Fertig stellen&quot;auf &quot;Aktuell&quot;:** Wenn alle Aufgaben und Probleme im Projekt abgeschlossen sind, stellen Sie sicher, dass der Abschlussmodus des Projekts auf &quot;Manuell&quot;eingestellt ist. Wenn der Abschlussmodus des Projekts automatisch ist, bleibt der Status des Projekts Complete.

## Projektstatus ändern

1. Wechseln Sie zu dem Projekt, dessen Status Sie aktualisieren möchten.
1. Klicken Sie in der Projektheader auf den Namen des Status im Feld **Status** und wählen Sie dann einen neuen Status aus.

   ![](assets/change-project-status-in-header-drop-down-nwe-350x371.png)

   Oder

   Klicken Sie auf das Menü **Mehr** neben dem Namen des Projekts, klicken Sie auf **Bearbeiten** und wählen Sie einen neuen Status im Feld **Status** aus. Klicken Sie dann auf **Speichern**.![](assets/qs-more-menu.png)

   Der Projektstatus wird auf den von Ihnen ausgewählten Status aktualisiert.
