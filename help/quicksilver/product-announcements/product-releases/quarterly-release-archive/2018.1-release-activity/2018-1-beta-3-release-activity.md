---
content-type: release-notes
navigation-topic: product-releases-archive
title: Beta 3-Release-Aktivität 2018.1
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 3 Version 2018.1 verfügbar waren. Die Funktion wurde am 7. Januar 2018 in der Vorschau-Umgebung bereitgestellt. Sie wird Anfang 2018 im Produktionsumfeld zur Verfügung gestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 26bbc4a0-e5ed-4b5f-bfc2-f888362c1d22
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1850'
ht-degree: 0%

---

# Beta 3-Release-Aktivität 2018.1

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 3 Version 2018.1 verfügbar waren. Die Funktion wurde am 7. Januar 2018 in der Vorschau-Umgebung bereitgestellt. Sie wird Anfang 2018 im Produktionsumfeld zur Verfügung gestellt.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktionalität kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen, die 2018.1 vorgenommen wurden, finden Sie unter  [Übersicht über die Veröffentlichungsaktivität 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

Die Beta-Version 2018.1 von 3 enthält Verbesserungen für Workfront-Administratoren und andere Benutzer:

**Für Administratoren**

* [Verbesserungen für Gruppenadministratoren](#group-administrator-improvements)

**Für alle Benutzer**

* [Verbesserungen beim HTML5-Testversand-Viewer](#html5-proofing-viewer-improvements)
* [Verbesserungen beim Testen in Workfront](#proofing-improvements-within-workfront)
* [Verbesserungen am Startbereich](#home-area-improvements) 
* [Agile Verbesserungen](#agile-improvements)
* [Verbesserungen des Gantt-Diagramms](#gantt-chart-improvements)
* [Verbesserungen beim Ressourcenplaner](#resource-planner-improvements)

## Verbesserungen für Gruppenadministratoren {#group-administrator-improvements}

* [Benutzeroberfläche zum Zurücksetzen des Kennworts für Gruppenadministratoren aktualisiert](#reset-password-ui-updated-for-group-administrators)
* [Optionen für die Einrichtung auf Zugriffsebene für Gruppenadministratoren](#access-level-setup-options-for-group-administrators)
* [Erstellen von Timesheet-Profilen für Gruppen](#create-timesheet-profiles-for-groups)
* [Gelöschte Elemente für Benutzer als Gruppenadministrator wiederherstellen](#recover-deleted-items-for-users-as-a-group-administrator)

### Benutzeroberfläche &quot;Kennwort zurücksetzen&quot;für Gruppenadministratoren aktualisiert {#reset-password-ui-updated-for-group-administrators}

Als Gruppenadministrator werden Sie beim Zurücksetzen des Kennworts für einen anderen Benutzer aufgefordert, Ihr eigenes Kennwort einzugeben, bevor Sie dessen ändern können. Die Benutzeroberfläche wurde entsprechend dieser Funktion aktualisiert. Vor dieser Änderung zeigte die Benutzeroberfläche, dass das Workfront-Administratorkennwort erforderlich war.

Weitere Informationen zum Zurücksetzen von Kennwörtern für andere Benutzer finden Sie unter [Profil eines Benutzers bearbeiten](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Weitere Informationen zu den Funktionen eines Gruppenadministrators finden Sie im Abschnitt &quot;Funktionen von Gruppenadministratoren&quot;unter [Erstellen einer Gruppe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Optionen für die Einrichtung auf Zugriffsebene für Gruppenadministratoren {#access-level-setup-options-for-group-administrators}

Als Workfront-Administrator können Sie jetzt steuern, ob Gruppenadministratoren sich als andere Benutzer anmelden können oder ob sie die Passwörter anderer Benutzer zurücksetzen können. In der Zugriffsebene wurde eine neue Einstellung hinzugefügt, um diesen Zugriff zu aktivieren oder zu deaktivieren. Vor dieser Änderung konnten sich alle Gruppenadministratoren als andere Benutzer anmelden und die Passwörter anderer Benutzer standardmäßig zurücksetzen. Diese Änderung betrifft nur die Planerzugriffsstufe.

Weitere Informationen zum Konfigurieren der Zugriffsebene für Benutzer finden Sie unter [Gewähren des Zugriffs für Benutzer](../../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Weitere Informationen zu den Funktionen eines Gruppenadministrators finden Sie im Abschnitt &quot;Funktionen von Gruppenadministratoren&quot;unter [Erstellen einer Gruppe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Erstellen von Datenblatt-Profilen für Gruppen {#create-timesheet-profiles-for-groups}

Als Gruppenadministrator können Sie nun für die von Ihnen verwalteten Gruppen oder für Benutzer dieser Gruppen Profile aus dem Datenblatt erstellen und diese Gruppen Gruppen zuordnen. Timesheet-Profile stellen sicher, dass Timesheets automatisch für die ihnen zugeordneten Benutzer erstellt werden.

Vor dieser Änderung konnte nur ein Workfront-Administrator Timesheet-Profile erstellen.

Weitere Informationen zum Erstellen von Timesheet-Profilen finden Sie unter [Erstellen, Bearbeiten und Zuweisen von Timesheet-Profilen](../../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Weitere Informationen zu den Funktionen eines Gruppenadministrators finden Sie im Abschnitt &quot;Funktionen von Gruppenadministratoren&quot;unter [Erstellen einer Gruppe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Gelöschte Elemente für Benutzer als Gruppenadministrator wiederherstellen {#recover-deleted-items-for-users-as-a-group-administrator}

Wenn ein Projekt mit einer Gruppe verknüpft ist, für die Sie Gruppenadministrator sind, können Sie das Projekt oder eine der gelöschten Aufgaben, Probleme oder Dokumente aus dem Papierkorb wiederherstellen. Vor dieser Änderung konnte nur ein Workfront-Administrator Elemente aus dem Papierkorb wiederherstellen.

Weitere Informationen zum Wiederherstellen gelöschter Elemente in Workfront finden Sie unter [Gelöschte Elemente wiederherstellen](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

Weitere Informationen zu den Funktionen eines Gruppenadministrators finden Sie im Abschnitt &quot;Funktionen von Gruppenadministratoren&quot;unter [Erstellen einer Gruppe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 

## HTML5-Viewer-Verbesserungen beim Testversand  {#html5-proofing-viewer-improvements}

* [Vergleichsmodus](#compare-mode)
* [Filtern der Kommentarliste](#filter-the-comment-list)
* [Die Kommentarliste wird durchsucht, nachdem das erste Zeichen eingegeben wurde.](#comment-list-is-searched-after-the-first-character-is-entered)

### Vergleichsmodus {#compare-mode}

Sie können jetzt den Vergleichsmodus im HTML5-Testversand-Viewer verwenden, wenn Sie statische und Videoproofs anzeigen. 

Der Vergleichsmodus im HTML5-Prüf-Viewer unterscheidet sich wie folgt vom alten Testversand-Viewer:

* Beim Starten des Vergleichsmodus wird die neuere Version auf die rechte Seite verschoben, wobei die Version, die Sie vergleichen, auf der linken Seite geöffnet wird.

  Zuvor wurde die neuere Version auf die linke Seite verschoben, wobei die Version, die Sie vergleichen, die Öffnung auf der rechten Seite.

* Sie können direkt im Testversand-Viewer auswählen, welche Version eines Testversands Sie vergleichen möchten. 
* Beim gleichzeitigen Navigieren werden der aktuelle Zoom-Wert und die aktuelle Position der Testsendungen im Testversand-Viewer beibehalten.
* Neue Option &quot;Zurücksetzen&quot;bei gleichzeitiger Navigation.
* Beim Beenden des Vergleichsmodus können Sie auswählen, welcher Testversand geschlossen werden soll. 

  Zuvor war die ältere Version immer geschlossen.

* Verschiedenes Erscheinungsbild und Benutzerfreundlichkeit verbessert.

Weitere Informationen finden Sie unter [Testsendungen im Testversand-Viewer vergleichen](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/compare-proofs.md).

### Filtern der Kommentarliste {#filter-the-comment-list}

Sie können nun Kommentare in der Kommentarliste filtern. Sie können nach Benutzer, Aktionen, ungelesenen Daten und mehr filtern.

### Die Kommentarliste wird durchsucht, nachdem das erste Zeichen eingegeben wurde. {#comment-list-is-searched-after-the-first-character-is-entered}

Bei der Suche nach der Kommentarliste wird die Liste nach der Eingabe des ersten Zeichens automatisch gefiltert.

Vor dieser Änderung mussten Sie mindestens 3 Zeichen in das Suchfeld eingeben, bevor die Kommentarliste gefiltert wurde.

Weitere Informationen finden Sie unter .

## Verbesserungen bei der Überprüfung in Workfront {#proofing-improvements-within-workfront}

* [Verknüpfen von Testsendungen von Workfront Proof mit Workfront](#link-proofs-from-workfront-proof-to-workfront)
* [Kann einen Testversand nicht mehr aus einem Dokument entfernen](#can-no-longer-remove-a-proof-from-a-document)
* [Aktualisiertes Erscheinungsbild beim Erstellen und Öffnen von Testsendungen](#updated-look-and-feel-when-generating-and-opening-proofs)

### Verknüpfen von Testsendungen von Workfront Proof mit Workfront {#link-proofs-from-workfront-proof-to-workfront}

Sie können jetzt Dokumentsendungen, die bereits in Ihrem Workfront Proof-Konto vorhanden sind, mit Workfront verknüpfen.

Vor dieser Änderung konnten Sie nicht auf Testsendungen zugreifen, die bereits in Workfront Proof in Workfront existierten. 

Weitere Informationen finden Sie unter [Verknüpfen von Dokumenten aus externen Anwendungen](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md) in [Verknüpfen von Dokumenten aus externen Anwendungen](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Kann einen Testversand nicht mehr aus einem Dokument entfernen {#can-no-longer-remove-a-proof-from-a-document}

Sie können einen Testversand nicht mehr aus einem Dokument entfernen. Um einen Testversand zu entfernen, müssen Sie stattdessen das gesamte Dokument löschen.

Diese Verbesserung verringert das Risiko, dass Benutzer versehentlich alle Versionen eines Testdokuments löschen. 

Informationen zum Löschen eines Dokuments finden Sie unter [Testversand löschen](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md) in [Testversand löschen](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md) .

### Aktualisiertes Erscheinungsbild beim Erstellen und Öffnen von Testsendungen {#updated-look-and-feel-when-generating-and-opening-proofs}

Es gibt jetzt einen aktualisierten Animations-Spinner, wenn ein Testversand erzeugt wird.

## Verbesserungen am Startbereich {#home-area-improvements}

Die folgenden Verbesserungen wurden am Home-Bereich vorgenommen:

* [Testversandgenehmigungen aus dem Startbereich anzeigen](#view-proof-approvals-from-the-home-area)
* [Standardfelder werden beim Konfigurieren der Layout-Vorlage für Elemente im Startbereich angezeigt](#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area)

### Anzeigen von Testversandgenehmigungen im Startbereich {#view-proof-approvals-from-the-home-area}

Zusätzlich zu den Standardgenehmigungen können Sie jetzt Testsendungen im Bereich Home anzeigen.

Bisher konnten Sie Workfront-Genehmigungen anzeigen, aber keine Genehmigungen für einen Testversand anzeigen.  

Weitere Informationen finden Sie unter [Verwenden des Startbereichs](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

### Standardfelder werden beim Konfigurieren der Layout-Vorlage für Elemente im Startbereich angezeigt {#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area}

Zuvor waren die Standardfelder nicht in der Layoutvorlage sichtbar.

Weitere Informationen finden Sie unter &quot;Erstellen und Verwalten von Layout-Vorlagen&quot;.

## Agile Verbesserungen {#agile-improvements}

* [Fügen Sie Aufgaben und Probleme direkt über die Seite mit den Aufgaben- oder Problemdetails zur Iteration hinzu](#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page)
* [Hinzufügen von Problemen im Scrum-Rückprotokoll und auf der Story-Pinnwand für ein Agile-Team](#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team)
* [Anwenden von Gruppierungen und Filtern auf das Rückprotokoll für ein Agile-Team](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [Erstellen Sie eine leere Iteration und aktualisieren Sie sie später ](#create-a-blank-iteration-and-update-it-later)
* [Die Felder &quot;Fokus&quot;und &quot;Kapazität&quot;werden bei der Erstellung einer Iteration vorausgefüllt](#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration)

### Aufgaben und Probleme direkt über die Seite &quot;Aufgaben&quot;oder &quot;Problemdetails&quot;zur Iteration hinzufügen {#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page}

Sie können jetzt Aufgaben und Probleme, die derzeit einem agilen Team zugewiesen sind, direkt aus der Aufgabe oder dem Problem einer Iteration hinzufügen.

Zuvor konnten Sie einer Iteration Aufgaben nur aus dem Rückstand hinzufügen. 

Weitere Informationen finden Sie unter [Erstellen einer Iteration](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md) in [Erstellen einer Iteration](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

### Einbeziehen von Problemen im Scrum-Rückholprotokoll und auf dem Story-Forum für ein Agile-Team {#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team}

Probleme werden jetzt bei der Verwendung der Scrum-agile-Methode standardmäßig im Rückstand Ihres agile Teams berücksichtigt (Probleme werden bei der Verwendung der Kanban-Methode nicht im Rückstand eines agilen Teams angezeigt).

Vor dieser Änderung konnten nur Aufgaben zum Rückstand hinzugefügt werden. Wenn Sie ein Problem hinzufügen möchten, mussten Sie das Problem zunächst in eine Aufgabe konvertieren, bevor es hinzugefügt werden konnte.

Informationen zur Verwendung von Problemen im Rückstau finden Sie unter  [Verwalten Sie den agilen Backlog](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

### Anwenden von Gruppierungen und Filtern auf das Rückprotokoll für ein Agile-Team {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

Die Optionen Gruppierung und Filter sind jetzt im agilen Backlog verfügbar, sodass Sie Ihren Rückstand nach Gruppierungen organisieren und nach bestimmten Aufgaben und Problemen filtern können.

Vor dieser Änderung können Sie Ansichten auf den agilen Rückstand anwenden.

Weitere Informationen finden Sie unter  [Verwalten Sie den agilen Backlog](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) in  [Verwalten Sie den agilen Backlog](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

### Erstellen Sie eine leere Iteration und aktualisieren Sie sie später. {#create-a-blank-iteration-and-update-it-later}

Es ist nicht mehr erforderlich, eine Aufgabe oder ein Problem zu einer Iteration hinzuzufügen, um sie zu erstellen. Sie können eine leere Iteration erstellen und Aufgaben und Probleme zu einem späteren Zeitpunkt hinzufügen.

Weitere Informationen finden Sie unter [Erstellen einer Iteration](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

### Die Felder &quot;Fokus&quot;und &quot;Kapazität&quot;werden bei der Erstellung einer Iteration vorausgefüllt {#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration}

Beim Erstellen einer Iteration werden nun die Felder &quot;Fokus&quot;und &quot;Kapazität&quot;vorab mit den Durchschnittswerten für alle früheren Iterationen ausgefüllt, die Ihr Team erstellt hat. Wenn Ihr Team noch keine Iterationen erstellt hat, werden diese Felder als 0 angezeigt.

Zuvor waren diese Felder immer auf 0 gesetzt.

Weitere Informationen finden Sie unter [Erstellen einer Iteration](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

## Gantt-Diagrammverbesserungen {#gantt-chart-improvements}

* [Aktivieren Sie den Bearbeitungsmodus im Gantt-Diagramm](#enable-edit-mode-in-the-gantt-chart)
* [Entfernen von Vorgängern bei der Bearbeitung des Gantt-Diagramms](#remove-predecessors-when-editing-the-gantt-chart)

### Aktivieren Sie den Bearbeitungsmodus im Gantt-Diagramm {#enable-edit-mode-in-the-gantt-chart}

Wenn Sie den Bearbeitungsmodus im Gantt-Diagramm aktivieren, können Sie Änderungen an Informationen innerhalb des Diagramms vornehmen. Vor dieser Änderung konnten Sie die Informationen im Gantt-Diagramm nicht bearbeiten. Sie konnten nur Aufgabeninformationen in der Aufgabenliste bearbeiten.

Weitere Informationen zum Bearbeiten des Gantt-Diagramms finden Sie unter [Informationen in der Aufgabenliste aktualisieren Gantt-Diagramm](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

### Entfernen von Vorgängern bei der Bearbeitung des Gantt-Diagramms {#remove-predecessors-when-editing-the-gantt-chart}

Mithilfe des Bearbeitungsmodus für das Gantt-Diagramm können Sie jetzt Vorgängerbeziehungen zwischen Aufgaben im Gantt-Diagramm eines Projekts entfernen. Vor dieser Verbesserung konnten Sie die Vorgängerbeziehung nur in der Aufgabenliste oder auf Aufgabenebene entfernen.

Weitere Informationen zum Bearbeiten des Gantt-Diagramms finden Sie unter [Informationen in der Aufgabenliste aktualisieren Gantt-Diagramm](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Verbesserungen beim Ressourcenplaner {#resource-planner-improvements}

* [Budget mit Nulldauer im Ressourcenplaner](#budget-with-zero-duration-in-the-resource-planner)

* [Anzeigen von Daten nach Kosten im Ressourcenplaner](#show-data-by-cost-in-the-resource-planner)

### Budget mit Null Dauer im Ressourcenplaner {#budget-with-zero-duration-in-the-resource-planner}

>[!NOTE]
>
>Diese Funktion wurde aus der Vorschau-Umgebung entfernt und wird mit Version 18.1 veröffentlicht.

Sie können Ihre Ressourcen jetzt im Ressourcenplaner für ein beliebiges Datum innerhalb oder außerhalb des Zeitrahmens des Projekts einplanen. Vor dieser Verbesserung konnten Sie Ihre Ressourcen nur für die Daten innerhalb des Zeitrahmens des Projekts einsetzen.

Weitere Informationen zu Budgetierungsressourcen im Ressourcenplaner finden Sie im Abschnitt &quot;Budgetierung von Ressourcen im Ressourcenplaner&quot;in der [Ressourcenplanerübersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Anzeigen von Daten nach Kosten im Ressourcenplaner {#show-data-by-cost-in-the-resource-planner}

Sie können die Informationen jetzt im Ressourcenplaner nach Kosten sowie nach Stunden- und FTE-Werten anzeigen. Sie können die Kosten im Ressourcenplaner anzeigen, wenn Sie sie in der Ansicht &quot;Nach Projekt&quot;oder &quot;Nach Rolle anzeigen&quot;anzeigen. Sie können die Kosten nicht anzeigen, wenn Sie den Ressourcenplaner in der Ansicht &quot;Ansicht nach Benutzer&quot;anzeigen.

Weitere Informationen zum Anzeigen des Ressourcenplaners nach Stunden-, FTE- oder Kostenwerten finden Sie unter [Navigationsübersicht für Ressourcenplaner](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).
