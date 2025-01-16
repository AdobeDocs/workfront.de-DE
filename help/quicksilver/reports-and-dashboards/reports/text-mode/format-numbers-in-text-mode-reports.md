---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formatieren von Zahlen, Währungs- und Prozentwerten in Textmodusberichten
description: Numerische Werte, einschließlich Währung, können so konfiguriert werden, dass sie in Berichten und Listen in Adobe Workfront in verschiedenen Formaten angezeigt werden.
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 6%

---

# Formatieren von Zahlen, Währungs- und Prozentwerten in Textmodusberichten

<!-- Audited: 1/2025 -->

Numerische Werte, einschließlich Währung, können so konfiguriert werden, dass sie in Berichten und Listen in Adobe Workfront in verschiedenen Formaten angezeigt werden.

Um das Format eines numerischen Werts zu ändern, müssen Sie die Zeile **valueFormat** Ihrer Spalte bearbeiten.

Wenn Sie beispielsweise die Budgetspalte als $1000 anzeigen möchten, würde die Zeile im Wertformat wie folgt aussehen:

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

Weitere Informationen zum Anwenden der bedingten Formatierung in Workfront-Berichten und -Listen im Textmodus finden Sie unter [Verwenden der bedingten Formatierung im Textmodus](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

Sie können Zahlen mithilfe der folgenden Werte für die `valueformat` Ihrer Spalte formatieren:

| Beispiel | `valueformat=` |
|---|---|
| 1234 | `doubleAsString`<br>oder<br>`int` |
| 1.234 | `doubleAsInt` |
| $1,234 | `currencyStringCurrencyRounded` |
| 1234,56 | `doubleAsDouble` |
| $1,234.56 | `currencyStringCurrency` |
| 12% | `doubleAsPercentRounded` |
| 12,34% | `doubleAsPercent` |
| (1,234.56) | `doubleAsFinancial` |
| (1,234) | `doubleAsFinancialRounded` |

