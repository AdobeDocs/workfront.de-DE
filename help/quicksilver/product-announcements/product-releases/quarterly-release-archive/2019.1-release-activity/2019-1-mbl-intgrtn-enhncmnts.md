---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: Verbesserungen bei Mobile und Integration in 2019.1
description: Auf dieser Seite werden alle Verbesserungen der Ressourcenverwaltung beschrieben, die in Version 2019.1 enthalten sind. Die Funktion ist jetzt in der Produktionsumgebung verfügbar.
author: Luke
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 6b86ba0d-977a-4c89-8832-e81bf28d9dad
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 0%

---

# Verbesserungen bei Mobile und Integration in 2019.1

Auf dieser Seite werden alle Verbesserungen der Ressourcenverwaltung beschrieben, die in Version 2019.1 enthalten sind. Die Funktion ist jetzt in der Produktionsumgebung verfügbar.

Eine Liste aller Änderungen, die in Version 2019.1 vorgenommen wurden, finden Sie unter [Übersicht über die Release-Aktivität 2019.1}.](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md)

## Aktualisierter Standardfilter im Ressourcenplaner

Der Standardfilter im Ressourcenplaner filtert nicht mehr von der Gruppe des Projekts.

Beim Anzeigen des Ressourcen-Planers sehen Sie jetzt nur die Projekte, die standardmäßig aktuell und datumsabhängig sind. Informationen aus den folgenden Projekten sind standardmäßig enthalten:

* Mit einem geplanten Abschlussdatum, das nach dem ersten Datum des heutigen Monats eintritt.
* Mit einem geplanten Startdatum, das vor dem letzten Datum des vierten Monats ab heute liegt.
* mit dem Status &quot;Aktuell&quot;oder &quot;Planung&quot;.

Zuvor wurden die Informationen aus den folgenden zusätzlichen Projekten vom Standardfilter abgerufen:

* Mit einem geplanten Abschlussdatum, das nach dem ersten Datum des heutigen Monats eintritt.
* Mit einem geplanten Startdatum, das vor dem letzten Datum des vierten Monats ab heute liegt.
* mit dem Status &quot;Aktuell&quot;oder &quot;Planung&quot;.
* Mit einer Gruppe, die mit der Home-Gruppe des Benutzers übereinstimmt, der angemeldet ist.

