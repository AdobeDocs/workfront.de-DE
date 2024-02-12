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
source-git-commit: b476c012f825afc4bc48b7172be26accc6bac0d1
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 1%

---

# Plattformbasierte Verwaltungsunterschiede (Adobe Workfront/Adobe Business Platform)

Wenn Ihr Unternehmen in die Adobe Business Platform integriert wurde, verwenden Ihre Benutzer die Adobe Business Platform, um auf Adobe Workfront zuzugreifen. Das bedeutet:

* Systemadministratoren werden über die Adobe Admin Console erstellt.
* Single Sign-On (SSO) wird über die Adobe Business Platform und nicht über Workfront durchgeführt

Als Adobe Workfront-Administrator unterscheiden sich Ihre Administrationsaufgaben und -verfahren je nachdem, ob Ihr Unternehmen in die Adobe Business Platform integriert wurde. In diesem Artikel werden die Verfahren aufgelistet, die unterschiedlich gehandhabt werden, sowie Links zu Anweisungen für Workfront und Adobe Admin Console.

## Benutzende



>[!NOTE]
>
>Es wird empfohlen, Benutzer ohne Systemadministrator direkt in Workfront hinzuzufügen. Es ist möglich, Benutzer in der Adobe Admin Console hinzuzufügen. Wenn Sie diese jedoch in Workfront hinzufügen, können Sie ihre Zugriffsebene bei der Erstellung festlegen, wodurch Sie Zeit sparen können.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Aktion</th> 
   <th>Anweisungen in Workfront finden Sie unter</th> 
   <th>Anweisungen in der Adobe Admin Console finden Sie unter</th> 
  </tr> 
 </thead> 
 <tbody> <!--
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
  --> 
  <tr> 
   <td role="rowheader">Gewähren eines Benutzeradministratorzugriffs</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Der Abschnitt "Benutzerdetails bearbeiten"in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Benutzer einzeln verwalten</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Benutzer zu Adobe Workfront hinzufügen</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Benutzer hinzufügen</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Verwalten von Benutzern in Adobe Admin Console</a> </p> </li> 
     <li> <p>Der Abschnitt "Benutzer hinzufügen"in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Benutzer einzeln verwalten</a></p> </li> 
    </ul> </td> 
  </tr> <!--
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
  --> 
  <tr> 
   <td role="rowheader">Deaktivieren eines Benutzers</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Benutzer deaktivieren oder reaktivieren</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Der Abschnitt "Benutzer entfernen"in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Benutzer einzeln verwalten</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Benutzer löschen</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md" class="MCXref xref">Benutzer löschen</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Den Abschnitt "Benutzer dauerhaft löschen"in <a href="https://helpx.adobe.com/enterprise/using/manage-directory-users.html">Ordnerbenutzer verwalten</a>
     </p><p>Hinweis: Löschen eines Benutzers aus dem [!DNL Adobe Admin Console] deaktiviert den Benutzer in [!DNL Workfront], aber löschen sie nicht aus [!DNL Workfront].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Benutzerprofil bearbeiten</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Profil eines Benutzers bearbeiten</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Der Abschnitt "Benutzerdetails bearbeiten"in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Benutzer einzeln verwalten</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Massenbearbeitungsbenutzerprofile</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md" class="MCXref xref">Massenbearbeitung von Benutzerprofilen</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Der Abschnitt "Benutzerdetails bearbeiten"in <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Massen-CSV-Upload</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Benutzer importieren </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Benutzer importieren</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Der Abschnitt "Benutzer hinzufügen"in <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Massen-CSV-Upload</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Anmelden als eine andere Benutzerin bzw. ein anderer Benutzer</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md" class="MCXref xref">Melden Sie sich als anderer Benutzer an</a> </p> </li> 
    </ul> </td> 
   <td>Nicht verfügbar</td> 
  </tr> 
  <tr> 
   <td role="rowheader">SAML-Zertifikat erneuern</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/manage-workfront/security/renew-wf-saml-2-certificate.md" class="MCXref xref">Adobe Workfront SAML 2.0-Metadatenzertifikat erneuern</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Der Abschnitt "Die digitale Signatur in der SAML-Antwort hat nicht validiert..."in <a href="https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html">Fehlerbehebung bei Federated ID</a></p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## SSO (Single Sign-On)

Da die Adobe Business Platform Single Sign-On (SSO) für Benutzer steuert, werden die folgenden Aktionen und Funktionen automatisch über die Adobe Business Platform verarbeitet. Wenn Ihr Unternehmen noch nicht in der Adobe Business Platform integriert wurde, müssen Sie diese Aktionen in Workfront durchführen.


* [Konfigurieren von Adobe Workfront mit SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)
* [Konfigurieren von Adobe Workfront mit SAML 2.0 mithilfe von ADFS](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)
* [Deaktivieren von Single Sign-on in Adobe Workfront](../../administration-and-setup/add-users/single-sign-on/deactivate-sso.md)
* [SAML 2.0-Metadaten in Ihrem Identitäts-Provider aktualisieren](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)
* [Benutzer für Single Sign-on aktualisieren](../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)
* [Kennwortrichtlinien für die Authentifizierung konfigurieren](../../administration-and-setup/manage-workfront/security/configure-password-policies-authentication.md)
* [Systemsicherheitsvoreinstellungen konfigurieren](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)
