---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Ändern der Adobe Workfront-Domäne
description: Als Adobe Workfront-Administrator und autorisierter Workfront-Support-Kontakt können Sie beim Workfront-Support Hilfe anfordern, um die Workfront-Domäne Ihres Unternehmens zu ändern.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: 22ea9b623d7bc7b216511538cf88e4d020529bd3
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# Ändern der Adobe Workfront-Domäne

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in die Admin Console integriert wurden. Wenn Ihr Unternehmen in der Adobe Admin Console integriert wurde, ist es nicht möglich, Ihre Workfront-Domäne zu ändern.
>
>Eine Liste der Verfahren, die je nachdem, ob Ihr Unternehmen in die Adobe Admin Console integriert wurde, unterschiedlich sind, finden Sie unter [Plattformbasierte Verwaltungsunterschiede (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Als Adobe Workfront-Administrator und autorisierter Workfront-Support-Kontakt können Sie beim Workfront-Support Hilfe anfordern, um die Workfront-Domäne Ihres Unternehmens zu ändern.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsstufe festgelegt hat. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Domain-Änderung anfordern

1. Erstellen Sie ein Support-Ticket auf dem Experience League.
1. Im **Beschreibung** enthalten die neue gewünschte Domäne sowie den Zeitraum, in dem die neue Domäne live geschaltet werden soll.
1. Füllen Sie die Felder für den Support-Fall aus und klicken Sie auf **Einsenden**.

Sie können auch den Workfront-Support anrufen, um Hilfe beim Ändern Ihrer Domäne zu erhalten.

## Neue Domäne aktualisieren, wenn Sie SSO-Kunde sind

Wenn Ihr Unternehmen SSO verwendet, sind die folgenden Schritte erforderlich, nachdem Sie Ihre Workfront-Domäne geändert haben.

>[!NOTE]
>
>Dies ist nicht verfügbar, wenn die Workfront-Instanz Ihres Unternehmens mit Adobe IMS aktiviert ist. Wenden Sie sich an Ihren Netzwerk- oder IT-Administrator, wenn Sie weitere Informationen benötigen.

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie in der linken Seitenleiste auf **System** > **Kundeninformationen** und stellen Sie sicher, dass Ihre Domäne auf der Seite &quot;Kundeninformationen&quot;aktualisiert wird.

1. Klicken Sie in der linken Seitenleiste auf **System** > **Single Sign-On (SSO)**.

1. Klicks **SAML 2.0-Metadaten herunterladen**.
1. Nachdem die Datei heruntergeladen wurde, öffnen Sie sie und stellen Sie Folgendes sicher:

   1. **entityID** verweist auf die neue Domäne.
   1. Alle Orte innerhalb von **`<md:AssertionConsumerService>`** auf die neue Domäne verweisen.

1. Stellen Sie die heruntergeladene Metadatendatei an Ihren Identitätsanbieter bereit, damit dieser sie am Ende aktualisieren kann.
1. Stellen Sie sicher, dass die Domäne für alle von Ihrem Unternehmen verwendeten Workfront-Integrationen aktualisiert wird.
