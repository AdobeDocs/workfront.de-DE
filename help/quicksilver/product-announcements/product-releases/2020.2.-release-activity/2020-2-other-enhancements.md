---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2 weitere Verbesserungen
description: Auf dieser Seite werden alle anderen Verbesserungen beschrieben, die mit der Version 2020.2 der Produktionsumgebung vorgenommen wurden. Diese Verbesserungen wurden in der Produktionsumgebung in der Woche vom 11. Mai 2020 bereitgestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 46ed705e-b966-4ae9-a602-a5a73a3de3aa
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# 2020.2 weitere Verbesserungen

Auf dieser Seite werden alle anderen Verbesserungen beschrieben, die mit der Version 2020.2 der Produktionsumgebung vorgenommen wurden. Diese Verbesserungen wurden in der Produktionsumgebung in der Woche vom 11. Mai 2020 bereitgestellt.

Eine Liste aller Änderungen, die mit Version 2020.2 verfügbar sind, finden Sie unter [Versionsübersicht 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Für Workfront-Administratoren: In Workfront Classic erstellte, neuere Layoutvorlagen sind jetzt im neuen Workfront-Erlebnis verfügbar

Ab Herbst 2019 in Workfront Classic erstellte Layoutvorlagen sind jetzt in der neuen Workfront-Version verfügbar. Es empfiehlt sich, diese Layoutvorlagen im neuen Workfront-Erlebnis zu aktualisieren, um neue Funktionen zu nutzen und sie für Benutzer in dieser Umgebung so nützlich wie möglich zu machen.

Weitere Informationen finden Sie unter [Layout-Vorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

**In diesen Umgebungen verfügbar:**

* Die neue Adobe Workfront-Erfahrung

## Gruppenspezifische Genehmigungsprozesse sind für alle Objekte verfügbar

Um gruppenspezifische Validierungsprozesse vollständig zu nutzen, können Sie sie jetzt bei der Bearbeitung dieser Objekte Aufgaben, Problemen und Projekten hinzufügen.

Sie können auch automatisch einen gruppenspezifischen Validierungsprozess an eine Aufgabe im Bereich Aufgaben des Felds Projekt bearbeiten sowie an Probleme anhängen, wenn Sie Anforderungswarteschlangen oder Warteschlangenthemen für ein Projekt konfigurieren.

Informationen zum Hinzufügen von Genehmigungsprozessen zu Projekten, Aufgaben und Problemen finden Sie in den folgenden Artikeln:

* [Bearbeiten von Projekten](../../../manage-work/projects/manage-projects/edit-projects.md)
* [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [Probleme bearbeiten](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
* [Erstellen von Warteschlangenthemen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)

## Erstellen von Genehmigungsprozessen für Gruppen mit benutzerdefinierten Status

Um Gruppen die Verwaltung ihrer eigenen eindeutigen Workflows zu erleichtern, können Sie jetzt gruppenspezifische benutzerdefinierte Status in Genehmigungsprozessen verwenden.

Zuvor war es einer Gruppe nicht möglich, ihre eigenen benutzerdefinierten Status mit den gruppenspezifischen Validierungsprozessen zu verwenden. Es waren nur systemweite Status verfügbar, die nicht immer den Gruppengenehmigungsprozessen entsprachen.

Benutzerdefinierte Status können jetzt sowohl in Einzelverwendungs- als auch in systemweiten Genehmigungsprozessen verwendet werden:

* Erstellen Sie einen Validierungsprozess für einzelne Verwendungszwecke für ein Objekt (Projekt, Aufgabe oder Problem) und basieren Sie es auf Status, die mit der Gruppe verknüpft sind, die an diesem Objekt arbeitet. Dazu gehören alle benutzerdefinierten Status, die mit der Gruppe verknüpft sind.
* Erstellen Sie einen globalen Genehmigungsprozess und stellen Sie ihn nur für die Gruppe oder für alle im System zur Verfügung.

Informationen zum Konfigurieren von Genehmigungsprozessen für Benutzer mit administrativem Zugriff auf Genehmigungsprozesse finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) (bzw. bei Verwendung von Adobe Workfront Classic finden Sie unter [Erstellen von Genehmigungsprozessen](https://one.workfront.com/s/article/Creating-Approval-Processes-1001577410)).

Informationen zum Verknüpfen von Genehmigungsprozessen mit Arbeitselementen finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) (bzw. bei Verwendung von Adobe Workfront Classic finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit](https://one.workfront.com/s/article/Associating-a-New-or-Existing-Approval-Process-with-Work-708455630)).

**In diesen Umgebungen verfügbar:**

* Adobe Workfront Classic
* Die neue Adobe Workfront-Erfahrung

## Neue Überlagerungsseiten für die Suche

Damit Benutzer im neuen Workfront-Erlebnis einfacher zwischen Suchseiten und vorherigen Seiten hin und her navigieren können, haben wir eine Überlagerungsseite für die Suche hinzugefügt, die teilweise den Bildschirm abdeckt.

Wenn Sie nun im Menü &quot;Suchen&quot;auf Erweiterte Suche klicken oder eine einfache Suche durchführen, wird eine Seite von der rechten Seite des Bildschirms aus eingeblendet.

Weitere Informationen finden Sie unter [Adobe Workfront durchsuchen](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

**In diesen Umgebungen verfügbar:**

* Die neue Adobe Workfront-Erfahrung

## Aktualisierungen von Ereignisanmeldungen

Um Benutzern die Möglichkeit zu geben, Probleme besser zu testen, zu beheben und zu beheben, haben wir das Verhalten geändert und der API für Ereignisabonnements weitere Daten hinzugefügt. Wir haben auch die folgenden Änderungen vorgenommen:

* Migrierte zugrunde liegende Messaging-Technologien
* Erstellen Sie den Dienst neu, um weniger komplexe Abhängigkeiten zu haben und so effizienter zu skalieren.
* Verbesserte Überwachung und Warnmeldung

Weitere Informationen finden Sie unter [FAQs - Ereignis-Abonnements](../../../wf-api/general/event-subs-faq.md) und [Best Practices für Ereignisabonnements](../../../wf-api/general/event-sub-best-practice.md).
