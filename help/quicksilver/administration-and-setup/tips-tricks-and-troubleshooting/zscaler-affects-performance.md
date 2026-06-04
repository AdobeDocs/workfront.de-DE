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
TQID: https://experienceleague.adobe.com/-3-p8fzXIiV-gnjIjhRzBmLfspAEEVAuD2lpmcsVjLA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 107
ht-degree: 44%

---

# Workfront: ZScaler-Einstellungen können die Leistung beeinträchtigen

>[!NOTE]
>
>Dies ist ein Problem mit ZScaler und wird von Workfront nicht behoben.

Der Web-Dienst von ZScaler verwendet standardmäßig `http/1.1`, was zu Leistungseinbußen in Workfront führen kann.

Um dieses Problem zu überprüfen und zu beheben, konfigurieren Sie Ihre ZScaler-Software für die Verwendung von `http/2`. Dies kann nicht in Workfront konfiguriert werden.

Informationen zu `http/2` finden Sie in der Dokumentation zu ZScaler.
