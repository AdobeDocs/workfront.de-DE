---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Dokument-Webhooks – Fehlerbehandlung
description: Dokument-Webhooks – Fehlerbehandlung
author: Becky
feature: Workfront API
role: Developer
exl-id: 6e0f3be7-5321-44bd-a404-d5bef1462d82
TQID: https://experienceleague.adobe.com/KoMJXXZbDdywLGIwYTu7o8GigPxQ5RG6sNQpOTMHWY0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 123
ht-degree: 9%

---

# Dokument-Webhooks – Fehlerbehandlung

Bei der Verarbeitung von API-Anfragen können Probleme auftreten. Dies sollte über alle API-Endpunkte hinweg konsistent gehandhabt werden. Wenn ein Fehler auftritt, sollte der Webhook-Anbieter einen Fehlercode in die Antwort-Kopfzeile aufnehmen. Zu den Fehlercodes gehören:

* 403 - Verboten. Gibt an, dass entweder die Anfrage-Token fehlen oder ungültig sind oder dass mit den Token verknüpfte Anmeldeinformationen keinen Zugriff auf die angegebene Ressource haben. Bei OAuth-basierten Webhook-Anbietern versucht Adobe Workfront, neue Zugriffstoken abzurufen.

* 404 - Nicht gefunden. Gibt an, dass die angegebene Datei oder der angegebene Ordner nicht vorhanden ist.

* 500 - Interner Server-Fehler. Jede andere Fehlerart.

* Beschreibung des Fehlers im Antworttext im folgenden Format:

  ```
  {status: "error"
   error: "Sample error message"}
  ```
