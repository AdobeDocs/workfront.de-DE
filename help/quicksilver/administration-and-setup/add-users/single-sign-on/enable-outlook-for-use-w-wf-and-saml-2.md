---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Outlook für die Verwendung mit Workfront und SAML 2.0 aktivieren
description: Wenn Sie die SAML 2.0-Authentifizierung aktivieren und möchten, dass sich Ihre Benutzer über Microsoft Outlook mit ihren SAML 2.0-Anmeldeinformationen bei Workfront anmelden können, müssen Sie SAML 2.0 aktivieren, um sich in Office-Add-Ins zu authentifizieren.
author: Caroline, Becky
feature: System Setup and Administration
role: Admin
exl-id: 8a55d364-962a-4eef-8968-b2233a71cf31
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 1%

---

# Outlook für die Verwendung mit Workfront und SAML 2.0 aktivieren

Wenn Sie die SAML 2.0-Authentifizierung aktivieren und möchten, dass sich Ihre Benutzer über Microsoft Outlook mit ihren SAML 2.0-Anmeldeinformationen bei Workfront anmelden können, müssen Sie SAML 2.0 aktivieren, um sich in Office-Add-Ins zu authentifizieren.

>[!NOTE]
>
>Dies ist nicht verfügbar, wenn die Workfront-Instanz Ihres Unternehmens ein benutzerdefiniertes SSO-Portal verwendet.>
><!--
>or is enabled with Adobe IMS>
>-->
>Weitere Informationen erhalten Sie von Ihrem Netzwerk- oder IT-Administrator.

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

## Outlook für die Verwendung mit Workfront und SAML 2.0 aktivieren

1. Klicken **Einrichtung** in der rechten oberen Ecke von Adobe Workfront in der Symbolleiste für globale Navigation.
1. Klicken **System** > **Voreinstellungen**.

1. Im **Sicherheit** müssen Sie sicherstellen, dass **SAML 2.0-Authentifizierung in Office 365-Add-Ins zulassen** aktiviert ist.

   Diese Option ermöglicht die Einbettung von Workfront in einen Iframe nur für Office 365-Add-Ins. Dadurch wird keine Clickjacking-Verletzung geöffnet, da kein anklickbarer Inhalt beteiligt ist.

   Diese Option ist standardmäßig aktiviert.

   >[!NOTE]
   >
   >Wenn Sie die Option **Einbetten von Workfront in einen iFrame zulassen**, die Option **SAML 2.0-Authentifizierung in Office 365-Add-Ins zulassen** ist abgeblendet und aktiviert.
   >
   >![](assets/if-you-enable.png)

1. Klicken Sie auf **Speichern**.

   Die hier gespeicherten Änderungen wirken sich auf das Erlebnis aller Benutzer in Workfront aus.
