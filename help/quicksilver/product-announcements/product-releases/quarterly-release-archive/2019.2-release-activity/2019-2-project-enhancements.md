---
content-type: release-notes
navigation-topic: 2019-2-release-activity
title: Projektverbesserungen in 2019.2
description: Auf dieser Seite werden alle in der Version 2019.2 enthaltenen Projektverbesserungen beschrieben. Die Funktion soll in der Produktionsumgebung ab der Woche vom 20. Mai 2019 verfügbar sein.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 76292f90-af1a-4740-9b8e-b02a6303625c
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 1%

---

# Projektverbesserungen in 2019.2

Auf dieser Seite werden alle in der Version 2019.2 enthaltenen Projektverbesserungen beschrieben. Die Funktion soll in der Produktionsumgebung ab der Woche vom 20. Mai 2019 verfügbar sein.

Eine Liste aller in Version 2019.2 vorgenommenen Änderungen finden Sie unter [Übersicht über die Versionsaktivität 2019.2](../../../../product-announcements/product-releases/quarterly-release-archive/2019.2-release-activity/2019-2-release-activity-overview.md).

## Schnellere Suche nach Gruppen beim Anpassen von Status

Das Dropdown-Menü auf der Registerkarte Status im Bereich Setup ist jetzt ein Menü mit automatischer Textvervollständigung . Auf diese Weise können Sie schnell jede beliebige Gruppe im System suchen und finden, was die Anpassung von Status erleichtert.

Zuvor wurde im Dropdown-Menü eine begrenzte Anzahl von Gruppen angezeigt. Wenn die gewünschte Gruppe nicht angezeigt wurde, mussten Sie zu Einstellungen > Gruppen navigieren und die jeweilige Gruppe finden, um den Status der Gruppe anzupassen.

Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Standardmäßige benutzerdefinierte Forms und Genehmigungsprozesse an Aufgaben anhängen

Sie können jetzt standardmäßige benutzerdefinierte Formulare und Genehmigungsprozesse konfigurieren, die an Aufgaben angehängt werden, wenn Sie Aufgaben zu einem Projekt hinzufügen. Sie können die Standardeinstellungen auf Projektebene konfigurieren.

Informationen zum Konfigurieren von standardmäßigen benutzerdefinierten Formularen und Genehmigungsprozessen für Aufgaben auf Projektebene finden Sie im Abschnitt „Aufgaben“ im Artikel [Projekte bearbeiten](../../../../manage-work/projects/manage-projects/edit-projects.md) .

## Gesamte Zeile einer übergeordneten Aufgabe fett in einer Aufgabenliste anzeigen

In einer Aufgabenliste wird die Zeile, die eine übergeordnete Aufgabe enthält, fett angezeigt. Diese Änderung ist sichtbar, wenn die Liste nach der Arbeitsaufschlüsselungsstruktur oder nach der Aufgabennummer in aufsteigender Reihenfolge sortiert wird.

## Änderungen in den Aufgabenlisten rückgängig machen

Über eine neue Schaltfläche Automatisches Speichern in der Aufgabenliste können Sie auswählen, ob die von Ihnen vorgenommenen Änderungen automatisch gespeichert werden sollen oder ob Sie die Auswirkungen sehen möchten, die Ihre Änderungen vor dem Speichern haben. Diese Einstellung gilt sowohl für die Aufgabenliste als auch für das Gantt-Diagramm.

Vor dieser Verbesserung wurden alle Änderungen immer automatisch gespeichert.

Informationen zum Bearbeiten von Aufgaben in einer Aufgabenliste finden Sie unter [Aufgaben bearbeiten](../../../../manage-work/tasks/manage-tasks/edit-tasks.md).

Informationen zum Bearbeiten von Aufgaben im Gantt-Diagramm finden Sie unter [Informationen in der Aufgabenliste aktualisieren Gantt-Diagramm](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Standardwerte für die Breite neuer Spalten in neuen Listen

Jetzt passt Workfront die Spaltenbreite automatisch an die Werteformatinformationen in den einzelnen Spalten an. Beispielsweise sind Spalten, die eine Zahl anzeigen, breiter als die Spalten, die das Feld Beschreibung anzeigen.

Vor dieser Verbesserung wurden die Spaltenbreiten in den neuen Projekt- und Aufgabenansichten auf 100 Pixel festgelegt, sofern nicht anders angegeben.

Informationen zu Spaltenbreiten finden Sie unter [Spaltenbreite und -reihenfolge ändern](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

## Nicht verwendete Objekte deaktivieren

>[!NOTE]
>
>Diese Funktion wurde im Vorschauzeitrahmen 2019.2 direkt in der Produktionsumgebung veröffentlicht.

Wenn Sie Objekte haben, die nicht mehr verwendet werden, können Sie diese jetzt deaktivieren, um sie aus Listen auszublenden, damit Benutzer sie nicht mit anderen Objekten verknüpfen.

Wenn Sie nun eines der Objekte unten bearbeiten, können Sie angeben, ob sie aktiv sein sollen. Objekte, die als Aktiv festgelegt sind, werden in Dropdown-Menüs und Feldern mit automatischer Textvervollständigung angezeigt und können an andere Objekte angehängt werden. Objekte, für die nicht „Aktiv“ festgelegt ist, werden nicht in Dropdown-Menüs und Feldern mit automatischer Textvervollständigung angezeigt, um sie an andere Objekte anzuhängen.

* Genehmigungsprozesse
* Firmen
* Benutzerdefinierte Formulare
* Meilensteinpfade
* Portfolios
* Programme
* Vorlagen

Alles, was Sie deaktivieren, das derzeit verwendet wird, funktioniert weiterhin wie immer und wird nicht entfernt oder blockiert.

>[!IMPORTANT]
>
>Beim Erstellen dieser Objekte über die Workfront-API ist der Standardwert für den Parameter „isActive“ „true“. Dies ist ein neues Feld für alle Objekte, das Sie nicht vor Version 11 der API bearbeiten können. Dieses Feld gab es bereits für das Portfolio , mit der Ausnahme, dass der Standardwert „false“ war. Ab Version 11 der API wird er in den Standardwert „true“ geändert.

## Budgetierte Kosten geplanter Arbeit (BCWS) und Ausgeführter Arbeit (BCWP) in Ansichten anzeigen

Sie können jetzt die budgetierten Kosten der geplanten Arbeit (BCWS) und die budgetierten Kosten der geleisteten Arbeit (BCWP) in Projekt- und Aufgabenansichten anzeigen.

Obwohl diese Projektleistungsmetriken zuvor in Finanzberechnungen in Workfront verwendet wurden, waren sie vor dieser Verbesserung nicht im System sichtbar.

Weitere Informationen zur Berechnung des SKBA finden [&#x200B; unter „Budgetierte Kosten für geplante Arbeit (SKBA) berechnen](../../../../manage-work/projects/project-finances/calculate-bcws.md).

Informationen zur Berechnung des SKAA finden Sie unter [Budgetierte Kosten der geleisteten Arbeit berechnen (SKAA)](../../../../manage-work/projects/project-finances/calculate-bcwp.md).

