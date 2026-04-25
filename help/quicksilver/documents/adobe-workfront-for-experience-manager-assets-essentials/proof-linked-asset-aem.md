---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Proof a linked asset for Experience Manager Assets or Assets Essentials
description: After you've linked an asset from Experience Manager Assets Essentials, you can create a proof and assign users to review and add comments to the asset.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abd641a1-081b-4b86-95ee-f0ed030d704c
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 14%

---

# Proof a linked asset for Experience Manager Assets or Assets Essentials

After you&#39;ve linked an asset from Experience Manager Assets Essentials, you can create a proof and assign users to review and add comments to the asset.

>[!NOTE]
>
>Diese Funktion ist im Bereich Neue Dokumente nicht verfügbar.<br>
>Wenn Ihr Unternehmen Enterprise-Speicher verwendet, wird der Bereich „Neue Dokumente“ angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. From there, you can add assets from Experience Manager Assets and review and approve them with the Frame.io viewer. Weitere Informationen finden Sie unter [Verwenden von Adobe Experience Manager mit der Frame.io-Integration](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

## Zugriffsanforderungen

<!-- Audited: 4/2025 -->

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
   <p>Standard</p>
   <p>Work oder höher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Additonal products</td> 
   <td>You must have Experience Manager as a Cloud Service or Assets Essentials, and you must be added to the product as a user in the Admin Console. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriffrecht „Bearbeiten“ für Dokumente</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>View access or higher</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Before you begin:

* Your Workfront Administrator must configure an Experience Manager integration. For more information, see [Configure the Experience Manager Assets as a Cloud Service integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) or [Configure the Experience Manager Assets Essentials integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Korrekturabzug erstellen

You can create static, video, or interactive proofs.

To create a proof:

1. Go to the project, task, or issue where you want the proof, then click the **Documents** section.
1. Hover over the document, then click the **Create Proof** link that appears below the document name.

   >[!NOTE]
   >
   >If you have **Automatically generate proofs when uploading documents** enabled in your user profile, the system automatically creates a simple proof.

1. Choose one of the following from the drop-down:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Simple Proof</strong></td> 
      <td>This option creates a proof with no workflow attached and applies the default proof settings. You can update the default proof settings or add a workflow after you've created the proof. For more information on proof settings, see <a href="../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Edit proof settings</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Advanced Proof</strong></td> 
      <td> <p>This option allows you to configure a Basic or Advanced workflow and modify proof settings for the proof you create. Weitere Informationen finden Sie unter: </p> 
       <ul> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Create an advanced proof with a Basic workflow</a> </p> </li> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Create an advanced proof with an Automated workflow</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## Manage an existing proof

Once you&#39;ve created a proof, you can do the following:

* View current stage activity
* Update reviewers and deadlines
* Edit the workflow

For more information about how to manage an existing proof, see [Manage proofs within Adobe Workfront: article index](../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## Überprüfen eines Korrekturabzugs

Assigned reviewers can do the following:

* View the asset and make comments
* Add actions to comments
* Compare versions
* Approve or reject the proof

For more information about what you can do with the proofing tool, see [Review proofs within Adobe Workfront: article index](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
