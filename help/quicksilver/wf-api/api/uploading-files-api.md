---
content-type: api
navigation-topic: api-navigation-topic
title: Hochladen von Dateien über die API
description: Hochladen von Dateien über die API
author: Becky
feature: Workfront API
role: Developer
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
TQID: https://experienceleague.adobe.com/Yd7byYJ1pYDXwdKvINXh4fKy-pWoEiNMj345jr1HHNs
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 176
ht-degree: 8%

---

# Hochladen von Dateien über die API

Sie können Dateien mithilfe von Workfront-APIs mit API-Tools wie Postman oder mit einfachen cURL-Befehlen hochladen.

Informationen zum Hochladen von Dokumenten finden Sie in den Anweisungen für **Hochladen von Dokumenten** in Workfront [Postverhalten](/help/quicksilver/wf-api/general/api-basics.md#post-behavior). Sie können dieselben Anweisungen auch für cURL-Anfragen verwenden.

**Befolgen Sie beim Hochladen von Dateien mit API-Tools die folgenden Richtlinien:**

* Verwenden Sie die Option Ihres API-Tools, um Ihre Datei hochzuladen. Oft befindet sich auf **Anfragebildschirm die Schaltfläche** Datei auswählen“.

* Verwenden Sie die POST-HTTP-Methode, um die Anfrage zum Hochladen der Datei zu stellen.

* Ihre Anfrage sollte zu einer Antwort führen, die einen Wert für ihr Handle enthält.

* Verwenden Sie den Handle-Wert, den Objekttyp und den GUID-Wert für die objID in einer JSON-Payload, um einen nachfolgenden Aufruf durchzuführen. Dies dient zum Erstellen des -Objekts für Ihre Datei, wie im folgenden Beispiel gezeigt:

```
{
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "1", "fileName" : "TestPDF"},
}
```

Sie sollten in der Antwort eine ID für das -Objekt erhalten.

Weitere Informationen finden Sie in der Hilfe des jeweiligen API-Tools, das Sie verwenden.
