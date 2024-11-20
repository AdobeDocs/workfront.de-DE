---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ZScalar-Einstellungen können zu Leistungseinbußen führen
description: Nach der Benutzererstellung können Sie den Benutzer bearbeiten und "Nur SAML 2.0-Authentifizierung zulassen"aktivieren, damit dessen Benutzer und Kennwort vom SAML-System gesteuert werden. Wenn diese Option aktiviert ist, darf sich der Benutzer nur über SAML anmelden.
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: 806a4c4835e47da4fbbdb28ec0c35c990f70239e
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Workfront: ZScalar-Einstellungen können zu Leistungseinbußen führen

>[!NOTE]
>
>Dies ist ein Problem mit ZScalar und wird von Workfront nicht behoben.

Der Webdienst von ZScalar verwendet standardmäßig `http/1.1`, was zu Leistungseinbußen in Workfront führen kann.

Um dieses Problem zu überprüfen und zu beheben, konfigurieren Sie Ihre ZScalar-Software für die Verwendung von `http/2`. Dies kann nicht in Workfront konfiguriert werden.

Informationen zu `http/2` finden Sie in der ZScalar-Dokumentation.
