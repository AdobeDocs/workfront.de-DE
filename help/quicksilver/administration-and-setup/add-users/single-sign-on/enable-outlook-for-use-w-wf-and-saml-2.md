---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Outlook für die Verwendung mit Workfront und SAML 2.0 aktivieren
description: Wenn Sie die SAML 2.0-Authentifizierung aktivieren und möchten, dass sich Ihre Benutzer über Microsoft Outlook mit ihren SAML 2.0-Anmeldeinformationen bei Workfront anmelden können, müssen Sie SAML 2.0 aktivieren, um sich in Office-Add-Ins zu authentifizieren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 8a55d364-962a-4eef-8968-b2233a71cf31
source-git-commit: a54200ceeaadfeaac6767f06676cb11814959601
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 0%

---

# Outlook für die Verwendung mit Workfront und SAML 2.0 aktivieren

Wenn Sie die SAML 2.0-Authentifizierung aktivieren und möchten, dass sich Ihre Benutzer über Microsoft Outlook mit ihren SAML 2.0-Anmeldeinformationen bei Workfront anmelden können, müssen Sie SAML 2.0 aktivieren, um sich in Office-Add-Ins zu authentifizieren.

>[!NOTE]
>
>Dies ist nicht verfügbar, wenn die Workfront-Instanz Ihres Unternehmens ein benutzerdefiniertes SSO-Portal verwendet.>
><!--
>or is enabled with Adobe IMS>
>-->
>Wenden Sie sich an Ihren Netzwerk- oder IT-Administrator, wenn Sie weitere Informationen benötigen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Outlook für die Verwendung mit Workfront und SAML 2.0 aktivieren

{{step-1-to-setup}}

1. Klicken Sie auf **System** > **Voreinstellungen**.

1. Stellen Sie im Abschnitt **Sicherheit** sicher, dass die Option **SAML 2.0-Authentifizierung in Office 365-Add-Ins zulassen** aktiviert ist.

   Diese Option ermöglicht die Einbettung von Workfront in einen Iframe nur für Office 365-Add-Ins. Dadurch wird keine Clickjacking-Verletzung geöffnet, da kein anklickbarer Inhalt beteiligt ist.

   Diese Option ist standardmäßig aktiviert.

   >[!NOTE]
   >
   >Wenn Sie die Option **Einbetten von Workfront in einen iframe zulassen** aktivieren, ist die Option **SAML 2.0-Authentifizierung in Office 365-Add-Ins zulassen** abgeblendet und aktiviert.
   >
   >![](assets/if-you-enable.png)
   >

1. Klicken Sie auf **Speichern**.

   Die hier gespeicherten Änderungen wirken sich auf das Erlebnis aller Benutzer in Workfront aus.
