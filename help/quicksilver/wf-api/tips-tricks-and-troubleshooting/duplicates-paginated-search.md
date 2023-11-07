---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Duplikate, die bei einer großen, paginierten Suche zurückgegeben werden
description: Duplikate, die bei einer großen, paginierten Suche zurückgegeben werden
author: Becky
feature: Workfront API
role: Developer
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 0%

---


# Duplikate, die bei einer großen, paginierten Suche zurückgegeben werden

## Problem

Bei einer großen, paginierten Suche in der API nach einem Objekt erhält der Kunde doppelte Einträge und fehlende Datensätze.

## Lösung

Wenn die Reihenfolge nicht formell definiert ist, verlassen wir uns auf die Reihenfolge der von der Oracle-Datenbank zurückgegebenen Zeilen, was keine deterministische Reihenfolge garantiert. Zwei aufeinander folgende Aufrufe mit derselben Abfrage können beispielsweise Zeilen in einer anderen Reihenfolge zurückgeben. Gleichermaßen werden die Zeilen beim Paging zufällig verschiedenen &quot;Seiten&quot;zugewiesen, was zu Duplikaten führt. Die einfachste Lösung besteht darin, eine Sortierung nach Kennung hinzuzufügen:

```
&ID_Sort=asc
```

