---
title: Verbesserungen bei der Berichterstellung für das dritte Quartal 2026
description: Verbesserungen bei der Berichterstellung für das dritte Quartal 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: c1ffa06ddca88f8679cf3886ce5c90f69984f30b
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 1%

---

# Verbesserungen bei der Berichterstellung für das dritte Quartal 2026

Auf dieser Seite werden die Verbesserungen beim Reporting in der Vorschau-Umgebung beschrieben, die mit der Version vom dritten Quartal 2026 vorgenommen wurden. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im dritten Quartal 2026 verfügbar sind, finden Sie unter [Versionsübersicht für das dritte Quartal 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Standardeinstellungen für Canvas-Dashboard-Eingabeaufforderung und Persistenz der Benutzereinstellungen

>[!NOTE]
>
>Vorschau: 25. Juni 2026>Produktions-Schnellversion: 15. Juli 2026>Produktion für alle: 16. Juli 2026

Um die Effizienz für Benutzer zu verbessern, die zwischen Dashboards und Datensätzen wechseln, indem ihr Arbeitsfilterstatus beibehalten wird, können Dashboard-Manager jetzt standardmäßige Eingabeaufforderungswerte für Arbeitsflächen-Dashboards definieren. Diese Standardeinstellungen werden automatisch auf alle Dashboard-Viewer angewendet.

Wenn ein(e) Benutzende(r) eine Eingabeaufforderung aktualisiert, wird seine/ihre Auswahl bei Aktualisierung, erneuten Öffnen oder nach der Navigation zu einem Datensatz und zurück gespeichert und wiederhergestellt.

Manager können den Standardstatus des Dashboards jederzeit zurücksetzen. Über das Dreipunkt-Menü können Benutzer auch schnell auf die Standardeinstellungen zurücksetzen.

Vor dieser Verbesserung hatten Dashboard-Eingabeaufforderungen keine konfigurierbare Standardeinstellung oder gespeicherte Benutzervoreinstellung für den Eingabeaufforderungsstatus.

Weitere Informationen finden Sie unter [Dashboard einer Arbeitsfläche filtern](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/filter-canvas-dashboard.md).

## Gleichzeitiges Hinzufügen mehrerer Power BI-IP-Adressbereiche zur Data Connect-Zulassungsliste

>[!NOTE]
>
>Vorschau: Nicht verfügbar>Produktions-Schnellveröffentlichung: 11. Juni 2026>Produktion für alle: 16. Juli 2026

Workfront-Admins, die Microsoft Power BI mit Workfront Data Connect verbinden, können jetzt in einem einzigen Schritt den Satz von Azure-IP-Adressbereichen einer gesamten Region zur -Zulassungsliste hinzufügen. Auf der Registerkarte **IP** in **Data Connect** enthält die Schaltfläche **Neue IP-Adresse** jetzt die Option **Power BI-IP-Adressblöcke hinzufügen**, mit der Sie ein Dialogfeld öffnen können, in das Sie Power BI-Service-Tag-Einträge aus den von Microsoft veröffentlichten Azure-IP-Bereichen und der Service-Tags-JSON-Datei einfügen können.

Dies ersetzt den vorherigen Workflow zum Hinzufügen jedes Power BI-CIDR-Blocks einzeln, was für Regionen, die Dutzende von Adresspräfixen veröffentlichen, zeitaufwendig war.

Weitere Informationen finden Sie unter [Herstellen einer Verbindung mit Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).


## Sortieren der Liste der Arbeitsflächen-Dashboards

>[!NOTE]
>
>Vorschau: 11. Juni 2026>Produktions-Schnellversion: 15. Juli 2026>Produktion für alle: 16. Juli 2026
>
>Canvas Dashboards befindet sich derzeit in der Beta-Phase.

Sie können die Liste der Arbeitsflächen-Dashboards jetzt nach einer der folgenden Spalten sortieren: **Name**, **Beschreibung**, **Erstellt von** oder **Erstellungsdatum**. Klicken Sie auf eine Spaltenüberschrift, um die Liste nach dieser Spalte zu sortieren, und klicken Sie dann erneut auf dieselbe Überschrift, um die Sortierrichtung umzukehren. Standardmäßig wird die Liste nach &quot;**&quot;** A bis Z sortiert. Die Sortierreihenfolge wird beibehalten, wenn Sie in der Liste der Arbeitsflächen-Dashboards zwischen Registerkarten wechseln.

Weitere Informationen finden Sie unter [Verwenden von Canvas-Dashboards](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md).

## Änderungen an den tatsächlichen Stunden in benutzerdefinierten Formeln

>[!NOTE]
>
>Vorschau: 1. Juni 2026>Produktions-Schnellveröffentlichung: 1. Juni 2026>Produktion für alle: 1. Juni 2026

Im Jahr 2025 wurde der Workfront-Datenbank ein neues Feld „Tatsächliche Stunden“ als `actualWorkRequiredDouble` hinzugefügt und das bestehende Feld „Tatsächliche Stunden“ (in der Datenbank `actualWorkRequired`) wurde in „Frühere Tatsächliche Stunden“ umbenannt. Weitere Informationen finden [ in ](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-project-enhancements.md) Versionshinweisen .

Im Juni 2026 wurden vorhandene benutzerdefinierte Formeln, die `actualWorkRequired` (veraltete tatsächliche Stunden) verwenden, migriert, um stattdessen `actualWorkRequiredDouble` (tatsächliche Stunden) zu verwenden. `actualWorkRequired` können nicht mehr in Berechnungen und Formeln verwendet werden.

Außerdem wird dringend empfohlen, `actualWorkRequiredDouble` in allen Berichten zu verwenden.

Beachten Sie beim Ersetzen des Felds, dass `actualWorkRequired` Werte in Minuten speichert, während `actualWorkRequiredDouble` Werte in Stunden mit Dezimalgenauigkeit speichert.

Weitere Informationen zu den tatsächlichen Stunden finden Sie unter [Tatsächliche Stunden anzeigen](/help/quicksilver/manage-work/tasks/task-information/actual-hours.md).

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
