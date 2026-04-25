---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Verknüpfen von Assets und Ordnern aus Experience Manager Assets Essentials
description: You can link an asset or folder from Experience Manager Assets Essentials to any Adobe Workfront object that supports documents. Assets sent from Assets Essentials don't count towards your overall document storage in Workfront. Documents uploaded and sent from Workfront to Assets Essentials do count towards overall storage.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 0b93f6f6-cf4b-4077-a464-be7f19f7cd25
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 12%

---

# Verknüpfen von Assets und Ordnern aus Experience Manager Assets Essentials

You can link an asset or folder from Experience Manager Assets Essentials to any Adobe Workfront object that supports documents.

To link assets and folders from Experience Manager Assets using Content Advisor, see [Link assets and folders with Content Advisor powered by Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem.md).

If you are on enterprise storage, see [Use the Adobe Experience Manager with the Frame.io integration](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).


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

Before you begin:

* Ihr Workfront-Administrator muss eine Experience Manager-Integration konfigurieren. For more information, see [Configure the Experience Manager Assets Essentials integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Link an asset from Experience Manager Assets Essentials

1. Go to the **Documents** area in Workfront where you want to add the document.
1. Select **Add New**, then select the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it may not specifically mention Experience Manager Assets Essentials.

1. Select the assets you want.

   ![Select an asset](assets/select-an-asset.png)

1. Klicken Sie auf **Auswählen**.

## Link a new version from Experience Manager Assets Essentials

You can pull a new asset over from Experience Manager Assets Essentials and add it to an existing asset as a new version. If the document is already linked and a new version is added in Experience Manager Assets Essentials, the new version appears automatically in Workfront.

To link a new version:

1. Go to the **Documents** area in Workfront where you want to add the document.
1. Select the asset you want to replace with a new version. You can&#39;t create a new version of an asset in a linked folder.
1. Select **Add New** > **Version**, then select the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it might not specifically mention Experience Manager Assets Essentials.

1. Select the asset you want to link.

1. Klicken Sie auf **Auswählen**.

## Link a folder from Experience Manager Assets Essentials

Permissions to view individual assets inside of a folder rely on Experience Manager Assets Essentials permissions.

1. Go to the **Documents** area in Workfront where you want the folder.
1. Select **Add New**, then select the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it might not specifically mention Experience Manager Assets Essentials.

1. Select the folders you want.

   ![Select a folder](assets/select-a-folder.png)

1. Klicken Sie auf **Auswählen**.

## Zu beachten

* Content Advisor functionality is not available for Assets Essentials. To link assets and folders using Content Advisor, see [Link assets and folders with Content Advisor powered by Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem.md).

* Assets sent from Assets Essentials don&#39;t count towards your overall document storage in Workfront. Documents uploaded and sent from Workfront to Assets Essentials do count towards overall storage.

* Metadata fields are first mapped when you send an asset from Workfront to Experience Manager Assets Essentials. If your Workfront administrator has enabled object metadata sync, fields remain up to date if they are changed in either application.
