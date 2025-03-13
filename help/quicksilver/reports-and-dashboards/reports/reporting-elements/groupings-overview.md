---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Übersicht über Gruppierungen in Adobe Workfront
description: Sie können Gruppierungen hinzufügen, um das Layout der Informationen in Ihren Berichten und Listen zu verwalten.
author: Nolan
feature: Reports and Dashboards
exl-id: d050372e-c4a0-4c49-b220-5b35334ab8d0
source-git-commit: 69dec186cdb8a6d29853703edb41073282cdd447
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---

# Übersicht über Gruppierungen in Adobe Workfront

<!-- Audited: 11/2024 -->

<!--(NOTE: This article was supposed to be replaced by "Groupings overview", but decided to keep this here because this is linked in too many places. "Create groupings" and "Edit existing groupings" have been added also (with videos) to replace portions of the old content here.)-->

Sie können Gruppierungen hinzufügen, um das Layout der Informationen in Ihren Berichten und Listen zu verwalten.

Sie können wie folgt Gruppierungen zu Berichten hinzufügen:

* Sie können Gruppierungen erstellen, indem Sie vorhandene Gruppierungen bearbeiten.

  Informationen zum Anpassen einer vorhandenen Gruppierung finden Sie unter [Bearbeiten vorhandener Gruppierungen](../../../reports-and-dashboards/reports/reporting-elements/edit-existing-groupings.md).

