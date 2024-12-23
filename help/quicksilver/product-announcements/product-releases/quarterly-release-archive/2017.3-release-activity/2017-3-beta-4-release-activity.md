---
content-type: release-notes
navigation-topic: product-releases-archive
title: Beta-Version 2017.3
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 4-Version 2017.3 verfügbar waren. Die Funktionalität auf dieser Seite wurde in der Vorschau-Umgebung in der Woche vom 25. September 2017 bereitgestellt. Sie wird Anfang November 2017 in der Produktionsumgebung zur Verfügung gestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d6bb889c-a057-453f-8f80-761cfb1ad4a1
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '1676'
ht-degree: 0%

---

# Beta-Version 2017.3

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 4-Version 2017.3 verfügbar waren. Die Funktionalität auf dieser Seite wurde in der Vorschau-Umgebung in der Woche vom 25. September 2017 bereitgestellt. Sie wird Anfang November 2017 in der Produktionsumgebung zur Verfügung gestellt.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktionalität kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller 2017.3 vorgenommenen Änderungen finden Sie unter  [Übersicht über die Veröffentlichungsaktivität 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

Die Version 2017.3 von Beta 4 enthält Verbesserungen für Workfront-Administratoren und andere Benutzer:

**Für Administratoren**

* [Neuer Bereich &quot;Voreinstellungen für die Ressourcenverwaltung&quot;im Setup-Bereich](#new-resource-management-preferences-area-in-the-setup-area)

**Für alle Benutzer**

* [Aufgaben duplizieren](#duplicate-tasks)
* [Automatisieren von Zuweisungen bei der Planung von Ressourcen](#automate-assignments-when-scheduling-resources)
* [Ändern von Zuweisungen für mehrere Aufgaben bei der Planung von Ressourcen](#modify-assignments-for-multiple-tasks-when-scheduling-resources)
* [Wenden Sie die FTE-Verteilung auf den Ressourcenplaner an](#apply-fte-distribution-to-the-resource-planner)
* [Aufgabenrollenabschnitt für Benutzereinstellungen enthält den Prozentsatz der FTE-Verfügbarkeit](#job-role-section-for-user-settings-includes-percentage-of-fte-availability)
* [Speichern und Verwalten von Filtern im Nutzungsbericht für ein Projekt](#save-and-manage-filters-in-the-utilization-report-on-a-project)
* [Zusätzliche Filteroptionen im Nutzungsbericht](#additional-filtering-options-in-the-utilization-report)
* [Anzeigen des Nutzungsberichts nach Programm oder Portfolio](#view-the-utilization-report-by-program-or-portfolio)
* [Informationen zum ursprünglichen Problem in Projekt- und Aufgabenberichten anzeigen](#show-original-issue-information-in-project-and-task-reports)
* [Filtern von Systemaktualisierungen im Aktualisierungs-Stream ist jetzt über Objekte hinweg persistent](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [Bericht zu aktiven Testsendungen in Workfront](#report-on-active-proof-stages-within-workfront)
* [Benutzerdefinierte Workfront Proof-Berechtigungsprofile Benutzern in Workfront zuweisen](#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront)
* [Stündliche Ressource zu Ereignisabonnements hinzugefügt](#hour-resource-added-to-event-subscriptions)

## Aufgaben duplizieren {#duplicate-tasks}

Sie können jetzt eine Aufgabe oder eine Reihe von Aufgaben in einem Projekt schnell duplizieren. Diese Aktion erstellt eine identische Aufgabe wie die ursprüngliche. Während des Duplizierungsvorgangs gibt es keine zusätzlichen Optionen, mit denen Sie Änderungen an der neu erstellten Aufgabe vornehmen können.  

Vor dieser Änderung können Sie eine Aufgabe in ein neues Projekt oder das vorhandene Projekt kopieren und Informationen beim Kopieren ändern.

Für  Weitere Informationen zum Duplizieren von Aufgaben finden Sie unter [Aufgaben kopieren und duplizieren](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

## Automatisieren von Zuweisungen bei der Planung von Ressourcen {#automate-assignments-when-scheduling-resources}

>[!NOTE]
>
>Die Tools für die Ressourcenplanung wurden mit Version 23.1 eingestellt und aus Workfront entfernt. Weitere Informationen zum Planen von Ressourcen mit dem Lastenausgleich finden Sie unter [Übersicht über den Lastenausgleich](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Sie können jetzt zulassen, dass Workfront automatisch Zuweisungen für nicht zugewiesene Aufgaben und Probleme vorschlägt, wenn Ressourcen für mehrere Projekte geplant werden (auf der Registerkarte Planung ) oder wenn Ressourcen für ein einzelnes Projekt geplant werden (auf der Registerkarte Strukturierung ).

Workfront analysiert aktuelle Arbeitsaufgaben für alle Benutzer und schlägt intelligente, logische Zuweisungen für Aufgaben oder Probleme vor, die noch nicht zugewiesen sind. Sie können alle vorgeschlagenen oder vorhandenen Zuweisungen ändern, bevor Sie die Zuweisungen abschließen.

Weitere Informationen finden Sie unter &quot;Nicht zugewiesene Aufgaben und Probleme manuell in den Planungsbereichen zuweisen&quot;.

## Ändern von Zuweisungen für mehrere Aufgaben bei der Planung von Ressourcen {#modify-assignments-for-multiple-tasks-when-scheduling-resources}

Beim Zuweisen, Austauschen oder Aufheben der Zuweisung von Benutzern in großen Mengen beim Planen von Ressourcen (entweder auf der Registerkarte Planung oder auf der Registerkarte Strukturierung ) können Sie jetzt Zuweisungen für bestimmte Aufgaben ändern, die Sie in einem oder mehreren Projekten (einschließlich aller Unteraufgaben und zugehörigen Probleme) festlegen.

Vor dieser Änderung konnten Sie Zuweisungen zu Aufgaben und Problemen nur in ganzen Projekten ändern (Sie konnten innerhalb eines Projekts keine bestimmten Aufgaben bestimmen).

Weitere Informationen finden Sie unter &quot;Nicht zugewiesene Aufgaben und Probleme manuell in den Planungsbereichen zuweisen&quot;.

## Anwenden der FTE-Verteilung auf den Ressourcenplaner {#apply-fte-distribution-to-the-resource-planner}

>[!NOTE]
>
>Diese Funktion ist derzeit nicht in der Vorschau für alle Cluster verfügbar.

Sie können jetzt die korrekte Anzahl der verfügbaren Stunden für jede Benutzerrolle basierend auf dem Prozentsatz der FTE-Verfügbarkeit für jede Rolle anzeigen, wenn Benutzer mehr als eine Rolle haben.

Wenn beispielsweise der Zeitplan eines Benutzers angibt, dass er 100 Stunden in einem Monat arbeiten kann und der Prozentsatz der FTE-Verfügbarkeit für die Primäre Rolle 75 % beträgt und der Prozentsatz der FTE-Verfügbarkeit seiner anderen Rolle 25 % beträgt, wird der Benutzer im Ressourcenplaner unter der Primären Rolle 75 Stunden und unter seiner anderen Rolle 25 Stunden aufgeführt. einnehmen.

Vor dieser Änderung wurde der Benutzername, der nur für die Primäre Rolle im Ressourcenplaner angezeigt wurde, und die vollständige Verfügbarkeit des Benutzers basierend auf seinem Zeitplan (100 Stunden) nur mit der Primären Rolle verknüpft. Die &quot;Andere Rolle&quot;des Benutzers wird nur dann im Ressourcenplaner angezeigt, wenn dem Benutzer eine Aufgabe mit dieser Rolle zugewiesen wurde und die &quot;Verfügbare Stunden&quot;für den Benutzer in der &quot;Andere Rolle&quot;null waren.

Weitere Informationen dazu, wie Verfügbare Stunden und verfügbare FTEs für Benutzer und Rollen im Resource Planer berechnet werden, finden Sie unter [Übersicht über die Berechnung von Stunden und FTE für Benutzer und Rollen im Resource Planer](../../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

## Aufgabenbereich für Benutzereinstellungen enthält den Prozentsatz der FTE-Verfügbarkeit {#job-role-section-for-user-settings-includes-percentage-of-fte-availability}

>[!NOTE]
>
>Diese Funktion ist derzeit nicht in der Vorschau für alle Cluster verfügbar.

Bei der Aktualisierung eines Benutzerprofils können Sie nun einem Benutzer zusätzliche Vorgangsrollen hinzufügen und den Prozentsatz der FTE definieren, der jeder Auftragsrolle zugewiesen ist.

Vor dieser Änderung konnten Sie keiner der Auftragsrollen, mit denen der Benutzer verknüpft war, eine bestimmte FTE zuweisen.

Weitere Informationen zum Aktualisieren des Prozentsatzes der FTE-Verfügbarkeit für die Benutzerrollen finden Sie unter [Profil eines Benutzers bearbeiten](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) oder [Meine Einstellungen konfigurieren](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

## Neuer Bereich &quot;Voreinstellungen für die Ressourcenverwaltung&quot;im Setup-Bereich {#new-resource-management-preferences-area-in-the-setup-area}

Sie können jetzt einen neuen Bereich unter Einrichtung finden, der &quot;Ressourcenverwaltung&quot;heißt. In diesem Bereich haben wir eine Einstellung eingeführt, mit der Sie angeben können, wie die Benutzerverfügbarkeit im Ressourcenplaner berechnet werden soll. Sie können sie mit den folgenden Methoden berechnen:

* Manuell: Der Standardzeitplan des Systems zusätzlich zur individuellen FTE des Benutzers wird verwendet, um die Stundenverfügbarkeit des Benutzers im Ressourcenplaner zu bestimmen. Der Zeitplan des Benutzers wird ignoriert.
* Automatisch: Der Zeitplan des Benutzers wird verwendet, um die Stundenverfügbarkeit des Benutzers im Ressourcenplaner zu bestimmen. Die FTE-Verfügbarkeit wird auf der Basis des Benutzerzeitplans und des Standardzeitplans berechnet. Der Wert der FTE des Benutzers wird ignoriert. 

Weitere Informationen zum Konfigurieren der Voreinstellungen für die Ressourcenverwaltung für Ihr System finden Sie unter [Voreinstellungen für die Ressourcenverwaltung konfigurieren](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Filter im Nutzungsbericht für ein Projekt speichern und verwalten {#save-and-manage-filters-in-the-utilization-report-on-a-project}

Jetzt können Sie Filter speichern, die Sie im Bericht &quot;Nutzung&quot;erstellen. Darüber hinaus können Sie einen gespeicherten Filter umbenennen, einen gespeicherten Filter duplizieren, einen gespeicherten Filter löschen oder einen gespeicherten Filter ändern.

Zuvor mussten Sie jedes Mal, wenn Sie den Bericht &quot;Nutzung&quot;gefiltert haben, einzelne Filteroptionen angeben.

Weitere Informationen zum Speichern und Verwalten von Filtern im Bericht &quot;Nutzung&quot;finden Sie unter [Überblick über den Bericht &quot;Ressourcenauslastung&quot;](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [Überblick über den Bericht &quot;Ressourcenauslastung&quot;](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Zusätzliche Filteroptionen im Nutzungsbericht {#additional-filtering-options-in-the-utilization-report}

Beim Ausführen des Nutzungsprogramms-Berichts stehen jetzt beim Erstellen des Filters neue Filterfelder für Portfolios, Programme und Projekte zur Verfügung, zusätzlich zu den zuvor verfügbaren Feldern Aufgaben, Probleme und Rollen .

Vor dieser Änderung konnten Sie nur durch Hinzufügen einer neuen Filterregel nach Portfolio, Programm und Projekt filtern.

Weitere Informationen finden Sie unter [Überblick über den Bericht &quot;Ressourcenauslastung&quot;](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [Überblick über den Bericht &quot;Ressourcenauslastung&quot;](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Anzeigen des Nutzungsberichts nach Programm oder Portfolio {#view-the-utilization-report-by-program-or-portfolio}

Sie können jetzt einen Nutzungsbericht nach Programm oder Portfolio anzeigen. Auf diese Weise können Sie Informationen aus mehreren Projekten in einem einzigen Nutzungsbericht anzeigen.

Um diese Änderung zu erleichtern, ist die Registerkarte &quot;Nutzung&quot;jetzt sowohl im Bereich &quot;Berichterstellung&quot;in Workfront als auch in einem einzelnen Projekt verfügbar.

Vor dieser Änderung konnte nur innerhalb eines Projekts auf Nutzungsberichte zugegriffen werden.

Weitere Informationen finden Sie unter  [Überblick über den Bericht &quot;Ressourcenauslastung&quot;](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md). 

## Informationen zum ursprünglichen Problem in Projekt- und Aufgabenberichten anzeigen {#show-original-issue-information-in-project-and-task-reports}

>[!NOTE]
>
>Diese Funktion ist derzeit nicht in der Vorschau für alle Cluster verfügbar.

Sie finden jetzt die folgenden Informationen zum ursprünglichen Problem in einem Projekt- oder Aufgabenbericht für die Projekte und Aufgaben, die durch Konvertieren eines Problems erstellt wurden:

* Ursprüngliches Ausgabedatum
* Ursprünglicher Name des Problems
* Ursprüngliche Ausgabe - Urheber-ID

Diese Informationen können in einem Aufgaben- oder Projektbericht oder einer Liste angezeigt werden, indem eine benutzerdefinierte Ansicht im Textmodus erstellt wird.

Vor dieser Änderung konnten Sie keine Berichte zu diesen Informationen erstellen.

Weitere Informationen zum Erstellen der benutzerdefinierten Textmodusansicht, in der die Informationen aus dem ursprünglichen Problem erfasst werden, finden Sie unter [Ansicht: Informationen zu ursprünglichen Problemen in Aufgaben- oder Projektlisten anzeigen](../../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

## Filtern von Systemaktualisierungen im Aktualisierungs-Stream ist jetzt über Objekte hinweg persistent {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

>[!NOTE]
>
>Diese Funktion wurde in der Vorschauumgebung mit Beta 4 nicht veröffentlicht. Sie wird in der ersten Oktober-Jahreshälfte in der Vorschau verfügbar sein.

Die Option &quot;Systemaktualisierungen filtern&quot;ist jetzt auf der gesamten Workfront-Site über Objekte hinweg persistent. Auf diese Weise können Sie Systemaktualisierungen ausblenden und nur Benutzerkommentare im Update-Stream eines Objekts anzeigen. Diese Einstellung bleibt erhalten, wenn Sie zu anderen Objekten navigieren.

Vor dieser Änderung mussten Sie bei der Navigation auf der Workfront-Site Systemaktualisierungen für jedes Objekt herausfiltern.

Weitere Informationen finden Sie unter [Funktionsweise aktualisieren](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Bericht zu aktiven Testsendungen in Workfront {#report-on-active-proof-stages-within-workfront}

Beim Erstellen eines Berichts &quot;Dokumentversion&quot;in Workfront gibt es jetzt eine Spalte namens &quot;Aktive Testsendungen&quot;. In dieser Spalte können Sie die Testversand-Phase einsehen, die derzeit für jede Dokumentversion des Berichts aktiv ist. Der Name der Bühne wird in der Spalte &quot;Aktive Testsendungen&quot;angezeigt. Wenn in der Dokumentversion derzeit keine Bühne aktiv ist, ist die Spalte leer.

Weitere Informationen zu verfügbaren Feldern in Ansichten und Berichten finden Sie unter [Glossar der Adobe Workfront-Terminologie](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Benutzerdefinierte Workfront Proof-Berechtigungsprofile Benutzern in Workfront zuweisen {#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront}

Wenn Sie jetzt Testversandfunktionen für einen Benutzer in Workfront aktivieren, können Sie ein benutzerdefiniertes Workfront Proof-Berechtigungsprofil zuweisen. 

Vor dieser Änderung waren nur die folgenden Berechtigungsprofile verfügbar: Supervisor, Manager, Administrator.

## Stündliche Ressource zu Ereignisabonnements hinzugefügt {#hour-resource-added-to-event-subscriptions}

Mit der neuen Ressource Stunde können Sie jetzt ein Ereignisabonnement erstellen, um Ihre Abrechnungsanwendung mit Workfront synchronisieren zu können.

Weitere Informationen zu Ereignisanmeldungen finden Sie unter [Ereignis-Abonnement-API](../../../../wf-api/general/event-subs-api.md).
