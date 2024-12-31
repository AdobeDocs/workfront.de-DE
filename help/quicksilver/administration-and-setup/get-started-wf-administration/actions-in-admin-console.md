---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Unterschiede bei der plattformbasierten Administration (Adobe Workfront/Adobe Business Platform)
description: Wenn Ihr Unternehmen die Adobe Business-Plattform nutzt, können Ihre Anwender über die Adobe Business-Plattform auf Adobe Workfront zugreifen. Das bedeutet, dass die Benutzerverwaltung größtenteils über Adobe Admin Console erfolgt und Single Sign-On (SSO) über die Adobe Business-Plattform und nicht über Workfront abgewickelt wird. Als Adobe Workfront-Administrator unterscheiden sich Ihre Administrationsaufgaben und -verfahren je nachdem, ob Ihr Unternehmen die Adobe-Geschäftsplattform verwendet. In diesem Artikel werden die Verfahren aufgeführt, die unterschiedlich gehandhabt werden müssen, sowie Links zu Anweisungen für Workfront und Adobe Admin Console.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: a84a5a8d-7c2a-4b51-a614-91a6dc9aa4ed
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Unterschiede bei der plattformbasierten Administration (Adobe Workfront/Adobe Business Platform)

Als Adobe Workfront-Administrator können Ihre Administrationsaufgaben und -verfahren unterschiedlich sein, je nachdem, ob Ihr Unternehmen die Adobe-Geschäftsplattform verwendet. In diesem Artikel werden die Verfahren aufgeführt, die unterschiedlich gehandhabt werden, sowie Links zu Anweisungen für Workfront und Adobe Admin Console.

Wenn Ihr Unternehmen die Adobe Business-Plattform nutzt, können Ihre Anwender über die Adobe Business-Plattform auf Adobe Workfront zugreifen. Dies bedeutet, dass:

* Systemadministratoren werden über die Adobe Admin Console erstellt
* Die Verlängerung eines SAML-Zertifikats wird über die Adobe Admin Console abgewickelt.
* Single Sign-On (SSO) wird über die Adobe Business-Plattform und nicht über Workfront abgewickelt

## Erstellen von Workfront-Systemadministratoren in der Adobe Admin Console

>[!NOTE]
>
>Es wird empfohlen, Benutzer, die keine Systemadministratoren sind, direkt in Workfront hinzuzufügen. Es ist möglich, Benutzende in der Adobe Admin Console hinzuzufügen. Durch das Hinzufügen in der Workfront können Sie jedoch deren Zugriffsebene beim Erstellen festlegen, was Ihnen Zeit sparen kann.

Anweisungen zum Erstellen von Workfront-Systemadministratoren finden Sie unter [Verwalten von Systemadministratoren in der Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

<!--
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Action</th> 
   <th>For instructions in Workfront, see</th> 
   <th>For instructions in the Adobe Admin console, see</th> 
  </tr> 
 </thead> 
 <tbody> 
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">View information about access levels and licenses for your users</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/list-access-levels-and-licenses-for-your-users.md" class="MCXref xref">List your users' access levels and licenses</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p>The section "View user list" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  <tr> 
   <td role="rowheader">Grant a user admin access</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Add a user to Adobe Workfront</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Add users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
     <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Add a user to Adobe Workfront Fusion</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../workfront-fusion/organizations/add-user-to-an-organization.md" class="MCXref xref">Add a user to an organization in Adobe Workfront Fusion</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
      <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  <tr> 
   <td role="rowheader">Deactivate a user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Remove users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Delete a user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md" class="MCXref xref">Delete users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Permanently delete users" in <a href="https://helpx.adobe.com/enterprise/using/manage-directory-users.html">Manage directory users</a>
     </p><p>Note: Deleting a user from the [!DNL Adobe Admin Console] deactivates the user in [!DNL Workfront], but does not delete them from [!DNL Workfront].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Edit a user profile</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bulk edit user profiles</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md" class="MCXref xref">Edit user profiles in bulk</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Bulk CSV upload</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Import users </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Import users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Add users" in <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Bulk CSV upload</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Log in as another user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md" class="MCXref xref">Log in as another user</a> </p> </li> 
    </ul> </td> 
   <td>Not available</td> 
  </tr> 
  <tr> 
    -->

## Verlängern des SAML-Zertifikats

Anweisungen zur Erneuerung des SAML-Zertifikats auf der Adobe Admin Console finden Sie im Abschnitt „Die digitale Signatur in der SAML-Antwort wurde nicht validiert…“ in [Fehlerbehebungs-Federated ID](https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html)

<!--

   <td role="rowheader">Renew SAML certificate</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/manage-workfront/security/renew-wf-saml-2-certificate.md" class="MCXref xref">Renew the Adobe Workfront SAML 2.0 metadata certificate</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "The digital signature in the SAML response did not validate..." in <a href="https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html">Troubleshooting Federated ID</a></p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

-->

## SSO (Single Sign-On)

Da die Adobe-Geschäftsplattform Single Sign-On (SSO) für Benutzende steuert, werden die folgenden Aktionen und Funktionen automatisch über die Adobe-Geschäftsplattform verarbeitet. Wenn Ihr Unternehmen noch nicht in die Adobe Business-Plattform integriert wurde, müssen Sie diese Aktionen in Workfront durchführen.


* [Konfigurieren von Adobe Workfront mit SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)
* [Konfigurieren von Adobe Workfront mit SAML 2.0 mithilfe von ADFS](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)
* [Deaktivieren von Single Sign-on in Adobe Workfront](../../administration-and-setup/add-users/single-sign-on/deactivate-sso.md)
* [Aktualisieren von SAML 2.0-Metadaten in Ihrem Identitätsanbieter](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)
* [Benutzer für einmaliges Anmelden aktualisieren](../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)
* [Konfigurieren von Passwortrichtlinien für die Authentifizierung](../../administration-and-setup/manage-workfront/security/configure-password-policies-authentication.md)
* [Systemsicherheitseinstellungen konfigurieren](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)
