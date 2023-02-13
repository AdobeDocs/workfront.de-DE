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
source-git-commit: b413ffc2416439629e073b32b5e9828df2f5de90
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Ändern der Adobe Workfront-Domäne

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in die Admin Console integriert wurden. Wenn Ihr Unternehmen in der Adobe Admin Console integriert wurde, müssen Sie diese Aktion über die Adobe Admin Console durchführen.
>
>Informationen zum Ändern der Adobe Workfront-Domäne, wenn Ihr Unternehmen in die Adobe Admin Console integriert wurde, finden Sie unter [Einrichten von Domänen](https://helpx.adobe.com/enterprise/using/set-up-identity.html#setup-domains).
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
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Domain-Änderung anfordern

1. Klicken Sie auf **Support** auf der Workfront One-Seite ein und erstellen Sie dann einen Support-Vorgang.
1. Im **Beschreibung** enthalten die neue gewünschte Domäne sowie den Zeitraum, in dem die neue Domäne live geschaltet werden soll.
1. Füllen Sie die Felder für den Support-Fall aus und klicken Sie auf **Einsenden**.

Sie können auch den Workfront-Support anrufen, um Hilfe beim Ändern Ihrer Domäne zu erhalten.

## Aktualisieren Sie die neue Domäne, wenn Sie SSO-Kunde sind.

Wenn Ihr Unternehmen SSO verwendet, sind die folgenden Schritte erforderlich, nachdem Sie Ihre Workfront-Domäne geändert haben.

>[!NOTE]
>
>Dies ist nicht verfügbar, wenn die Workfront-Instanz Ihres Unternehmens mit Adobe IMS aktiviert ist. Weitere Informationen erhalten Sie von Ihrem Netzwerk- oder IT-Administrator.

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie in der linken Seitenleiste auf **System** > **Kundeninformationen** und stellen Sie sicher, dass Ihre Domäne auf der Seite &quot;Kundeninformationen&quot;aktualisiert wird.

1. Klicken Sie in der linken Seitenleiste auf **System** > **Single Sign-On (SSO)**.

1. Klicken **SAML 2.0-Metadaten herunterladen**.
1. Nachdem die Datei heruntergeladen wurde, öffnen Sie sie und stellen Sie Folgendes sicher:

   1. **entityID** verweist auf die neue Domäne.
   1. Alle Orte innerhalb von **`<md:AssertionConsumerService>`** auf die neue Domäne verweisen.

1. Stellen Sie die heruntergeladene Metadatendatei an Ihren Identitätsanbieter bereit, damit dieser sie am Ende aktualisieren kann.
1. Stellen Sie sicher, dass die Domäne für alle von Ihrem Unternehmen verwendeten Workfront-Integrationen aktualisiert wird.
