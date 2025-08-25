---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Übersicht über Single Sign-On in Adobe Workfront
description: Workfront bietet eine zentral verwaltete Single Sign-On (SSO)-Konfiguration, die Workfront einfach in Ihre bestehende SSO-Unternehmenslösung integriert. Diese Konfiguration lässt sich einfach einrichten und verwalten und steht sowohl OnDemand- als auch OnPremise-Unternehmenskunden zur Verfügung.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 87f1b6c0-6b74-4eac-87cd-899b1c74af25
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# Übersicht über Single Sign-on in Adobe Workfront

<!--Audited: 12/2023-->

{{important-admin-console-onboard}}


Workfront bietet eine zentral verwaltete Single-Sign-On-Konfiguration (SSO), die Workfront in Ihre bestehende SSO-Unternehmenslösung integriert. Diese Konfiguration ist sowohl für OnDemand- als auch für OnPremise Enterprise-Kunden verfügbar.

Um die SSO-Funktion in Workfront verwenden zu können, muss Ihr Unternehmen eine SSO-Anwendung einrichten. Anschließend können Sie Workfront so konfigurieren, dass es mit Ihrer SSO-Lösung kommunizieren kann.

Federated Solutions ermöglichen es Benutzern, sich bei all ihren Anwendungen anzumelden, indem sie ihren Benutzernamen und ihr Passwort in einem zentralen Anmeldeportal eingeben.

![SSO Federated](assets/overview-sso-wf-fed-only.png)


## Firewall konfigurieren

Bei Verwendung einer SSO-Lösung initiiert Workfront eine Verbindung zu Ihrem Server über den angegebenen Port.

Wenn Ihr Firewall- oder Mailserver so konfiguriert ist, dass er nur bestimmten Anbietern Zugriff gewährt, müssen Sie bestimmte Workfront-IP-Adressen zu Ihrer Firewall-Zulassungsliste hinzufügen. Weitere Informationen finden Sie [Zulassungsliste zum Konfigurieren der Firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Konfigurieren von Single Sign-on

Workfront lässt sich mit den folgenden SSO-Lösungen integrieren:

* Federated Solutions, die SAML 2.0 unterstützen

  Informationen zur Integration von Workfront mit SAML 2.0 finden Sie unter [Konfigurieren von Adobe Workfront mit SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

* Federated Solutions, die SAML 2.0 mit ADFS unterstützen

  Informationen zur Integration von Workfront mit SAML 2.0 mithilfe von ADFS finden Sie unter [Konfigurieren von Adobe Workfront mit SAML 2.0 mithilfe von ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
