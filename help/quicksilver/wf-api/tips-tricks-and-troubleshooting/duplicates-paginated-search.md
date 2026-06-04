---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Bei einer großen paginierten Suche zurückgegebene Duplikate
description: Bei einer großen paginierten Suche zurückgegebene Duplikate
author: Becky
feature: Workfront API
role: Developer
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
TQID: https://experienceleague.adobe.com/1FXTHSro-rlUVHaajM1monR2Y-sxVHN6KIviogoXqRc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 111
ht-degree: 20%

---

# Bei einer großen paginierten Suche zurückgegebene Duplikate

## Problem

Bei der Durchführung einer großen paginierten Suche in der API nach einem Objekt erhält der Kunde doppelte Einträge und fehlende Datensätze.

## Lösung

Wenn die Reihenfolge nicht formal definiert ist, verlassen wir uns auf die Reihenfolge der Zeilen, die von der Oracle-Datenbank zurückgegeben werden, was keine deterministische Reihenfolge garantiert. Beispielsweise können zwei aufeinander folgende Aufrufe mit derselben Abfrage Zeilen in einer anderen Reihenfolge zurückgeben. Ebenso können beim Paging die Zeilen nach dem Zufallsprinzip verschiedenen „Seiten“ zugewiesen werden, was zu Duplikaten führt. Die einfachste Lösung besteht darin, eine Sortierung nach ID hinzuzufügen:

```
&ID_Sort=asc
```

