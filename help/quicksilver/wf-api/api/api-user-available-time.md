---
content-type: api
navigation-topic: wf-api
title: Verfügbare Zeit-API für Benutzer abrufen
description: Verfügbare Zeit-API für Benutzer abrufen
author: Becky
feature: Workfront API
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '94'
ht-degree: 7%

---

# Verfügbare Zeit-API

**URI: attask/api/v15.0/user/getUsersAvailableTime**

Der verfügbare Zeit-Endpunkt der Benutzer ruft Daten zur verfügbaren Zeit des Benutzers ab. Dies ermöglicht Integrationen zur Aggregation von Daten entsprechend Benutzerattributen und Zeitintervallen.

## Beispielanfrage

`curl -XPUT /attask/api/v15.0/user/getUsersAvailableTime`

## Anforderungsparameter

* **userIDs**: Array von Zeichenfolgen. Erforderlich. Beispiel: `"61a9cc0500002f9fdaa7a6f824f557e1"`.

* **fromDate**: datetime. Zeichenfolge. Erforderlich. Beispiel:  `"2022-07-10T00:00:00"`.

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

* **AVL**: Tatsächliche verfügbare Stunden. Array von Zahlen.
* **PAVL**: Reine verfügbare Stunden für die Planung, die keine Arbeits- oder Benutzerzeit beinhalten. Zeichenfolge.
