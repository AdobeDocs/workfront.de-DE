---
content-type: release-notes
navigation-topic: product-releases-archive
title: Beta 2-Release-Aktivität 2018.2
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 2 Version 2018.2 verfügbar waren. Die Funktion wurde am 5. April 2018 in der Vorschau-Umgebung bereitgestellt. Sie wird im Juni 2018 im Produktionsumfeld zur Verfügung gestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: c8ef68f5-53db-4c3c-af0f-e1c98521ec27
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Beta 2-Release-Aktivität 2018.2

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 2 Version 2018.2 verfügbar waren. Die Funktion wurde am 5. April 2018 in der Vorschau-Umgebung bereitgestellt. Sie wird im Juni 2018 im Produktionsumfeld zur Verfügung gestellt.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktionalität kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen, die 2018.2 vorgenommen wurden, finden Sie unter  [Übersicht über die Veröffentlichungsaktivität 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

Die Beta 2-Version 2018.2 enthält folgende Verbesserungen:

* [Felder direkt im Startbereich bearbeiten](#edit-fields-directly-from-the-home-area)
* [Protokollzeit in Tagen](#log-time-in-days)
* [Anzeigen von projektübergreifenden Vorgängerbeziehungen im Gantt-Diagramm in einer Liste von Projekten](#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects)
* [Verwenden Sie die im Portfolio Optimizer veranschlagten Kosten zur Berechnung der Portfolio-Finanzen](#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances)
* [Nutzungsbericht: Füllt die budgetierten Stunden aus dem neuen Ressourcen-Budgetierungsbereich](#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area) (nur Vorschau)

* [Nutzungsbericht: Budgetierte Stunden nach Benutzer für ein Projekt anzeigen](#utilization-report-view-budgeted-hours-by-user-on-a-project) (nur Vorschau)

* [Testversand des Fortschritts aus der Dokumentliste für Benutzer ohne Testversand verfügbar](#proof-progress-from-the-document-list-available-to-non-proofing-users)
* [Mobile Verbesserungen](#mobile-improvements)

## Felder direkt im Startbereich bearbeiten {#edit-fields-directly-from-the-home-area}

Wenn Sie jetzt ein Objekt im Startbereich auswählen, können Sie die mit diesem Objekt verknüpften Felder direkt im rechten Bereich des Startbereichs bearbeiten. 

Vor dieser Änderung konnten Informationen nur im Home-Bereich angezeigt und nicht bearbeitet werden.

Weitere Informationen finden Sie unter [Aktualisieren oder Bearbeiten eines Arbeitselements im Startbereich](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md) im Artikel  [Aktualisieren oder bearbeiten Sie ein Arbeitselement im Startbereich](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).

## Protokollzeit in Tagen {#log-time-in-days}

Workfront-Administratoren können jetzt konfigurieren, ob Benutzer in ihrer Organisation die Protokollzeit in Tagen oder Stunden eingeben. Benutzer mit einer Planner-Lizenz können diese Einstellung selbst konfigurieren.

Vor dieser Änderung konnten Benutzer die Zeit nur in Stunden protokollieren.

Sie können diese Einstellung konfigurieren, indem Sie das Benutzerprofil bearbeiten. Weitere Informationen finden Sie unter [Konfigurieren, ob die Zeit in Stunden oder Tagen protokolliert wird](../../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md).

Informationen dazu, wie Benutzer die Zeit in Tagen nach der Aktualisierung dieser Einstellung protokollieren können, finden Sie unter [Protokollzeit](../../../../timesheets/create-and-manage-timesheets/log-time.md).

## Anzeigen von projektübergreifenden Vorgängerbeziehungen auf dem Gantt-Diagramm in einer Projektliste {#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects}

Sie können jetzt projektübergreifende Vorgängerbeziehungen im Gantt-Diagramm in den folgenden Projektlisten anzeigen:

* Registerkarte &quot;Projekte&quot;innerhalb eines Portfolios oder Programms
* In einem Projektbericht

Vor dieser Änderung konnten Sie projektübergreifende Vorgängerbeziehungen nur für einzelne Aufgaben auf Projektebene anzeigen.

Weitere Informationen finden Sie unter [Konfigurieren der Anzeige von Informationen im Gantt-Diagramm](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). 

## Verwenden von Budgeting-Kosten im Portfolio Optimizer zur Berechnung von Portfolio-Finanzierungen {#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances}

Der neue Portfolio Optimizer verwendet jetzt die Budgetierung der Kosten aus dem neuen Ressourcen-Budgeting-Bereich des Business Case oder aus dem Resource Planer, um die folgenden Felder zu berechnen:

* Nettowert
* Kapitalrendite (ROI)
* Kosten

Zuvor verwendete sowohl der neue als auch der alte Portfolio Optimizer die veralteten Budgetierungskosten. Der veraltete Portfolio Optimizer verwendet weiterhin die veralteten budgetierten Kosten zur Berechnung des Nettowerts, der Kapitalrendite und der Kosten.

Außerdem haben wir zwei neue Felder zu den Portfolio-Finanzfeldern hinzugefügt: Alter ROI und Alter Net Value , um die neuen Werte aus den neuen Tools für die Ressourcenverwaltung zu erfassen.

Weitere Informationen finden Sie unter [Portfolio Optimizer - Übersicht](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md) im Artikel  [Portfolio Optimizer - Übersicht](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

## Nutzungsbericht: Füllt die budgetierten Stunden aus dem neuen Ressourcenbudgeting-Bereich aus {#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area}

>[!NOTE]
>
>Diese Funktion ist in der offiziellen Version der Vorschau-Umgebung mit Version 2018.2 nicht enthalten. Sie wird während der Beta-Phase der Version 2018.3 erneut eingeführt und mit der Version 2018.3 in die Produktionsumgebung freigegeben. 

Die im Nutzungsbericht veranschlagten Stunden werden jetzt aus den Informationen im neuen Bereich Ressourcenbudgetierung des Geschäftsfalls gefüllt.

Vor dieser Änderung wurden Informationen aus dem Bereich &quot;Ressourcenschätzungen&quot;verwendet.

Weitere Informationen finden Sie unter [Überblick über den Bericht &quot;Ressourcenauslastung&quot;](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) im Artikel  [Überblick über den Bericht &quot;Ressourcenauslastung&quot;](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Nutzungsbericht: Budgetierte Stunden nach Benutzer in einem Projekt anzeigen {#utilization-report-view-budgeted-hours-by-user-on-a-project}

>[!NOTE]
>
>Diese Funktion ist in der offiziellen Version der Vorschau-Umgebung mit Version 2018.2 nicht enthalten. Sie wird während der Beta-Phase der Version 2018.3 erneut eingeführt und mit der Version 2018.3 in die Produktionsumgebung freigegeben. 

Der Nutzungsbericht zu einem Projekt zeigt jetzt die budgetierten Stunden nach Benutzer an.

Vor dieser Änderung wurden im Nutzungsbericht nur die geplanten Stunden nach der Rolle des Auftrags angezeigt. 

Weitere Informationen finden Sie unter [Überblick über den Bericht &quot;Ressourcenauslastung&quot;](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) im Artikel [Überblick über den Bericht &quot;Ressourcenauslastung&quot;](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Testfortschritt von der Dokumentliste für Benutzer ohne Testversand verfügbar {#proof-progress-from-the-document-list-available-to-non-proofing-users}

Fortschrittsanzeigen für Testsendungen (Gesendet, Geöffnet, Kommentar erstellt und Entscheidung) werden jetzt für alle Benutzer angezeigt, wenn sie die Dokumentliste anzeigen. Dies schließt Benutzer ein, die keine Testsendungen erstellen können (weitere Informationen zum Erstellen von Testsendungen durch Benutzer finden Sie im Abschnitt .

Vor dieser Änderung waren die Fortschrittsanzeigen für Testsendungen nur für Benutzer verfügbar, die Testsendungen durchführen konnten.

Weitere Informationen finden Sie unter [Fortschrittsnachweis und Statusübersicht](../../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md).

## Mobile Verbesserungen {#mobile-improvements}

Die Mobile App enthält die folgenden Verbesserungen:

* Links, die für Sie in anderen Mobile Apps freigegeben wurden, werden jetzt in der mobilen Workfront-App geöffnet.

  Weitere Informationen zur Freigabe von Links finden Sie unter .

  Dieses Update ist jetzt in iOS und Android verfügbar.

* Wir haben unsere Supportanforderungen für die iOS-Plattform aktualisiert, um iPhone X zu unterstützen.

  Weitere Informationen zu unterstützten Mobilgeräten und Betriebssystemen finden Sie in der . 
