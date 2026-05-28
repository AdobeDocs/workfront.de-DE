---
title: Verbesserungen bei der Berichterstellung für das dritte Quartal 2026
description: Verbesserungen bei der Berichterstellung für das dritte Quartal 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: a177e2887c2b8b281b19cda45ce59c6f8149cefb
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 4%

---

# Verbesserungen bei der Berichterstellung für das dritte Quartal 2026

Auf dieser Seite werden die Verbesserungen beim Reporting in der Vorschau-Umgebung beschrieben, die mit der Version vom dritten Quartal 2026 vorgenommen wurden. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im dritten Quartal 2026 verfügbar sind, finden Sie unter [Versionsübersicht für das dritte Quartal 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Benutzerdefinierte Währungsdatenfelder in Dashboard-Berichten der Arbeitsfläche

>[!NOTE]
>
>Vorschau: 28. Mai 2026>Produktions-Schnellversion: 11. Juni 2026>Produktion für alle: 16. Juli 2026

Arbeitsflächen-Dashboard-Berichte unterstützen jetzt benutzerdefinierte Währungsdatenfelder als Spalten, Filter, Gruppierungen und Aggregationen, auch wenn im System-Setup mehrere Wechselkurse konfiguriert sind. Wenn ein benutzerdefiniertes Währungsdatenfeld als Spalte oder Aggregation angezeigt wird, konvertieren Sie Werte in die Währung, die im Umschalter Wechselkurs des Dashboards ausgewählt ist, es sei denn, das Feld ist auf Berichtsebene gesperrt.

Berichte, die zuvor nach Hinzufügen einer zweiten Wechselkurswährung mit der Meldung „Eingeschränktes Feld“ fehlgeschlagen sind, werden jetzt gerendert. Felder in der Planungswährung bleiben eingeschränkt, wenn mehrere Wechselkurse definiert werden.

Weitere Informationen finden Sie unter [Verwenden von Währungsfeldern in Arbeitsflächen-Dashboards](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/switch-currencies.md).

## Verbesserte Datengenauigkeit in Dashboard-Berichten der Arbeitsfläche

>[!NOTE]
>
>Vorschau: 14. Mai 2026>Produktions-Schnellversion: 11. Juni 2026>Produktion für alle: 16. Juli 2026
>
>Canvas Dashboards befindet sich derzeit in der Beta-Phase.

In Arbeitsflächen-Dashboards werden jetzt Berichtsabfragen strukturiert, um doppelte Zeilen zu verhindern, wenn Filter oder Felder verwandte Datensätze überschneiden, sodass Zählungen, Summen und andere Aggregate genaue Werte zurückgeben.

Zuvor konnte eine Verknüpfung zwischen verwandten Datensätzen übergeordnete Datensätze für jeden verwandten Datensatz einmal wiederholen. Beispielsweise wird in einem Projektbericht nach Aufgaben gefiltert, die einem bestimmten Benutzer zugewiesen sind, jedes Projekt einmal für jede übereinstimmende Aufgabe wiederholt. Ein KPI, der das Projektbudget zusammenfasst, könnte 6.000 Dollar anstelle der korrekten 1.250 Dollar anzeigen.

Die Benutzeroberfläche des Arbeitsflächen-Dashboards wird nicht geändert. Vorhandene Berichte geben nach dieser Version automatisch genaue Daten zurück.
