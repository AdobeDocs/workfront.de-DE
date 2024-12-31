---
content-type: release-notes
navigation-topic: product-releases-archive
title: Versionsaktivität von Beta 2 2018.2
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 2 Version 2018.2 verfügbar waren. Die Funktion wurde am 5. April 2018 in der Vorschau-Umgebung bereitgestellt. Sie wird im Juni 2018 in der Produktionsumgebung bereitgestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: c8ef68f5-53db-4c3c-af0f-e1c98521ec27
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Versionsaktivität von Beta 2 2018.2

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 2 Version 2018.2 verfügbar waren. Die Funktion wurde am 5. April 2018 in der Vorschau-Umgebung bereitgestellt. Sie wird im Juni 2018 in der Produktionsumgebung bereitgestellt.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktion kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen in Version 2018.2 finden Sie unter  Übersicht über die Versionsaktivität [2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

Die Beta-Version 2018.2 enthält die folgenden Verbesserungen:

* [Bearbeiten von Feldern direkt im Bereich „Startseite“](#edit-fields-directly-from-the-home-area)
* [Zeit in Tagen erfassen](#log-time-in-days)
* [Zeigen Sie projektübergreifende Vorgängerbeziehungen im Gantt-Diagramm in einer Projektliste an](#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects)
* [Budgetierte Kosten im Portfolio-Optimizer zur Berechnung der Portfolio-Finanzen verwenden](#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances)
* [Auslastungsbericht: Befüllt budgetierte Stunden aus dem neuen Bereich für Ressourcenbudgetierung](#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area) (nur Vorschau)

* [Auslastungsbericht: Budgetierte Stunden nach Benutzer für ein Projekt anzeigen](#utilization-report-view-budgeted-hours-by-user-on-a-project) (nur Vorschau)

* [Korrekturabzug-Fortschritt aus der Dokumentliste für Benutzende ohne Korrekturabzug verfügbar](#proof-progress-from-the-document-list-available-to-non-proofing-users)
* [Verbesserungen für Mobilgeräte](#mobile-improvements)

## Bearbeiten von Feldern direkt im Bereich „Startseite“ {#edit-fields-directly-from-the-home-area}

Wenn Sie jetzt ein Objekt im Bereich „Startseite“ auswählen, können Sie Felder, die mit diesem Objekt verknüpft sind, direkt im rechten Bereich des Bereichs „Startseite“ bearbeiten. 

Vor dieser Änderung konnten Informationen nur im Bereich Startseite angezeigt, aber nicht bearbeitet werden.

Weitere Informationen finden Sie unter [Aktualisieren oder Bearbeiten eines Arbeitselements im Bereich „Startseite](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md) im Artikel  [Aktualisieren oder Bearbeiten eines Arbeitselements im Bereich „Startseite“](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).

## Zeit in Tagen erfassen {#log-time-in-days}

Workfront-Admins können jetzt konfigurieren, ob Benutzende in ihrer Organisation die Zeit in Tagen oder Stunden protokollieren. Benutzer mit einer Planerlizenz können diese Einstellung für sich selbst konfigurieren.

Vor dieser Änderung konnten Benutzer die Zeit nur in Stunden protokollieren.

Sie können diese Einstellung konfigurieren, indem Sie das Benutzerprofil bearbeiten. Weitere Informationen finden Sie unter [Konfigurieren, ob die Zeit in Stunden oder Tagen protokolliert wird](../../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md).

Informationen dazu, wie Benutzer die Zeit in Tagen nach der Aktualisierung dieser Einstellung protokollieren können, finden Sie unter [Zeit protokollieren](../../../../timesheets/create-and-manage-timesheets/log-time.md).

## Zeigen Sie projektübergreifende Vorgängerbeziehungen im Gantt-Diagramm in einer Projektliste an {#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects}

Sie können jetzt projektübergreifende Vorgängerbeziehungen im Gantt-Diagramm in den folgenden Projektlisten anzeigen:

* Die Registerkarte Projekte innerhalb eines Portfolios oder Programms
* In einem Projektbericht

Vor dieser Änderung konnten Sie projektübergreifende Vorgängerbeziehungen nur für einzelne Aufgaben auf Projektebene anzeigen.

Weitere Informationen finden Sie unter [Konfigurieren der Anzeige von Informationen im Gantt-Diagramm](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). 

## Budgetierte Kosten im Portfolio-Optimizer zur Berechnung der Portfolio-Finanzen verwenden {#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances}

Der neue Portfolio-Optimizer verwendet jetzt die budgetierten Kosten aus dem neuen Bereich Ressourcenbudgetierung des Business Case oder aus dem Ressourcenplaner, um die folgenden Felder zu berechnen:

* Nettowert
* Return on Investment (ROI)
* Kosten

Zuvor verwendeten sowohl der neue als auch der alte Portfolio-Optimizer die budgetierten Legacy-Kosten. Der Legacy Portfolio Optimizer verwendet weiterhin die budgetierten Legacy-Kosten, um Nettowert, Kapitalrendite und Kosten zu berechnen.

Wir haben außerdem zwei neue Felder zu den Finanzfeldern des Portfolios hinzugefügt: Legacy ROI und Legacy Net Value , um die neuen Werte aus den neuen Tools für das Ressourcenmanagement zu erfassen.

Weitere Informationen finden Sie unter Übersicht über den [Portfolio Optimizer](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md) im Artikel  [Übersicht über Portfolio Optimizer](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

## Auslastungsbericht: Befüllt budgetierte Stunden aus dem neuen Ressourcenbudgetierungsbereich {#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area}

>[!NOTE]
>
>Diese Funktion wird in der offiziellen Version der Version 2018.2 nicht in die Vorschau-Umgebung aufgenommen. Sie wird während der Beta-Phase für die Version 2018.3 wieder eingeführt und mit der Version 2018.3 in die Produktionsumgebung veröffentlicht. 

Budgetierte Stunden im Auslastungsbericht werden jetzt mit Informationen ausgefüllt, die im neuen Bereich Ressourcenbudgetierung des Business Case verfügbar sind.

Vor dieser Änderung wurden Informationen aus dem Bereich Legacy-Ressourcenkalkulationen verwendet.

Weitere Informationen finden Sie unter [Übersicht über den Bericht zur Ressourcenauslastung](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) im Artikel  [Überblick über den Bericht zur Ressourcenauslastung](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Auslastungsbericht: Budgetierte Stunden nach Benutzer für ein Projekt anzeigen {#utilization-report-view-budgeted-hours-by-user-on-a-project}

>[!NOTE]
>
>Diese Funktion wird in der offiziellen Version der Version 2018.2 nicht in die Vorschau-Umgebung aufgenommen. Sie wird während der Beta-Phase für die Version 2018.3 wieder eingeführt und mit der Version 2018.3 in die Produktionsumgebung veröffentlicht. 

Der Auslastungsbericht für ein Projekt zeigt jetzt Budgetierte Stunden nach Benutzer an.

Vor dieser Änderung wurde im Auslastungsbericht „Budgetierte Stunden“ nur nach Aufgabengebiet angezeigt. 

Weitere Informationen finden Sie [Überblick über den Ressourcenauslastungsbericht](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) im Artikel [Überblick über den Ressourcenauslastungsbericht](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Korrekturabzug-Fortschritt aus der Dokumentliste für Nicht-Proofing-Benutzer verfügbar {#proof-progress-from-the-document-list-available-to-non-proofing-users}

Die Fortschrittsanzeigen für den Korrekturabzug (gesendet, geöffnet, Kommentare abgegeben und Entscheidung) werden jetzt für alle Benutzer angezeigt, wenn die Dokumentliste angezeigt wird. Dazu gehören Benutzende, die keine Korrekturabzüge erstellen können (weitere Informationen dazu, wie Sie Benutzenden die Erstellung von Korrekturabzügen ermöglichen, finden Sie in Abschnitt .

Vor dieser Änderung waren Korrekturabzugsstatusanzeigen nur für Benutzende verfügbar, die Korrekturabzüge generieren konnten.

Weitere Informationen finden Sie unter [Testversand-Fortschritt und Statusübersicht](../../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md).

## Verbesserungen für Mobilgeräte {#mobile-improvements}

Die Mobile App enthält die folgenden Verbesserungen:

* Links, die in anderen Mobile Apps für Sie freigegeben sind, werden jetzt in der Mobile App von Workfront geöffnet.

  Weitere Informationen zur Freigabe von Links finden Sie unter .

  Dieses Update ist jetzt in iOS und Android verfügbar.

* Wir haben unsere Support-Anforderungen für die iOS-Plattform aktualisiert, um iPhone X zu unterstützen.

  Weitere Informationen zu unterstützten Mobilgeräten und Betriebssystemen finden Sie unter . 