Informationen zum Anwenden von Filtern auf den Ressourcenplaner finden Sie unter [Filterinformationen im Ressourcenplaner](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

## Verwenden von Platzhaltern für Filter für Ressourcenplaner

Sie können jetzt beim Erstellen von Filtern im Ressourcenplaner Platzhalter verwenden. Sie können beispielsweise $$USER.ID verwenden, um nach Informationen über den angemeldeten Benutzer zu filtern, oder $$USER.companyID, um Informationen über alle Benutzer zu filtern, die zum selben Unternehmen gehören wie der angemeldete Benutzer. Eine vollständige Liste der benutzerbasierten Variablen finden Sie im Abschnitt [Benutzerbasierte Platzhalterfiltervariablen](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md#user-based-variables) in [Platzhalterfiltervariablen](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

Zuvor waren für die Filter &quot;Ressourcenplaner&quot;keine Platzhalter verfügbar.

Informationen zum Filtern im Ressourcen-Planer finden Sie unter [Filtern von Informationen im Ressourcen-Planer](../../../../resource-mgmt/resource-planning/filter-resource-planner.md)

VIDEO

## Unterstützung für datumsbasierte Wildcard-Filtervariablen im Ressourcenplaner

Sie können jetzt eine beliebige Version der Platzhalterfiltervariablen $$TODAY verwenden, wenn Sie einen Filter im Ressourcenplaner erstellen.

Vor dieser Verbesserung konnten Sie nur benutzerbasierte Platzhalterfiltervariablen verwenden.

Informationen zum Filtern im Ressourcen-Planer finden Sie unter [Filtern von Informationen im Ressourcen-Planer](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

Weitere Informationen zu Platzhalterfiltervariablen finden Sie unter [Platzhalterfiltervariablen](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

VIDEO

## Exportoptionen für die Rollenansicht im Ressourcenplaner

Sie können jetzt in der Rollenansicht auswählen, welche Informationsstufen aus dem Ressourcenplaner exportiert werden sollen.

Sie können Folgendes exportieren:

* Nur Rollen
* Aufgabengebiete und Projekte
* Rollen, Projekte und Benutzer

Vor dieser Verbesserung wurden alle Informationsstufen in die Rollenansicht exportiert. Diese Optionen wurden in einer früheren Version in die Projekt- und Benutzeransichten eingeführt.

Informationen zum Exportieren von Informationen aus dem Ressourcenplaner finden Sie unter [Informationen aus dem Ressourcenplaner exportieren](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

VIDEO

## Datenformatierungsoptionen für den Export des Ressourcenplaners

Sie können jetzt auswählen, wie Informationen in der Excel-Datei angezeigt werden sollen, wenn sie aus dem Ressourcenplaner exportiert werden.

Sie können die Verfügbarkeit und Zuordnung von aus dem Ressourcenplaner exportierten Informationen wie folgt anzeigen:

* Gruppierung nach dem Namen der Objekte, zu denen sie gehört, aufgehoben. In diesem Fall werden die Namen der Objekte, zu denen es gehört, in jeder Datenzeile angezeigt. (Dies ist die Standardoption)
* Gruppiert nach dem Namen der Objekte, zu denen es gehört. In diesem Fall werden die Informationen in der exportierten Datei so angezeigt, wie sie in Workfront angezeigt werden.

Vor dieser Verbesserung wurden die Informationen in der exportierten Datei so angezeigt, wie sie in Workfront angezeigt wurden.

Informationen zum Exportieren von Informationen aus dem Ressourcenplaner finden Sie unter [Informationen aus dem Ressourcenplaner exportieren](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

VIDEO

## Persistente Planung - Timeline

>[!NOTE]
>
>Die Tools für die Ressourcenplanung wurden mit Version 23.1 eingestellt und aus Workfront entfernt. Weitere Informationen zum Planen von Ressourcen mit dem Lastenausgleich finden Sie unter [Übersicht über den Lastenausgleich](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Bei der Planung von Zeitleisten bleibt der ausgewählte Zeitrahmen jetzt erhalten, wenn Sie die Timeline aktualisieren oder von der Seite weg navigieren.

Vor dieser Verbesserung kehrten die Zeitpläne beim Aktualisieren oder Verlassen der Seite in den Standardzeitrahmen zurück.

Diese Verbesserung ist in den folgenden Bereichen verfügbar:

* Registerkarte &quot;Planung&quot;im Bereich &quot;Personen&quot;
* Registerkarte &quot;Teamarbeit&quot;
* Unterregisterkarte &quot;Planung&quot;auf der Registerkarte &quot;Staffelung&quot;eines Projekts

Weitere Informationen zum Arbeiten mit der Timeline in den Bereichen &quot;Ressourcenplanung&quot;finden Sie unter &quot;Erste Schritte mit der Ressourcenplanung&quot;.

VIDEO

## Neue Exportoptionen im Ressourcenplaner

Sie können jetzt im Ressourcenplaner auswählen, welche Informationsstufen exportiert werden sollen.

In der Projektansicht können Sie Folgendes exportieren:

* Nur Projekte
* Projekte und Aufgabengebiete
* Projekte, Rollen und Benutzer

In der Benutzeransicht können Sie Folgendes exportieren:

* Nur Benutzer
* Benutzende und Projekte
* Benutzer, Projekte, Rollen, Aufgaben und Probleme

Vor dieser Verbesserung wurden alle Informationsstufen standardmäßig in alle Ansichten des Ressourcenplaners exportiert.

Informationen zum Exportieren von Informationen aus dem Ressourcenplaner finden Sie unter [Informationen aus dem Ressourcenplaner exportieren](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

VIDEO

## Aktualisierung der Benutzeransicht im Ressourcenplaner

Alle Benutzer des Systems werden jetzt in der Benutzeransicht des Ressourcenplaners angezeigt, aber nur die mit den gefilterten Projekten verknüpften Benutzer zeigen auch Stundeninformationen an.

Vor dieser Aktualisierung wurden nur die Benutzer zugewiesen, die Arbeitselementen der Projekte zugewiesen waren, nach denen Sie filtern, und die in der Benutzeransicht des Ressourcenplaners angezeigt wurden.

Sie können benutzerbasierte Filter verwenden, um die Anzahl der in der Benutzeransicht angezeigten Benutzer auf diejenigen zu reduzieren, die den anzuzeigenden Projekten zugewiesen sind.

Informationen zu Filtern im Ressourcenplaner finden Sie unter [Filterinformationen im Ressourcenplaner](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).
