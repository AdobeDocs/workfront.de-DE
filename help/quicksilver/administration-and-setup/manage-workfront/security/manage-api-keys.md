---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: API-Schlüssel verwalten
description: Um Sicherheitslücken in der API zu minimieren, können Adobe Workfront-Admins die API-Schlüssel verwalten, mit denen Anwendungen für einen Benutzerzugriff auf Workfront ermöglicht werden.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: be11c7417023ce2f310fce3e0cf77724d101b89e
workflow-type: tm+mt
source-wordcount: '740'
ht-degree: 17%

---

# API-Schlüssel verwalten

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->



>[!IMPORTANT]
>
>Workfront empfiehlt die Verwendung des `/login`-Endpunkts oder der API-Schlüssel nicht mehr. Verwenden Sie stattdessen eine der folgenden Authentifizierungsmethoden:
>
>* Server-Authentifizierung mit JWT
>* Benutzerauthentifizierung mit OAuth2
>
>Anweisungen zum Einrichten dieser Authentifizierungsmethoden finden Sie unter [Erstellen von OAuth2-Anwendungen für Workfront-Integrationen](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)
>
>Anweisungen zur Verwendung der Server-Authentifizierung in Workfront finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe des JWT-Flusses](/help/quicksilver/wf-api/api/oauth-app-jwt-flow.md)
>
>Anweisungen zur Verwendung der Benutzerauthentifizierung in Workfront finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihrer Organisation mithilfe des Autorisierungs-Code-Flusses](/help/quicksilver/wf-api/api/oauth-app-code-token-flow.md)

Um Sicherheitslücken in der API zu minimieren, können Adobe Workfront-Admins die API-Schlüssel verwalten, mit denen Anwendungen für einen Benutzerzugriff auf Workfront ermöglicht werden.

Sie können Ihren aktuellen Administrator-API-Schlüssel zurücksetzen oder entfernen, API-Schlüssel für den Ablauf konfigurieren und die API-Schlüssel für alle Benutzer entfernen.

Beispiele für Programme, die die Workfront-API nutzen:

* Dokumentenintegrationen wie Dropbox, Google Drive und Workfront DAM
* Workfront Mobile Apps

>[!IMPORTANT]
>
>Beim Zurücksetzen oder Entfernen eines API-Schlüssels muss jede Anwendung, die die Workfront-API nutzt und sich über diesen API-Schlüssel bei Workfront authentifiziert, neu konfiguriert werden, um den Zugriff auf Workfront wiederzuerlangen.

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

## Workfront-API-Schlüssel

Jeder Benutzer in Workfront verfügt über einen eindeutigen API-Schlüssel. Dieser Schlüssel wird pro Benutzer generiert, wenn der Benutzer auf eine Integration zugreift, die die Workfront-API nutzt (z. B. die Workfront Mobile App oder eine Dokumentenintegration).

>[!NOTE]
>
> API-Schlüssel, die Sie in der Produktionsumgebung generieren, werden während der wöchentlichen Aktualisierung in Ihre Vorschau-Umgebung kopiert. Alle API-Schlüssel, die Sie in der Vorschau-Umgebung generieren, werden während der wöchentlichen Aktualisierung mit Ihren Produktions-API-Schlüsseln überschrieben.

Workfront-Administratoren verfügen außerdem über einen eindeutigen API-Schlüssel. Wenn eine Anwendung einen Administrator-API-Schlüssel für den Zugriff auf Workfront verwendet, hat die Anwendung Administratorzugriff auf Workfront.

## Administrator-API-Schlüssel verwalten

Sie können den API-Schlüssel für Ihr Administrator-Benutzerkonto generieren, zurücksetzen oder entfernen.

{{step-1-to-setup}}

1. Klicken Sie auf **System >** **Kundeninformationen.**
1. (Bedingt) Führen Sie eine der folgenden Aktionen aus:

   So generieren Sie einen API-Schlüssel: Klicken Sie **Abschnitt** API-Schlüsseleinstellungen **auf API-Schlüssel generieren**.

   ODER\
   Zurücksetzen eines API-Schlüssels: Klicken Sie im Abschnitt **API** Schlüsseleinstellungen“ auf **Zurücksetzen** und dann auf **Zurücksetzen.**

   ODER

   So entfernen Sie den API-Schlüssel: Klicken Sie im Abschnitt **API** Schlüsseleinstellungen **auf „Entfernen** und dann auf **Entfernen**.

<!--

   Remove me October 2026

## Generate an API Key for Non-Admin Users

You can generate and manage API Keys for users in roles other than Workfront administrator.

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

1. (Conditional) If your organization uses Single Sign-On (SSO) access management, temporarily disable the option requiring SSO authentication.

   {{step-1-to-setup}} 
   
   1. Expand **System**, then click **Single Sign-on (SSO)**. 
   1. In the **Type** field, select the type of SSO your organization uses.
   1. With the type selected, scroll down and clear the **Enable** checkbox. 
      ![Enable SSO](assets/sysadmin-security-sso-disable-31620-350x320.png)  
   1. Click **Save**.


1. In the address bar of a browser, enter the following API call:

   `<domain>`.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&username=**username**&password=**password**&method=PUT

   Replace `<domain>` with your Workfront domain name, and username and password with the user's Workfront credentials.

1. (Conditional) Enable the option requiring SSO authentication if you disabled it in Step 1.

   {{step-1-to-setup}}
   
   1. Expand **System**, then click **Single Sign-on (SSO)**.
   
   1. Select your SSO method in the **Type** drop down menu.
   1. Check the checkbox requiring SSO authentication.

   -->

