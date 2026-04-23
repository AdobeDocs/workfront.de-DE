---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Ändern der Adobe Workfront-Domain
description: Als Adobe Workfront-Administrator und autorisierter Workfront-Support-Kontakt können Sie Hilfe vom Workfront-Support-Team anfordern, um die Workfront-Domain Ihres Unternehmens zu ändern.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: 51d0989bdbf4ecdc799658f30500c68bf5867e65
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 17%

---

# Ändern der Adobe Workfront-Domain

<!--Remove me October 2026-->

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch keine Einführung in Admin Console erhalten haben. Da nun alle Organisationen in die Adobe Admin Console integriert wurden (**kann die Workfront-Domain nicht geändert werden**.
>
>Eine Liste der Verfahren, die sich je nachdem, ob Ihr Unternehmen in die Adobe Admin Console integriert wurde, unterscheiden, finden Sie unter [Plattformbasierte Administrationsunterschiede (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>
>Dieser Artikel wird in naher Zukunft entfernt.

Als Adobe Workfront-Administrator und autorisierter Workfront-Support-Kontakt können Sie Hilfe vom Workfront-Support-Team anfordern, um die Workfront-Domain Ihres Unternehmens zu ändern.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p><p>Abo</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Domain-Änderung anfordern

1. Beginnen Sie mit der Erstellung eines Support-Tickets in Experience League.
1. Geben **im Feld** die neue Domain ein, die Sie möchten, sowie den Zeitrahmen, in dem die neue Domain live geschaltet werden soll.
1. Füllen Sie alle Felder für den Support-Fall aus und klicken Sie dann auf **Senden**.

Sie können auch den Workfront-Support anrufen, um Hilfe beim Ändern Ihrer Domain zu erhalten.

<!--

## Update the new domain if you are an SSO customer

If your company utilizes SSO, the following steps are required after you have your Workfront domain changed.

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

{{step-1-to-setup}}

1. In the left sidebar, click **System** > **Customer Info** and make sure that your domain is updated on the Customer Info page.

1. In the left sidebar, click **System** > **Single Sign-On (SSO)**.

1. Click **Download SAML 2.0 Metadata**.
1. After the file is downloaded, open it and make sure of the following:

   1. **entityID** is pointing to the new domain.
   1. All locations within **`<md:AssertionConsumerService>`** point to the new domain.

1. Provide the downloaded metadata file to your Identity Provider so that they can update it on their end.
1. Make sure the domain is updated for all Workfront integrations used by your organization.


-->
