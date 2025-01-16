---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formatieren von Datumsangaben in Berichten im Textmodus
description: Datumsangaben können so konfiguriert werden, dass sie in Berichten und Listen in Adobe Workfront in einer Vielzahl von Formaten angezeigt werden. Um ein Datumsformat festzulegen, müssen Sie die Zeile valueFormat des Textmodus-Codes in der Spalte ändern.
author: Nolan
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Formatieren von Datumsangaben in Berichten im Textmodus

<!-- Audited: 1/2025 -->

Datumsangaben können so konfiguriert werden, dass sie in Berichten und Listen in Adobe Workfront in einer Vielzahl von Formaten angezeigt werden. Um ein Datumsformat festzulegen, müssen Sie die `valueformat` Zeile des Textmodus-Codes in der Spalte ändern.

`valueformat= [new date format]` Wenn Sie beispielsweise das voraussichtliche Abschlussdatum als MM/TT/JJ anzeigen möchten, würde der Code wie folgt aussehen:

```
valueformat=atDate
valuefield=projectedCompletionDate
```

Wenn Sie das geplante Abschlussdatum als (*, TT, Jahr)* möchten, würde der Code wie folgt aussehen:

```
valueformat=mediumAtdate
valuefield=plannedCompletionDate
```

Weitere Informationen zum Anwenden der bedingten Formatierung in Workfront-Berichten und -Listen im Textmodus finden Sie unter [Verwenden der bedingten Formatierung im Textmodus](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

Sie können Datumsangaben mithilfe der folgenden `valueformat` Textmoduswerte formatieren:

| **format** | Beispiel  | ***valueFormat=*** |
|---|---|---|
| MM/TT/JJ | 10/11/18 | `atDate` |
| MM/TT/JJ Zeit | 10/11/18 12:00 | `longAtDate` |
| MM/TT/JJ | 10/11/18 | `shortAtDate` |
| Math, TT, JR | 11. Oktober 2018 | `mediumAtDate` |
| DW, Math, Tag, JR | Mo, 11. Oktober 2018 | `partialAtDate` |
| DW, Math, Tag, YR-Zeit | Mo, 11. Oktober 2018 12:00 Uhr | `fullAtDate` |
