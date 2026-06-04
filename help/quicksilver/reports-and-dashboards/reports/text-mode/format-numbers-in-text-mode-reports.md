---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formatieren von Zahlen, Währungs- und Prozentwerten in Berichten im Textmodus
description: Numerische Werte, einschließlich Währung, können so konfiguriert werden, dass sie in Berichten und Listen in Adobe Workfront in verschiedenen Formaten angezeigt werden.
author: Courtney
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/z96Rvp54iQcZxVWJ4Evoe1Qasl-VrEZ-IrVy11n9cDc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 145
ht-degree: 20%

---

# Formatieren von Zahlen, Währungs- und Prozentwerten in Berichten im Textmodus

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

