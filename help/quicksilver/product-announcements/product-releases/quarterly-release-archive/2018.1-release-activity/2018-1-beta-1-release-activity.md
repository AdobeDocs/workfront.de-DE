---
content-type: release-notes
navigation-topic: product-releases-archive
title: Beta 1-Release-Aktivität von 2018.1
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 1-Version 2018.1 verfügbar waren. Die Funktionalität auf dieser Seite wurde am 1. Dezember 2017 in der Vorschau-Umgebung bereitgestellt. Sie wird im März 2018 im Produktionsumfeld zur Verfügung gestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: efcc2217-ab69-4ac4-8e9a-f811eba77d49
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1065'
ht-degree: 0%

---

# Beta 1-Release-Aktivität von 2018.1

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 1-Version 2018.1 verfügbar waren. Die Funktionalität auf dieser Seite wurde am 1. Dezember 2017 in der Vorschau-Umgebung bereitgestellt. Sie wird im März 2018 im Produktionsumfeld zur Verfügung gestellt.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktionalität kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen, die 2018.1 vorgenommen wurden, finden Sie unter  [Übersicht über die Veröffentlichungsaktivität 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

Die Version 2018.1 von Beta 1 enthält Verbesserungen für Workfront-Administratoren und andere Benutzer:

**Für Administratoren**

* [Aktualisierte Layoutvorlage zur Unterstützung des Startbereichs](#updated-layout-template-to-support-the-home-area)
* [Deaktivieren von von von Workfront gesendeten Testversand-E-Mail-Benachrichtigungen](#disable-proofing-email-notifications-sent-from-workfront)
* [Neue Ressourcen zu Ereignisabonnements hinzugefügt](#new-resources-added-to-event-subscriptions)

**Für alle Benutzer**

* [Startbereich (mein Arbeitsbereich wurde aktualisiert)](#home-area-updated-my-work-area)
* [Anzeigen von Ressourcenplandaten unter &quot;Geschäftsfall&quot;und aktualisierte Zusammenfassung der Geschäftsfälle](#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary)
* [Anzeigen des Prozentsatzes der geplanten Stundenzuordnung im Ressourcenplaner](#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner)
* [Der Trigger &quot;Automatische und bei Änderung&quot;und &quot;Nur ändern&quot;-Aktualisierungstypen aktualisiert die übergeordneten Objekte gleichzeitig mit den Aufgaben.](#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated)
* [Timeline-Schnappschuss im Gantt-Diagramm verfügbar](#timeline-snapshot-available-in-the-gantt-chart)

## Home Area (mein Arbeitsbereich wurde aktualisiert) {#home-area-updated-my-work-area}

Der neue Startbereich bietet eine alternative, erweiterte Ansicht zu denselben Daten, die derzeit im Arbeitsbereich &quot;Meine Arbeit&quot;verfügbar sind. Der Bereich &quot;Home&quot;bietet im Vergleich zum Bereich &quot;My Work&quot;die folgenden Vorteile:

* Eine optimierte und intuitivere Benutzeroberfläche
* Verbesserte Leistung
* Aufgaben und Probleme mit der Rich-Text-Formatierung aktualisieren

## Aktualisierte Layoutvorlage zur Unterstützung des Startbereichs {#updated-layout-template-to-support-the-home-area}

Als Workfront-Administrator können Sie durch Konfiguration der Layout-Vorlage, der Sie zugewiesen sind, feststellen, ob Benutzer in Ihrem Unternehmen Zugriff auf den Startbereich haben. Benutzer, denen keine Layoutvorlage zugewiesen wurde, können immer auf den Startbereich zugreifen.

Weitere Informationen finden Sie unter &quot;Erstellen und Verwalten von Layoutvorlagen&quot;.

## Deaktivieren von von Workfront gesendeten Testversand-E-Mail-Benachrichtigungen {#disable-proofing-email-notifications-sent-from-workfront}

Sie können jetzt konfigurieren, ob Benutzer in Ihrer Workfront-Instanz E-Mail-Benachrichtigungen von Workfront erhalten, wenn ein Kommentar zu einem Testversand erstellt wird.

Zuvor wurden Testversand-E-Mails immer von Workfront gesendet, wenn ein Kommentar zu einem Testversand abgegeben wurde. Wenn Benachrichtigungen auch in Workfront Proof aktiviert waren, erhielten Benutzer doppelte Benachrichtigungen. 

Für Bestandskunden von Workfront ist Workfront standardmäßig so konfiguriert, dass E-Mails gesendet werden, wenn ein Kommentar zu einem Testversand abgegeben wird.

Informationen zum Deaktivieren von E-Mail-Benachrichtigungen für Testsendungen in Workfront, sodass Testversand-E-Mails nur von Workfront Proof gesendet werden, finden Sie unter .  

## Anzeigen von Ressourcen-Planer-Daten unter &quot;Geschäftsfall&quot;und aktualisierte Geschäftsfallzusammenfassung {#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary}

Der Bereich Ressourcenbudgetierung ist jetzt im Business Case eines Projekts verfügbar. In diesem Bereich können Sie die für Ihre Ressourcen geschätzten budgetierten Stunden im Ressourcenplaner und die damit verbundenen budgetierten Arbeitskosten einsehen.

Der Bereich &quot;Ressourcenschätzungen&quot;im Geschäftsfall wurde in &quot;Ältere Ressourcenschätzungen&quot;umbenannt.

Im Rahmen dieser Änderung enthält die Zusammenfassung der Geschäftsszenarios nun Finanzinformationen, die sowohl auf Ressourcenschätzungen als auch auf Ressourcenbudgetierung basieren.

Vor dieser Änderung konnten Sie keine Ressourcen-Planer-Informationen zum Geschäftsfall des Projekts sehen. Sie konnten nur die Informationen zu Ressourcenschätzungen sehen, die im Kapazitätsplaner der Legacy-Ressourcen-Pools angegeben sind.

Weitere Informationen zum Erstellen eines Geschäftsszenarios finden Sie unter [Erstellen eines Geschäftsszenarios für ein Projekt](../../../../manage-work/projects/define-a-business-case/create-business-case.md).

## Anzeigen des Prozentsatzes der geplanten Stundenzuweisung im Ressourcenplaner {#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner}

Die Benutzeransicht des Ressourcen-Planers enthält jetzt eine neue Spalte, mit der Sie die geplante Stundenzuordnung als Prozentsatz der insgesamt verfügbaren Stunden für den Benutzer und der Auftragsrolle anzeigen können.

Vor dieser Änderung konnten Sie die Gesamtanzahl der geplanten und verfügbaren Stunden für Benutzer und Stellenrollen nur in separaten Spalten anzeigen.

Weitere Informationen zur Spalte &quot;Prozentualer Anteil der geplanten Stundenzuweisung&quot;finden Sie im Abschnitt &quot;Unterschiede zwischen verfügbaren und geplanten Stunden oder FTE im Ressourcenplaner anzeigen&quot;in der [Ressourcenplanübersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Der Trigger &quot;Automatische und Nur Änderung&quot;und &quot;Nur Änderung aktualisieren&quot;aktualisiert die übergeordneten Objekte gleichzeitig mit den aktualisierten Aufgaben {#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated}

Die Art und Weise, wie übergeordnete Aufgaben und das Projekt aktualisiert werden, wenn ein Objekt der unteren Ebene in einem Projekt aktualisiert wird, wurde geändert. Der Zeitpunkt, zu dem ein übergeordnetes Objekt aktualisiert wird, wird durch das Feld Aktualisierungstyp für ein Projekt bestimmt. Sie können aus den folgenden Aktualisierungstypen auswählen:

* Automatisch UND bei Änderung
* Nur Änderung
* Nur automatisch
* Nur manuell

Wenn Sie nun die Aktualisierungstypen &quot;Automatisch und Bei Änderung&quot;oder &quot;Nur ändern&quot;auswählen, werden die Änderungen, die Sie auf die einzelnen Aufgaben anwenden, auch auf die übergeordnete Aufgabe und das Projekt sofort angewendet.

Vor dieser Änderung mussten Sie die Seite aktualisieren, um sicherzustellen, dass die übergeordneten Objekte und die Timeline des Projekts ebenfalls aktualisiert wurden.

Weitere Informationen zum Aktualisierungstyp eines Projekts finden Sie unter [Auswählen des Aktualisierungstyps für das Projekt](../../../../manage-work/projects/manage-projects/select-project-update-type.md).

## Timeline-Schnappschuss im Gantt-Diagramm verfügbar {#timeline-snapshot-available-in-the-gantt-chart}

Sie können jetzt schnell zu einem bestimmten Punkt in der Lebensdauer eines Projekts scrollen, indem Sie den neuen Timeline-Schnappschuss im Gantt-Diagramm verwenden.

Wenn Sie beim Anzeigen einer Aufgabe oder einer Projektliste einen genaueren Zeitrahmen für das Gantt-Diagramm auswählen, wird unten im Gantt-Diagramm eine horizontale Bildlaufleiste angezeigt. Durch Klicken auf die Bildlaufleiste können Sie die gesamte Timeline des Projekts in einer Momentaufnahme anzeigen. Sie können auf eine beliebige Stelle innerhalb des Gantt-Diagramm-Snapshots klicken, um zu einem bestimmten Punkt in der Lebensdauer des Projekts zu navigieren.

Vor dieser Änderung musste ein horizontaler Bildlauf im gesamten Gantt-Diagramm durchgeführt werden, um einen bestimmten Zeitpunkt zu finden, oder man musste aus der granularen Ansicht herauszoomen.

Weitere Informationen dazu, wie Informationen im Gantt-Diagramm angezeigt werden, finden Sie unter [Konfigurieren der Anzeige von Informationen im Gantt-Diagramm](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Neue Ressourcen zu Ereignisabonnements hinzugefügt {#new-resources-added-to-event-subscriptions}

Jetzt können Sie Ereignisanmeldungen für die folgenden Ressourcen erstellen:

* **Kosten:** Benachrichtigt Sie beim Hinzufügen oder Ändern von Ausgaben.
* **Zuweisung:** Benachrichtigt Sie beim Hinzufügen oder Ändern einer Zuweisung zu einer Aufgabe oder einem Problem für einen Benutzer, eine Jobrolle oder ein Team.
* **Datenblatt:** Benachrichtigt Sie beim Senden, Zurückweisen oder Genehmigen eines Zeitblatts.

Weitere Informationen zu Ereignisanmeldungen finden Sie unter [Ereignis-Abonnement-API](../../../../wf-api/general/event-subs-api.md).
