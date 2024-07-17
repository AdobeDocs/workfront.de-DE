---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Sortieren von Abfrageergebnissen in der API
description: Sortieren von Abfrageergebnissen in der API
author: Becky
feature: Workfront API
role: Developer
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 0%

---


# Sortieren von Abfrageergebnissen in der API

Sie können Ihre Ergebnisse nach jedem Feld sortieren, wenn Sie Folgendes an Ihren API-Aufruf anhängen:

```
&entryDate_Sort=asc
```

Wenn Sie beispielsweise nach Aufgabe &quot;Geplantes Startdatum&quot;sortieren möchten, entfernen Sie `entryDate` und ersetzen Sie es durch `plannedCompletionDate`.

Dies funktioniert für die meisten Felder in Adobe Workfront.
