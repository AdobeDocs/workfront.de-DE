---
content-type: release-notes
navigation-topic: product-releases-archive
title: Versionsaktivität von Beta 3 2018.1
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 3 Version 2018.1 verfügbar waren. Die Funktion wurde am 7. Januar 2018 in der Vorschau-Umgebung bereitgestellt. Es wird Anfang 2018 in der Produktionsumgebung verfügbar gemacht.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 26bbc4a0-e5ed-4b5f-bfc2-f888362c1d22
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '1850'
ht-degree: 0%

---

# Versionsaktivität von Beta 3 2018.1

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 3 Version 2018.1 verfügbar waren. Die Funktion wurde am 7. Januar 2018 in der Vorschau-Umgebung bereitgestellt. Es wird Anfang 2018 in der Produktionsumgebung verfügbar gemacht.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktion kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen in Version 2018.1 finden Sie unter  Übersicht über die Versionsaktivität [2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

Die Beta-Version 3 2018.1 enthält Verbesserungen für Workfront-Administratoren und andere Benutzende:

**Für Administratoren**

* [Verbesserungen für Gruppenadministratoren](#group-administrator-improvements)

**Für alle Benutzer**

* [Verbesserungen am HTML5 Proofing Viewer](#html5-proofing-viewer-improvements)
* [Proofing-Verbesserungen in Workfront](#proofing-improvements-within-workfront)
* [Verbesserungen im Home-Bereich](#home-area-improvements) 
* [Agile-Verbesserungen](#agile-improvements)
* [Verbesserungen am Gantt-Diagramm](#gantt-chart-improvements)
* [Verbesserungen am Ressourcenplaner](#resource-planner-improvements)

## Verbesserungen für Gruppenadministratoren {#group-administrator-improvements}

* [Die Benutzeroberfläche zum Zurücksetzen des Kennworts wurde für Gruppenadministratoren aktualisiert](#reset-password-ui-updated-for-group-administrators)
* [Optionen für die Einrichtung der Zugriffsebene für Gruppenadministratoren](#access-level-setup-options-for-group-administrators)
* [Arbeitszeittabellen-Profile für Gruppen erstellen](#create-timesheet-profiles-for-groups)
* [Gelöschte Elemente für Benutzer als Gruppenadministrator wiederherstellen](#recover-deleted-items-for-users-as-a-group-administrator)

### Benutzeroberfläche zum Zurücksetzen des Kennworts für Gruppenadministratoren aktualisiert {#reset-password-ui-updated-for-group-administrators}

Wenn Sie als Gruppenadministrator das Kennwort eines anderen Benutzers zurücksetzen, werden Sie nach dem eigenen Kennwort gefragt, bevor Sie dessen Kennwort ändern können. Die Benutzeroberfläche wurde mit dieser Funktion aktualisiert. Vor dieser Änderung wurde in der Benutzeroberfläche angezeigt, dass das Workfront-Administratorkennwort erforderlich war.

Weitere Informationen zum Zurücksetzen von Passwörtern für andere Benutzer finden Sie [Bearbeiten des Benutzerprofils](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Weitere Informationen zu den Funktionen eines Gruppenadministrators finden Sie im Abschnitt „Funktionen von Gruppenadministratoren“ in [Gruppe erstellen](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Optionen zur Einrichtung der Zugriffsebene für Gruppenadministratoren {#access-level-setup-options-for-group-administrators}

Als Workfront-Administrator können Sie jetzt steuern, ob sich Gruppenadministratoren als andere Benutzer anmelden können oder ob sie die Passwörter anderer Benutzer zurücksetzen können. Wir haben eine neue Einstellung in der Zugriffsebene hinzugefügt, um diesen Zugriff zu aktivieren oder zu deaktivieren. Vor dieser Änderung konnten sich alle Gruppenadministratoren als andere Benutzer anmelden und die Passwörter anderer Benutzer standardmäßig zurücksetzen. Diese Änderung betrifft nur die Zugriffsebene des Planers.

Weitere Informationen zum Konfigurieren der Zugriffsebene für Benutzer finden Sie unter [Gewähren des Zugriffs für Benutzer](../../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Weitere Informationen zu den Funktionen eines Gruppenadministrators finden Sie im Abschnitt „Funktionen von Gruppenadministratoren“ in [Gruppe erstellen](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Arbeitszeittabellen-Profile für Gruppen erstellen {#create-timesheet-profiles-for-groups}

Als Gruppenadministrator können Sie jetzt Arbeitszeittabellen-Profile für die von Ihnen verwalteten Gruppen erstellen und diese Gruppen mit von Ihnen verwalteten Gruppen oder Benutzern aus diesen Gruppen verknüpfen. Arbeitszeittabellen-Profile stellen sicher, dass Arbeitszeittabellen automatisch für die ihnen zugeordneten Benutzer erstellt werden.

Vor dieser Änderung konnte nur ein Workfront-Administrator Arbeitszeittabellen-Profile erstellen.

Weitere Informationen zum Erstellen von Arbeitszeittabellen-Profilen finden Sie unter [Erstellen, Bearbeiten und Zuweisen von Arbeitszeittabellen-Profilen](../../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Weitere Informationen zu den Funktionen eines Gruppenadministrators finden Sie im Abschnitt „Funktionen von Gruppenadministratoren“ in [Gruppe erstellen](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Gelöschte Elemente für Benutzer als Gruppenadministrator wiederherstellen {#recover-deleted-items-for-users-as-a-group-administrator}

Wenn ein Projekt mit einer Gruppe verknüpft ist, für die Sie als Gruppenadministrator fungieren, können Sie das Projekt oder eine seiner gelöschten Aufgaben, Probleme oder Dokumente aus dem Papierkorb wiederherstellen. Vor dieser Änderung konnte nur ein Workfront-Administrator Elemente aus dem Papierkorb wiederherstellen.

Weitere Informationen zum Wiederherstellen gelöschter Elemente in Workfront finden Sie unter [Wiederherstellen gelöschter Elemente](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

Weitere Informationen zu den Funktionen eines Gruppenadministrators finden Sie im Abschnitt „Funktionen von Gruppenadministratoren“ in [Gruppe erstellen](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 

## HTML5 Proofing Viewer-Verbesserungen  {#html5-proofing-viewer-improvements}

* [Vergleichsmodus](#compare-mode)
* [Filtern Sie die Kommentarliste](#filter-the-comment-list)
* [Die Kommentarliste wird nach dem ersten Zeichen durchsucht](#comment-list-is-searched-after-the-first-character-is-entered)

### Vergleichsmodus {#compare-mode}

Sie können jetzt den Vergleichsmodus im HTML5-Proofing-Viewer verwenden, wenn Sie statische und Video-Korrekturabzüge anzeigen. 

Der Vergleichsmodus im HTML5 Proofing Viewer unterscheidet sich vom alten Proofing Viewer folgendermaßen:

* Beim Starten des Vergleichsmodus wird die neuere Version auf die rechte Seite verschoben, wobei die Version, die Sie vergleichen, auf der linken Seite geöffnet wird.

  Zuvor wurde die neuere Version auf die linke Seite verschoben, wobei die Version, die Sie vergleichen, auf der rechten Seite geöffnet wurde.

* Sie können direkt in der Proofing-Anzeige auswählen, welche Version eines Korrekturabzugs Sie vergleichen möchten. 
* Der aktuelle Zoom-Faktor und die aktuelle Position von Korrekturabzügen im Proofing Viewer werden bei der gleichzeitigen Eingabe der Navigation beibehalten.
* Neue Option „Zurücksetzen“ bei gleichzeitiger Navigation.
* Wenn Sie den Vergleichsmodus beenden, können Sie auswählen, welcher Korrekturabzug geschlossen werden soll. 

  Zuvor war die ältere Version immer geschlossen.

* Verschiedene Verbesserungen des Erscheinungsbilds und der Benutzerfreundlichkeit.

Weitere Informationen finden Sie unter [Testsendungen im Proofing Viewer vergleichen](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/compare-proofs.md).

### Filtern der Kommentarliste {#filter-the-comment-list}

Sie können jetzt Kommentare in der Kommentarliste filtern. Sie können nach Benutzer, Aktionen, ungelesenen Inhalten und mehr filtern.

### Die Kommentarliste wird nach dem ersten Zeichen durchsucht {#comment-list-is-searched-after-the-first-character-is-entered}

Beim Durchsuchen der Kommentarliste wird die Liste nun nach Eingabe des ersten Zeichens automatisch gefiltert.

Vor dieser Änderung mussten Sie mindestens 3 Zeichen in das Suchfeld eingeben, bevor die Kommentarliste gefiltert wurde.

Weitere Informationen finden Sie unter in .

## Proofing-Verbesserungen in Workfront {#proofing-improvements-within-workfront}

* [Verknüpfen von Testsendungen von Workfront Proof mit Workfront](#link-proofs-from-workfront-proof-to-workfront)
* [Korrekturabzug kann nicht mehr aus einem Dokument entfernt werden](#can-no-longer-remove-a-proof-from-a-document)
* [Das Erscheinungsbild beim Erstellen und Öffnen von Korrekturabzügen wurde aktualisiert](#updated-look-and-feel-when-generating-and-opening-proofs)

### Korrekturabzüge von Workfront Proof mit Workfront verknüpfen {#link-proofs-from-workfront-proof-to-workfront}

Sie können jetzt Korrekturabzüge, die bereits in Ihrem Workfront Proof-Konto vorhanden sind, mit Workfront verknüpfen.

Vor dieser Änderung konnten Sie nicht auf Korrekturabzüge zugreifen, die bereits in Workfront Proof in Workfront vorhanden waren. 

Weitere Informationen finden Sie unter [Verknüpfen von Dokumenten aus externen Anwendungen](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md) in [Verknüpfen von Dokumenten aus externen Anwendungen](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Korrekturabzug kann nicht mehr aus einem Dokument entfernt werden {#can-no-longer-remove-a-proof-from-a-document}

Sie können einen Korrekturabzug nicht mehr aus einem Dokument entfernen. Stattdessen müssen Sie zum Entfernen eines Korrekturabzugs das gesamte Dokument löschen.

Durch diese Verbesserung verringert sich das Risiko, dass Benutzende versehentlich alle Versionen eines Korrekturabzugs löschen. 

Informationen zum Löschen eines Dokuments finden Sie unter [Löschen eines Korrekturabzugs](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md) in [Löschen eines Korrekturabzugs](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md).

### Das Erscheinungsbild beim Erstellen und Öffnen von Korrekturabzügen wurde aktualisiert {#updated-look-and-feel-when-generating-and-opening-proofs}

Es gibt jetzt einen aktualisierten Animationsdrehzahler, wenn ein Korrekturabzug erstellt wird.

## Verbesserungen beim Home-Bereich {#home-area-improvements}

Im Bereich Startseite wurden folgende Verbesserungen vorgenommen:

* [Korrekturabzugsgenehmigungen aus dem Bereich „Startseite“ anzeigen](#view-proof-approvals-from-the-home-area)
* [Standardfelder werden beim Konfigurieren der Layout-Vorlage für Elemente im Bereich Startseite angezeigt](#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area)

### Genehmigungen von Korrekturabzügen im Bereich Startseite anzeigen {#view-proof-approvals-from-the-home-area}

Zusätzlich zu den Standardgenehmigungen können Sie jetzt Korrekturabzugsgenehmigungen im Bereich Startseite anzeigen.

Zuvor konnten Sie Workfront-Genehmigungen anzeigen, aber keine Genehmigungen für einen Korrekturabzug.  

Weitere Informationen finden Sie unter [Verwenden des Bereichs „Startseite](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

### Standardfelder werden beim Konfigurieren der Layout-Vorlage für Elemente im Bereich Startseite angezeigt {#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area}

Zuvor waren die Standardfelder in der Layout-Vorlage nicht sichtbar.

Weitere Informationen finden Sie unter „Erstellen und Verwalten von Layout-Vorlagen“.

## Agile-Verbesserungen {#agile-improvements}

* [Aufgaben und Probleme direkt von der Seite mit den Aufgaben- oder Problemdetails zur Iteration hinzufügen](#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page)
* [Probleme im Scrum-Rückstand und im Story Board für ein Agile-Team einbeziehen](#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team)
* [Wenden Sie Gruppierungen und Filter auf den Rückstand für ein agiles Team an](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [Leere Iteration erstellen und später aktualisieren](#create-a-blank-iteration-and-update-it-later)
* [Die Felder „Fokus“ und „Kapazität“ werden beim Erstellen einer Iteration vorab ausgefüllt](#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration)

### Fügen Sie der Iteration direkt auf der Seite Aufgaben- oder Problemdetails Aufgaben und Probleme hinzu {#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page}

Sie können jetzt Aufgaben und Probleme, die derzeit einem agilen Team zugewiesen sind, direkt aus der Aufgabe oder dem Problem zu einer Iteration hinzufügen.

Zuvor konnten Sie Aufgaben nur aus dem Rückstand zu einer Iteration hinzufügen. 

Weitere Informationen finden Sie unter [Erstellen einer Iteration](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md) in [Erstellen einer Iteration](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

### Probleme im Scrum-Rückstand und im Story Board für ein Agile-Team einschließen {#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team}

Probleme werden jetzt standardmäßig in den Rückstand Ihres Agile-Teams aufgenommen, wenn Sie die agile Scrum-Methode verwenden (Probleme werden nicht im Rückstand eines Agile-Teams angezeigt, wenn Sie die Kanban-Methode verwenden).

Vor dieser Änderung konnten nur Aufgaben zum Rückstand hinzugefügt werden. Wenn Sie ein Problem hinzufügen möchten, müssen Sie das Problem zunächst in eine Aufgabe konvertieren, bevor es hinzugefügt werden kann.

Informationen zur Verwendung von Problemen im Auftragsbestand finden Sie unter  [Verwalten des Agile-Rückstands](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

### Anwenden von Gruppierungen und Filtern auf den Rückstand eines agilen Teams {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

Die Gruppierungs- und Filteroptionen sind jetzt im agilen Rückstand verfügbar, sodass Sie Ihren Rückstand nach Gruppierungen organisieren und nach bestimmten Aufgaben und Problemen filtern können.

Vor dieser Änderung konnten Sie Ansichten auf den Agile-Rückstand anwenden.

Weitere Informationen finden Sie unter  [Verwalten des Agile-](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) in  [Verwalten des Agile-Rückstands](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

### Leere Iteration erstellen und später aktualisieren {#create-a-blank-iteration-and-update-it-later}

Sie müssen eine Aufgabe oder ein Problem nicht mehr zu einer Iteration hinzufügen, um sie bzw. es zu erstellen. Sie können eine leere Iteration erstellen und Aufgaben und Probleme zu einem späteren Zeitpunkt hinzufügen.

Weitere Informationen finden Sie unter [Erstellen einer Iteration](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

### Die Felder „Fokus“ und „Kapazität“ werden beim Erstellen einer Iteration vorab ausgefüllt {#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration}

Bei der Erstellung einer Iteration werden die Felder „Fokus“ und „Kapazität“ mit den Durchschnittswerten aller vergangenen Iterationen vorab ausgefüllt, die Ihr Team erstellt hat. Wenn Ihr Team in der Vergangenheit keine Iterationen erstellt hat, werden diese Felder als 0 angezeigt.

Zuvor waren diese Felder immer auf 0 gesetzt.

Weitere Informationen finden Sie unter [Erstellen einer Iteration](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

## Verbesserungen am Gantt-Diagramm {#gantt-chart-improvements}

* [Bearbeitungsmodus im Gantt-Diagramm aktivieren](#enable-edit-mode-in-the-gantt-chart)
* [Vorgänger beim Bearbeiten des Gantt-Diagramms entfernen](#remove-predecessors-when-editing-the-gantt-chart)

### Aktivieren des Bearbeitungsmodus im Gantt-Diagramm {#enable-edit-mode-in-the-gantt-chart}

Wenn Sie den Bearbeitungsmodus im Gantt-Diagramm aktivieren, können Sie Änderungen an den Informationen innerhalb des Diagramms vornehmen. Vor dieser Änderung konnten Sie die Informationen im Gantt-Diagramm nicht bearbeiten. Sie konnten nur Aufgabeninformationen in der Aufgabenliste bearbeiten.

Weitere Informationen zum Bearbeiten des Gantt-Diagramms finden Sie unter [Aktualisierungsinformationen in der Aufgabenliste Gantt-Diagramm](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

### Vorgänger beim Bearbeiten des Gantt-Diagramms entfernen {#remove-predecessors-when-editing-the-gantt-chart}

Mithilfe des Bearbeitungsmodus für das Gantt-Diagramm können Sie jetzt Vorgängerbeziehungen zwischen Aufgaben im Gantt-Diagramm eines Projekts entfernen. Vor dieser Verbesserung konnten Sie die Vorgängerbeziehung nur in der Aufgabenliste oder auf Aufgabenebene entfernen.

Weitere Informationen zum Bearbeiten des Gantt-Diagramms finden Sie unter [Aktualisierungsinformationen in der Aufgabenliste Gantt-Diagramm](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Verbesserungen am Ressourcenplaner {#resource-planner-improvements}

* [Budget mit Null-Dauer im Ressourcenplaner](#budget-with-zero-duration-in-the-resource-planner)

* [Daten nach Kosten im Ressourcenplaner anzeigen](#show-data-by-cost-in-the-resource-planner)

### Budget mit Null-Dauer im Ressourcenplaner {#budget-with-zero-duration-in-the-resource-planner}

>[!NOTE]
>
>Diese Funktion wurde aus der Vorschau-Umgebung entfernt und wird mit Version 18.1 veröffentlicht.

Sie können Ihre Ressourcen jetzt im Ressourcenplaner für ein beliebiges Datum innerhalb oder außerhalb des Zeitrahmens des Projekts budgetieren. Vor dieser Verbesserung konnten Sie Ihre Ressourcen nur für die Termine innerhalb des Zeitrahmens des Projekts budgetieren.

Weitere Informationen zur Budgetierung von Ressourcen im Ressourcenplaner finden Sie im Abschnitt „Budgetierung von Ressourcen im Ressourcenplaner“ in [Ressourcenplaner - Übersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Daten nach Kosten im Ressourcenplaner anzeigen {#show-data-by-cost-in-the-resource-planner}

Sie können jetzt die Informationen im Ressourcenplaner neben Stunden und FTE-Werten auch nach Kosten anzeigen. Sie können die Kosten im Ressourcenplaner anzeigen, wenn Sie sie in der Ansicht Nach Projekt anzeigen oder Nach Funktion anzeigen anzeigen. Kosten können nicht angezeigt werden, wenn Sie den Ressourcenplaner in der Ansicht Nach Benutzer anzeigen.

Weitere Informationen zum Anzeigen des Ressourcenplaners nach Stunden, FTE oder Kosten finden Sie unter [Übersicht über die Ressourcenplaner-Navigation](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).
