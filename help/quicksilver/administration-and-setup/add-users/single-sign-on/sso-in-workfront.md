---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Überblick über Single Sign-on in Adobe Workfront
description: Workfront bietet eine zentral verwaltete SSO-Konfiguration (Single Sign-on), die Workfront einfach in Ihre bestehende SSO-Lösung integriert. Diese Konfiguration ist einfach einzurichten und zu verwalten und steht sowohl OnDemand- als auch OnPremise-Unternehmenskunden zur Verfügung.
author: Caroline, Becky
feature: System Setup and Administration
role: Admin
exl-id: 87f1b6c0-6b74-4eac-87cd-899b1c74af25
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---

# Überblick über Single Sign-on in Adobe Workfront

{{important-admin-console-onboard}}


Workfront bietet eine zentral verwaltete SSO-Konfiguration (Single Sign-on), die Workfront einfach in Ihre bestehende SSO-Lösung integriert. Diese Konfiguration ist einfach einzurichten und zu verwalten und steht sowohl OnDemand- als auch OnPremise-Unternehmenskunden zur Verfügung.

Um die SSO-Funktion in Workfront verwenden zu können, muss Ihr Unternehmen eine SSO-Anwendung einrichten. Anschließend können Sie Workfront so konfigurieren, dass es mit Ihrer SSO-Lösung kommunizieren kann.

Federated-Lösungen ermöglichen es Benutzern, sich bei allen Anwendungen anzumelden, indem sie ihren Benutzernamen und ihr Passwort in einem zentralen Anmeldeportal eingeben.

![](assets/overview-sso-wf.png)


## Konfigurieren der Firewall

Bei Verwendung einer SSO-Lösung initiiert Workfront eine Verbindung zu Ihrem Server an dem angegebenen Port.

Wenn Sie Workfront On-Demand abonnieren und Ihre Firewall oder Ihren E-Mail-Server so konfiguriert haben, dass nur bestimmte Anbieter Zugriff erhalten, müssen Sie bestimmte Workfront-IP-Adressen zu Ihrer Firewall-Zulassungsliste hinzufügen. Weitere Informationen finden Sie unter [Konfigurieren der Zulassungsliste Ihrer Firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Single Sign-on konfigurieren

Workfront ist mit den folgenden SSO-Lösungen integriert:

* Federated-Lösungen, die SAML 2.0 unterstützen

   Informationen zur Integration von Workfront in SAML 2.0 finden Sie unter [Konfigurieren von Adobe Workfront mit SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

* Federated-Lösungen, die SAML 2.0 mit ADFS unterstützen

   Informationen zur Integration von Workfront in SAML 2.0 mithilfe von ADFS finden Sie unter [Konfigurieren von Adobe Workfront mit SAML 2.0 mithilfe von ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
