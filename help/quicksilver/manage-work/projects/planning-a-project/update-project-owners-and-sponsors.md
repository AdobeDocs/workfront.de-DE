---
product-area: projects
navigation-topic: plan-a-project
title: Projektbesitzer und Sponsoren aktualisieren
description: Wenn Sie ein Projekt in Adobe Workfront erstellen, werden Sie automatisch als Projektbesitzer des Projekts festgelegt. Sie können dieses Feld mit einem anderen Benutzer aktualisieren. Sie können auch das Feld Projektsponsor eines Projekts aktualisieren.
author: Alina
feature: Work Management
exl-id: 10421cab-237a-49a5-bb5b-5be510dc4c46
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---


# Projektbesitzer und Sponsoren aktualisieren

<!--Audited: 07/2024-->

Wenn Sie ein Projekt in Adobe Workfront erstellen, werden Sie automatisch als Projektbesitzer des Projekts festgelegt. Sie können dieses Feld mit einem anderen Benutzer aktualisieren. Sie können auch das Feld Projektsponsor eines Projekts aktualisieren.

Informationen zu Projektbesitzern und Sponsoren finden Sie unter [Übersicht über Projektbesitzer und Sponsoren](../../../manage-work/projects/planning-a-project/project-owners-and-sponsors.md).

>[!TIP]
>
>Sie können einen Eigentümer und einen Sponsor für eine Vorlage identifizieren. Wenn Sie ein Projekt aus dieser Vorlage erstellen, wird der Vorlagenbesitzer zum Projektbesitzer und der Vorlagensponsor zum Projektsponsor.
>
>Wenn die Vorlage keinen Eigentümer hat, wird der Benutzer, der das Projekt aus der Vorlage erstellt, zum Projektbesitzer.
>
>Informationen zum Bearbeiten von Vorlagen finden Sie unter [Projektvorlagen bearbeiten](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Zugriffsanforderungen

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> <p>  </p> </td> 
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
   <td> <p>Edit permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td><p>Neu: Standard</p> 
   <p>Aktuell: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Bearbeiten von Berechtigungen für ein Projekt</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aktualisieren des Projektbesitzers eines Projekts

Wenn Sie einen Benutzer als Projektbesitzer eines Projekts hinzufügen, erteilt Workfront ihm automatisch die Berechtigungen zum Anzeigen des Projekts.

1. Wechseln Sie zu dem Projekt, das Sie aktualisieren möchten.
1. Klicken Sie **linken** auf „Projektdetails“.
1. Klicken Sie auf **Bearbeiten**-Symbol ![Bearbeiten](assets/qs-edit-icon.png) in der oberen rechten Ecke des Bereichs Projektdetails und dann auf **Übersicht**.

1. Geben Sie den Namen eines Benutzers für das Feld **Projektbesitzer** an.

   Nur aktive Benutzer können als Projektbesitzer angegeben werden.

1. Klicken Sie **Änderungen speichern**.

   Der Projektbesitzer wird im Projekt-Header und im Bereich Projektdetails aktualisiert.

   ![](assets/project-stakeholders-owner-highlighted-nwe-350x149.png)

## Aktualisieren des Projektsponsors eines Projekts

Wenn Sie einen Benutzer als Projektsponsor eines Projekts hinzufügen, erteilt Workfront ihm automatisch die Berechtigungen zum Anzeigen des Projekts.

>[!TIP]
>
>Wenn der Benutzer, den Sie als Projektsponsor hinzufügen, Systemadministrator ist, wird er nicht zur Freigabeliste des Projekts hinzugefügt.

1. Wechseln Sie zu dem Projekt, das Sie aktualisieren möchten.
1. Klicken Sie **linken** auf „Projektdetails“.
1. Klicken Sie auf **Bearbeiten**-Symbol ![Bearbeiten](assets/qs-edit-icon.png) in der oberen rechten Ecke des Bereichs Projektdetails und dann auf **Übersicht**.

1. Geben Sie den Namen eines Benutzers für das Feld **Projektsponsor** an.

   Nur aktive Benutzer können als Projektsponsoren angegeben werden.

1. Klicken Sie **Änderungen speichern**.

   Der Projektsponsor aktualisiert sich im Bereich Projektdetails .

   ![](assets/project-stakeholders-sponsor-highlighted-nwe-350x147.png)