* Sie können Gruppierungen von Grund auf erstellen.

  Informationen zum Erstellen einer neuen Gruppierung finden Sie unter [Gruppierungen in Adobe Workfront erstellen](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

Gruppierungen werden in Ihrem Bericht oder Ihrer Liste standardmäßig mit einer grauen Hervorhebung angezeigt. Die Ergebnisse des Berichts oder der Liste werden unter ihrer jeweiligen Gruppierung ohne Hervorhebung aufgelistet.

![Gruppierungsbeispiel](assets/grouping-example-blue.png)

Sie können einem Bericht bis zu drei Gruppierungen hinzufügen. Sie können Ihre Informationen mit bis zu vier Gruppierungen organisieren, indem Sie einen Matrixbericht erstellen. Weitere Informationen zu Matrixberichten finden Sie unter [Erstellen eines Matrixberichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

Die Zahl in Klammern nach dem Namen der Gruppierung gibt die Anzahl der Ergebnisse unter dieser Gruppierung an. Wenn Ihr Bericht mehrere Seiten umfasst, stellen Sie sicher, dass Sie *Alle* Ergebnisse im Bericht oder in der Liste anzeigen, um eine genaue Anzahl für Ihre Ergebnisse unter jeder Gruppierung zu erhalten.

Beachten Sie beim Arbeiten mit Gruppierungen Folgendes:

* Sie können die Informationen in vorhandenen Gruppierungen anpassen. Alle Benutzer, die die Gruppierungen anzeigen können, können auch Ihre Änderungen sehen.
* Ihr Workfront-Administrator muss Ihnen Zugriff auf das Bearbeiten von Filtern, Ansichten und Gruppierungen gewähren, um Gruppierungen zu erstellen.

  Informationen zum Gewähren des Zugriffs auf Filter, Ansichten und Gruppierungen finden Sie unter [Gewähren des Zugriffs auf Filter, Ansichten und Gruppierungen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Die Berechtigungsstufe einer Gruppierung bestimmt, wie eine Gruppierung gespeichert wird. Wenn Sie die Gruppierung ursprünglich erstellt haben, können Sie die Änderungen speichern. Andernfalls werden Sie aufgefordert, eine Version der Gruppierung zu speichern. Wenn Sie Änderungen an einer Gruppierung vornehmen, die Sie für andere freigegeben haben, wirkt sich dies auch auf sie aus.
* Sie können eine Gruppierung, die für Sie freigegeben wurde, nur dann anpassen, wenn Ihnen der Benutzer, der sie freigegeben hat, Zugriff verwalten gewährt hat. Informationen zur Freigabe einer Gruppierung finden Sie unter [Freigeben eines Filters, einer Ansicht oder einer Gruppierung](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
* Eine Gruppierung kann nicht inline bearbeitet werden.
* Sie können nicht nach benutzerdefinierten Feldern mit Mehrfachauswahl (z. B. Kontrollkästchen) oder nach Feldern gruppieren, die mehrere Werte haben können (z. B. Ressourcen-Manager).

## Zusätzliche Informationen zu Gruppierungen

Sie können Berichtsinformationen bei der Verwendung von Gruppierungen weiter verwalten, indem Sie die Werte in den einzelnen Spalten der Gruppierungszeile aggregieren und Ihre Informationen nach dem Feld Ihrer Gruppierung sortieren. Sie können eine Gruppierung auch entfernen, wenn sie nicht mehr benötigt wird.

* [Aggregierte Werte in Gruppierungen](#aggregate-values-in-groupings)
* [Nach Gruppierung sortieren](#sort-by-a-grouping)
* [Gruppierung entfernen](#remove-a-grouping)

### Aggregierte Werte in Gruppierungen {#aggregate-values-in-groupings}

Sie können die im Bericht angezeigten Daten in Ihrer Gruppierungszeile aggregieren, indem Sie die Werte in den einzelnen Spalten des Berichts zusammenfassen. Weitere Informationen über die Zusammenfassung von Spaltendaten in einer Gruppierung finden Sie unter [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).


>[!NOTE]
>
>Die folgenden Ausnahmen gelten für übergeordnete Objekte (z. B. übergeordnete Aufgaben), wenn Sie Werte für die folgenden Felder in > Gruppierungen aggregieren:
>
>* Alle Zahlen-, Währungs- und Datumsfelder außer „Tatsächliche Stunden“ aggregieren Werte nur für untergeordnete Aufgaben und eigenständige Aufgaben. Sie aggregieren keine Werte für übergeordnete Aufgaben oder übergeordnete Elemente von übergeordneten Elementen. Bei der Aggregation von Zahlen-, Währungs- und Datumsfeldern in einer Liste, die nur übergeordnete Aufgaben enthält, wird in der Gruppierungsleiste kein aggregierter Wert angezeigt.
>
>* Tatsächliche Stunden aggregieren Werte für die übergeordneten und eigenständigen Hauptaufgaben. Sie aggregieren nicht die Zahlen für untergeordnete Aufgaben oder die übergeordneten Aufgaben. <!--Examples of Actual hours include Planned/Actual Labor Cost, Planned/Actual Expense Cost, Planned/Actual Cost, and Planned Hours.-->
>
>* Benutzerdefinierte Datenfelder für Zahlen- und Währungswerte aggregieren alle Aufgaben: Eltern, Kinder, Eltern von Eltern und eigenständige Aufgaben.


### Nach Gruppierung sortieren {#sort-by-a-grouping}

Gruppierungen können nicht sortiert werden. Ansichten können sortiert werden. Um eine Liste nach dem in der Gruppierung erfassten Wert zu sortieren, müssen Sie denselben Wert in eine der Spalten der Ansicht aufnehmen und die Sortierung in der Ansicht anwenden. Auf diese Weise sortiert die Liste indirekt nach dem Wert in der Gruppierung (sie sortiert nach dem Wert in der Ansicht, der auch in der Gruppierung erfasst wird). Weitere Informationen zum Erstellen von Ansichten und Sortieren nach Werten in den Ansichten finden Sie unter [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### Gruppierung entfernen {#remove-a-grouping}

Wie Sie eine Gruppierung entfernen, hängt davon ab, ob Sie die Gruppierung ursprünglich erstellt haben oder ob die Gruppierung für Sie freigegeben wurde. Standardgruppierung kann nicht entfernt werden.

* **Wenn Sie die Gruppierung erstellt und entfernt haben** wird die Gruppierung aus dem Workfront-System entfernt. Die Gruppierung steht Benutzern, für die Sie sie zuvor freigegeben haben, nicht mehr zur Verfügung.
* **Wenn die Gruppierung für Sie freigegeben wurde und Sie sie entfernen** wird die Gruppierung nur für Sie entfernt. Der Benutzer, der sie ursprünglich erstellt hat, und alle anderen Benutzer, für die sie freigegeben wurde, haben weiterhin Zugriff auf die Gruppierung.

Informationen zum Entfernen einer Gruppierung finden Sie im Artikel [Entfernen von Filtern, Ansichten und Gruppierungen](../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).


<!--Original note

The following exceptions apply for parent objects (for example, parent tasks) when you are aggregating values for the following fields in groupings:
All the number and currency fields except Actual Hours (for example, Planned/ Actual Labor Cost, Planned/ Actual Expense Cost, Planned/ Actual Cost, Planned Hours) aggregate only the values for the children tasks, and standalone tasks. They do not aggregate the values for the parent tasks or parents of parents.
Actual Hours aggregate the values for the main parent and the standalone tasks; they do not aggregate the numbers for the parents of parent tasks or the children tasks.
Custom data fields for number and currency values aggregate all tasks: parents, children, parents of parents, and standalone tasks.

-->