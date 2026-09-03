---
title: Verbesserungen bei Berichten für das vierte Quartal 2026
description: Verbesserungen bei Berichten für das vierte Quartal 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: ee1fceee828c97db535ccc03c8b428940d6f7eed
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 8%

---

# Verbesserungen bei Berichten für das vierte Quartal 2026

Auf dieser Seite werden die Verbesserungen beim Reporting in der Vorschau-Umgebung beschrieben, die mit der Version vom vierten Quartal 2026 vorgenommen wurden. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im vierten Quartal 2026 des Versionszyklus verfügbar sind, finden Sie unter [Versionsübersicht für das vierte Quartal 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

<!--

## Duplicate dashboards in Canvas Dashboards

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

You can now duplicate a Canvas Dashboard using the new **Duplicate dashboard** action. This action is available to any user whose access level grants edit or create rights to Dashboards, even if they only have view access to the specific dashboard being copied. Users without edit or create rights to Dashboards do not see this action.

When you duplicate a dashboard, you can rename it, update its description and currency, and choose which widgets, dashboard filters, and dashboard prompts to carry over to the copy.

Run as user configurations on widgets are only preserved if you are the designated user or a system administrator. Sharing preferences are not copied to the new dashboard, and a confirmation message with a link to the new dashboard displays once the copy is complete.

Previously, there was no way to duplicate a dashboard; users had to rebuild dashboards from scratch to create audience-specific variations.

For more information, see 

-->

## Feld „Validierungstyp“ in den Dashboards der Arbeitsfläche

>[!NOTE]
>
>Produktion für alle: 28. August 2026
>[!BADGE Außerplanmäßig]{type=Neutral}

Die Genehmigungsentität enthält jetzt ein Feld **Genehmigungstyp**, mit dem Benutzende zwischen Korrekturabzugs-, Dokumentversions-, Aufnahmegenehmigungen und anderen Genehmigungstypen unterscheiden können.

## Aktualisierung der Validierungsterminologie in den Arbeitsflächen-Dashboards

>[!NOTE]
>
>Produktion für alle: 28. August 2026
>[!BADGE Außerplanmäßig]{type=Neutral}

Die folgenden Feldnamen, die in Arbeitsflächen-Dashboards für Dokument- und Arbeitsgenehmigungen verwendet werden, wurden aus Gründen der Klarheit umbenannt:

| Vorheriger Name | Neuer Name |
| --- | --- |
| Dokumentengenehmigung | Genehmigung |
| Dokumentengenehmigungsphase | Genehmigungsphase |
| Teilnehmerin oder Teilnehmer der Dokumentengenehmigungsphase | Teilnehmerin oder Teilnehmer der Genehmigungsphase |
| Genehmigungsprozess | Arbeitsgenehmigungsprozess |
| Genehmigungsphase | Arbeitsgenehmigungsphase |
| Status der genehmigenden Person | Status der Arbeitsgenehmigenden Person |
| Warten auf Genehmigung | Warten auf Arbeitsgenehmigung |

Diese Änderung hat keine Auswirkungen auf die Funktionsweise aktueller Berichte.

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
