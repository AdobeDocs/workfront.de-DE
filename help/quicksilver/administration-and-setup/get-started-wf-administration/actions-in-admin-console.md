---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Plattformbasierte Verwaltungsunterschiede (Adobe Workfront/Adobe Business Platform)
description: Wenn Ihr Unternehmen in die Adobe Business Platform integriert wurde, verwenden Ihre Benutzer die Adobe Business Platform, um auf Adobe Workfront zuzugreifen. Das bedeutet, dass die Benutzerverwaltung überwiegend über die Adobe Admin Console erfolgt und Single Sign-On (SSO) über die Adobe Business Platform und nicht über Workfront erfolgt. Als Adobe Workfront-Administrator unterscheiden sich Ihre Administrationsaufgaben und -verfahren je nachdem, ob Ihr Unternehmen in die Adobe Business Platform integriert wurde. In diesem Artikel werden die Verfahren aufgelistet, die unterschiedlich gehandhabt werden müssen, sowie Links zu Anweisungen für Workfront und Adobe Admin Console.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a84a5a8d-7c2a-4b51-a614-91a6dc9aa4ed
source-git-commit: 5d4434d090c4b6cdefc9c313fecccf6d6e9a510b
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Plattformbasierte Verwaltungsunterschiede (Adobe Workfront/Adobe Business Platform)

Als Adobe Workfront-Administrator können Ihre Administrationsaufgaben und -verfahren unterschiedlich sein, je nachdem, ob Ihr Unternehmen in die Adobe Business Platform integriert wurde. In diesem Artikel werden die Verfahren aufgelistet, die unterschiedlich gehandhabt werden, sowie Links zu Anweisungen für Workfront und Adobe Admin Console.

Wenn Ihr Unternehmen in die Adobe Business Platform integriert wurde, verwenden Ihre Benutzer die Adobe Business Platform, um auf Adobe Workfront zuzugreifen. Das bedeutet:

* Systemadministratoren werden über die Adobe Admin Console erstellt.
* Das Verlängern eines SAML-Zertifikats wird über die Adobe Admin Console verarbeitet.
* Single Sign-On (SSO) wird über die Adobe Business Platform statt über Workfront durchgeführt

## Erstellen von Workfront-Systemadministratoren in der Adobe Admin Console

>[!NOTE]
>
>Es wird empfohlen, Benutzer ohne Systemadministrator direkt in Workfront hinzuzufügen. Es ist möglich, Benutzer in der Adobe Admin Console hinzuzufügen. Wenn Sie diese jedoch in Workfront hinzufügen, können Sie ihre Zugriffsebene bei der Erstellung festlegen, wodurch Sie Zeit sparen können.

Anweisungen zum Erstellen von Workfront-Systemadministratoren finden Sie unter [Verwalten von Systemadministratoren in Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

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

Anweisungen zur Verlängerung des SAML-Zertifikats auf dem Adobe Admin Console finden Sie im Abschnitt &quot;Die digitale Signatur in der SAML-Antwort hat nicht validiert...&quot;in [Fehlerbehebung bei Federated ID](https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html)

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

Da die Adobe Business Platform Single Sign-On (SSO) für Benutzer steuert, werden die folgenden Aktionen und Funktionen automatisch über die Adobe Business Platform verarbeitet. Wenn Ihr Unternehmen noch nicht in der Adobe Business Platform integriert wurde, müssen Sie diese Aktionen in Workfront durchführen.


* [Konfigurieren von Adobe Workfront mit SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)
* [Konfigurieren von Adobe Workfront mit SAML 2.0 mithilfe von ADFS](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)
* [Deaktivieren von Single Sign-on in Adobe Workfront](../../administration-and-setup/add-users/single-sign-on/deactivate-sso.md)
* [SAML 2.0-Metadaten in Ihrem Identitäts-Provider aktualisieren](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)
* [Benutzer für Single Sign-on aktualisieren](../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)
* [Kennwortrichtlinien für die Authentifizierung konfigurieren](../../administration-and-setup/manage-workfront/security/configure-password-policies-authentication.md)
* [Systemsicherheitsvoreinstellungen konfigurieren](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)
