---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: Konfigurieren des Proofing-Zugriffs von Benutzern
description: Als Adobe Workfront- oder Workfront Proof-Administrator können Sie den Zugriff eines Benutzers konfigurieren, um in Workfront und Workfront Proof Testsendungen zu erstellen und anzuzeigen.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
TQID: 'https://experienceleague.adobe.com/L-AMDvQYgtXJwxmtwekimbEA9OQQN72QHIcoQ2iKzGU'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4ea8bc003ce17978be5e5a6fd838012dfcfeae78
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 6%
---
# Konfigurieren des Proofing-Zugriffs von Benutzenden

Als Adobe Workfront- oder Workfront Proof-Administrator können Sie den Zugriff eines Benutzers konfigurieren, um in Workfront und Workfront Proof Testsendungen zu erstellen und anzuzeigen.

Informationen zu den für grundlegendes und integriertes Proofing verfügbaren Proofing-Funktionen finden Sie [Zugriff auf die Proofing-Funktionen in Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

Sie benötigen die folgenden Zugriffsrechte, um die Schritte in diesem Artikel auszuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Sie müssen ein Workfront- oder Workfront Proof-Administrator sein. Informationen zu Workfront-Administratoren finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollständigen Administratorzugriffs für einen Benutzer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

+++

<!--

## Configure a user's proof permission profile

The permission profile you select is granted to the users for each proof that exists within your organization.

{{step-1-to-users}}
 
1. Select one or more users, then click **Edit**.  

1. In the **Access** section, click one of the following Workfront Proof permission options in the **Proof Permission Profile** drop-down menu:

   >[!NOTE]
   >
   >If you are on a legacy Workfront plan, make sure the **User can generate proofs** option is enabled, as explained above in the section [Enable and disable proofing for a user (legacy plans only)](#enable-and-disable-proofing-for-a-user-legacy-plans-only). 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Supervisor</strong> </td> 
      <td>Users can manage and view all proofs created on your organization's account. They can also edit reviewers added to these proofs. Users with this permission profile can't manage users or edit Workfront Proof settings.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Manager</strong> </td> 
      <td> <p> Users can manage and view proofs created or owned on your organization's account. They can view other users' proofs only when added as a reviewer. This is a default setting. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrator</strong> </td> 
      <td> Users are given Administrator permissions in Workfront Proof and can edit account settings. Users can manage and view all proofs created on your organization's account. This includes adding and removing reviewers, proofs, and comments.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Custom</strong> </td> 
      <td> <p>Available only if you have configured a custom permission profile within Workfront Proof.</p> <p><b>NOTE</b>:  <p>Ensure that the permission profile you grant here does not provide higher access than the user's Access Level setting in Workfront (see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>). If it does provide higher access, the user can access proofs within Workfront Proof that he or she cannot access within Workfront.</p> <p>This is especially important if you plan to allow all Workfront users to access Workfront Proof directly from the Workfront as described in <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Access Workfront Proof from Adobe Workfront</a>.</p> <p>By default, only Workfront administrators have access to a direct link to the Workfront Proof site from the Workfront Global Navigation Bar.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   The permission profile you select is granted to the users for each proof that exists within your organization.

1. Click **Save Changes** to complete the update to the user settings.

   >[!NOTE]
   >
   >When you create or update a user in Workfront and the user's Workfront email address matches that of a licensed Workfront Proof user, the system enables proofing for the user within Workfront. For more information, see [User synchronization between Adobe Workfront and Workfront Proof](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Considerations

Consider the following information when setting permissions:

* If you change a user's permission profile to a profile with fewer permissions, the user might lose visibility to existing proofs within Workfront. This can occur when someone shares a task with a user within Workfront, but doesn't share the proof attached to the task (see [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* You can set Workfront Proof permissions from Workfront only if your Workfront environment is integrated with a Workfront Proof Premium account. If you cannot use proofing as discussed in this section, contact your Workfront administrator.
* At least one user in your Workfront environment must have Administrator permissions for proofing. An error message appears if you try to attempt to remove Administrator permissions for proofing from all users.
* When you change a user's Workfront Access level to any level other than System Administrator, the user's Workfront Proof permission profile defaults to Manager.   

* When you change the Workfront Access level to System Administrator, the Proof Permission profile changes to Administrator.

-->

## Konfigurieren des Workfront Proof-Zugriffs für alle Benutzer über das Workfront-Hauptmenü {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

Standardmäßig können nur Benutzende mit Administratorrechten in Workfront wie unter (Zugriff auf Workfront Proof [&#x200B; Adobe Workfront) beschrieben auf Workfront Proof &#x200B;](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

Sie können allen Benutzenden Zugriff auf die Schaltfläche Workfront Proof im Hauptmenü von Workfront gewähren, indem Sie sich an den Workfront-Support wenden und eine Anfrage senden.

>[!IMPORTANT]
>
> Wenn Sie allen Workfront-Benutzenden erlauben möchten, direkt über die globale Navigationsleiste von Workfront auf Workfront Proof zuzugreifen, stellen Sie sicher, dass das Berechtigungsprofil der einzelnen Benutzenden nicht mehr Zugriff bietet als die Zugriffsebene der Benutzenden in Workfront. Dadurch wird verhindert, dass Benutzende in Workfront Proof auf Korrekturabzüge zugreifen, auf die sie nicht in Workfront zugreifen können. Weitere Informationen finden Sie unter [Aktivieren und Deaktivieren des Proofings für einen Benutzer (nur für ältere Pläne)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

## Konfigurieren des Benutzerzugriffs auf den Desktop Proofing Viewer

Wenn Benutzende in Ihrer Organisation lieber den Desktop Proofing Viewer anstelle des Web Proofing Viewers zur Überprüfung interaktiver Inhalte verwenden möchten, können Sie den Desktop Proofing Viewer so konfigurieren, dass er automatisch gestartet wird, wenn Benutzende interaktive Korrekturabzüge für Inhalte öffnen. Weitere Informationen dazu, wie sich der Desktop Proofing Viewer vom Web Proofing Viewer unterscheidet, finden Sie unter [Grundlegendes zum Desktop Proofing Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) und [Unterschiede zwischen dem Web Proofing Viewer und dem Desktop Proofing Viewer](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

1. Klicken Sie in Workfront in der globalen Navigationsleiste auf das Workfront Proof-Symbol, um auf Workfront Proof zuzugreifen.

   ![Korrekturabzug-Symbol](assets/proof-access-proofhq-350x39.png)

1. Klicken **oben rechts** Workfront Proof auf „Kontoeinstellungen“ und dann auf die Registerkarte **Einstellungen**.

1. Klicken **unter** Testversand-Standardeinstellungen“ am Ende der Zeile **Desktop Proofing Viewer für interaktives**&quot; auf **Setup**.

1. Ändern Sie die Einstellungen für die Desktop-Proofing-Viewer, wie [Desktop-Proofing](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer)Viewer) im Artikel [Konfigurieren der Korrekturabzugseinstellungen für Ihr Unternehmen](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md) beschrieben.

1. Klicken Sie auf **Speichern**.

## Konfigurieren von benutzerdefinierten Geräten für interaktive Korrekturabzüge

Sie können Ihrem System beliebige benutzerdefinierte Geräte hinzufügen, damit Benutzer interaktive Inhalte überprüfen und simulieren können, wie die Inhalte auf einem bestimmten Gerät angezeigt werden, wenn sie den Desktop Proofing Viewer verwenden. (Diese Funktion ist im Web Proofing Viewer nicht verfügbar, in dem Benutzende interaktive Inhalte überprüfen können, sondern nur so, wie sie in verschiedenen Auflösungen und nicht auf verschiedenen Geräten angezeigt werden.)

Weitere Informationen finden Sie unter [Ändern der interaktiven Korrekturabzugsauflösung im Proofing Viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

1. Greifen Sie über Workfront auf die Workfront Proof-Benutzeroberfläche zu, wie in [Zugriff auf Workfront Proof über Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md) beschrieben.
1. Ändern Sie die Einstellungen der Desktop-Korrekturabzugsanzeige, wie unter [Konfigurieren benutzerdefinierter Geräte für Korrekturabzüge](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs) im Artikel [Konfigurieren der Korrekturabzugseinstellungen für Ihre Organisation](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md) beschrieben.
