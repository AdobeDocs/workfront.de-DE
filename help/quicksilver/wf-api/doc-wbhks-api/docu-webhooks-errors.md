---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Umgang mit Fehlern bei Document Webhooks
description: Umgang mit Fehlern bei Document Webhooks
author: Becky
feature: Workfront API
role: Developer
exl-id: 6e0f3be7-5321-44bd-a404-d5bef1462d82
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 0%

---

# Umgang mit Fehlern bei Document Webhooks

Bei der Verarbeitung von API-Anfragen können Probleme auftreten. Dies sollte über alle API-Endpunkte hinweg einheitlich gehandhabt werden. Wenn ein Fehler auftritt, sollte der Webhook-Provider einen Fehlercode in die Antwortheader aufnehmen. Zu den Fehlercodes gehören:

* 403 - Verboten. Gibt an, dass entweder die Anfrage-Token fehlen oder ungültig sind oder dass die mit den Token verknüpften Anmeldeinformationen keinen Zugriff auf die angegebene Ressource haben. Bei OAuth-basierten Webhook-Anbietern versucht Adobe Workfront, neue Zugriffstoken abzurufen.

* 404 - Nicht gefunden. Gibt an, dass die angegebene Datei oder der angegebene Ordner nicht vorhanden ist.

* 500 - Interner Server-Fehler. Jeder andere Fehlertyp.

* Beschreibung des Fehlers im Antworttext im folgenden Format:

  ```
  {status: "error"
   error: "Sample error message"}
  ```
