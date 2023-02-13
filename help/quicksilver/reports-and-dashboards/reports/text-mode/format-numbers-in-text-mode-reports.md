---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formatnummern, Währungs- und Prozentwerte in Textmodusberichten
description: Numerische Werte wie die Währung können so konfiguriert werden, dass sie in Adobe Workfront in verschiedenen Formaten in Berichten und Listen angezeigt werden.
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 7%

---

# Formatnummern, Währungs- und Prozentwerte in Textmodusberichten

Numerische Werte wie die Währung können so konfiguriert werden, dass sie in Adobe Workfront in verschiedenen Formaten in Berichten und Listen angezeigt werden.

Um das Format eines numerischen Werts zu ändern, müssen Sie die **valueFormat** -Zeile Ihrer Spalte.

Wenn Sie beispielsweise die Spalte Budget als 1000 USD anzeigen möchten, würde die Zeile für das Wertformat wie folgt aussehen:

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

Weitere Informationen zum Anwenden der bedingten Formatierung in Workfront-Berichten und -Listen im Textmodus finden Sie unter [Bedingte Formatierung im Textmodus verwenden](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

Sie können Zahlen mit den folgenden Werten für die `valueformat` Zeile Ihrer Spalte:

| Beispiel | `valueformat=` |
|---|---|
| 1234 | <pre>doubleAsString</pre> <br>oder <br><pre>int</pre> |
| 1.234 | <pre>doubleAsInt</pre> |
| $1,234 | <pre>currencyStringCurrencyRounded</pre> |
| 1234.56 | <pre>doubleAsDouble</pre> |
| $1,234.56 | <pre>currencyStringCurrency</pre> |
| 12% | <pre>doubleAsPercentRounded</pre> |
| 12,34% | <pre>doubleAsPercent</pre> |
| (1,234.56) | <pre>doubleAsFinancial</pre> |
| (1,234) | <pre>doubleAsFinanceRounded</pre> |
