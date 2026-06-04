---
content-type: api
navigation-topic: wf-api
title: Abrufen von Benutzern zur verfügbaren Zeit API
description: Abrufen von Benutzern zur verfügbaren Zeit API
author: Becky
feature: Workfront API
role: Developer
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
TQID: https://experienceleague.adobe.com/JPvalH2RQRfMeqbYyWXyjyXCx-bdaZwRoR6WDRerZ5U
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 95
ht-degree: 8%

---

# API für verfügbare Benutzende

**URI: attask/api/v15.0/user/getUsersAvailableTime**

Der Endpunkt für die verfügbare Zeit des Benutzers ruft Daten zur verfügbaren Zeit des Benutzers ab. Dies ermöglicht Integrationen für die Aggregation von Daten anhand von Benutzerattributen und Zeitintervallen.

## Beispielanfrage

`curl -XPUT /attask/api/v15.0/user/getUsersAvailableTime`

## Anfrageparameter

* **userIDs**: Array von Zeichenfolgen. Erforderlich. Beispiel: `"61a9cc0500002f9fdaa7a6f824f557e1"`.

* **fromDate**: datetime. Zeichenfolge. Erforderlich. Beispiel: `"2022-07-10T00:00:00"`.

* **toDate**: datetime. Zeichenfolge. Erforderlich. Beispiel `"2022-07-20T23:59:59"`.

## Beispielantwort:

```
{
    "data": {
        "result": {
            "PAVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            },
            "AVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    480.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            }
        }
    }
}
```

## Antwortparameter

* **AVL**: Tatsächlich verfügbare Stunden. Array von Zahlen.
* **PAVL**: Reine verfügbare Stunden für die Planung, die keine arbeitsfreien Tage oder Ausfallzeiten von Benutzenden beinhalten. Zeichenfolge.
