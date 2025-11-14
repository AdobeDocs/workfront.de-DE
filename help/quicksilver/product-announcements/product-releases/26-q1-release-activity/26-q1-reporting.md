---
title: Berichtsverbesserungen für das erste Quartal 2026
description: Berichtsverbesserungen für das erste Quartal 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 00483638948941c933e5f8bc8cb3edaf8e43fea1
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Berichtsverbesserungen für das erste Quartal 2026

Auf dieser Seite werden die Verbesserungen beim Reporting in der Vorschau-Umgebung beschrieben, die mit der Version vom ersten Quartal 2026 vorgenommen wurden. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im ersten Quartal 2026 des Versionszyklus verfügbar sind, finden Sie unter [Übersicht über die Version im ersten Quartal 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Duplizieren eines Berichts in einem Arbeitsflächen-Dashboard

>[!NOTE]
>
>Vorschau der Version: 23. Oktober 2025
>Produktion für alle Kunden: 23. Oktober 2025
>[!BADGE Aus dem Zeitplan]{type=Neutral}

Sie können jetzt einen KPI-, Tabellen- oder Diagrammbericht in einem Arbeitsflächen-Dashboard duplizieren, nachdem er erstellt wurde. Nach dem Duplizieren können Sie den Bericht nach Bedarf bearbeiten, bevor Sie ihn speichern.

## Entfernen von Feldoptionen aus Berichtsfiltern

>[!NOTE]
>
>Vorschau: 6. November 2025
>Produktions-Schnellveröffentlichung: 13. November 2025
>Produktion für alle: 15. Januar 2026

Wir haben die folgenden Feldoptionen entfernt, die zuvor beim Anwenden eines Filters auf einen Bericht verfügbar waren:

* Andere Gruppen-IDs
* Andere Rollen-IDs
* Andere Team-IDs

Diese wurden aufgrund von Problemen mit den Operatoren „ungleich“ und „leer“ entfernt. Wenn Sie über einen vorhandenen Filter verfügen, der eines dieser Felder verwendet, funktioniert er weiterhin wie erwartet. Alternativ können Sie diese Felder im Textmodus <code> verwenden</code>, es wird jedoch empfohlen, dabei die Operatoren „ungleich“ oder „Ist leer“ zu vermeiden.

Die folgenden Feldoptionen sind als Alternativen verfügbar:

* Andere Gruppen: ID
* Andere Rollen: ID
* Andere Teams: ID

## Verbesserte Anzeige der Gruppierungsanzahl in Arbeitsflächen-Dashboards

>[!NOTE]
>
>Vorschau: 6. November 2025
>Produktions-Schnellveröffentlichung: 13. November 2025
>Produktion für alle: 15. Januar 2026

Wenn ein Tabellenbericht mehrere Ergebnisseiten enthält und die Tabelle mit Gruppierungen konfiguriert ist, zeigt die Tabelle jetzt sowohl den Datensatzbetrag für die aktuelle Seite als auch die Gesamtanzahl der Datensätze für alle Seiten an. Wenn Ihr Tabellenbericht beispielsweise 7 Gruppierungen aufweist und die erste Seite 3 anzeigt, zeigt die Tabelle 3 von 7 an.


## Neue Leitplanken zur Verbesserung der Ladezeiten in Arbeitsflächen-Dashboards

>[!NOTE]
>
>Vorschau: 6. November 2025
>Produktions-Schnellveröffentlichung: 13. November 2025
>Produktion für alle: 15. Januar 2026

Um Ladezeitverzögerungen zu vermeiden und die Gesamtleistung in Arbeitsflächen-Dashboards zu verbessern, haben wir Grenzwerte für die Anzahl der Dashboard-Komponenten angewendet, die einem Dashboard hinzugefügt werden können:

* Berichte pro Dashboard: maximal 25
* Gruppierungen in Tabellenansichten: maximal 5
* Entfernung vom Basisobjekt des Berichts: 10 Grenze
* Spalten in einer Tabellenansicht: maximal 25
* Filter auf Dashboard-Ebene - Eingabeaufforderungen: 10 Grenze