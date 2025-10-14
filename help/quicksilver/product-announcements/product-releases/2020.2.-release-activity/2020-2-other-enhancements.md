---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2 Weitere Verbesserungen
description: Auf dieser Seite werden alle anderen Verbesserungen beschrieben, die mit der Version 2020.2 an der Produktionsumgebung vorgenommen wurden. Diese Verbesserungen wurden in der Woche vom 11. Mai 2020 in der Produktionsumgebung verfügbar gemacht.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 46ed705e-b966-4ae9-a602-a5a73a3de3aa
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# 2020.2 Weitere Verbesserungen

Auf dieser Seite werden alle anderen Verbesserungen beschrieben, die mit der Version 2020.2 an der Produktionsumgebung vorgenommen wurden. Diese Verbesserungen wurden in der Woche vom 11. Mai 2020 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller mit Version 2020.2 verfügbaren Änderungen finden Sie unter [Übersicht über die Version 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Für Workfront-Administratoren: Neuere Layout-Vorlagen, die in Workfront Classic erstellt wurden, jetzt in der neuen Workfront-Version verfügbar

Layout-Vorlagen, die nach Herbst 2019 in Workfront Classic erstellt wurden, sind jetzt in der neuen Workfront-Version verfügbar. Es empfiehlt sich, diese Layout-Vorlagen im neuen Workfront-Erlebnis zu aktualisieren, um neue Funktionen zu nutzen und sie für Benutzende in dieser Umgebung so nützlich wie möglich zu machen.

Weitere Informationen finden Sie unter [Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

**In diesen Umgebungen verfügbar:**

* Das neue Adobe Workfront-Erlebnis

## Für alle Objekte stehen gruppenspezifische Validierungsprozesse zur Verfügung

Um gruppenspezifische Genehmigungsprozesse vollständig zu nutzen, können sie jetzt zu Aufgaben, Problemen und Projekten hinzugefügt werden, wenn Sie diese Objekte bearbeiten.

Sie können einen gruppenspezifischen Genehmigungsprozess auch automatisch an eine Aufgabe im Bereich Aufgaben des Felds Projekt bearbeiten sowie an Probleme anhängen, wenn Sie Anfrage-Warteschlangen oder Warteschlangenthemen für ein Projekt konfigurieren.

Informationen zum Hinzufügen von Genehmigungsprozessen zu Projekten, Aufgaben und Problemen finden Sie in den folgenden Artikeln:

* [Bearbeiten von Projekten](../../../manage-work/projects/manage-projects/edit-projects.md)
* [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [Probleme bearbeiten](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Anfrage-Warteschlange erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
* [Warteschlangenthemen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)

## Erstellen von Genehmigungsprozessen für Gruppen mit benutzerdefinierten Status

Um es Gruppen zu erleichtern, ihre eigenen eindeutigen Workflows zu verwalten, können Sie jetzt gruppenspezifische benutzerdefinierte Status in Genehmigungsprozessen verwenden.

Zuvor konnte eine Gruppe keine eigenen benutzerdefinierten Status mit ihren gruppenspezifischen Genehmigungsprozessen verwenden. Es waren nur systemweite Status verfügbar, die nicht immer den Gruppengenehmigungsprozessen entsprachen.

Benutzerdefinierte Status können jetzt sowohl in einmaligen als auch systemweiten Genehmigungsprozessen verwendet werden:

* Erstellen Sie einen einmaligen Genehmigungsprozess für ein Objekt (Projekt, Aufgabe oder Problem) und basieren Sie ihn auf Status, die mit der Gruppe verknüpft sind, die an diesem Objekt arbeitet. Dazu gehören alle benutzerdefinierten Status, die mit der Gruppe verknüpft sind.
* Erstellen Sie einen globalen Genehmigungsprozess und stellen Sie ihn nur für die Gruppe oder für alle Personen im System zur Verfügung.

Für Benutzer mit administrativem Zugriff auf Genehmigungsprozesse sind Informationen zum Konfigurieren von Genehmigungsprozessen unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) verfügbar (oder wenn Sie Adobe Workfront Classic verwenden, siehe [Erstellen von Genehmigungsprozessen](https://experienceleague.adobe.com/de/docs/workfront/using/home)).

Für Benutzende sind Informationen zum Verknüpfen von Genehmigungsprozessen mit Arbeitselementen unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit Arbeit](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) verfügbar (oder wenn Sie Adobe Workfront Classic verwenden, siehe &quot;[&#x200B; eines neuen oder vorhandenen Genehmigungsprozesses mit Arbeit](https://experienceleague.adobe.com/de/docs/workfront/using/home)).

**In diesen Umgebungen verfügbar:**

* Adobe Workfront Classic
* Das neue Adobe Workfront-Erlebnis

## Neue Überlagerungsseiten für die Suche

Damit Benutzende in der neuen Workfront-Version leichter zwischen Suchseiten und vorherigen Seiten hin- und hernavigieren können, haben wir eine Suchüberlagerungsseite hinzugefügt, die den Bildschirm teilweise abdeckt.

Wenn Sie jetzt im Menü Suche auf Erweiterte Suche klicken oder eine einfache Suche durchführen, wird eine Seite von der rechten Seite des Bildschirms geöffnet.

Weitere Informationen finden Sie unter [Adobe Workfront durchsuchen](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

**In diesen Umgebungen verfügbar:**

* Das neue Adobe Workfront-Erlebnis

## Aktualisierungen der Ereignisabonnements

Um Benutzenden die Möglichkeit zu geben, Probleme zu klassifizieren, zu beheben und zu beheben, haben wir das Verhalten geändert und weitere Daten zur Ereignisabonnement-API hinzugefügt. Wir haben außerdem folgende Änderungen vorgenommen:

* Migrierte zugrunde liegende Messaging-Technologien
* Service neu erstellt, um weniger komplexe Abhängigkeiten zu haben und somit effizienter zu skalieren
* Überwachung und Warnhinweise wurden verbessert

Weitere Informationen finden Sie unter [FAQs - Ereignisabonnements](../../../wf-api/general/event-subs-faq.md) und [Best Practices für Ereignisabonnements](../../../wf-api/general/event-sub-best-practice.md).
