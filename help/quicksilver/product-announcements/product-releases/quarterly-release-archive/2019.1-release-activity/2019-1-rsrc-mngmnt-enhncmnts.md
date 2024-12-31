---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: Verbesserungen beim Ressourcenmanagement in 2019.1
description: Auf dieser Seite werden alle in der Version 2019.1 enthaltenen Verbesserungen beim Ressourcen-Management beschrieben. Die Funktion ist jetzt in der Produktionsumgebung verfügbar.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6eed6023-96cc-45d7-8dae-a36d45e92068
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 0%

---

# Verbesserungen beim Ressourcenmanagement in 2019.1

Auf dieser Seite werden alle in der Version 2019.1 enthaltenen Verbesserungen beim Ressourcen-Management beschrieben. Die Funktion ist jetzt in der Produktionsumgebung verfügbar.

Eine Liste aller in 2019.1 vorgenommenen Änderungen finden Sie unter [Übersicht über die Versionsaktivität von 2019.1](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md).

## Der Standardfilter im Ressourcenplaner wurde aktualisiert

Der Standardfilter im Ressourcenplaner wird nicht mehr nach der Gruppe des Projekts gefiltert.

Beim Anzeigen des Ressourcenplaners werden jetzt nur noch die Projekte angezeigt, die standardmäßig aktuell und datumsabhängig sind. Informationen aus den folgenden Projekten sind standardmäßig enthalten:

* Mit einem geplanten Abschlussdatum, das nach dem ersten Datum des heutigen Monats liegt.
* Mit einem geplanten Startdatum, das vor dem letzten Datum des vierten Monats ab heute liegt.
* Mit dem Status „Aktuell“ oder „Planung“.

Zuvor ruft der Standardfilter die Informationen aus den folgenden zusätzlichen Projekten ab:

* Mit einem geplanten Abschlussdatum, das nach dem ersten Datum des heutigen Monats liegt.
* Mit einem geplanten Startdatum, das vor dem letzten Datum des vierten Monats ab heute liegt.
* Mit dem Status „Aktuell“ oder „Planung“.
* Mit einer Gruppe, die der Hauptgruppe des angemeldeten Benutzers entspricht.

