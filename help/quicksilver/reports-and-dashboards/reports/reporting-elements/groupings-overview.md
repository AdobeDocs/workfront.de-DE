---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Gruppierungsübersicht in Adobe Workfront
description: Sie können Gruppierungen hinzufügen, um das Layout der Informationen in Ihren Berichten und Listen zu verwalten.
author: Nolan
feature: Reports and Dashboards
exl-id: d050372e-c4a0-4c49-b220-5b35334ab8d0
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 0%

---

# Gruppierungsübersicht in Adobe Workfront

<!-- Audited: 11/2024 -->

<!--(NOTE: This article was supposed to be replaced by "Groupings overview", but decided to keep this here because this is linked in too many places. "Create groupings" and "Edit existing groupings" have been added also (with videos) to replace portions of the old content here.)-->

Sie können Gruppierungen hinzufügen, um das Layout der Informationen in Ihren Berichten und Listen zu verwalten.

Es gibt folgende Möglichkeiten, Berichte mit Gruppierungen zu versehen:

* Gruppierungen lassen sich durch die Bearbeitung vorhandener Gruppierungen erstellen.

  Informationen zum Anpassen einer vorhandenen Gruppierung finden Sie unter [Vorhandene Gruppierungen bearbeiten](../../../reports-and-dashboards/reports/reporting-elements/edit-existing-groupings.md).

