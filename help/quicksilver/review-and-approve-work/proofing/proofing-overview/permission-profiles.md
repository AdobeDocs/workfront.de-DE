---
content-type: overview
product-area: documents
keywords: proof,permission
navigation-topic: proofing-overview
title: Übersicht über das Profil für Testberechtigungen
description: Testberechtigungsprofile bestimmen, welche Gesamtberechtigungen Benutzer für alle Testsendungen in Ihrem Konto haben. Profile für Testberechtigungen werden Benutzern in ihrem Benutzerprofil zugewiesen. Profile für Testberechtigungen unterscheiden sich von Testversandrollen.
author: Courtney
feature: Digital Content and Documents
exl-id: fb6faa48-d97b-4b7b-83ae-fe39d40b3963
source-git-commit: 4e3cafafb121371249fb73f2f001477bdbad2d77
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 2%

---

# Übersicht über das Profil für Testberechtigungen

<!--Audited: 12/2023-->

Testberechtigungsprofile bestimmen, welche Gesamtberechtigungen Benutzer für alle Testsendungen in Ihrem Konto haben. Profile für Testberechtigungen werden Benutzern in ihrem Benutzerprofil zugewiesen.

Profile für Testberechtigungen unterscheiden sich von Testversandrollen. Weitere Informationen zu Proof-Rollen finden Sie unter [Übersicht über Proof Roles](../../../review-and-approve-work/proofing/proofing-overview/proof-roles.md).

