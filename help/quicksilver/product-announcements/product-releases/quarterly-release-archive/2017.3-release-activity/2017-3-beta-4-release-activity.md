---
content-type: release-notes
navigation-topic: product-releases-archive
title: Versionsaktivität von Beta 4 2017.3
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 4 Version 2017.3 verfügbar waren. Die Funktion auf dieser Seite wurde in der Woche vom 25. September 2017 in der Vorschau-Umgebung verfügbar gemacht. Sie wird Anfang November 2017 in der Produktionsumgebung bereitgestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d6bb889c-a057-453f-8f80-761cfb1ad4a1
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '1676'
ht-degree: 0%

---

# Versionsaktivität von Beta 4 2017.3

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 4 Version 2017.3 verfügbar waren. Die Funktion auf dieser Seite wurde in der Woche vom 25. September 2017 in der Vorschau-Umgebung verfügbar gemacht. Sie wird Anfang November 2017 in der Produktionsumgebung bereitgestellt.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktion kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen in Version 2017.3 finden Sie unter  [Übersicht über die Versionsaktivität 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

Die Beta 4-Version 2017.3 enthält Verbesserungen für Workfront-Administratoren und andere Benutzende:

**Für Administratoren**

* [Neuer Bereich „Voreinstellungen für Ressourcenverwaltung“ im Bereich „Setup“](#new-resource-management-preferences-area-in-the-setup-area)

**Für alle Benutzer**

* [Aufgaben duplizieren](#duplicate-tasks)
* [Automatisieren von Zuweisungen beim Planen von Ressourcen](#automate-assignments-when-scheduling-resources)
* [Ändern von Zuweisungen für mehrere Aufgaben beim Planen von Ressourcen](#modify-assignments-for-multiple-tasks-when-scheduling-resources)
* [FTE-Verteilung auf den Ressourcenplaner anwenden](#apply-fte-distribution-to-the-resource-planner)
* [Abschnitt „Aufgabengebiet“ für Benutzereinstellungen enthält Prozentsatz der FTE-Verfügbarkeit](#job-role-section-for-user-settings-includes-percentage-of-fte-availability)
* [Speichern und Verwalten von Filtern im Auslastungsbericht für ein Projekt](#save-and-manage-filters-in-the-utilization-report-on-a-project)
* [Zusätzliche Filteroptionen im Auslastungsbericht](#additional-filtering-options-in-the-utilization-report)
* [Anzeigen des Auslastungsberichts nach Programm oder Portfolio &#x200B;](#view-the-utilization-report-by-program-or-portfolio)
* [Ursprüngliche Anfrageinformationen in Projekt- und Aufgabenberichten anzeigen](#show-original-issue-information-in-project-and-task-reports)
* [Filtersystemaktualisierungen im Aktualisierungsstrom sind jetzt objektübergreifend persistent](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [Berichte zu aktiven Korrekturabzugsschritten in Workfront](#report-on-active-proof-stages-within-workfront)
* [Zuweisen benutzerdefinierter Workfront Proof-Berechtigungsprofile zu Benutzenden in Workfront](#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront)
* [Stundenressource wurde zu Ereignisabonnements hinzugefügt](#hour-resource-added-to-event-subscriptions)

## Aufgaben duplizieren {#duplicate-tasks}

Sie können jetzt eine Aufgabe oder eine Reihe von Aufgaben innerhalb eines Projekts schnell duplizieren. Diese Aktion erstellt eine Aufgabe, die mit der ursprünglichen Aufgabe identisch ist. Während des Duplizierungsprozesses gibt es keine zusätzlichen Optionen, mit denen Sie Änderungen an der neu erstellten Aufgabe vornehmen können.  

Vor dieser Änderung konnten Sie eine Aufgabe entweder in ein neues Projekt oder in das vorhandene Projekt kopieren und einige Informationen ändern, während Sie sie kopiert haben.

für  Weitere Informationen zum Duplizieren von Aufgaben finden Sie unter [Aufgaben kopieren und duplizieren](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

## Zuweisungen beim Planen von Ressourcen automatisieren {#automate-assignments-when-scheduling-resources}

>[!NOTE]
>
>Die Tools zur Ressourcenplanung werden nicht mehr unterstützt und mit Version 23.1 aus Workfront entfernt. Informationen zur Planung von Ressourcen mit dem Workload Balancer finden Sie unter [Übersicht über den Workload Balancer](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Sie können jetzt Workfront erlauben, automatisch Arbeitsaufträge für nicht zugewiesene Aufgaben und Probleme vorzuschlagen, wenn Ressourcen für mehrere Projekte geplant werden (über die Registerkarte Planung ) oder wenn Ressourcen für ein einzelnes Projekt geplant werden (über die Registerkarte Personal ).

Workfront analysiert aktuelle Arbeitszuweisungen Ihrer verfügbaren Anwender und schlägt intelligente, logische Zuweisungen für alle Aufgaben oder Probleme vor, die noch nicht zugewiesen sind. Sie können alle vorgeschlagenen oder vorhandenen Zuweisungen ändern, bevor Sie die Zuweisungen abschließen.

Weitere Informationen finden Sie unter „Manuelles Zuweisen nicht zugewiesener Aufgaben und Probleme in den Zeitplanbereichen“.

## Ändern von Zuweisungen für mehrere Aufgaben beim Planen von Ressourcen {#modify-assignments-for-multiple-tasks-when-scheduling-resources}

Beim Massenzuweisen, Austauschen oder Aufheben der Zuweisung von Benutzern bei der Ressourcenplanung (entweder über die Registerkarte Planung oder die Registerkarte Personal) können Sie jetzt Zuordnungen für bestimmte Aufgaben ändern, die Sie in einem oder mehreren Projekten festlegen (einschließlich aller Unteraufgaben und zugehörigen Probleme).

Vor dieser Änderung konnten Sie Zuweisungen zu Aufgaben und Problemen nur projektübergreifend ändern (Sie konnten keine spezifischen Aufgaben innerhalb eines Projekts festlegen).

Weitere Informationen finden Sie unter „Manuelles Zuweisen nicht zugewiesener Aufgaben und Probleme in den Zeitplanbereichen“.

## FTE-Verteilung auf Ressourcenplaner anwenden {#apply-fte-distribution-to-the-resource-planner}

>[!NOTE]
>
>Diese Funktion ist derzeit nicht in der Vorschau für alle Cluster verfügbar.

Sie können jetzt für jede Rolle des Benutzers die richtige Anzahl verfügbarer Stunden basierend auf dem Prozentsatz der FTE-Verfügbarkeit für jede Rolle anzeigen, wenn Benutzer mehr als eine Rolle haben.

Wenn beispielsweise der Zeitplan eines Benutzers angibt, dass er in einem Monat 100 Stunden arbeiten kann und sein Prozentsatz der FTE-Verfügbarkeit für die Primäre Rolle 75 % und der Prozentsatz der FTE-Verfügbarkeit für die andere Rolle 25 % beträgt, listet der Ressourcenplaner den Benutzer mit 75 verfügbaren Stunden für die Primäre Rolle und mit 25 verfügbaren Stunden für die andere Rolle auf.

Vor dieser Änderung wurde der Name des/r Benutzenden, der/die nur für die Primäre Rolle im Ressourcenplaner angezeigt wurde, und die vollständige Verfügbarkeit des/r Benutzenden auf der Grundlage des Zeitplans (100 Stunden) nur mit der Primären Rolle verknüpft. Die Funktion „Sonstige“ des Benutzers wird nur dann im Ressourcenplaner angezeigt, wenn der Benutzer einer Aufgabe in dieser Funktion zugewiesen wurde und die verfügbaren Stunden für den Benutzer in der Funktion „Andere“ gleich null waren.

Weitere Informationen dazu, wie verfügbare Stunden und verfügbare VZÄ für Benutzer und Funktionen im Ressourcenplaner berechnet werden, finden Sie unter [Übersicht über die Berechnung von Stunden und VZÄ für Benutzer und Funktionen im Ressourcenplaner](../../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

## Aufgabengebiet für Benutzereinstellungen Enthält Prozentsatz der FTE-Verfügbarkeit {#job-role-section-for-user-settings-includes-percentage-of-fte-availability}

>[!NOTE]
>
>Diese Funktion ist derzeit nicht in der Vorschau für alle Cluster verfügbar.

Beim Aktualisieren eines Benutzerprofils können Sie jetzt einem Benutzer zusätzliche Aufgabengebiete hinzufügen und den Prozentsatz des VZÄ definieren, der jedem Aufgabengebiet zugewiesen ist.

Vor dieser Änderung konnten Sie keinem der Aufgabengebiete, mit denen der Benutzer verknüpft war, eine bestimmte FTE-Menge zuweisen.

Weitere Informationen zum Aktualisieren des Prozentsatzes der VZÄ-Verfügbarkeit für die Aufgabengebiete der Benutzenden finden Sie unter [Bearbeiten des Benutzerprofils](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) oder [Konfigurieren meiner Einstellungen](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

## Neuer Bereich „Voreinstellungen für Ressourcenverwaltung“ im Bereich „Setup“ {#new-resource-management-preferences-area-in-the-setup-area}

Im Setup finden Sie jetzt einen neuen Bereich namens Ressourcenverwaltung. In diesem Bereich haben wir eine Einstellung eingeführt, mit der Sie angeben können, wie die Benutzerverfügbarkeit im Ressourcenplaner berechnet werden soll. Sie können ihn mithilfe der folgenden Methoden berechnen:

* Manuell: Der Standardzeitplan des Systems wird zusätzlich zum individuellen FTE des Benutzers verwendet, um die Stundenverfügbarkeit des Benutzers im Ressourcenplaner zu bestimmen. Der Zeitplan des Benutzers wird ignoriert.
* Automatisch: Der Zeitplan des Benutzers wird verwendet, um die Stundenverfügbarkeit des Benutzers im Ressourcenplaner zu bestimmen. Die FTE-Verfügbarkeit wird anhand des Zeitplans des Benutzers und des Standardzeitplans berechnet. Der Wert des Vollzeitäquivalents (FTE) des Benutzers wird ignoriert. 

Weitere Informationen zum Konfigurieren der Ressourcenverwaltungseinstellungen für das System finden Sie unter [Ressourcenverwaltungseinstellungen konfigurieren](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Speichern und Verwalten von Filtern im Nutzungsbericht für ein Projekt {#save-and-manage-filters-in-the-utilization-report-on-a-project}

Jetzt können Sie Filter speichern, die Sie im Auslastungsbericht erstellen. Darüber hinaus können Sie einen gespeicherten Filter umbenennen, einen gespeicherten Filter duplizieren, einen gespeicherten Filter löschen oder einen gespeicherten Filter ändern.

Zuvor mussten Sie jedes Mal, wenn Sie den Auslastungsbericht filterten, einzelne Filteroptionen angeben.

Weitere Informationen zum Speichern und Verwalten von Filtern im Auslastungsbericht finden Sie unter [Übersicht über den &#x200B;](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [Übersicht über den Bericht zur Ressourcenauslastung](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Zusätzliche Filteroptionen im Auslastungsbericht {#additional-filtering-options-in-the-utilization-report}

Beim Ausführen des Auslastungsberichts sind jetzt beim Erstellen des Filters neue Filterfelder für Portfolios, Programme und Projekte verfügbar, zusätzlich zu den zuvor verfügbaren Feldern „Aufgaben“, „Probleme“ und „Rollen“.

Vor dieser Änderung konnten Sie nur durch Hinzufügen einer neuen Filterregel nach Portfolio, Programm und Projekt filtern.

Weitere Informationen finden Sie [Übersicht über den Ressourcenauslastungsbericht](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) unter [Übersicht über den Ressourcenauslastungsbericht](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Auslastungsbericht nach Programm oder Portfolio anzeigen {#view-the-utilization-report-by-program-or-portfolio}

Sie können jetzt einen Auslastungsbericht nach Programm oder Portfolio anzeigen. Auf diese Weise können Sie Informationen aus mehreren Projekten in einem einzigen Auslastungsbericht anzeigen.

Um diese Änderung zu erleichtern, ist die Registerkarte Nutzung jetzt sowohl im Bereich Reporting in Workfront als auch in einem einzelnen Projekt verfügbar.

Vor dieser Änderung konnten Nutzungsberichte nur innerhalb eines Projekts aufgerufen werden.

Weitere Informationen finden Sie unter  [Überblick über den Bericht zur Ressourcenauslastung](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md). 

## Ursprüngliche Anfrageinformationen in Projekt- und Aufgabenberichten anzeigen {#show-original-issue-information-in-project-and-task-reports}

>[!NOTE]
>
>Diese Funktion ist derzeit nicht in der Vorschau für alle Cluster verfügbar.

Die folgenden Informationen zur ursprünglichen Anfrage finden Sie jetzt in einem Projekt- oder Aufgabenbericht für die Projekte und Aufgaben, die durch die Konvertierung einer Anfrage erstellt wurden:

* Ursprüngliches Problem-Eingabedatum
* Name der ursprünglichen Anfrage
* Ursprüngliche Anfrage-Urheber-ID

Diese Informationen können in einem Aufgaben- oder Projektbericht oder einer Liste angezeigt werden, indem eine benutzerdefinierte Ansicht im Textmodus erstellt wird.

Vor dieser Änderung konnten Sie keine Berichte zu diesen Informationen erstellen.

Weitere Informationen zum Erstellen der benutzerdefinierten Textmodusansicht, in der die Informationen des ursprünglichen Problems erfasst werden, finden Sie unter [Ansicht: ursprüngliche Probleminformationen in Aufgaben- oder Projektlisten anzeigen](../../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

## Filtersystemaktualisierungen im Aktualisierungsstrom sind jetzt objektübergreifend persistent {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

>[!NOTE]
>
>Diese Funktion wurde nicht in der Vorschau-Umgebung mit Beta 4 veröffentlicht. Es wird in der ersten Oktoberhälfte in der Vorschau verfügbar sein.

Die Option Systemaktualisierungen filtern ist jetzt objektübergreifend auf der gesamten Workfront-Site persistent. Auf diese Weise können Sie Systemaktualisierungen ausblenden und nur Benutzerkommentare im Aktualisierungsverlauf für ein Objekt anzeigen. Diese Einstellung bleibt erhalten, wenn Sie zu anderen Objekten navigieren.

Vor dieser Änderung mussten Sie beim Durchsuchen der Workfront-Site für jedes Objekt Systemaktualisierungen herausfiltern.

Weitere Informationen finden Sie unter [Arbeit aktualisieren](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Berichte zu aktiven Korrekturabzugsschritten in Workfront {#report-on-active-proof-stages-within-workfront}

Beim Erstellen eines Dokumentversionsberichts in Workfront gibt es jetzt eine Spalte mit der Bezeichnung „Aktive Korrekturabzugsschritte“. In dieser Spalte können Sie die Phase des Korrekturabzugs anzeigen, die derzeit für jede Dokumentversion im Bericht aktiv ist. Der Name des Schritts wird in der Spalte „Aktive Korrekturabzugsschritte“ angezeigt. Wenn derzeit kein Schritt in der Dokumentversion aktiv ist, ist die Spalte leer.

Weitere Informationen zu den verfügbaren Feldern in Ansichten und Berichten finden Sie im [Glossar der Adobe Workfront-Terminologie](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Zuweisen benutzerdefinierter Workfront Proof-Berechtigungsprofile zu Benutzenden in Workfront {#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront}

Beim Aktivieren der Proofing-Funktionen für Benutzende in Workfront können Sie jetzt ein benutzerdefiniertes Workfront Proof-Berechtigungsprofil zuweisen. 

Vor dieser Änderung waren nur die folgenden Berechtigungsprofile verfügbar: Supervisor, Manager, Administrator.

## Stundenressource wurde zu Ereignisabonnements hinzugefügt {#hour-resource-added-to-event-subscriptions}

Mit der neuen Stundenressource können Sie jetzt ein Ereignisabonnement erstellen, um Ihre Abrechnungsanwendung mit Workfront synchronisiert zu halten.

Weitere Informationen zu Ereignisabonnements finden Sie unter [Ereignisabonnement-API](../../../../wf-api/general/event-subs-api.md).
