---
product-area: projects
navigation-topic: manage-projects
title: Exportieren eines Projekts in ein Microsoft-Projekt
description: Sie können Adobe Workfront-Projekte in Microsoft Project exportieren.
author: Alina
feature: Work Management
exl-id: 3f0f3644-a763-4b72-a93a-85af8626b5b3
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---

# Exportieren eines Projekts in ein Microsoft-Projekt

Sie können Adobe Workfront-Projekte in Microsoft Project exportieren. 

>[!IMPORTANT]
>
>* Nicht alle Workfront-Felder werden in die Microsoft-Projektdatei übertragen.\
>  Weitere Informationen zur Kompatibilität von Feldern zwischen Workfront und Microsoft Project finden Sie im Artikel [Zuordnen von Microsoft-Projektfeldern zu Adobe Workfront-Projekten](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).
>* Es wird empfohlen, die Anzahl der Übertragungen von Projekten von einer Anwendung auf eine andere zu begrenzen. 
>

## Zugriffsanforderungen

<!--drafted for P&P:

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
   <td>  <p>Current license: Light or higher</p>
   Or
   <p>Legacy license: Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> View or higher permissions to the project</p> <p>For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte anzeigen oder höher</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen zum Zugriff auf Projekte finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Zugriff auf Projekte gewähren</a>. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p> Anzeigen von oder höheren Berechtigungen für das Projekt</p> <p>Informationen zu Projektberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Freigeben eines Projekts in Adobe Workfront</a>.</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Exportieren eines Projekts aus Workfront in das Microsoft-Projekt

Sie können ein Projekt aus Workfront über die Projektseite oder aus einer Projektliste oder einem Bericht exportieren.

1. Gehen Sie zu dem Projekt, das Sie exportieren möchten, und klicken Sie auf das **Mehr**-Symbol ![Mehr ](assets/qs-more-menu.png) rechts neben dem Projektnamen

   ![Dropdown „Mehr“](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Oder

   Gehen Sie zu einer Projektliste oder einem Bericht und wählen Sie ein Projekt aus, und klicken Sie dann oben in der Liste ![ das Symbol Mehr ](assets/qs-more-menu.png)Mehr Menü).

   ![Mehr Menü erweitert](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. Klicken Sie **MS Project exportieren**.

   Das Projekt wird als XML-Datei auf Ihren Computer heruntergeladen und kann in Microsoft Project importiert werden. 
