---
product-area: projects
navigation-topic: plan-a-project
title: Projektbesitzer und Sponsoren aktualisieren
description: Wenn Sie ein Projekt in Adobe Workfront erstellen, werden Sie automatisch als Projektbesitzer des Projekts festgelegt. Sie können dieses Feld mit einem anderen Benutzer aktualisieren. Sie können auch das Feld Projektsponsor eines Projekts aktualisieren.
author: Alina
feature: Work Management
exl-id: 10421cab-237a-49a5-bb5b-5be510dc4c46
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/YqTw5b0p4p605v7O0wVx99A7gLvJYF8xEPtthwW0CWc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 433
ht-degree: 9%

---

# Aktualisieren von Projektbesitzern bzw. -besitzerinnen und Sponsoren

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

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p> 
   <p>Abo</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Bearbeiten von Berechtigungen für ein Projekt</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>New: Standard</p> 
   <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Edit permissions to a project</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Aktualisieren des Projektbesitzers eines Projekts

Wenn Sie einen Benutzer als Projektbesitzer eines Projekts hinzufügen, erteilt Workfront ihm automatisch die Berechtigungen zum Anzeigen des Projekts.

1. Wechseln Sie zu dem Projekt, das Sie aktualisieren möchten.
1. Klicken Sie **linken** auf „Projektdetails“.
1. Klicken Sie auf **Bearbeiten**-Symbol ![Bearbeiten](assets/qs-edit-icon.png) in der oberen rechten Ecke des Bereichs Projektdetails und dann auf **Übersicht**.

1. Geben Sie den Namen eines Benutzers für das Feld **Projektbesitzer** an.

   Nur aktive Benutzer können als Projektbesitzer angegeben werden.

1. Klicken Sie **Änderungen speichern**.

   Der Projektbesitzer wird im Projekt-Header und im Bereich Projektdetails aktualisiert.

   ![Verantwortlicher für das Projekt hervorgehoben](assets/project-stakeholders-owner-highlighted-nwe-350x149.png)

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

   ![Projekt-Stakeholder-Sponsor hervorgehoben](assets/project-stakeholders-sponsor-highlighted-nwe-350x147.png)
