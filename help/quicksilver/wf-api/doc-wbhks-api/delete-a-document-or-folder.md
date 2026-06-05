---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Dokument oder Ordner löschen
description: Dokument oder Ordner löschen
author: Becky
feature: Workfront API
role: Developer
exl-id: b56ec13a-1ee1-4bef-b39b-e625d00e4952
TQID: https://experienceleague.adobe.com/7-f8Z3qQQ2z7ZHHfSrGgJqIQCKdeqEoL96XlfCGzYSo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 75
ht-degree: 20%

---

# Löschen eines Dokuments oder eines Ordners (noch nicht implementiert)

Löscht ein Dokument oder einen Ordner mit der angegebenen ID im externen System. Beim Löschen eines Ordners werden auch die Ordnerinhalte gelöscht.

## URL

PUT/delete

## Abfrageparameter

| Name  | Beschreibung |
|---|---|
| documentId  | Die zu löschende Dokument-ID |
| folderId  |  Die zu löschende Ordner-ID |



## Antwort

Eine JSON-Zeichenfolge, die Erfolg oder Fehler anzeigt, wie im Abschnitt Fehlerbehandlung unten angegeben.

### Beispiel

```
PUT https://www.example.com/api/deleteid=1234

* returns `status: "success"`

* returns `status: "failure", error: "File not found"`
```