* Sie können Gruppierungen von Grund auf neu erstellen.

  Informationen zum Erstellen einer neuen Gruppierung finden Sie unter [Erstellen von Gruppierungen in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

Standardmäßig werden Gruppierungen in einem grau hervorgehobenen Bericht oder einer Liste angezeigt. Die Ergebnisse des Berichts bzw. der Liste werden ohne Hervorhebung in ihrer individuellen Gruppierung aufgelistet.

![Gruppierungsbeispiel](assets/grouping-example-blue.png)

Sie können einem Bericht bis zu drei Gruppierungen hinzufügen. Sie können Ihre Informationen mit bis zu vier Gruppierungen organisieren, indem Sie einen Matrix-Bericht erstellen. Weitere Informationen zu Matrix-Berichten finden Sie unter [Erstellen eines Matrix-Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

Die Zahl in Klammern hinter dem Gruppierungsnamen stellt die Anzahl der Ergebnisse unter dieser Gruppierung dar. Wenn Ihr Bericht mehrere Seiten umfasst, stellen Sie sicher, dass Sie die Ergebnisse im Bericht oder in der Liste mit &quot;*Alle*&quot; anzeigen, um unter jeder Gruppierung eine genaue Anzahl Ihrer Ergebnisse zu erhalten.

Beachten Sie beim Arbeiten mit Gruppierungen Folgendes:

* Sie können die Informationen in bestehenden Gruppierungen anpassen. Alle Benutzer, die die Gruppierungen anzeigen können, können Ihre Änderungen ebenfalls sehen.
* Ihr Workfront-Administrator muss Ihnen Zugriff auf die Optionen Filter, Ansichten und Gruppierungen bearbeiten gewähren, um Gruppierungen erstellen zu können.

  Informationen zum Gewähren des Zugriffs auf Filter, Ansichten und Gruppierungen finden Sie unter [Gewähren des Zugriffs auf Filter, Ansichten und Gruppierungen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Ihre Berechtigungen für eine Gruppierung bestimmen, wie eine Gruppierung gespeichert wird. Wenn Sie die Gruppierung ursprünglich erstellt haben, können Sie die Änderungen speichern. Andernfalls werden Sie aufgefordert, eine Version der Gruppierung zu speichern. Wenn Sie Änderungen an einer Gruppierung vornehmen, die Sie für andere freigegeben haben, wirkt sich dies auch auf diese aus.
* Sie können eine Gruppierung anpassen, die nur dann für Sie freigegeben wurde, wenn Ihnen der Benutzer, der sie freigegeben hat, Zugriff auf Verwalten gewährt hat. Informationen zum Freigeben einer Gruppierung finden Sie unter [Freigeben eines Filters, einer Ansicht oder einer Gruppierung](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
* Eine inline-Gruppierung kann nicht bearbeitet werden.
* Sie können keine Gruppierung nach benutzerdefinierten Feldern mit Mehrfachauswahl (z. B. Kontrollkästchen) oder nach Feldern vornehmen, die mehrere Werte aufweisen können (z. B. Resource Manager).

## Zusätzliche Informationen zu Gruppierungen

Bei der Verwendung von Gruppierungen können Sie die Berichtinformationen weiter verwalten, indem Sie die Werte in den einzelnen Spalten der Gruppierungszeile aggregieren und Ihre Daten nach dem Feld Ihrer Gruppierung sortieren. Sie können eine Gruppierung auch entfernen, wenn sie nicht mehr benötigt wird.

* [Aggregierte Werte in Gruppierungen](#aggregate-values-in-groupings)
* [Sortieren nach einer Gruppierung](#sort-by-a-grouping)
* [Gruppierung entfernen](#remove-a-grouping)

### Aggregierte Werte in Gruppierungen {#aggregate-values-in-groupings}

Sie können die in Ihrem Bericht angezeigten Daten in Ihrer Gruppierungszeile aggregieren, indem Sie die Werte in den einzelnen Spalten des Berichts zusammenfassen. Weitere Informationen zur Zusammenfassung von Spaltendaten in einer Gruppierung finden Sie unter [Übersicht über Ansichten in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

>[!NOTE]
>
>Die folgenden Ausnahmen gelten für übergeordnete Objekte (z. B. übergeordnete Aufgaben), wenn Sie Werte für die folgenden Felder in Gruppierungen aggregieren:
>
>* Alle Zahlungs- und Währungsfelder außer &quot;Tatsächliche Stunden&quot;(z. B. geplante/tatsächliche Arbeitskosten, Geplante/tatsächliche Kosten, Geplante/tatsächliche Kosten, Geplante/tatsächliche Kosten, Geplante Stunden) aggregieren nur die Werte für die untergeordneten Aufgaben und eigenständigen Aufgaben. Sie aggregieren nicht die Werte für die übergeordneten Aufgaben oder die übergeordneten Elemente der übergeordneten Aufgaben.
>* Die tatsächlichen Stunden aggregieren die Werte für die Hauptaufgaben und Einzelaufgaben; sie aggregieren nicht die Zahlen für die übergeordneten Aufgaben oder die untergeordneten Aufgaben.
>* Benutzerdefinierte Datenfelder für Zahlungs- und Währungswerte aggregieren alle Aufgaben: Eltern, Kinder, Eltern und eigenständige Aufgaben.

### Nach Gruppierung sortieren {#sort-by-a-grouping}

Gruppierungen können nicht sortiert werden. Ansichten können sortiert werden. Um eine Liste nach dem in der Gruppierung erfassten Wert zu sortieren, müssen Sie denselben Wert in eine der Spalten der Ansicht einfügen und die Sortierung in der Ansicht anwenden. Auf diese Weise sortiert die Liste indirekt nach dem Wert in der Gruppierung (sie sortiert nach dem Wert in der Ansicht, der auch in der Gruppierung erfasst wird). Weitere Informationen zum Erstellen von Ansichten und Sortieren nach Werten in den Ansichten finden Sie unter [Übersicht über Ansichten in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### Gruppierung entfernen {#remove-a-grouping}

Wie Sie eine Gruppierung entfernen, hängt davon ab, ob Sie die Gruppierung ursprünglich erstellt haben oder ob die Gruppierung für Sie freigegeben wurde. Eine Standardgruppierung kann nicht entfernt werden.

* **Wenn Sie die Gruppierung erstellt und entfernt haben**, wird die Gruppierung aus dem Workfront-System entfernt. Die Gruppierung steht Benutzern, für die Sie sie zuvor freigegeben haben, nicht mehr zur Verfügung.
* **Wenn die Gruppierung für Sie freigegeben wurde und Sie sie entfernen**, wird die Gruppierung nur für Sie entfernt. Der Benutzer, der die Gruppe ursprünglich erstellt hat, und alle anderen Benutzer, für die sie freigegeben wurde, haben weiterhin Zugriff auf die Gruppierung.

Informationen zum Entfernen einer Gruppierung finden Sie im Artikel [Filter, Ansichten und Gruppierungen entfernen](../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).
