---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Bei einer großen paginierten Suche zurückgegebene Duplikate
description: Bei einer großen paginierten Suche zurückgegebene Duplikate
author: Becky
feature: Workfront API
role: Developer
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 0%

---


# Bei einer großen paginierten Suche zurückgegebene Duplikate

## Problem

Bei der Durchführung einer großen paginierten Suche in der API nach einem Objekt erhält der Kunde doppelte Einträge und fehlende Datensätze.

## Lösung

Wenn die Reihenfolge nicht formal definiert ist, verlassen wir uns auf die Reihenfolge der Zeilen, die von der Oracle-Datenbank zurückgegeben werden, was keine deterministische Reihenfolge garantiert. Beispielsweise können zwei aufeinander folgende Aufrufe mit derselben Abfrage Zeilen in einer anderen Reihenfolge zurückgeben. Ebenso können beim Paging die Zeilen nach dem Zufallsprinzip verschiedenen „Seiten“ zugewiesen werden, was zu Duplikaten führt. Die einfachste Lösung besteht darin, eine Sortierung nach ID hinzuzufügen:

```
&ID_Sort=asc
```

