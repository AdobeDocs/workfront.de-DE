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
TQID: 'https://experienceleague.adobe.com/8paS2GIumamOltxTC8Gw2mBZ4bKB6TOgbly7IBPKhDw'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%
---
# Adobe Workfront-Benutzeranmeldeinformationen im Vergleich zu SAML-Benutzeranmeldeinformationen

Dieser Artikel konzentriert sich speziell auf [!DNL Adobe Workfront] und SAML und behandelt keine anderen SSO-Authentifizierungsmethoden.

In einer Datenbank speichert [!DNL Workfront] die E-Mail-Adresse jedes Benutzers als seinen [!DNL Workfront] Benutzernamen zusammen mit seinem [!DNL Workfront]. Diese Anmeldeinformationen werden in die Sandboxes Vorschau und Benutzerdefinierte Aktualisierung repliziert.

Wenn [!DNL Workfront] bei der Benutzererstellung erkennt, dass SAML 2.0 konfiguriert ist, wird für den Benutzer standardmäßig „Nur SAML 2.0-Authentifizierung zulassen“ verwendet. Wenn das Feld „Einladungs-E-Mail an diese Person senden“ aktiviert ist, deaktiviert [!DNL Workfront] „Nur SAML 2.0-Authentifizierung zulassen“ und blendet diese Option aus. Sobald „Einladungs-E-Mail an diese Person senden“ aktiviert ist, wird der Benutzer zu einem Nicht-SAML-[!DNL Workfront].

Nach der Benutzererstellung können Sie den Benutzer bearbeiten und die Option **[!UICONTROL Nur SAML 2.0-Authentifizierung zulassen]** aktivieren, sodass sein Benutzer und sein Kennwort vom SAML-System gesteuert werden.

Danach kann sich der Benutzer nur noch über SAML anmelden. Wenn sie die [!DNL Workfront]-URL aufrufen, werden sie automatisch zum SAML-System weitergeleitet und nach ihrem SAML-Benutzernamen und -Kennwort gefragt.

SAML-Anmeldeinformationen werden in einem externen SAML-System wie dem ADFS von Microsoft gespeichert, nicht in Workfront.
