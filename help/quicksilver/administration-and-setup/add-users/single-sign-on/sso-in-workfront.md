---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Übersicht über Single Sign-On in Adobe Workfront
description: Workfront bietet eine zentral verwaltete SSO-Konfiguration (Single Sign-on), die Workfront einfach in Ihre bestehende SSO-Lösung integriert. Diese Konfiguration ist einfach einzurichten und zu verwalten und steht Kunden von OnDemand und OnPremise Enterprise zur Verfügung.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 87f1b6c0-6b74-4eac-87cd-899b1c74af25
source-git-commit: a54200ceeaadfeaac6767f06676cb11814959601
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---

# Überblick über Single Sign-on in Adobe Workfront

<!--Audited: 12/2023-->

{{important-admin-console-onboard}}


Workfront bietet eine zentral verwaltete SSO-Konfiguration (Single Sign-on), die Workfront in Ihre bestehende SSO-Lösung integriert. Diese Konfiguration ist für OnDemand- und OnPremise-Unternehmenskunden verfügbar.

Um die SSO-Funktion in Workfront verwenden zu können, muss Ihr Unternehmen eine SSO-Anwendung einrichten. Anschließend können Sie Workfront so konfigurieren, dass es mit Ihrer SSO-Lösung kommunizieren kann.

Federated-Lösungen ermöglichen es Benutzern, sich bei allen Anwendungen anzumelden, indem sie ihren Benutzernamen und ihr Passwort in einem zentralen Anmeldeportal eingeben.

![](assets/overview-sso-wf-fed-only.png)


## Konfigurieren der Firewall

Bei Verwendung einer SSO-Lösung initiiert Workfront eine Verbindung zu Ihrem Server an dem angegebenen Port.

Wenn Ihre Firewall oder Ihr E-Mail-Server so konfiguriert ist, dass nur bestimmte Anbieter Zugriff erhalten, müssen Sie bestimmte Workfront IP-Adressen zu Ihrer Firewall-Zulassungsliste hinzufügen. Weitere Informationen finden Sie unter [Konfigurieren der Zulassungsliste Ihrer Firewall-](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Single Sign-on konfigurieren

Workfront ist mit den folgenden SSO-Lösungen integriert:

* Federated-Lösungen, die SAML 2.0 unterstützen

  Informationen zur Integration von Workfront in SAML 2.0 finden Sie unter [Adobe Workfront mit SAML 2.0 konfigurieren](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

* Federated-Lösungen, die SAML 2.0 mit ADFS unterstützen

  Informationen zur Integration von Workfront in SAML 2.0 mithilfe von ADFS finden Sie unter [Adobe Workfront mit SAML 2.0 mit ADFS konfigurieren](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