Informationen zum Anwenden von Filtern auf den Ressourcenplaner finden Sie unter [Filterinformationen im Ressourcenplaner](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

## Verwenden von Platzhaltern für Ressourcenplaner-Filter

Sie können jetzt Platzhalter beim Erstellen von Filtern im Ressourcenplaner verwenden. Sie können beispielsweise $$USER.ID zum Filtern von Informationen über den angemeldeten Benutzer oder $$USER.companyID zum Filtern von Informationen über alle Benutzer verwenden, die derselben Firma angehören wie der angemeldete Benutzer. Eine vollständige Liste der benutzerbasierten Variablen finden Sie im Abschnitt [Benutzerbasierte Platzhalterfiltervariablen](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md#user-based-variables) in [Platzhalterfiltervariablen](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

Zuvor waren für die Ressourcenplaner-Filter keine Platzhalter verfügbar.

Informationen zum Filtern im Ressourcenplaner finden Sie unter [Filtern von Informationen im Ressourcenplaner](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

<!--
<iframe class="mt-media" src="assets/290697527?title=0&byline=0&portrait=0" width="640px" height="360px" frameborder="0" allowfullscreen></iframe>
-->

## Unterstützung für datumsbasierte Platzhalterfiltervariablen im Ressourcenplaner

Sie können jetzt jede Version der $$TODAY-Platzhalter-Filtervariablen verwenden, wenn Sie einen Filter im Ressourcenplaner erstellen.

Vor dieser Verbesserung konnten Sie nur benutzerbasierte Platzhalterfiltervariablen verwenden.

Informationen zum Filtern im Ressourcenplaner finden Sie unter [Filtern von Informationen im Ressourcenplaner](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

Informationen zu Platzhalterfiltervariablen finden Sie unter [Platzhalterfiltervariablen](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Exportoptionen für die Rollenansicht im Ressourcenplaner

Sie können jetzt in der Rollenansicht aus dem Ressourcenplaner auswählen, welche Informationsebenen exportiert werden sollen. Sie können eine der folgenden Aktionen exportieren:

* Nur Rollen
* Aufgabengebiete und Projekte
* Rollen, Projekte und Benutzer

Vor dieser Verbesserung wurden alle Informationsebenen in die Rollenansicht exportiert. Diese Optionen wurden in einer früheren Version mit den Projekt- und Benutzeransichten eingeführt.

Informationen zum Exportieren von Informationen aus dem Ressourcenplaner finden Sie unter [Exportieren von Informationen aus dem Ressourcenplaner](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Datenformatierungsoptionen für den Export des Ressourcenplaners

Sie können jetzt auswählen, wie Informationen in der Excel-Datei angezeigt werden sollen, wenn sie aus dem Ressourcenplaner exportiert wurde.

Sie können die Verfügbarkeit und Zuordnung der aus dem Ressourcenplaner exportierten Informationen wie folgt anzeigen:

* Gruppierung nach Namen der Objekte aufgehoben, zu denen sie gehört. In diesem Fall werden die Namen der Objekte, zu denen es gehört, in jeder Datenzeile angezeigt. (dies ist die Standardoption)
* Gruppiert nach dem Namen der Objekte, zu denen sie gehört. In diesem Fall werden die Informationen in der exportierten Datei so angezeigt, wie sie in Workfront angezeigt werden.

Vor dieser Verbesserung wurden die Informationen in der exportierten Datei so angezeigt, wie sie in Workfront angezeigt wurden.

Informationen zum Exportieren von Informationen aus dem Ressourcenplaner finden Sie unter [Exportieren von Informationen aus dem Ressourcenplaner](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Zeitleiste für persistente Planung

>[!NOTE]
>
>Die Tools zur Ressourcenplanung werden nicht mehr unterstützt und mit Version 23.1 aus Workfront entfernt. Informationen zur Planung von Ressourcen mit dem Workload Balancer finden Sie unter [Übersicht über den Workload Balancer](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Zeitpläne behalten jetzt den Zeitrahmen bei, den Sie ausgewählt haben, wenn Sie die Zeitleiste aktualisieren oder die Seite verlassen.

Vor dieser Verbesserung wurden die Zeitpläne beim Aktualisieren oder Verlassen der Seite auf den Standardzeitrahmen zurückgesetzt.

Diese Verbesserung ist in den folgenden Bereichen verfügbar:

* Registerkarte „Planung“ im Bereich „Personen“
* Team arbeitet an Registerkarte
* Registerkarte „Planung“ auf der Registerkarte „Personal“ eines Projekts

Informationen zum Arbeiten mit der Zeitleiste in den Bereichen für die Ressourcenplanung finden Sie unter „Erste Schritte mit der Ressourcenplanung“.

## Neue Exportoptionen im Ressourcenplaner

Sie können jetzt aus dem Ressourcenplaner auswählen, welche Informationsebenen exportiert werden sollen. In der Projektansicht können Sie eine der folgenden Aktionen exportieren:

* Nur Projekte
* Projekte und Aufgabengebiete
* Projekte, Rollen und Benutzer

In der Benutzeransicht können Sie Folgendes exportieren:

* Nur Benutzer
* Benutzende und Projekte
* Benutzer, Projekte, Rollen, Aufgaben und Probleme

Vor dieser Verbesserung wurden standardmäßig alle Informationsebenen in alle Ansichten des Ressourcenplaners exportiert.

Informationen zum Exportieren von Informationen aus dem Ressourcenplaner finden Sie unter [Exportieren von Informationen aus dem Ressourcenplaner](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Aktualisieren der Benutzeransicht im Ressourcenplaner

Alle Benutzer des Systems werden jetzt in der Benutzeransicht des Ressourcenplaners angezeigt, aber nur die Benutzer, die mit den gefilterten Projekten verknüpft sind, zeigen auch Stundeninformationen an.

Vor diesem Update wurden in der Benutzeransicht des Ressourcenplaners nur die Benutzer angezeigt, die Arbeitselementen der Projekte zugewiesen waren, nach denen Sie filtern.

Sie können benutzerbasierte Filter verwenden, um die Anzahl der in der Benutzeransicht angezeigten Benutzer auf diejenigen zu reduzieren, die den Projekten zugewiesen sind, die Sie anzeigen möchten.

Informationen zu Filtern im Ressourcenplaner finden Sie unter [Filtern von Informationen im Ressourcenplaner](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).
