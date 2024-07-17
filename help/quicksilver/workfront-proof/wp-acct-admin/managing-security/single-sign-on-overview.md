---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: Single Sign-On in [!DNL Workfront Proof]
description: Single Sign-On (SSO) ermöglicht es Ihren Benutzern, sich mit dem vorhandenen Benutzernamen und Kennwort Ihres Unternehmens bei [!DNL Workfront Proof] anzumelden.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb1f6883-6209-4a55-b181-67af4b496ca0
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# Single Sign-On in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Für die Verwendung dieser Funktion ist ein [!UICONTROL Enterprise] [!DNL Workfront] -Plan erforderlich. Weitere Informationen zu den verschiedenen verfügbaren Plänen finden Sie unter [Workfront-Pläne](https://www.workfront.com/plans).

Single Sign-On (SSO) ermöglicht es Ihren Benutzern, sich mit dem vorhandenen Benutzernamen und Kennwort Ihres Unternehmens bei [!DNL Workfront Proof] anzumelden.

Um diese Funktion bereitzustellen, verwenden wir [!DNL Security Assertion Markup Language] (SAML) 2.0, ein XML-basiertes Protokoll, mit dem Sie Daten autorisieren und die Authentifizierung zwischen einem Identitäts-Provider und einem Webdienst austauschen können.

Dies bedeutet, dass Sie sich bei Ihrem eigenen Anmeldesystem authentifizieren, nicht bei der Anmeldeseite von [!DNL Workfront Proof].

Sie müssen in Ihrem [!DNL Workfront] Testkonto über benutzerdefinierte Sub-Domains oder Domänen verfügen, um SAML zu aktivieren:

<!--* Custom sub-domains are free to set up. See our [Configure a branded domain in Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/configure-branded-domain-in-wp.md) for more information.-->
* Weitere Informationen zu vollständig angepassten Domänen finden Sie in der [Marke der [!DNL Workfront Proof] Site - erweitert](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

Informationen zum Einrichten von SSO in Ihrem Konto finden Sie unter [Konfigurieren von Single Sign-On für  [!DNL Workfront Proof] Benutzer](../../../workfront-proof/wp-acct-admin/account-settings/configure-sso-for-wp-users.md) .
