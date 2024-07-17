---
product-area: templates
navigation-topic: templates-navigation-topic
title: Projektvorlagen freigeben
description: Sie können eine Vorlage für Benutzer freigeben oder festlegen, wie die aus einer Vorlage erstellten Projekte für Benutzer freigegeben werden, indem Sie die folgenden Freigabeoptionen auf Vorlagenebene verwenden.
author: Alina
feature: Work Management
exl-id: 99c6b241-a2c9-4b6c-b605-177bbbc3f21a
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '780'
ht-degree: 2%

---

# Projektvorlagen freigeben

Sie können eine Vorlage für Benutzer freigeben oder festlegen, wie die aus einer Vorlage erstellten Projekte für Benutzer freigegeben werden, indem Sie die folgenden Freigabeoptionen auf Vorlagenebene verwenden.

Beim Freigeben eines Objekts in Adobe Workfront können andere Benutzer dieses Objekt anzeigen, dazu beitragen oder bearbeiten.

Weitere Informationen zu Workfront-Berechtigungen finden Sie unter [Überblick über die Freigabe von Berechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Informationen zu den Berechtigungen, die Sie Benutzern beim Freigeben einer Vorlage gewähren können, finden Sie unter [Freigeben einer Vorlage](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Vorlagen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für eine Vorlage verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Vorlage freigeben {#share-a-template}

Sie können Ihre Vorlagen mithilfe der Vorlagenfreigabe für andere Benutzer freigeben. Diese Aktion definiert, wer über Berechtigungen für die Vorlage verfügt.

>[!NOTE]
>
>Wenn Sie einen aktiven Benutzer als Vorlageneigentümer festlegen, erhält dieser Benutzer automatisch Verwaltungsberechtigungen für die Vorlage. Weitere Informationen zum Benennen einer Person als Vorlageninhaber finden Sie unter [Bearbeiten von Projektvorlagen](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

So geben Sie eine Vorlage frei:

1. Klicken Sie im Symbol **Hauptmenü** auf ![](assets/main-menu-icon.png) auf **Vorlagen**.

1. Führen Sie einen der folgenden Schritte aus:\
   Klicken Sie auf den Namen einer Vorlage, um sie zu öffnen, und klicken Sie dann auf das Menü **Mehr** ![](assets/qs-more-icon-on-an-object.png) und dann auf **Vorlagenfreigabe**.

   Oder

   Wählen Sie eine Vorlage aus der Liste aus, klicken Sie auf das Freigabesymbol ![](assets/share-icon.png) und dann auf **Vorlage**.

   >[!TIP]
   >
   >Sie können ein Objekt nur für aktive Benutzer, Teams, Rollen oder Unternehmen freigeben.

1. Wählen Sie im Feld **Vorlagenzugriff** die Personen, Teams, Rollen, Gruppen oder Unternehmen aus, für die Sie die Vorlage freigeben möchten.

   Sie können auch auf das Symbol **Optionen** klicken, um die Vorlage systemweit verfügbar zu machen:

1. Wählen Sie aus dem Dropdown-Menü für jede Entität, für die Sie eine Freigabe durchführen, eine der folgenden Optionen aus:

   * **Anzeigen**: Benutzer mit diesen Berechtigungen können die Vorlage anzeigen und ein Projekt mit ihr erstellen oder sie an ein vorhandenes Projekt anhängen.

     >[!TIP]
     >
     >Ihr Workfront-Administrator muss der Bearbeitung von Projekten Zugriff gewähren, damit Sie Projekte erstellen können.

   * **Verwalten**: Benutzer mit diesen Berechtigungen können die Vorlage bearbeiten oder löschen.

     Informationen zu den hier verfügbaren erweiterten Einstellungen ![](assets/gear-icon-in-access-levels.png) finden Sie im Abschnitt [Erweiterte Einstellungen für die Vorlagenfreigabe](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md#template-permissions) im Artikel [Vorlagenfreigabe](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. Klicken Sie auf **Speichern**.

## Freigeben eines Projekts aus einer Vorlage {#share-a-project-from-a-template}

Mit der Vorlagenfreigabe für Projekte können Sie festlegen, wer auf Vorlagenebene für die in der Vorlage erstellten Projekte berechtigt ist.

So geben Sie zukünftige, aus einer Vorlage erstellte Projekte für Benutzer frei:

1. Führen Sie einen der folgenden Schritte aus:\
   Klicken Sie auf den Namen einer Vorlage, um sie zu öffnen, und klicken Sie dann auf das Menü **Mehr** ![](assets/qs-more-icon-on-an-object.png) und dann auf **Vorlagenfreigabe**.

   ![Projekt aus Vorlage freigeben](assets/project-sharing-on-template-nwe-2022-350x172.png)

   Oder

   Wählen Sie eine Vorlage aus der Liste aus, klicken Sie auf **Freigabe** und dann auf **Projekt**.

1. Wählen Sie im Feld **Projektzugriff** die Personen, Teams, Rollen, Gruppen oder Unternehmen aus, für die die Vorlage freigegeben ist.

   >[!TIP]
   >
   >Sie können ein Objekt nur für aktive Benutzer, Teams, Rollen oder Unternehmen freigeben.

1. Wählen Sie aus dem Dropdown-Menü für jede Entität eine der folgenden Optionen aus:

   * **Kein Zugriff**: Sie können angeben, welche Benutzer keinen Zugriff auf die Vorlage haben sollen.\
     Diese Option ist nur verfügbar, wenn Projekte für die Massenweitergabe aus Vorlagen ausgewählt werden. 
   * **Anzeigen**: Benutzer mit diesen Berechtigungen können Projekte anzeigen, die aus der Vorlage erstellt wurden.
   * **Contribute**: Benutzer mit diesen Berechtigungen können zu Projekten beitragen, die aus der Vorlage erstellt wurden 
   * **Verwalten**: Benutzer mit diesen Berechtigungen können Projekte verwalten oder löschen, die aus dieser Vorlage erstellt wurden.

1. (Optional) Klicken Sie auf das Symbol **Optionen** , um die Projekte systemweit verfügbar zu machen.
1. Klicken Sie auf **Speichern**.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Overview of project sharing from other sources</h3>
<p>You may already have been assigned access to projects from other areas of Workfront. <br>You may have been assigned access to projects from the following areas: </p>
<ul>
<li>When a project is created<br>For more information about sharing projects when the project is created, see the "Access" section in <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
<li>When your Workfront administrator sets user access levels<br>For more information about setting access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</li>
<li>When using the project access template</li>
</ul>
<p>When using the Template Project Sharing feature, if a user's access to a project is View, but you set the access permissions for Template Project Sharing to Manage, the user will have Manage permission for every project created using this specific template. The user will only have View permission for the other projects they are on.</p>
</div>
-->

## Vorlagen und Projekte aus Vorlagen stapelweise freigeben

Sie können mehrere Vorlagen sowie Projekte aus mehreren Vorlagen gleichzeitig freigeben.

>[!NOTE]
>
>Wenn Sie mehrere Vorlagen auswählen, können Sie nicht anzeigen, wer bereits über Berechtigungen für die einzelnen Vorlagen verfügt.

1. Gehen Sie zu einer Liste von Vorlagen.
1. Wählen Sie mehrere Vorlagen aus und klicken Sie dann auf ![Freigeben](assets/share-icon.png).

   ![Vorlagen oder Projekte stapelweise freigeben](assets/share-templates-projects-in-bulk-link-in-toolbar-nwe-2022.png)

   >[!TIP]
   >
   >Sie können ein Objekt nur für aktive Benutzer, Teams, Rollen oder Unternehmen freigeben.

1. Klicken Sie auf **Vorlage** , um die ausgewählten Vorlagen freizugeben.

   Oder

   Klicken Sie auf **Projekt** , um die Projekte freizugeben, die aus den ausgewählten Vorlagen erstellt werden.

1. Fahren Sie mit der Freigabe der Vorlagen oder Projekte fort, wie in den folgenden Abschnitten in diesem Artikel beschrieben:

   * [Vorlage freigeben](#share-a-template)
   * [Freigeben eines Projekts aus einer Vorlage](#share-a-project-from-a-template)
