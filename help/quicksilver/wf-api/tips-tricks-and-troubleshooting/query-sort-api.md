---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Sortieren von Abfrageergebnissen in der API
description: Sortieren von Abfrageergebnissen in der API
author: Becky
feature: Workfront API
role: Developer
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: 5936982217adc6cfcaf9e400bfff67a1496d3a78
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 0%

---


# Sortieren von Abfrageergebnissen in der API

Sie können Ihre Ergebnisse nach einem beliebigen Feld sortieren, wenn Sie Folgendes an Ihren API-Aufruf anhängen:

```
&entryDate_Sort=asc
```

Wenn Sie beispielsweise nach dem geplanten Abschlussdatum der Aufgabe sortieren möchten, entfernen Sie `entryDate` und ersetzen Sie sie durch `plannedCompletionDate`.

```
&plannedCompletionDate_Sort=asc
```

Dies funktioniert für die meisten Felder in Adobe Workfront.
