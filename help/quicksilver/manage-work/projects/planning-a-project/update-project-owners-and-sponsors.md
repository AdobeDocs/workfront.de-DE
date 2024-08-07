---
product-area: projects
navigation-topic: plan-a-project
title: Projekteigentümer und -sponsoren aktualisieren
description: Wenn Sie ein Projekt in Adobe Workfront erstellen, werden Sie automatisch als Projekteigentümer des Projekts festgelegt. Sie können dieses Feld mit einem anderen Benutzer aktualisieren. Sie können auch das Feld Projektsponsor eines Projekts aktualisieren.
author: Alina
feature: Work Management
exl-id: 10421cab-237a-49a5-bb5b-5be510dc4c46
source-git-commit: 49bd393af77a67aa1e3a443c4189569178e99ada
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---


# Projekteigentümer und -sponsoren aktualisieren

<!--Audited: 07/2024-->

Wenn Sie ein Projekt in Adobe Workfront erstellen, werden Sie automatisch als Projekteigentümer des Projekts festgelegt. Sie können dieses Feld mit einem anderen Benutzer aktualisieren. Sie können auch das Feld Projektsponsor eines Projekts aktualisieren.

Weitere Informationen zu Projekteigentümern und Sponsoren finden Sie unter [Überblick über Projekteigentümer und Sponsoren](../../../manage-work/projects/planning-a-project/project-owners-and-sponsors.md).

>[!TIP]
>
>Sie können einen Inhaber und einen Sponsor für eine Vorlage identifizieren. Wenn Sie ein Projekt aus dieser Vorlage erstellen, wird der Vorlageninhaber zum Projekteigentümer und der Vorlagen-Sponsor zum Projektsponsor.
>
>Wenn die Vorlage keinen Eigentümer hat, wird der Benutzer, der das Projekt aus der Vorlage erstellt, zum Projektinhaber.
>
>Weitere Informationen zum Bearbeiten von Vorlagen finden Sie unter [Bearbeiten von Projektvorlagen](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

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

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td><p>Neu: Standard</p> 
   <p>Aktuell: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für ein Projekt bearbeiten</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aktualisieren des Projekteigentümers eines Projekts

Wenn Sie einen Benutzer als Projekteigentümer eines Projekts hinzufügen, gewährt Workfront ihm automatisch Berechtigungen zum Anzeigen des Projekts.

1. Wechseln Sie zu dem Projekt, das Sie aktualisieren möchten.
1. Klicken Sie im linken Bereich auf **Projektdetails** .
1. Klicken Sie oben rechts im Bereich &quot;Projektdetails&quot;auf das Symbol **Bearbeiten** ![](assets/qs-edit-icon.png) und klicken Sie dann auf **Überblick**.

1. Geben Sie den Namen eines Benutzers für das Feld **Projekteigentümer** an.

   Nur aktive Benutzer können als Projekteigentümer angegeben werden.

1. Klicken Sie auf **Änderungen speichern**.

   Der Projekteigentümer wird im Projektheader und im Bereich Projektdetails aktualisiert.

   ![](assets/project-stakeholders-owner-highlighted-nwe-350x149.png)

## Aktualisieren des Projektsponsors eines Projekts

Wenn Sie einen Benutzer als Projektsponsor eines Projekts hinzufügen, gewährt Workfront ihm automatisch die Berechtigung zum Anzeigen des Projekts.

>[!TIP]
>
>Wenn der Benutzer, den Sie als Projekt-Sponsor hinzufügen, ein Systemadministrator ist, wird er nicht zur Freigabeliste des Projekts hinzugefügt.

1. Wechseln Sie zu dem Projekt, das Sie aktualisieren möchten.
1. Klicken Sie im linken Bereich auf **Projektdetails** .
1. Klicken Sie oben rechts im Bereich &quot;Projektdetails&quot;auf das Symbol **Bearbeiten** ![](assets/qs-edit-icon.png) und klicken Sie dann auf **Überblick**.

1. Geben Sie den Namen eines Benutzers für das Feld **Projektsponsor** an.

   Als Projektsponsoren können nur aktive Benutzer angegeben werden.

1. Klicken Sie auf **Änderungen speichern**.

   Der Projektsponsor aktualisiert den Bereich Projektdetails .

   ![](assets/project-stakeholders-sponsor-highlighted-nwe-350x147.png)
