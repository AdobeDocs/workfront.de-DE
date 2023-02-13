---
product-area: reporting
navigation-topic: text-mode-reporting
title: Datumsangaben in Textmodusberichten formatieren
description: Datumswerte können so konfiguriert werden, dass sie in Adobe Workfront in verschiedenen Formaten in Berichten und Listen angezeigt werden. Um ein Datumsformat festzulegen, müssen Sie die Zeile valueFormat des Textmoduscodes in der Spalte ändern.
author: Nolan
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 2%

---

# Datumsangaben in Textmodusberichten formatieren

Datumswerte können so konfiguriert werden, dass sie in Adobe Workfront in verschiedenen Formaten in Berichten und Listen angezeigt werden. Um ein Datumsformat festzulegen, müssen Sie die `valueformat` -Zeile des Textmoduscodes in der Spalte.

`valueformat= [new date format]` Wenn Sie beispielsweise möchten, dass das geplante Abschlussdatum als MM/TT/JJ angezeigt wird, würde der Code wie folgt aussehen:

```
valueformat=atDate
valuefield=projectedCompletionDate
```

Wenn Sie das geplante Abschlussdatum als *Mth, DD, Year*, würde der Code wie folgt aussehen:

```
valueformat=mediumAtdate
valuefield=plannedCompletionDate
```

Weitere Informationen zum Anwenden der bedingten Formatierung in Workfront-Berichten und -Listen im Textmodus finden Sie unter [Bedingte Formatierung im Textmodus verwenden](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

Sie können Datumsangaben wie folgt formatieren:

```
valueformat
```

 Textmoduswerte:

| **Format** | Beispiel  | ***valueFormat=*** |
|---|---|---|
| MM/TT/JJ | 10/11/18 | `atDate` |
| MM/TT/JJJ Zeit | 11.10.18 12:00 pm | `longAtDate` |
| MM/TT/JJ | 10/11/18 | `shortAtDate` |
| Mth, DD, YR | 11. Oktober 2018 | `mediumAtDate` |
| DW, Mth, Day, YR | Mo., 11. Oktober 2018 | `partialAtDate` |
| DW, Mth, Day, YR Time | Mo., 11. Oktober 2018 12:00 pm | `fullAtDate` |
