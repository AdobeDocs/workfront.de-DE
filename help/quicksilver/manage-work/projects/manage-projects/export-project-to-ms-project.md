---
product-area: projects
navigation-topic: manage-projects
title: Projekt in ein Microsoft-Projekt exportieren
description: Sie können Adobe Workfront-Projekte in Microsoft Project exportieren.
author: Alina
feature: Work Management
exl-id: 3f0f3644-a763-4b72-a93a-85af8626b5b3
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Projekt in ein Microsoft-Projekt exportieren

Sie können Adobe Workfront-Projekte in Microsoft Project exportieren. 

>[!IMPORTANT]
>
>* Nicht alle Workfront-Felder werden in die Microsoft-Projektdatei übertragen.\
>  Weitere Informationen zur Kompatibilität von Feldern zwischen Workfront und Microsoft Project finden Sie im Artikel [Zuordnen von Microsoft-Projektfeldern zu Adobe Workfront-Projekten](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).
>* Es wird empfohlen, die Anzahl der Projektübertragungen von einer Anwendung auf eine andere zu begrenzen. 
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
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Anzeigen oder höherer Zugriff auf Projekte</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen zum Zugriff auf Projekte finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Gewähren des Zugriffs auf Projekte</a>. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p> Anzeigen von oder höheren Berechtigungen für das Projekt</p> <p>Weitere Informationen zu Projektberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Freigeben eines Projekts in Adobe Workfront</a>.</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Projekt aus Workfront in Microsoft-Projekt exportieren

Sie können ein Projekt aus Workfront von der Projektseite oder von einer Projektliste oder einem Bericht exportieren.

1. Wechseln Sie zu dem Projekt, das Sie exportieren möchten, und klicken Sie auf das Symbol **Mehr** ![](assets/qs-more-menu.png) rechts neben dem Projektnamen

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Oder

   Wechseln Sie zu einer Projektliste oder einem Bericht und wählen Sie ein Projekt aus. Klicken Sie dann oben in der Liste auf das Symbol Mehr . ![](assets/qs-more-menu.png) .

   ![](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. Klicken Sie auf **MS-Projekt exportieren**.

   Das Projekt wird als XML-Datei auf Ihren Computer heruntergeladen und kann in das Microsoft-Projekt importiert werden. 
