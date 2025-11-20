---
content-type: release-notes
title: Versionsaktivität für Adobe Workfront Planning im ersten Quartal 2026
description: Dies ist die Veröffentlichungsaktivität für das Adobe Workfront Planning-Produkt im ersten Quartal 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 0964ad24535bf43a23c740cd63abcf8fea705b8d
workflow-type: tm+mt
source-wordcount: '642'
ht-degree: 0%

---

# Versionsaktivität für Adobe Workfront Planning im ersten Quartal 2026

In diesem Artikel werden die Funktionen beschrieben, die in der Version vom ersten Quartal 2026 für Workfront Planning veröffentlicht werden.

<!--keep the sentence below for all future quarterly release pages-->

Eine Liste aller für Adobe Workfront Planning veröffentlichten Funktionen finden Sie unter [Adobe Workfront Planning Release-Aktivität: Artikelindex](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Verbinden von GenStudio for Performance Marketing Brands mit Workfront Planning-Datensatztypen

>[!NOTE]
>
>Vorschau: 13. November 2025
>Produktions-Schnellveröffentlichung: 13. November 2025
>Produktion für alle: 13. November 2025

Sie können jetzt Datensatztypen für Workfront Planning mit Marken aus Adobe GenStudio for Performance Marketing verbinden. Ihr Unternehmen muss sowohl über Workfront Planning als auch über Adobe GenStudio for Performance Marketing verfügen.

Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).


## Neues Suchfeld für Felder in den Symbolen für Filter, Felder und Zeilenfarben in Planning-Ansichten

>[!NOTE]
>
>Vorschau: 6. November 2025
>Produktions-Schnellveröffentlichung: 11. Dezember 2025
>Produktion für alle: 15. Januar 2026

Sie können jetzt beim Erstellen eines Ansichtselements in einer Datensatztypansicht nach einem bestimmten Feld suchen. Wir haben Suchfelder hinzugefügt, wenn Sie einen Filter, eine Sortierung, eine Gruppierung oder Ihre Felder- oder Zeilenfarben konfigurieren. Vor dieser Verbesserung konnten Sie einfach durch die Liste der verfügbaren Felder scrollen.

Diese Verbesserung ist in allen Ansichten vom Typ Datensatz verfügbar.

Weitere Informationen finden Sie unter [Verwalten der Tabellenansicht](/help/quicksilver/planning/views/manage-the-table-view.md).


## Globale Datensatztypen und die Möglichkeit, sie als vorhandene Datensatztypen zu anderen Arbeitsbereichen hinzuzufügen

>[!NOTE]
>
>Vorschau: 16. Oktober 2025
>Produktions-Schnellveröffentlichung: 13. November 2025
>Produktion für alle: 15. Januar 2026

Bei der Implementierung von Workfront Planning für ein Unternehmen mit mehreren Teams mit gemeinsamen Workflows müssen Sie möglicherweise eine zusammenhängende Struktur und Metadaten für wichtige Datensatztypen (wie Kampagnen oder Ergebnisse) definieren, die den Arbeitsbereichen jedes Teams hinzugefügt werden können, um ihre Arbeit zu erfassen und zu verwalten.

Außerdem benötigen Sie möglicherweise die Arbeit jedes Teams, um eine zentrale Ebene zu erreichen.

In einem solchen Workflow können Sie sicherstellen, dass Teams ihre Arbeit konsistent erfassen, während Sie die Team-übergreifende Sichtbarkeit erschließen, ohne dass alle Personen in der Organisation zu jedem Arbeitsbereich hinzugefügt werden müssen. Sie können dazu globale Datensatztypen verwenden.

Sie können jetzt einen Datensatztyp als „global“ festlegen und ihn über mehrere Arbeitsbereiche hinweg verwenden. Benutzer können dieselbe Feldstruktur und dieselben Verbindungen verwenden, die bereits in einem zentralen Arbeitsbereich konfiguriert sind.

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Arbeitsbereichsübergreifende Übersicht über den Datensatztyp](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)

* [Konfigurieren von arbeitsbereichsübergreifenden Datensatztyp-Funktionen](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)

* [Hinzufügen vorhandener Datensatztypen aus einem anderen Arbeitsbereich](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)

## Neues Limit für Verbindungsfelder für einen Datensatztyp

>[!NOTE]
>
>Vorschau: 16. Oktober 2025
>Produktions-Schnellveröffentlichung: 13. November 2025
>Produktion für alle: 15. Januar 2026

Wir haben für jeden Datensatztyp ein Limit von 30 Verbindungsfeldern eingeführt.

HINWEIS: Wenn Ihr Unternehmen derzeit mehr als 30 Verbindungsfelder für einen Datensatztyp hat, können Sie die zusätzlichen Felder beibehalten, die das Limit von 30 überschreiten. Sie können jedoch nicht mehr Verbindungsfelder zu diesen Datensatztypen hinzufügen, die das Limit überschreiten. In Zukunft wird die neue Beschränkung von 30 Verbindungsfeldern erzwungen.

Weitere Informationen finden Sie unter [Übersicht über verbundene Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Festlegen benutzerfreundlicher Werte für Feldoptionen vom Typ Auswahl

>[!NOTE]
>
>Vorschau: 16. Oktober 2025
>Produktions-Schnellveröffentlichung: 13. November 2025
>Produktion für alle: 15. Januar 2026

Beim Hinzufügen von Feldoptionen zu einem Ein- oder Mehrfachauswahlfeld weist Workfront jeder Auswahl jetzt benutzerfreundliche Werte zu. Vor dieser Verbesserung generierte Workfront eine alphanumerische ID, die in API-Aufrufen und anderen Integrationen schwer zu verstehen und zu verwenden war.

Beachten Sie bei dieser Verbesserung Folgendes:

* Die neuen Werte werden den neuen Feldoptionen hinzugefügt. Vorhandene Feldoptionen behalten ihre alphanumerischen IDs bei.

* Auswahlwerte sind für ein Feld eindeutig, können jedoch zwischen verschiedenen Feldern wiederholt werden.

* Beim Umbenennen einer Auswahl wird ihr ursprünglicher Wert nicht aktualisiert.

* Bei Auswahl mit mehreren Wörtern werden die Auswahlwerte in Kleinbuchstaben angezeigt und bei Auswahl mit mehreren Wörtern durch Unterstriche getrennt. Wenn Sie eine bereits als anderer Auswahlname für dasselbe Feld verwendete Beschriftung verwenden, fügt Workfront eine sequenzielle Zahl zum Wert hinzu.

Weitere Informationen finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).