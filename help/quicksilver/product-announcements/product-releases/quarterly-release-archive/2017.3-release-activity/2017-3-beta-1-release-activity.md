---
content-type: release-notes
navigation-topic: product-releases-archive
title: Versionsaktivität von Beta 1 2017.3
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit der Version 2017.3 verfügbar waren. Die Funktion auf dieser Seite wurde am 9. August 2017 in der Vorschau-Umgebung verfügbar gemacht. Sie wird Anfang November 2017 in der Produktionsumgebung bereitgestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 33a91c25-98ec-4f08-b444-4e11e05e464b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1426'
ht-degree: 0%

---

# Versionsaktivität von Beta 1 2017.3

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit der Version 2017.3 verfügbar waren. Die Funktion auf dieser Seite wurde am 9. August 2017 in der Vorschau-Umgebung verfügbar gemacht. Sie wird Anfang November 2017 in der Produktionsumgebung bereitgestellt.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktion kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen in Version 2017.3 finden Sie unter  [Übersicht über die Versionsaktivität 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

Die Beta 1-Version 2017.3 enthält Verbesserungen sowohl für Workfront-Administratoren als auch für andere Benutzer:

**Für Administratoren:**

* [Verhindern, dass Aufgaben und Probleme gelöscht werden, wenn Stunden protokolliert werden](#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged)
* [Entfernen der Einstellung „Early Access“ aus dem Setup-Bereich](#removal-of-the-early-access-setting-from-the-setup-area)
* [Standardmäßige Workfront-E-Mail-Adressänderung](#workfront-default-email-address-change)

**Für alle Benutzer:**

* [Verbesserungen bei der Ressourcenplanung](#resource-scheduling-improvements)
* [Breitbild-Display](#widescreen-display)
* [Ändern der Größe und Neuanordnung von Spalten in Berichten und Listen](#resize-and-reorder-columns-in-reports-and-lists)
* [Option „Benutzerdefinierte Daten löschen“ beim Kopieren von Aufgaben und Problemen](#clear-custom-data-option-when-copying-tasks-and-issues)
* [Erstellen eines Projekts direkt aus einer Vorlage](#create-a-project-directly-from-a-template)
* [In-App-Benachrichtigung für abonnierte Objekte](#in-app-notification-for-subscribed-objects)
* [@Tagging Derzeit nicht in der Vorschau-Umgebung verfügbar](#tagging-currently-not-available-in-the-preview-environment)
* [Benutzerzuordnungsinformationen in den Auslastungsbericht für ein Projekt einschließen](#include-user-allocation-information-in-the-utilization-report-on-a-project)

## Verbesserungen bei der Ressourcenplanung {#resource-scheduling-improvements}

>[!NOTE]
>
>Die Tools zur Ressourcenplanung werden nicht mehr unterstützt und mit Version 23.1 aus Workfront entfernt. Informationen zur Planung von Ressourcen mit dem Workload Balancer finden Sie unter [Übersicht über den Workload Balancer](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Die folgenden Verbesserungen bei der Ressourcenplanung sind bei der Planung von Ressourcen für ein Team, für ein Projekt oder für mehrere Projekte als Ressourcenmanager verfügbar:

* [Anzeigen des Planungsbereichs im Vollbildmodus](#view-scheduling-area-in-full-screen-mode)
* [Weitere Datumsbereichsoptionen zum Anzeigen des Bereichs „Ressourcenplanung“](#more-date-range-options-for-viewing-the-resource-scheduling-area)
* [Voraussichtliche Termine in der Zeitleiste anzeigen](#view-projected-dates-on-the-scheduling-timeline)

### Anzeigen des Planungsbereichs im Vollbildmodus {#view-scheduling-area-in-full-screen-mode}

Sie können die Zeitleiste im Vollbildmodus anzeigen, sodass Sie weitere Informationen in einer einzigen Ansicht anzeigen können. 

Weitere Informationen finden Sie unter Erste Schritte mit der Ressourcenplanung .

### Weitere Datumsbereichsoptionen zum Anzeigen des Bereichs „Ressourcenplanung“ {#more-date-range-options-for-viewing-the-resource-scheduling-area}

In der Zeitleiste für die Planung können Sie die folgenden zusätzlichen Datumsbereichsoptionen anzeigen:

* Eintägige Ansicht
* 4-Wochen-Ansicht
* 6-Wochen-Ansicht

Vor dieser Änderung konnten Sie die Zeitplanung nur in einer 1-, 2- oder 3-Wochen-Ansicht anzeigen. Diese Datumsbereiche sind zusätzlich zu den neuen Datumsbereichen weiterhin verfügbar.

Wenn Sie die Zeitleiste für die Planung in einer einzigen Tagesansicht anzeigen, können Benutzerzuweisungen (einschließlich der täglichen Gesamtstunden) nicht angezeigt werden.

Weitere Informationen finden Sie unter Erste Schritte mit der Ressourcenplanung .

### Voraussichtliche Termine in der Zeitleiste anzeigen {#view-projected-dates-on-the-scheduling-timeline}

Jetzt können Sie die Zeitleiste so konfigurieren, dass für Aufgaben und Probleme die voraussichtlichen Termine anstelle der geplanten Termine angezeigt werden. 

Vor dieser Änderung wurden für Aufgaben und Probleme in der Zeitleiste nur geplante Termine angezeigt.

Wenn Sie das voraussichtliche Datum auf der Zeitleiste für die Planung anzeigen, können Benutzerzuweisungen (einschließlich der täglichen Gesamtstunden) nicht angezeigt werden.

Weitere Informationen finden Sie unter Erste Schritte mit der Ressourcenplanung .

## Breitbild-Display {#widescreen-display}

Wenn Sie eines der folgenden Objekte in Workfront anzeigen, wird das gesamte Browserfenster automatisch ausgefüllt:

* Projekte
* Aufgaben
* Probleme
* Berichte
* Dashboards
* Kalender

Vor dieser Änderung gab es zwei weiße Seitenleisten auf beiden Seiten des angezeigten Bereichs. Jetzt passt sich die Breitbildansicht dynamisch an die Breite Ihres Bildschirms und Ihres Browser-Fensters an.

## Ändern der Größe und Neuanordnung von Spalten in Berichten und Listen {#resize-and-reorder-columns-in-reports-and-lists}

Sie können jetzt Spalten in einem Bericht oder einer Liste neu anordnen und ihre Größe ändern, ohne den Bericht bearbeiten zu müssen. (Diese Funktion wurde mit der Einstellung der Early Access-Umgebung Anfang dieses Jahres entfernt. Sie wird jetzt wieder eingeführt.)

Diese Funktion ist nicht für Dashboard-Listen oder Berichte verfügbar, da diese Listen in einer neuen Datenrasterstruktur neu gestaltet wurden. Für alle anderen Listen wird diese Funktion mit dieser Version aktiviert.

Weitere Informationen zum Ändern der Größe und Neuanordnung von Spalten finden Sie unter [Ändern der Spaltenbreite und -reihenfolge](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

## Option „Benutzerdefinierte Daten löschen“ beim Kopieren von Aufgaben und Problemen {#clear-custom-data-option-when-copying-tasks-and-issues}

Beim Kopieren einer Aufgabe oder eines Problems können Sie jetzt eine Option auswählen, um alle benutzerdefinierten Daten zu löschen. Wenn Sie die benutzerdefinierten Daten einer Aufgabe oder eines Problems löschen möchten, wird das Formular in das neue Element kopiert, die benutzerdefinierten Daten im Formular jedoch nicht. Das Löschen benutzerdefinierter Daten wirkt sich auch auf die benutzerdefinierten Formulare aus, die an die Dokumente angehängt sind, die den Elementen angehängt sind, oder auf die benutzerdefinierten Formulare, die an die Ausgaben für die Aufgabe angehängt sind.

Vor dieser Änderung wurden die benutzerdefinierten Daten in einem benutzerdefinierten Formular auch in das neue Element kopiert, wenn Sie die Aufgabe oder das Problem kopiert haben. 

Weitere Informationen zum Kopieren von Aufgaben finden Sie unter [Aufgaben kopieren und duplizieren](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Weitere Informationen zum Kopieren von Problemen finden Sie unter [Probleme kopieren](../../../../manage-work/issues/manage-issues/copy-issues.md).

## Erstellen eines Projekts direkt aus einer Vorlage {#create-a-project-directly-from-a-template}

Sie können jetzt ein Projekt aus einer Vorlage auf Vorlagenebene erstellen.

Vor dieser Änderung konnten Sie ein Projekt über eine Vorlage nur auf der Registerkarte Projekte im Bereich Projekte von Workfront erstellen, indem Sie die Option **Neues Projekt aus Vorlage** verwendeten.

Weitere Informationen zum Erstellen eines Projekts über eine Vorlage finden Sie unter [Erstellen eines Projekts über eine Vorlage](../../../../manage-work/projects/create-projects/create-project-from-template.md).

## Verhindern, dass Aufgaben und Probleme gelöscht werden, wenn Stunden protokolliert werden {#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged}

Sie können Workfront jetzt so konfigurieren, dass das Löschen von Aufgaben und Problemen, für die Stunden protokolliert wurden, zugelassen oder verhindert wird.

Vor dieser Änderung wurden beim Löschen einer Aufgabe oder eines Problems, in dem Stunden protokolliert wurden, je nach Arbeitszeittabelle und Stundeneinstellungen die Stunden entweder mit der Aufgabe oder dem Problem gelöscht oder sie wurden in das Projekt verschoben.

Weitere Informationen zum Löschen von Aufgaben finden Sie unter [Aufgaben löschen](../../../../manage-work/tasks/manage-tasks/delete-tasks.md).

Weitere Informationen zum Löschen von Anfragen finden Sie unter [Probleme löschen](../../../../manage-work/issues/manage-issues/delete-issues.md).

Weitere Informationen zur Aktivierung der Systemeinstellung zum Löschen von Aufgaben und Problemen finden Sie unter [Systemweite Aufgaben- und Problemeinstellungen konfigurieren](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Entfernen der Einstellung „Early Access“ aus dem Setup-Bereich {#removal-of-the-early-access-setting-from-the-setup-area}

Wir entfernen die Einstellung, die es Workfront-Administratoren ermöglicht hat, Benutzer für die Teilnahme an der Early Access-Umgebung zu registrieren. Diese Funktion wird seit Ende 2016 nicht mehr unterstützt. Wir haben 2017 keine neuen Funktionen für Early Access veröffentlicht und alle Funktionen, die in dieser Umgebung verbleiben, wurden in die Produktion verschoben.

Vor dieser Änderung konnten Workfront-Admins weiterhin Benutzende zur Early-Access-Umgebung hinzufügen, obwohl es keine neuen Funktionen gab, auf die zugegriffen werden konnte.

## Standardmäßige Workfront-E-Mail-Adressänderung {#workfront-default-email-address-change}

Die Standard-E-Mail-Adresse für ausgehende Workfront-E-Mails wurde von [noreply@attask.com](mailto:noreply@attask.com) in [noreply@my.workfront.com](mailto:noreply@workfront.com) geändert.

Wenn Sie derzeit E-Mails filtern, die von Workfront gesendet werden, müssen Sie Ihren Filter ändern, damit die neue Standardadresse angezeigt wird. 

Die Änderung der Standardadresse hat keine Auswirkungen auf konfigurierte Workfront-E-Mail-Adressen. 

Weitere Informationen finden Sie unter .

## In-App-Benachrichtigung für abonnierte Objekte {#in-app-notification-for-subscribed-objects}

Wenn ein(e) Benutzende(r) einen Kommentar zu Projekten, Aufgaben und Problemen abgibt, die von Ihnen abonniert wurden, erhalten Sie jetzt eine In-App-Benachrichtigung. Weitere Informationen zu In-App-Benachrichtigungen für Abonnements finden Sie unter [In-App-Benachrichtigungen anzeigen und verwalten](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

Je nach den Funktionen, die Ihr Workfront-Administrator aktiviert hat, können Sie auch E-Mail-Benachrichtigungen für abonnierte Elemente erhalten. Sie können das Abonnement eines Elements einfach über einen Link in einer Abonnement-E-Mail kündigen, wie in [Adobe Workfront-Benachrichtigungen](../../../../workfront-basics/using-notifications/wf-notifications.md) beschrieben.

Vor dieser Änderung haben Sie immer eine E-Mail-Benachrichtigung für abonnierte Elemente erhalten und es gab keine Option, eine In-App-Benachrichtigung zu erhalten.

Sie können zwar Abonnement-E-Mails deaktivieren, aber keine In-App-Benachrichtigungen für abonnierte Elemente. Weitere Informationen finden Sie [Konfigurieren von Ereignisbenachrichtigungen für alle Benutzer im System](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Weitere Informationen zum Abonnieren von Elementen finden Sie unter [Abonnieren von Elementen in Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md).

## @Tagging derzeit nicht in der Vorschau-Umgebung verfügbar {#tagging-currently-not-available-in-the-preview-environment}

Da wir daran arbeiten, die Funktionalität „Rich-Text-Format“ in den Aktualisierungsstrom einzufügen, können Sie das @-Symbol vorübergehend nicht verwenden, um andere Benutzer im Aktualisierungsstrom für die folgenden Objekte in der Vorschau-Umgebung zu taggen:

* Projekt
* Aufgabe
* Problem
* Arbeitszeittabelle

Sie können weiterhin andere taggen, indem Sie auf das Symbol **Andere in dieses Update einschließen** klicken.

Weitere Informationen finden Sie unter [Andere bei Updates taggen](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Benutzerzuordnungsinformationen in den Auslastungsbericht für ein Projekt einschließen {#include-user-allocation-information-in-the-utilization-report-on-a-project}

>[!NOTE]
>
>Die Tools zur Ressourcenplanung werden nicht mehr unterstützt und mit Version 23.1 aus Workfront entfernt. Informationen zur Planung von Ressourcen mit dem Workload Balancer finden Sie unter [Übersicht über den Workload Balancer](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Der Auslastungsbericht für ein Projekt berücksichtigt jetzt, ob die geplanten Stunden während der Dauer einer Aufgabe neu zugewiesen wurden. Wenn die Benutzerzuordnung für Stunden geändert wurde (wie in „Benutzerzuordnungen in den Planungsbereichen verwalten“ beschrieben), können die Daten im Auslastungsbericht beeinflusst werden, wenn die im Auslastungsbericht ausgewählten Datumsangaben nur einen Teil einer Aufgabe enthalten.

Weitere Informationen finden Sie unter [Übersicht über den Bericht zur Ressourcenauslastung](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).
