---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ZScaler-Einstellungen können die Leistung beeinträchtigen
description: Nach der Benutzererstellung können Sie den Benutzer bearbeiten und „Nur SAML 2.0-Authentifizierung zulassen“ aktivieren, sodass sein Benutzer und sein Kennwort vom SAML-System gesteuert werden. Wenn diese Option aktiviert ist, darf sich der Benutzer nur über SAML anmelden.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 2752a9e2-44fe-49b5-a7ab-4021d91ed37b
source-git-commit: f66b219e9fd203f108844ad397bcfa848b8f1134
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Workfront: ZScaler-Einstellungen können die Leistung beeinträchtigen

>[!NOTE]
>
>Dies ist ein Problem mit ZScaler und wird von Workfront nicht behoben.

Der Webdienst von ZScaler verwendet standardmäßig `http/1.1`, was zu Leistungseinbußen in Workfront führen kann.

Um dieses Problem zu überprüfen und zu beheben, konfigurieren Sie Ihre ZScaler-Software für die Verwendung von `http/2`. Dies kann nicht in Workfront konfiguriert werden.

Informationen zu `http/2` finden Sie in der ZScaler-Dokumentation.
