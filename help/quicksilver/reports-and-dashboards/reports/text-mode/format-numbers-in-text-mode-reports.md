---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formatieren von Zahlen, Währungs- und Prozentwerten in Textmodusberichten
description: Numerische Werte, einschließlich Währung, können so konfiguriert werden, dass sie in Berichten und Listen in Adobe Workfront in verschiedenen Formaten angezeigt werden.
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 8de9c79f6c62b74a652482ec10bf38fada8c5fc8
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 7%

---

# Formatieren von Zahlen, Währungs- und Prozentwerten in Textmodusberichten

<!-- Audited: 2/2024 -->

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
| 1234 | <pre>doubleAsString</pre> <br>oder <br><pre>int</pre> |
| 1.234 | <pre>doubleAsInt</pre> |
| $1,234 | <pre>currencyStringCurrencyRounded</pre> |
| 1234,56 | <pre>doubleAsDouble</pre> |
| $1,234.56 | <pre>currencyStringCurrency</pre> |
| 12% | <pre>doubleAsPercentRounded</pre> |
| 12,34% | <pre>doubleAsPercent</pre> |
| (1,234.56) | <pre>doubleAsFinancial</pre> |
| (1,234) | <pre>doubleAsFinancialRounded</pre> |

