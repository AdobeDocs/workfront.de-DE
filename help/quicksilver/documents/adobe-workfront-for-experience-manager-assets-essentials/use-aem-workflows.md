---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Verwenden von Workflows in der Integration von Experience Manager Assets Essentials
description: Verwenden von Workflows in der Integration von Experience Manager Assets Essentials
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4c1e5ec1-3fd1-4527-ba8a-9db1a2350f69
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '1023'
ht-degree: 7%

---

# Use workflows in the Experience Manager Assets integration

A workflow is a set of actions that connect Workfront to Adobe Experience Manager as a Cloud Service. A Workfront administrator can configure workflows in Workfront, then assign them to Project Templates.

When a Project is created using a Project Template to which a workflow is assigned, the actions defined in the workflow are triggered.

>[!NOTE]
>
>Workflows are available only in an Adobe Experience Manager as a Cloud Service integration. They are not available in integrations with Adobe Experience Manager Assets Essentials.<br>
>Diese Funktion ist im Bereich Neue Dokumente nicht verfügbar.


## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p> Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen</td> 
   <td> 
   <p>Mitwirkende oder höher</p> 
   <p>Anfragende oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zusätzliche Produkte</td> 
   <td>You must have Experience Manager as a Cloud Service or Assets Essentials, and you must be added to the product as a user in the Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager Permissions</td> 
    <td>You must have write access to the folder.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriffrecht „Bearbeiten“ für Dokumente</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>View access or higher</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie beginnen,

* Your Workfront administrator must configure workflows in an Adobe Experience Manager integration. For more information, see [Configure the Experience Manager Assets as a Cloud Service integration](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## Add a workflow to a template

You can add a workflow to a project template. The workflow will be applied to any projects created from the template.

1. Open a template by clicking **Templates** in the Main Menu, then selecting the template from the list.
1. Click **Experience Manager Assets** in the left navigation panel.

   >[!NOTE]
   >
   >If the Experience Manager Assets section is not visible in the left navigation, your Workfront administrator has not enabled workflows for your organization. <!--Is this right?-->

1. In the **Select an integration for automated workflows field**, select the integration with the workflows you want to use for projects created from this template.
1. (Optional) Edit any workflow values that you want to apply to projects created from this template.

   For instructions on specific workflows, see [Edit workflow values in a project](#edit-workflow-values-in-a-project) in this article.

   Only workflows that have been activated in the Experience Manager area of Setup are available in templates or projects.

1. Your changes save automatically. <!-- do they though??-->

## Add a workflow to a project

You can add a workflow when creating a project, or add a workflow to an existing project. In both cases, you will use a project template to add the workflow.

### Add a workflow when creating a project

1. Begin creating a project.

   For instructions, see [Create a project using a template](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. When selecting a template for the project, select the template that contains the workflows you want to use for this project.
1. (Optional) Edit any workflow values for the project, as described in [Edit workflow values in a project](#edit-workflow-values-in-a-project).

   Only workflows that have been activated in the Experience Manager area of Setup are available in templates or projects.


### Add a workflow to an existing project

>[!NOTE]
>
>Workflows that run when a project is created (such as linked folder creation) do not run when the template is attached to an existing project. They only run when a project is created from a template.

1. Begin adding a template to the project.

   For instructions, see [Attach a template to a project](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. When selecting a template for the project, select the template that contains the workflows you want to use for this project.
1. (Optional) Edit any workflow values for the project, as described in [Edit workflow values in a project](#edit-workflow-values-in-a-project).

   Only workflows that have been activated in the Experience Manager area of Setup are available in templates or projects.



### Edit workflow values in a project

You can edit workflow values on the project level. Project-level workflow values override values set on the project template, which override the default values set in the Adobe Experience Manager Assets integration.

All workflow values can be found in:

* The Workflows or Linked folders section of the Create project or Edit project window.
* The Adobe Experience Manager section of the left navigation.


  >[!NOTE]
  >
  >If these areas are not visible, your Workfront administrator has not enabled Workflows for your organization.



#### Verknüpfte Ordner

>[!NOTE]
>
>Because linked folders are created when the project is created, editing the linked folder workflow on an existing project is ineffective. Das Bearbeiten dieser Werte beim Erstellen eines Projekts funktioniert erwartungsgemäß.

So bearbeiten Sie den Workflow für verknüpfte Ordner:

1. Schalten Sie den **[!UICONTROL Verknüpften Ordner erstellen]** nach Bedarf ein oder aus. Wenn Sie sie aktivieren, können Sie die Konfiguration Verknüpfter Ordner bearbeiten.

   Weitere Informationen zur Konfiguration verknüpfter Ordner finden Sie unter [Erstellen verknüpfter Adobe Experience Manager-Ordner](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#create-adobe-experience-manager-linked-folders) im Artikel [Konfigurieren der [!UICONTROL Experience Manager Assets as a Cloud Service]-Integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

1. (Optional) Wenn die Ordnerstruktur nur erstellt werden soll, wenn bestimmte Werte in einem benutzerdefinierten Formular vorhanden sind, das an das Projekt angehängt ist, klicken Sie auf **Filter anwenden** für diese Ordnerstruktur und wählen Sie dann das benutzerdefinierte Formular aus, das das Feld, das Feld und den Feldwert enthält. Wenn das Feld im benutzerdefinierten Formular, das an das neue Projekt angehängt ist, den ausgewählten Wert enthält, wird die Ordnerstruktur erstellt.
1. (Optional) Bei der Konfiguration von Ordnernamen können Sie aus den folgenden Optionen auswählen:

   * **Name**: Geben Sie einen Namen für den Ordner ein.

   * **Objektdaten**: Wählen Sie die Quelle für den Ordnernamen aus, z. B. Projektnamen.

   * **Benutzerdefinierte Formulardaten**: Wählen Sie die benutzerdefinierten Formulardaten aus, die als Ordnername verwendet werden sollen.

     Die Verwendung benutzerdefinierter Formulardaten für Ordnernamen ist nur auf Vorlagenebene verfügbar und kann nicht auf Integrationsebene konfiguriert werden.

     Wenn ein Ordnername auf benutzerdefinierte Daten festgelegt ist, die im benutzerdefinierten für, das an das Projekt angehängt ist, nicht vorhanden sind, wird eine zufällige ID als Ordnername zugewiesen.

1. Um die Ordnerstruktur anzuzeigen, klicken Sie auf das Symbol **Vorschau** ![Vorschau](assets/preview-icon.png) .
1. Klicken Sie auf **[!UICONTROL Speichern]**.

#### Veröffentlichen von Assets

So bearbeiten Sie den Workflow zum Veröffentlichen von Assets:

1. Schalten Sie **Assets automatisch veröffentlichen** nach Bedarf ein oder aus.
1. (Bedingt) Wenn Sie die Veröffentlichung aktivieren, wählen Sie aus, ob Sie im Veröffentlichungs-Service, Brand Portal oder in beiden veröffentlichen möchten.
1. Klicken Sie auf **[!UICONTROL Speichern]**.
