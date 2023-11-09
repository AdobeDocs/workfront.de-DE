---
product-area: projects
navigation-topic: plan-a-project
title: Projekteigentümer und -sponsoren aktualisieren
description: Wenn Sie ein Projekt in Adobe Workfront erstellen, werden Sie automatisch als Projekteigentümer des Projekts festgelegt. Sie können dieses Feld mit einem anderen Benutzer aktualisieren. Sie können auch das Feld Projektsponsor eines Projekts aktualisieren.
author: Alina
feature: Work Management
exl-id: 10421cab-237a-49a5-bb5b-5be510dc4c46
source-git-commit: 4cdebe4890b775a097469e7d7035a38397b71094
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# Projekteigentümer und -sponsoren aktualisieren

Wenn Sie ein Projekt in Adobe Workfront erstellen, werden Sie automatisch als Projekteigentümer des Projekts festgelegt. Sie können dieses Feld mit einem anderen Benutzer aktualisieren. Sie können auch das Feld Projektsponsor eines Projekts aktualisieren.

Weitere Informationen zu Projekteigentümern und Sponsoren finden Sie unter [Übersicht über Projekteigentümer und Projektsponsoren](../../../manage-work/projects/planning-a-project/project-owners-and-sponsors.md).

>[!TIP]
>
>Sie können einen Inhaber und einen Sponsor für eine Vorlage identifizieren. Wenn Sie ein Projekt aus dieser Vorlage erstellen, wird der Vorlageninhaber zum Projekteigentümer und der Vorlagen-Sponsor zum Projektsponsor.
>
>Wenn die Vorlage keinen Eigentümer hat, wird der Benutzer, der das Projekt aus der Vorlage erstellt, zum Projektinhaber.
>
>Informationen zum Bearbeiten von Vorlagen finden Sie unter [Bearbeiten von Projektvorlagen](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

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

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> <p>  </p> </td> 
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
   <td> <p>Berechtigungen für ein Projekt bearbeiten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Aktualisieren des Projekteigentümers eines Projekts

Wenn Sie einen Benutzer als Projekteigentümer eines Projekts hinzufügen, gewährt Workfront ihm automatisch Berechtigungen zum Anzeigen des Projekts.

1. Wechseln Sie zu dem Projekt, das Sie aktualisieren möchten.
1. Klicks **Projektdetails** im linken Bereich.
1. Klicken Sie auf **Bearbeiten** icon ![](assets/qs-edit-icon.png) in der oberen rechten Ecke des Bereichs Projektdetails klicken Sie auf  **Übersicht**.

1. Geben Sie den Namen eines Benutzers für die **Projektinhaber** -Feld.

   Nur aktive Benutzer können als Projekteigentümer angegeben werden.

1. Klicks  **Änderungen speichern**.

   Der Projekteigentümer wird im Projektheader und im Bereich Projektdetails aktualisiert.

![](assets/project-stakeholders-owner-highlighted-nwe-350x149.png)

## Aktualisieren des Projektsponsors eines Projekts

Wenn Sie einen Benutzer als Projektsponsor eines Projekts hinzufügen, gewährt Workfront ihm automatisch die Berechtigung zum Anzeigen des Projekts.

>[!TIP]
>
>Wenn der Benutzer, den Sie als Projekt-Sponsor hinzufügen, ein Systemadministrator ist, wird er nicht zur Freigabeliste des Projekts hinzugefügt.

1. Wechseln Sie zu dem Projekt, das Sie aktualisieren möchten.
1. Klicks **Projektdetails** im linken Bereich.
1. Klicken Sie auf **Bearbeiten** icon ![](assets/qs-edit-icon.png) in der oberen rechten Ecke des Bereichs Projektdetails klicken Sie auf  **Übersicht**.

1. Geben Sie den Namen eines Benutzers für die **Projektsponsor** -Feld.

   Als Projektsponsoren können nur aktive Benutzer angegeben werden.

1. Klicks  **Änderungen speichern**.

   Der Projektsponsor aktualisiert den Bereich Projektdetails .

   ![](assets/project-stakeholders-sponsor-highlighted-nwe-350x147.png)
