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

Sie können Dateien mit Workfront-APIs mit API-Tools wie Postman oder mit einfachen cURL-Befehlen hochladen.

Informationen zum Hochladen von Dokumenten finden Sie in den Anweisungen unter **Hochladen von Dokumenten** in Workfront [Verhalten des Beitrags](/help/quicksilver/wf-api/general/api-basics.md#post-behavior). Sie können diese Anweisungen auch für cURL-Anfragen verwenden.

**Befolgen Sie beim Hochladen von Dateien mithilfe von API-Tools die folgenden Richtlinien:**

* Verwenden Sie Ihre API-Tool-Option, um Ihre Datei hochzuladen. Dies ist häufig ein **Datei auswählen** auf dem Anfragebildschirm.

* Verwenden Sie die POST-HTTP-Methode, um die Anfrage zum Hochladen der Datei zu stellen.

* Ihre Anfrage sollte zu einer Antwort führen, die einen Wert für das Handle enthält.

* Verwenden Sie den Handle-Wert, den Objekttyp und den GUID-Wert für die objID in einer JSON-Payload, um einen nachfolgenden Aufruf durchzuführen. Dies dient zum Erstellen des Objekts für Ihre Datei, wie im folgenden Beispiel gezeigt:

```
}
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "v1.0", "fileName" : "TestPDF"},
}
```

Sie sollten eine ID für das -Objekt in der Antwort erhalten.

Weitere Informationen finden Sie in der Hilfe des jeweiligen API-Tools, das Sie verwenden.
