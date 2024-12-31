---
content-type: api
navigation-topic: api-navigation-topic
title: Hochladen von Dateien über die API
description: Hochladen von Dateien über die API
author: Becky
feature: Workfront API
role: Developer
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# Hochladen von Dateien über die API

Sie können Dateien mithilfe von Workfront-APIs mit API-Tools wie Postman oder mit einfachen cURL-Befehlen hochladen.

Informationen zum Hochladen von Dokumenten finden Sie in den Anweisungen für **Hochladen von Dokumenten** in Workfront [Postverhalten](/help/quicksilver/wf-api/general/api-basics.md#post-behavior). Sie können dieselben Anweisungen auch für cURL-Anfragen verwenden.

**Befolgen Sie beim Hochladen von Dateien mit API-Tools die folgenden Richtlinien:**

* Verwenden Sie die Option Ihres API-Tools, um Ihre Datei hochzuladen. Dabei handelt es sich häufig um **Schaltfläche „Datei auswählen** auf dem Anfragebildschirm.

* Verwenden Sie die HTTP-Methode der POST , um die Anfrage zum Hochladen der Datei zu stellen.

* Ihre Anfrage sollte zu einer Antwort führen, die einen Wert für ihr Handle enthält.

* Verwenden Sie den Handle-Wert, den Objekttyp und den GUID-Wert für die objID in einer JSON-Payload, um einen nachfolgenden Aufruf durchzuführen. Dies dient zum Erstellen des -Objekts für Ihre Datei, wie im folgenden Beispiel gezeigt:

```
}
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "v1.0", "fileName" : "TestPDF"},
}
```

Sie sollten in der Antwort eine ID für das -Objekt erhalten.

Weitere Informationen finden Sie in der Hilfe des jeweiligen API-Tools, das Sie verwenden.
