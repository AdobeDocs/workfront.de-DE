---
content-type: release-notes
navigation-topic: product-releases-archive
title: Versionsaktivität von Beta 1 2018.1
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 1 Version 2018.1 verfügbar waren. Die Funktion auf dieser Seite wurde am 1. Dezember 2017 in der Vorschau-Umgebung verfügbar gemacht. Sie wird im März 2018 in der Produktionsumgebung bereitgestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: efcc2217-ab69-4ac4-8e9a-f811eba77d49
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1065'
ht-degree: 0%

---

# Versionsaktivität von Beta 1 2018.1

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 1 Version 2018.1 verfügbar waren. Die Funktion auf dieser Seite wurde am 1. Dezember 2017 in der Vorschau-Umgebung verfügbar gemacht. Sie wird im März 2018 in der Produktionsumgebung bereitgestellt.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktion kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen in Version 2018.1 finden Sie unter  Übersicht über die Versionsaktivität [2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

Die Beta-Version 2018.1 enthält Verbesserungen für Workfront-Administratoren und andere Benutzende:

**Für Administratoren**

* [Die Layoutvorlage wurde aktualisiert, um den Bereich „Startseite“ zu unterstützen](#updated-layout-template-to-support-the-home-area)
* [Deaktivieren von Proofing-E-Mail-Benachrichtigungen, die von Workfront gesendet werden](#disable-proofing-email-notifications-sent-from-workfront)
* [Neue Ressourcen zu Ereignisabonnements hinzugefügt](#new-resources-added-to-event-subscriptions)

**Für alle Benutzer**

* [Home-Bereich (Bereich „Meine Arbeit“ aktualisiert)](#home-area-updated-my-work-area)
* [Anzeigen von Ressourcenplaner-Daten unter dem Business-Case und der aktualisierten Business-Case-Zusammenfassung](#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary)
* [Zeigt den Prozentsatz der geplanten Stundenzuordnung im Ressourcenplaner an](#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner)
* [Der Trigger „Automatisch und bei Änderung“ und „Nur Änderung“ aktualisiert die übergeordneten Objekte gleichzeitig mit der Aktualisierung von Aufgaben](#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated)
* [Im Gantt-Diagramm verfügbare Zeitleisten-Momentaufnahme](#timeline-snapshot-available-in-the-gantt-chart)

## Home-Bereich (Bereich „Meine Arbeit“ aktualisiert) {#home-area-updated-my-work-area}

Der neue Bereich Startseite bietet eine alternative, erweiterte Ansicht der gleichen Daten, die derzeit im Bereich Meine Arbeit verfügbar sind. Der Bereich Startseite bietet im Bereich Meine Arbeit die folgenden Vorteile:

* Eine optimierte und intuitivere Benutzeroberfläche
* Verbesserte Leistung
* Aktualisieren von Aufgaben und Problemen mit Rich-Text-Formatierung

## Die Layout-Vorlage zur Unterstützung des Home-Bereichs wurde aktualisiert {#updated-layout-template-to-support-the-home-area}

Als Workfront-Administrator können Sie festlegen, ob Benutzende in Ihrem Unternehmen Zugriff auf den Bereich Startseite haben, indem Sie die Layout-Vorlage konfigurieren, der sie zugewiesen sind. Benutzende, denen keine Layout-Vorlage zugewiesen ist, können jederzeit auf den Bereich Startseite zugreifen.

Weitere Informationen finden Sie unter „Erstellen und Verwalten von Layout-Vorlagen“.

## Von Workfront gesendete Proofing-E-Mail-Benachrichtigungen deaktivieren {#disable-proofing-email-notifications-sent-from-workfront}

Sie können jetzt konfigurieren, ob Benutzende in Ihrer Workfront-Instanz E-Mail-Benachrichtigungen von Workfront erhalten, wenn ein Korrekturabzug kommentiert wird.

Zuvor wurden Korrekturabzugs-E-Mails immer von Workfront aus gesendet, wenn ein Korrekturabzug kommentiert wurde. Wenn Benachrichtigungen auch in Workfront Proof aktiviert waren, erhielten Benutzende dadurch doppelte Benachrichtigungen. 

Für bestehende Workfront-Kundinnen und -Kunden ist Workfront standardmäßig so konfiguriert, dass E-Mails gesendet werden, wenn ein Korrekturabzug kommentiert wird.

Informationen dazu, wie Sie E-Mail-Benachrichtigungen für Korrekturabzüge in Workfront deaktivieren, sodass Korrekturabzugs-E-Mails nur von Workfront Proof aus gesendet werden, finden Sie unter .  

## Anzeigen von Ressourcenplaner-Daten unter dem Business-Case und der aktualisierten Business-Case-Zusammenfassung {#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary}

Der Bereich Ressourcenbudgetierung ist jetzt für den Business Case eines Projekts verfügbar. In diesem Bereich können Sie die budgetierten Stunden, die für Ihre Ressourcen im Ressourcenplaner geschätzt wurden, und die damit verbundenen budgetierten Lohnkosten überprüfen.

Der Bereich Ressourcenkalkulationen des Business Case wurde in Legacy-Ressourcenkalkulationen umbenannt.

Im Rahmen dieser Änderung enthält die Zusammenfassung des Business Case jetzt Finanzinformationen, die sowohl auf Ressourcenkalkulationen als auch auf der Ressourcenbudgetierung basieren.

Vor dieser Änderung konnten Sie keine Ressourcenplaner-Informationen zum Business-Case des Projekts sehen. Es werden nur die Informationen zu den Ressourcenkalkulationen angezeigt, die im Kapazitätsplaner der Legacy-Ressourcenpools angegeben sind.

Weitere Informationen zum Erstellen eines Business-Case finden Sie unter [Erstellen eines Business-Case für ein Projekt](../../../../manage-work/projects/define-a-business-case/create-business-case.md).

## Zeigt den Prozentsatz der geplanten Stundenzuordnung im Ressourcenplaner an {#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner}

Die Benutzeransicht des Ressourcenplaners enthält jetzt eine neue Spalte, mit der Sie die Zuordnung der geplanten Stunde als Prozentsatz der insgesamt verfügbaren Stunden für den Benutzer und das Aufgabengebiet anzeigen können.

Vor dieser Änderung konnten Sie die Summe der geplanten und verfügbaren Stunden für Benutzer und Aufgabengebiete nur in separaten Spalten anzeigen.

Weitere Informationen zur Spalte „Geplante Stunden - Zuordnungsprozentsatz“ finden Sie im Abschnitt „Unterschiede zwischen verfügbaren und geplanten Stunden bzw. VZÄ im Ressourcenplaner anzeigen“ in [Ressourcenplaner - Übersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Der Trigger „Automatisch und bei Änderung“ und „Nur Änderung“ aktualisiert die übergeordneten Objekte gleichzeitig mit der Aktualisierung von Aufgaben {#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated}

Wir haben die Art und Weise geändert, wie übergeordnete Aufgaben und das Projekt aktualisiert werden, wenn ein Objekt auf einer niedrigeren Ebene in einem Projekt aktualisiert wird. Der Zeitpunkt, zu dem ein übergeordnetes Objekt aktualisiert wird, wird durch das Feld Aktualisierungstyp in einem Projekt bestimmt. Sie können aus den folgenden Aktualisierungstypen auswählen:

* Automatisch UND bei Änderung
* Nur Änderung
* Nur automatisch
* Nur manuell

Wenn Sie nun die Aktualisierungstypen „Automatisch und bei Änderung“ oder „Nur Änderung“ auswählen, werden die Änderungen, die Sie auf die einzelnen Aufgaben anwenden, auch auf die übergeordnete Aufgabe und das Projekt sofort angewendet.

Vor dieser Änderung mussten Sie die Seite aktualisieren, um sicherzustellen, dass die übergeordneten Objekte und die Zeitleiste des Projekts ebenfalls aktualisiert wurden.

Weitere Informationen zum Aktualisierungstyp eines Projekts finden Sie unter [Auswahl des Projektaktualisierungstyps](../../../../manage-work/projects/manage-projects/select-project-update-type.md).

## Im Gantt-Diagramm verfügbare Zeitleisten-Momentaufnahme {#timeline-snapshot-available-in-the-gantt-chart}

Sie können jetzt schnell zu einem bestimmten Zeitpunkt während der Lebensdauer eines Projekts scrollen, indem Sie die neue Momentaufnahme der Zeitleiste im Gantt-Diagramm verwenden.

Wenn Sie beim Anzeigen einer Aufgabe oder einer Projektliste einen detaillierteren Zeitrahmen für das Gantt-Diagramm auswählen, wird unten im Gantt-Diagramm ein horizontaler Bildlaufbalken angezeigt. Durch Klicken auf die Bildlaufleiste können Sie die gesamte Zeitleiste des Projekts in einem Schnappschuss anzeigen. Sie können in der Momentaufnahme des Gantt-Diagramms auf eine beliebige Stelle klicken, um zu einem bestimmten Punkt während der Lebensdauer des Projekts zu navigieren.

Vor dieser Änderung mussten Sie horizontal im gesamten Gantt-Diagramm scrollen, um einen bestimmten Zeitpunkt zu finden, oder Sie mussten die granulare Ansicht verkleinern.

Weitere Informationen zur Anzeige von Informationen im Gantt-Diagramm finden Sie unter [Konfigurieren der Anzeige von Informationen im Gantt-Diagramm](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Neue Ressourcen zu Ereignisabonnements hinzugefügt {#new-resources-added-to-event-subscriptions}

Jetzt können Sie Ereignisabonnements für die folgenden Ressourcen erstellen:

* **Ausgabe:** Benachrichtigung, wenn eine Ausgabe hinzugefügt oder geändert wird.
* **Arbeitsauftrag:** Benachrichtigt Sie, wenn ein Arbeitsauftrag zu einer Aufgabe oder einem Problem für einen Benutzer, ein Aufgabengebiet oder ein Team hinzugefügt oder geändert wird.
* **Arbeitszeittabelle:** Benachrichtigt Sie, wenn eine Arbeitszeittabelle eingereicht, abgelehnt oder genehmigt wird.

Weitere Informationen zu Ereignisabonnements finden Sie unter [Ereignisabonnement-API](../../../../wf-api/general/event-subs-api.md).
