---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Adobe Workfront-Benutzeranmeldeinformationen vs. [!DNL SAML] Benutzerberechtigungen
description: Nach der Benutzererstellung können Sie den Benutzer bearbeiten und "Nur SAML 2.0-Authentifizierung zulassen"aktivieren, damit dessen Benutzer und Kennwort vom SAML-System gesteuert werden. Wenn diese Option aktiviert ist, darf sich der Benutzer nur über SAML anmelden. Wenn sie zur [!DNL Workfront] URL, werden sie automatisch zum SAML-System umgeleitet und nach ihrem SAML-Benutzernamen und -Passwort gefragt.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Adobe Workfront-Benutzeranmeldeinformationen und SAML-Benutzeranmeldeinformationen

Dieser Artikel konzentriert sich speziell auf [!DNL Adobe Workfront] und SAML und deckt keine anderen SSO-Authentifizierungsmethoden ab.

In einer Datenbank [!DNL Workfront] speichert die E-Mail-Adresse jedes Benutzers als [!DNL Workfront] Benutzername und [!DNL Workfront] Kennwort. Diese Anmeldeinformationen werden in den Sandboxes &quot;Vorschau&quot;und &quot;Benutzerdefinierte Aktualisierung&quot;repliziert.

Bei der Benutzererstellung, wenn [!DNL Workfront] erkennt, dass SAML 2.0 konfiguriert ist, wird für den Benutzer standardmäßig &quot;Nur SAML 2.0-Authentifizierung zulassen&quot;verwendet. Wenn das Feld &quot;Einladungs-E-Mail an diese Person senden&quot;aktiviert ist, [!DNL Workfront] deaktiviert &quot;Nur SAML 2.0-Authentifizierung zulassen&quot;und blendet diese Option aus. Sobald &quot;Einladungs-E-Mail an diese Person senden&quot;aktiviert ist, wird der Benutzer zu einem Nicht-SAML-Benutzer. [!DNL Workfront] Benutzer.

Nach der Benutzererstellung können Sie den Benutzer bearbeiten und aktivieren **[!UICONTROL Nur SAML 2.0-Authentifizierung zulassen]** damit Benutzer und Kennwort vom SAML-System gesteuert werden.

Auf diese Weise kann sich der Benutzer nur über SAML anmelden. Wenn sie zur [!DNL Workfront] URL, werden sie automatisch zum SAML-System umgeleitet und nach ihrem SAML-Benutzernamen und -Passwort gefragt.

SAML-Anmeldeinformationen werden in einem externen SAML-System wie dem ADFS von Microsoft gespeichert, nicht in Workfront.
