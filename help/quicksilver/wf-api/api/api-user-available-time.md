---
content-type: api
navigation-topic: wf-api
title: Abrufen von Benutzern zur verfügbaren Zeit API
description: Abrufen von Benutzern zur verfügbaren Zeit API
author: Becky
feature: Workfront API
role: Developer
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '94'
ht-degree: 0%

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