>[!NOTE]
>
>Wenn Sie Administrator sind, können Sie benutzerdefinierte Profile für Benutzer in Ihrem Unternehmen erstellen. Weitere Informationen finden Sie unter [Benutzerdefinierte Profile in Workfront Proof konfigurieren](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Consider the following about roles and permissions:</p>
-->

<!--
<ul data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li> <p>Assigned profile permissions relate only to the users and items in your own account. The exception is in the case of Satellite accounts, where the Administrator and Billing Administrator for the main (hub) accounts can access and manage the account settings and billing of those accounts from the hub account level.</p> </li>
<li> <p>Billing Administrators and Administrators can delete users. This can only be done in Account settings.</p> </li>
<li>When Billing Administrators and Administrators view proofs that are owned by other users in their account, they view them with the role of a Reviewer.</li>
<li>Using the Read Only role, Billing Administrators and Administrators can access proofs in folders shared with them or in folders created by them. </li>
</ul>
-->

## Profile für Testberechtigungen

In der folgenden Tabelle sind die für jedes Profil mit Testberechtigungen verfügbaren Berechtigungen aufgeführt.

<table>
  <tr>
   <td colspan="1" ><strong></strong>
   </td>
   <td colspan="4" ><strong>Eigene Elemente</strong>
   </td>
   <td colspan="3" ><strong>Elemente anderer Benutzer</strong>
   </td>
   <td><strong>Admin</strong>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td><strong>Hinzufügen</strong>
   </td>
   <td><strong>Anzeigen</strong>
   </td>
   <td><strong>Bearbeiten</strong>
   </td>
   <td><strong>Löschen</strong>
   </td>
   <td><strong>Anzeigen</strong>
   </td>
   <td><strong>Bearbeiten</strong>
   </td>
   <td><strong>Löschen</strong>
   </td>
   <td><strong>Bearbeiten und Löschen</strong>
   </td>
  </tr>
  <tr>
   <td>Admin
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
  </tr>
  <tr>
   <td>Supervisor
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Managerin bzw. Manager
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
</table>

### Administrator

Administratoren haben Zugriff auf [Kontoeinstellungen](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings) und die folgenden Berechtigungen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Administratoren können:</td> 
   <td>Administratoren können nicht:</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Testsendungen erstellen, Dateien hochladen und Ordner erstellen</p> </li> 
     <li> <p>Anzeigen, Bearbeiten und Löschen von von ihnen erstellten Testsendungen und Dateien</p> </li> 
     <li> <p>Anzeigen, Bearbeiten und Löschen von Testsendungen und Dateien, die von allen Benutzern in der Organisation erstellt wurden</p> </li> 
     <li> <p>Löschen der öffentlichen Ordner anderer Benutzer</p> </li> 
     <li> <p>Bearbeiten aller im Konto erstellten Testsendungen</p> </li> 
     <li> <p>Als Eigentümer der Dropzone festlegen*</p> </li> 
     <li> <p>Öffnen Sie die Seite Kontoeinstellungen und bearbeiten Sie die Kontodetails.</p> </li> 
     <li> <p>Löschen Sie den Müll</p> </li> 
     <li> <p>Benutzer hinzufügen, bearbeiten und löschen</p> </li> 
     <li> <p>Gruppen erstellen und neue Kontakte hinzufügen</p> </li> 
     <li> <p>Kontakte löschen</p> </li> 
     <li> <p>Testsendungen bearbeiten, wenn keine Antworten darauf vorliegen</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Testversand-Antworten bearbeiten.</p> </li> 
     <li> <p>Löschen der privaten Ordner anderer Benutzer</p> </li> 
     <li> <p>Öffnen Sie die Seite Rechnungsstellung oder bearbeiten Sie die Rechnungsdetails.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Nur im eigenständigen Workfront Proof-Produkt verfügbar.

### Supervisor

Supervisoren haben die folgenden Berechtigungen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Supervisoren können:</td> 
   <td>Supervisoren können nicht:</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Testsendungen erstellen, Dateien hochladen und Ordner erstellen</p> </li> 
     <li> <p>Anzeigen, Bearbeiten und Löschen von von ihnen erstellten Testsendungen und Dateien</p> </li> 
     <li> <p>Anzeigen, Bearbeiten und Löschen von Testsendungen und Dateien, die von allen Benutzern in der Organisation erstellt wurden</p> </li> 
     <li> <p>Löschen der öffentlichen Ordner anderer Benutzer</p> </li> 
     <li> <p>Bearbeiten aller im Konto erstellten Testsendungen</p> </li> 
     <li> <p>Gruppen erstellen und neue Kontakte hinzufügen</p> </li> 
     <li> <p>Kontakte löschen</p> </li> 
     <li> <p>Testsendungen bearbeiten, wenn keine Antworten darauf vorliegen</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Testversand-Antworten bearbeiten.</p> </li> 
     <li> <p>Löschen der privaten Ordner anderer Benutzer</p> </li> 
     <li> <p>Öffnen Sie die Seite Rechnungsstellung oder bearbeiten Sie die Rechnungsdetails.</p> </li> 
     <li> <p>Benutzer hinzufügen, bearbeiten oder löschen</p> </li> 
     <li> <p>Löschen Sie den Müll</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Managerin bzw. Manager

Manager haben die folgenden Berechtigungen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Manager können:</td> 
   <td>Manager können nicht:</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Testsendungen erstellen, Dateien hochladen und Ordner erstellen</p> </li> 
     <li> <p>Anzeigen, Bearbeiten und Löschen von von ihnen erstellten Testsendungen und Dateien</p> </li> 
     <li> <p>Testsendungen anderer Benutzer anzeigen, überprüfen und genehmigen, die explizit für sie freigegeben wurden (Schreibgeschützte Berechtigungen für alle in einem freigegebenen Ordner)</p> </li> 
     <li> <p>Bearbeiten aller im Konto erstellten Testsendungen</p> </li> 
     <li> <p>Gruppen erstellen und neue Kontakte hinzufügen</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Anzeigen, Bearbeiten oder Löschen von Testsendungen und Dateien, die von anderen Benutzern in der Organisation erstellt wurden. </p> </li><li><p>Testversand-Antworten bearbeiten.</p> </li> 
     <li> <p>Löschen Sie die privaten oder öffentlichen Ordner anderer Benutzer</p> </li> 
     <li> <p>Öffnen Sie die Seite Rechnungsstellung oder bearbeiten Sie die Rechnungsdetails.</p> </li> 
     <li> <p>Benutzer hinzufügen, bearbeiten oder löschen</p> </li> 
     <li> <p> Kontakte löschen</p> </li> 
     <li> <p>Löschen Sie den Müll</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Observer</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers have the following permissions:</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can see, review, and approve proofs of other users that are explicitly shared with them (Read-only rights to everything in a shared folder). For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view files that are explicitly shared with them. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot create proofs, upload files, and create folders. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md" class="MCXref xref">Upload Files and Web Content to Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot view, edit, or delete proofs and files created by other users in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot edit proofs or replies.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete any items created in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot access the Billing page or Account settings. For more information, see <a href="../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md" class="MCXref xref">The Workfront Proof Billing Page</a> and <a href="../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md" class="MCXref xref">Account settings in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot be set as the Dropzone owner. For more information, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md" class="MCXref xref">Configure the dropzone in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot empty the trash. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md" class="MCXref xref">Restore and Empty the Trash in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot add, edit, or delete users. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot create groups or add new contacts. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete contacts. </p>
-->


><!--
><p data-mc-conditions="QuicksilverOrClassic.Draft mode">Menus and functions available to Observers are limited. </p>>
>-->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the Header menu or the green New menu in their Dashboard</li>>
>  -->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the following links in their Settings: Account settings, Billing </li>>
>  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Guest</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Guest profile is used to give access to proofs for reviewers who do not have their own Workfront Proof account. Guests can access proofs shared with them directly via their personal email notifications.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view, review, and approve proofs that are explicitly shared with them.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view files that are explicitly shared with them.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot access the Dashboard.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot have folders shared with them. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md" class="MCXref xref">Manage Folders in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot be added as Authors or Moderators to the proofs. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p>
-->

<!--
<note type="note">
 Guests are not Workfront Proof users, so they cannot see all the proofs shared with them in their own Dashboard.
</note>
-->
