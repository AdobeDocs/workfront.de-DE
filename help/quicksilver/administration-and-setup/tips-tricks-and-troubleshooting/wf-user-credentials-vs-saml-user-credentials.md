---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Adobe Workfront-Benutzeranmeldeinformationen im Vergleich zu SAML-Benutzeranmeldeinformationen
description: Nach der Benutzererstellung können Sie den Benutzer bearbeiten und „Nur SAML 2.0-Authentifizierung zulassen“ aktivieren, sodass sein Benutzer und sein Kennwort vom SAML-System gesteuert werden. Wenn diese Option aktiviert ist, darf sich der Benutzer nur über SAML anmelden.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Adobe Workfront-Benutzeranmeldeinformationen im Vergleich zu SAML-Benutzeranmeldeinformationen

Dieser Artikel konzentriert sich speziell auf [!DNL Adobe Workfront] und SAML und behandelt keine anderen SSO-Authentifizierungsmethoden.

In einer Datenbank speichert [!DNL Workfront] die E-Mail-Adresse jedes Benutzers als seinen [!DNL Workfront] Benutzernamen zusammen mit seinem [!DNL Workfront]. Diese Anmeldeinformationen werden in die Sandboxes Vorschau und Benutzerdefinierte Aktualisierung repliziert.

Wenn [!DNL Workfront] bei der Benutzererstellung erkennt, dass SAML 2.0 konfiguriert ist, wird für den Benutzer standardmäßig „Nur SAML 2.0-Authentifizierung zulassen“ verwendet. Wenn das Feld „Einladungs-E-Mail an diese Person senden“ aktiviert ist, deaktiviert [!DNL Workfront] „Nur SAML 2.0-Authentifizierung zulassen“ und blendet diese Option aus. Sobald „Einladungs-E-Mail an diese Person senden“ aktiviert ist, wird der Benutzer zu einem Nicht-SAML-[!DNL Workfront].

Nach der Benutzererstellung können Sie den Benutzer bearbeiten und die Option **[!UICONTROL Nur SAML 2.0-Authentifizierung zulassen]** aktivieren, sodass sein Benutzer und sein Kennwort vom SAML-System gesteuert werden.

Danach kann sich der Benutzer nur noch über SAML anmelden. Wenn sie die [!DNL Workfront]-URL aufrufen, werden sie automatisch zum SAML-System weitergeleitet und nach ihrem SAML-Benutzernamen und -Kennwort gefragt.

SAML-Anmeldeinformationen werden in einem externen SAML-System wie dem ADFS von Microsoft gespeichert, nicht in Workfront.