## Konfigurieren, wann API-Schlüssel ablaufen

Sie können API-Schlüssel so konfigurieren, dass sie für alle Benutzer in Ihrem System ablaufen. Wenn der API-Schlüssel einer Benutzerin oder eines Benutzers abläuft, muss sich die Benutzerin bzw. der Benutzer erneut bei allen Anwendungen authentifizieren, die die Workfront-API für den Zugriff auf Workfront verwenden. Sie können die Häufigkeit ändern, mit der die API-Schlüssel ablaufen. Sie können auch konfigurieren, ob API-Schlüssel ablaufen, wenn das Kennwort eines Benutzers abläuft.

{{step-1-to-setup}}

1. Klicken Sie **System** > **Kundeninformationen**.
1. Wählen Sie im Bereich **API** Schlüsseleinstellungen in der Dropdown-Liste **Nach** Erstellung **API-Schlüssel laufen ab in** den Zeitrahmen aus, in dem die API-Schlüssel ablaufen sollen.

   Wenn Sie diese Option ändern, beginnt der neue Zeitrahmen ab dem Zeitpunkt, an dem Sie die Änderung vorgenommen haben. Wenn Sie diese Option beispielsweise von *1 Monat* auf *6 Monate* ändern, laufen die API-Schlüssel 6 Monate nach der Änderung ab.

   Standardmäßig laufen API-Schlüssel jeden Monat ab.

1. Um API-Schlüssel so zu konfigurieren, dass sie zum Zeitpunkt des Ablaufs der Benutzerkennwörter ablaufen, aktivieren Sie **API-Schlüssel entfernen, wenn das Kennwort eines Benutzers abläuft**.

   Standardmäßig ist diese Option nicht aktiviert.

   Informationen zum Konfigurieren von Benutzerkennwörtern für den Ablauf finden Sie unter [Konfigurieren von Systemsicherheitseinstellungen](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

1. Klicken Sie auf **Speichern**.

## API-Schlüssel für alle Benutzer entfernen

Wenn Sie wegen einer bestimmten Sicherheitsverletzung in Bezug auf Ihr Workfront-System besorgt sind, können Sie API-Schlüssel gleichzeitig für alle Benutzer entfernen.

>[!IMPORTANT]
>
>Das Entfernen von API-Schlüsseln für alle Benutzer macht ALLE API-Schlüssel für alle Benutzer im System ungültig. Diese Aktion führt dazu, dass alle Ihre Integrationen in Workfront fehlschlagen, bis Sie einen neuen API-Schlüssel in Workfront generieren und alle Ihre Integrationen aktualisieren.

{{step-1-to-setup}}

1. Erweitern Sie **System** und klicken Sie dann auf **Kundeninformationen**.

1. Klicken Sie im Bereich **API** Schlüsseleinstellungen auf **Alle API-Schlüssel entfernen** und klicken Sie dann auf **Entfernen** **Alle**.

<!--

Remove me October 2026

## Restricting API logins with an X.509 certificate

>[!IMPORTANT]
>
>The procedure described in this section applies only to organizations that have not yet been onboarded to the Adobe Business Platform. Logging in to Workfront through the Workfront API is not available if your organization has been onboarded to the Adobe Business Platform.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see [Administration differences between Adobe Workfront and Adobe Business Platform](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

Third-party applications can communicate with Workfront through the API. To increase the security of your Workfront site, you can configure Workfront to restrict API login requests by uploading an X.509 certificate to Workfront. Once enabled, all login requests through the API must include a client certificate in addition to username and password.

* [Obtain the X.509 certificate](#obtain-the-x-509-certificate) 
* [Upload the certificate to Workfront](#upload-the-certificate-to-workfront) 
* [Verify API login calls are restricted](#verify-api-login-calls-are-restricted)

### Obtain the X.509 certificate {#obtain-the-x-509-certificate}

Obtain a valid X.509 certificate from a trusted Certificate Authority (such as Verisign), and save it to a temporary location on your workstation. 

### Upload the certificate to Workfront {#upload-the-certificate-to-workfront}

After you have obtained the X.509 certificate from your Certificate Authority, you need to upload it to Workfront.

1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).  

1. Expand **System**, then click **Customer Info**.

1. In the **API Key Settings** area, select **Require X.509 Certificate for API logins**.
1. Click **Change Certificate**.
1. On your workstation, browse to and select the X.509 certificate that you previously downloaded.
1. (Optional) Click **View Details** next to the certificate name to view the following details about the certificate:

   * Subject Common Name
   * Subject Organization
   * Subject Organization Unit
   * Issuer Common Name
   * Issuer Organization
   * Issuer Organization Unit
   * Serial Number
   * Issue Date
   * Expiration Date

1. Click **Save**. 

### Verify API login calls are restricted {#verify-api-login-calls-are-restricted}

Prior to configuring your instance of Workfront to require an X.509 certificate, perform an API request to the `/login` endpoint using valid username and password parameters. You will receive a 200 response that contains a sessionID.

After making the X.509 certificate a requirement via the customer info page in your instance of Workfront, make another login attempt. This time you will receive a 500 error response with the following message: "Untrusted request. Please contact your system administrator and attach certificate."

After confirming that the X.509 certificate is required, perform the same login request with an additional parameter for apiCertificate set to the value of your certificate. If this operation was performed correctly you will receive a 200 response that contains a valid sessionID.

-->
