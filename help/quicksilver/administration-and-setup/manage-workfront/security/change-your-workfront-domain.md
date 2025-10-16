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
source-git-commit: 6b2d93d2573d72e4390761038d8078f47d96d55e
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---

# Ändern der Adobe Workfront-Domain

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch keine Einführung in Admin Console erhalten haben. Wenn Ihre Organisation in die Adobe Admin Console integriert wurde, ist es nicht möglich, Ihre Workfront-Domain zu ändern.
>
>Eine Liste der Verfahren, die sich je nachdem, ob Ihr Unternehmen in die Adobe Admin Console integriert wurde, unterscheiden, finden Sie unter [Plattformbasierte Administrationsunterschiede (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Als Adobe Workfront-Administrator und autorisierter Workfront-Support-Kontakt können Sie Hilfe vom Workfront-Support-Team anfordern, um die Workfront-Domain Ihres Unternehmens zu ändern.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Domain-Änderung anfordern

1. Beginnen Sie mit der Erstellung eines Support-Tickets in Experience League.
1. Geben **im Feld** die neue Domain ein, die Sie möchten, sowie den Zeitrahmen, in dem die neue Domain live geschaltet werden soll.
1. Füllen Sie alle Felder für den Support-Fall aus und klicken Sie dann auf **Senden**.

Sie können auch den Workfront-Support anrufen, um Hilfe beim Ändern Ihrer Domain zu erhalten.

## Aktualisieren der neuen Domain, wenn Sie SSO-Kunde sind

Wenn Ihr Unternehmen SSO verwendet, sind nach dem Ändern Ihrer Workfront-Domain die folgenden Schritte erforderlich.

>[!NOTE]
>
>Dies ist nicht verfügbar, wenn die Workfront-Instanz Ihres Unternehmens mit Adobe IMS aktiviert ist. Wenden Sie sich an Ihren Netzwerk- oder IT-Administrator, wenn Sie weitere Informationen benötigen.

{{step-1-to-setup}}

1. Klicken Sie in der linken Seitenleiste auf **System** > **Kundeninformationen** und stellen Sie sicher, dass Ihre Domain auf der Seite „Kundeninformationen“ aktualisiert wird.

1. Klicken Sie in der linken Seitenleiste auf **System** > **Single Sign-On (SSO)**.

1. Klicken Sie **SAML 2.0-Metadaten herunterladen**.
1. Nachdem die Datei heruntergeladen wurde, öffnen Sie sie und stellen Sie Folgendes sicher:

   1. **entityID** verweist auf die neue Domain.
   1. Alle Speicherorte in **`<md:AssertionConsumerService>`** verweisen auf die neue Domain.

1. Stellen Sie die heruntergeladene Metadatendatei Ihrem Identitätsanbieter zur Verfügung, damit er sie an seinem Ende aktualisieren kann.
1. Stellen Sie sicher, dass die Domain für alle von Ihrem Unternehmen verwendeten Workfront-Integrationen aktualisiert wird.
