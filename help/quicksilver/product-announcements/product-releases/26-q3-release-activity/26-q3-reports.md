---
title: Verbesserungen bei der Berichterstellung für das dritte Quartal 2026
description: Verbesserungen bei der Berichterstellung für das dritte Quartal 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 9a86968cf8fff2c7c930aa6c8408ab8566905cb8
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 6%

---

# Verbesserungen bei der Berichterstellung für das dritte Quartal 2026

Auf dieser Seite werden die Verbesserungen beim Reporting in der Vorschau-Umgebung beschrieben, die mit der Version vom dritten Quartal 2026 vorgenommen wurden. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im dritten Quartal 2026 verfügbar sind, finden Sie unter [Versionsübersicht für das dritte Quartal 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Verbesserte Datengenauigkeit in Dashboard-Berichten der Arbeitsfläche

>[!NOTE]
>
>Vorschau: 14. Mai 2026>Produktions-Schnellveröffentlichung: 11. Juni 2026>Produktion für alle: 16. Juli 2026
>
>Canvas Dashboards befindet sich derzeit in der Beta-Phase.

In Arbeitsflächen-Dashboards werden jetzt Berichtsabfragen strukturiert, um doppelte Zeilen zu verhindern, wenn Filter oder Felder verwandte Datensätze überschneiden, sodass Zählungen, Summen und andere Aggregate genaue Werte zurückgeben.

Zuvor konnte eine Verknüpfung zwischen verwandten Datensätzen übergeordnete Datensätze für jeden verwandten Datensatz einmal wiederholen. Beispielsweise wird in einem Projektbericht nach Aufgaben gefiltert, die einem bestimmten Benutzer zugewiesen sind, jedes Projekt einmal für jede übereinstimmende Aufgabe wiederholt. Ein KPI, der das Projektbudget zusammenfasst, könnte 6.000 Dollar anstelle der korrekten 1.250 Dollar anzeigen.

Die Benutzeroberfläche des Arbeitsflächen-Dashboards wird nicht geändert. Vorhandene Berichte geben nach dieser Version automatisch genaue Daten zurück.
