---
title: Verbesserungen bei Berichten für das vierte Quartal 2026
description: Verbesserungen bei Berichten für das vierte Quartal 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 63bdc885983f60c316409c3bba400ad82d475a5f
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 4%

---

# Verbesserungen bei Berichten für das vierte Quartal 2026

Auf dieser Seite werden die Verbesserungen beim Reporting in der Vorschau-Umgebung beschrieben, die mit der Version vom vierten Quartal 2026 vorgenommen wurden. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im vierten Quartal 2026 des Versionszyklus verfügbar sind, finden Sie unter [Versionsübersicht für das vierte Quartal 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

## Pivot-Tabellenberichte in Arbeitsflächen-Dashboards

>[!NOTE]
>
>Vorschau: 27. August 2026
>Produktions-Schnellveröffentlichung: 17. September 2026
>Produktion für alle: 15. Oktober 2026

Der neue Berichtstyp „Pivot-Tabelle“ in Arbeitsflächen-Dashboards aggregiert Daten mit genauen, vollständigen Rollups. Sie können Metriken wie Zahlen, Summen und Durchschnittswerte direkt in Ihrem Dashboard erstellen und dann die zugrunde liegenden Datensätze hinter jedem Gesamtwert detailliert anzeigen.

Weitere Informationen finden Sie unter [Erstellen eines Pivot-Tabellenberichts in einem Arbeitsflächen-Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-pivot-table-report.md).

## Erzwingen von Enddaten für terminierte Berichte

>[!NOTE]
>
>Vorschau: 13. August 2026
>Produktions-Schnellveröffentlichung: 17. September 2026
>Produktion für alle: 15. Oktober 2026

Terminierte Berichte benötigen jetzt ein Enddatum, um den Versand auf unbestimmte Zeit zu verhindern. Zeitpläne, die ihr Enddatum überschritten haben, werden automatisch deaktiviert.

Bestehende Zeitpläne wurden mit Enddaten aktualisiert, um die Zuverlässigkeit zu verbessern und unnötige Systemnutzung zu reduzieren. Workfront bietet außerdem zusätzliche Sichtbarkeit und Warnhinweise, mit denen Sie die Lebenszyklen von Berichten verwalten können, wenn sie sich ihrem Enddatum nähern.

Weitere Informationen finden Sie unter [Planen einer automatischen Berichtsbereitstellung](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

## Native Referenzfelder stehen für Listen und Berichte zur Verfügung

>[!NOTE]
>
>Vorschau: 30. Juli 2026
>Produktions-Schnellveröffentlichung: 13. August 2026
>Produktion für alle: 15. Oktober 2026

Sie können jetzt in Workfront native Referenzfelder zu Listen und Berichten hinzufügen.

Ein natives Referenzfeld ist ein benutzerdefiniertes Feld. Wenn sich das Feld in einem benutzerdefinierten Formular befindet, das an ein Objekt angehängt ist, wird das Feld aus den Objektdaten gefüllt. Wenn das Feld beispielsweise auf das Feld Beschreibung verweist und es sich auf einem benutzerdefinierten Formular befindet, das an ein Projekt angehängt ist, wird die Projektbeschreibung abgerufen. (Wenn keine Daten verfügbar sind, wird in dem Feld möglicherweise „K. A.“ angegeben.)

Informationen zum Erstellen nativer Referenzfelder, einschließlich der Liste unterstützter nativer Felder, finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
Informationen zum Hinzufügen von Feldern zu Berichten finden Sie unter [Erstellen eines benutzerdefinierten Berichts](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Konsistente Sortierung von Mehrfachauswahl-Feldwerten in Legacy-Listen und -Berichten

>[!NOTE]
>
>Vorschau: 30. Juli 2026
>Produktions-Schnellveröffentlichung: 13. August 2026
>Produktion für alle: 15. Oktober 2026

Jetzt werden ausgewählte Optionen für die Mehrfachauswahl benutzerdefinierter Felder in einer konsistenten, vorhersehbaren Reihenfolge in veralteten Listen und Berichten angezeigt. Die Reihenfolge der Felder wird durch die Anordnung der Felder im benutzerdefinierten Formular bestimmt.

![Die Reihenfolge der benutzerdefinierten Formularfelder entspricht der Reihenfolge der ausgewählten Werte in einer Liste oder einem Bericht](assets/new-field-order-multi-select.png)

Zuvor wurden ausgewählte Optionen in der Reihenfolge angezeigt, in der Sie sie ausgewählt haben, oder in einer inkonsistenten Reihenfolge, wodurch das Scannen und Vergleichen von Zeilen erschwert wurde.

Hinweis: Die neue Sortierung gilt nicht, wenn das Feld den Textmodus verwendet.
