---
content-type: release-notes
navigation-topic: 2019-2-release-activity
title: 2019.2 Projektverbesserungen
description: Auf dieser Seite werden alle in Version 2019.2 enthaltenen Projektverbesserungen beschrieben. Die Funktion soll in der Produktionsumgebung ab der Woche des 20. Mai 2019 verfügbar sein.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 76292f90-af1a-4740-9b8e-b02a6303625c
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 1%

---

# 2019.2 Projektverbesserungen

Auf dieser Seite werden alle in Version 2019.2 enthaltenen Projektverbesserungen beschrieben. Die Funktion soll in der Produktionsumgebung ab der Woche des 20. Mai 2019 verfügbar sein.

Eine Liste aller 2019.2 vorgenommenen Änderungen finden Sie unter [Übersicht über die Release-Aktivitäten 2019.2](../../../../product-announcements/product-releases/quarterly-release-archive/2019.2-release-activity/2019-2-release-activity-overview.md).

## Schnellere Suche nach Gruppen beim Anpassen von Status

Das Dropdown-Menü auf der Registerkarte Status im Bereich Einrichtung ist jetzt ein typeahead-Menü. Auf diese Weise können Sie schnell nach einer beliebigen Gruppe im System suchen und diese suchen, was die Anpassung der Status erleichtert.

Zuvor wurde im Dropdown-Menü eine begrenzte Anzahl von Gruppen angezeigt. Wenn die gewünschte Gruppe nicht angezeigt wurde, mussten Sie zu Einrichtung > Gruppen navigieren und die spezifische Gruppe suchen, um den Status der Gruppe anzupassen.

Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Standardmäßige benutzerdefinierte Forms- und Genehmigungsprozesse an Aufgaben anhängen

Sie können jetzt benutzerdefinierte Standardformulare und Genehmigungsprozesse konfigurieren, die an Aufgaben angehängt werden, wenn Sie Aufgaben zu einem Projekt hinzufügen. Sie können die Standardeinstellungen auf Projektebene konfigurieren.

Informationen zum Konfigurieren von benutzerdefinierten Standardformularen und Genehmigungsprozessen für Aufgaben auf Projektebene finden Sie im Abschnitt &quot;Aufgaben&quot;im [Projekte bearbeiten](../../../../manage-work/projects/manage-projects/edit-projects.md) Artikel.

## Gesamte Zeile einer übergeordneten Aufgabe in Fettdruck in einer Aufgabenliste anzeigen

In einer Aufgabenliste wird die Zeile, die eine übergeordnete Aufgabe enthält, fett dargestellt. Diese Änderung ist sichtbar, wenn die Liste nach der Struktur der Aufschlüsselung &quot;Arbeit&quot;oder nach der Aufgabennummer in aufsteigender Reihenfolge sortiert wird.

## Umkehren von Änderungen in den Aufgabenlisten

Mit der neuen Schaltfläche Automatisches Speichern in der Aufgabenliste können Sie auswählen, ob die von Ihnen vorgenommenen Änderungen automatisch gespeichert werden sollen oder ob Sie die Auswirkungen sehen möchten, die Ihre Änderungen vor dem Speichern haben. Diese Einstellung gilt sowohl für die Aufgabenliste als auch für das Gantt-Diagramm.

Vor dieser Verbesserung wurden alle Änderungen immer automatisch gespeichert.

Informationen zum Bearbeiten von Aufgaben in einer Aufgabenliste finden Sie unter [Aufgaben bearbeiten](../../../../manage-work/tasks/manage-tasks/edit-tasks.md).

Informationen zum Bearbeiten von Aufgaben in der Gantt-Grafik finden Sie unter [Aktualisieren von Informationen in der Aufgabenliste Gantt-Diagramm](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Neue Standardwerte für die Spaltenbreite in neuen Listen

Jetzt passt Workfront die Breite der Spalten automatisch an die in den einzelnen Spalten enthaltenen Informationen zum Werteformat an. Beispielsweise sind Spalten, die eine Zahl anzeigen, größer als die, die das Feld Beschreibung anzeigen.

Vor dieser Verbesserung wurden die Spaltenbreiten in den neuen Projekt- und Aufgabenansichten auf 100 Pixel festgelegt, sofern nicht anders angegeben.

Weitere Informationen zu Spaltenbreiten finden Sie unter [Spaltenbreite und -reihenfolge ändern](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

## Nicht verwendete Objekte deaktivieren

>[!NOTE]
>
>Diese Funktion wurde während des Zeitrahmens der Vorschau 2019.2 direkt in der Produktionsumgebung veröffentlicht.

Wenn Sie nicht mehr verwendete Objekte haben, können Sie diese nun deaktivieren, um sie vor Listen zu verbergen und so zu verhindern, dass Benutzer sie anderen Objekten zuordnen.

Wenn Sie jetzt eines der unten stehenden Objekte bearbeiten, können Sie angeben, ob diese aktiv sein sollen. Objekte, die auf &quot;Aktiv&quot;eingestellt sind, werden in Dropdown-Menüs und Typvorlagenfeldern angezeigt und können an andere Objekte angehängt werden. Objekte, die nicht auf &quot;Aktiv&quot;gesetzt sind, sind nicht in Dropdown-Menüs und Typvorlagenfeldern sichtbar, die an andere Objekte angehängt werden sollen.

* Genehmigungsprozesse
* Firmen
* Benutzerdefinierte Formulare
* Meilensteinpfade
* Portfolios
* Programme
* Vorlagen

Alles, was Sie deaktivieren, funktioniert weiterhin wie bisher und wird weder entfernt noch blockiert.

>[!IMPORTANT]
>
>Beim Erstellen dieser Objekte über die Workfront-API lautet der Standardwert für den Parameter &quot;isActive&quot;&quot;true&quot;. Dies ist ein neues Feld für alle Objekte und steht Ihnen nicht zur Bearbeitung vor Version 11 der API zur Verfügung. Dieses Feld war zuvor für Portfolio vorhanden, außer dass der Standardwert false war. Es wird ab Version 11 der API in den Standardwert true geändert.

## Anzeige der geplanten und durchgeführten Kosten für geplante Arbeit (BCWS) in Ansichten

Sie können jetzt die budgetierten Kosten der geplanten Arbeit (BCWS) und die veranschlagten Kosten der durchgeführten Arbeit (BCWP) in Projekt- und Aufgabenansichten anzeigen.

Obwohl diese Projektleistungsmetriken bereits in Workfront in Finanzberechnungen verwendet wurden, waren sie im System vor dieser Verbesserung nicht sichtbar.

Informationen zur Berechnung der BCWS finden Sie unter [Geplante Arbeitskosten berechnen (BCWS)](../../../../manage-work/projects/project-finances/calculate-bcws.md).

Informationen zur Berechnung von BCWP finden Sie unter [Berechnung der veranschlagten Arbeitskosten (BCWP)](../../../../manage-work/projects/project-finances/calculate-bcwp.md).

