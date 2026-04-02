---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formatieren von Datumsangaben in Berichten im Textmodus
description: Datumsangaben können so konfiguriert werden, dass sie in Berichten und Listen in Adobe Workfront in einer Vielzahl von Formaten angezeigt werden. Um ein Datumsformat festzulegen, müssen Sie die Zeile valueFormat des Textmodus-Codes in der Spalte ändern.
author: Courtney
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 6%

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

| **Format** | Beispiel  | ***valueFormat=*** |
|---|---|---|
| MM/TT/JJ | 10/11/18 | `atDate` |
| MM/TT/JJ Zeit | 10/11/18 12:00pm | `longAtDate` |
| MM/TT/JJ | 10/11/18 | `shortAtDate` |
| Math, TT, JR | &#x200B;11. Oktober 2018 | `mediumAtDate` |
| DW, Math, Tag, JR | Mo, 11. Oktober 2018 | `partialAtDate` |
| DW, Math, Tag, YR-Zeit | Mo, Okt, 11, 2018 12:00 pm | `fullAtDate` |
