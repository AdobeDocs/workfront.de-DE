---
content-type: release-notes
navigation-topic: product-releases-archive
title: Beta 1-Release-Aktivität von 2017.3
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Version 2017.3 verfügbar waren. Die Funktionalität auf dieser Seite wurde am 9. August 2017 in der Vorschau-Umgebung bereitgestellt. Sie wird Anfang November 2017 in der Produktionsumgebung zur Verfügung gestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 33a91c25-98ec-4f08-b444-4e11e05e464b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1426'
ht-degree: 0%

---

# Beta 1-Release-Aktivität von 2017.3

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Version 2017.3 verfügbar waren. Die Funktionalität auf dieser Seite wurde am 9. August 2017 in der Vorschau-Umgebung bereitgestellt. Sie wird Anfang November 2017 in der Produktionsumgebung zur Verfügung gestellt.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktionalität kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller 2017.3 vorgenommenen Änderungen finden Sie unter  [Übersicht über die Veröffentlichungsaktivität 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

Die Version 2017.3 von Beta 1 enthält Verbesserungen für Workfront-Administratoren und andere Benutzer:

**Für Administratoren:**

* [Verhindern, dass Aufgaben und Probleme gelöscht werden, wenn Stunden protokolliert werden](#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged)
* [Entfernung der Einstellung &quot;Frühzeitiger Zugriff&quot;aus dem Setup-Bereich](#removal-of-the-early-access-setting-from-the-setup-area)
* [Änderung der Standard-E-Mail-Adresse in Workfront](#workfront-default-email-address-change)

**Für alle Benutzer:**

* [Verbesserungen bei der Ressourcenplanung](#resource-scheduling-improvements)
* [Breitbildanzeige](#widescreen-display)
* [Spaltengröße ändern und in Berichten und Listen neu anordnen](#resize-and-reorder-columns-in-reports-and-lists)
* [Option &quot;Benutzerdefinierte Daten löschen&quot;beim Kopieren von Aufgaben und Problemen](#clear-custom-data-option-when-copying-tasks-and-issues)
* [Erstellen eines Projekts direkt aus einer Vorlage](#create-a-project-directly-from-a-template)
* [ In-App-Benachrichtigung für abonnierte Objekte](#in-app-notification-for-subscribed-objects)
* [@Tagging derzeit nicht in der Vorschauumgebung verfügbar](#tagging-currently-not-available-in-the-preview-environment)
* [Einbeziehen von Informationen zur Benutzerzuordnung in den Nutzungsbericht in ein Projekt](#include-user-allocation-information-in-the-utilization-report-on-a-project)

## Verbesserungen bei der Ressourcenplanung {#resource-scheduling-improvements}

>[!NOTE]
>
>Die Tools für die Ressourcenplanung wurden mit Version 23.1 eingestellt und aus Workfront entfernt. Weitere Informationen zum Planen von Ressourcen mit dem Lastenausgleich finden Sie unter [Übersicht über den Lastenausgleich](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Die folgenden Verbesserungen der Ressourcenplanung sind verfügbar, wenn Sie Ressourcen für ein Team, für ein Projekt oder für mehrere Projekte als Ressourcen-Manager planen:

* [Anzeigen des Planungsbereichs im Vollbildmodus](#view-scheduling-area-in-full-screen-mode)
* [Weitere Datumsbereichsoptionen zum Anzeigen des Zeitplanbereichs für Ressourcen](#more-date-range-options-for-viewing-the-resource-scheduling-area)
* [Anzeigen der prognostizierten Daten in der Timeline für die Planung](#view-projected-dates-on-the-scheduling-timeline)

### Anzeigen des Planungsbereichs im Vollbildmodus {#view-scheduling-area-in-full-screen-mode}

Sie können die Planung im Vollbildmodus anzeigen, um weitere Informationen in einer Ansicht anzuzeigen. 

Weitere Informationen finden Sie unter &quot;Erste Schritte mit der Ressourcenplanung&quot;.

### Weitere Datumsbereichsoptionen zum Anzeigen des Ressourcenzeitplanbereichs {#more-date-range-options-for-viewing-the-resource-scheduling-area}

Sie können die folgenden zusätzlichen Datumsbereichsoptionen anzeigen, wenn Sie die Zeitleistensegment der Planung anzeigen:

* Einzeltagsansicht
* 4-wöchige Ansicht
* 6-wöchige Ansicht

Vor dieser Änderung konnten Sie die Planung nur in einer 1-wöchigen, 2-wöchigen oder 3-wöchigen Ansicht anzeigen. Diese Datumsbereiche sind zusätzlich zu den neuen Datumsbereichen weiterhin verfügbar.

Wenn Sie die Planung in einer eintägigen Ansicht anzeigen, können die Benutzerzuordnungen (einschließlich der täglichen Gesamtstunden) nicht angezeigt werden.

Weitere Informationen finden Sie unter &quot;Erste Schritte mit der Ressourcenplanung&quot;.

### Anzeigen der prognostizierten Daten in der Timeline für die Planung {#view-projected-dates-on-the-scheduling-timeline}

Jetzt können Sie die Planung so konfigurieren, dass anstelle der geplanten Daten für Aufgaben und Probleme die geplanten Daten angezeigt werden. 

Vor dieser Änderung wurden bei Aufgaben und Problemen in der Planung nur die geplanten Daten angezeigt.

Wenn Sie in der Zeitleiste der Planung die geplanten Daten anzeigen, können keine Benutzerzuordnungen (einschließlich der täglichen Gesamtstunden) angezeigt werden.

Weitere Informationen finden Sie unter &quot;Erste Schritte mit der Ressourcenplanung&quot;.

## Breitbildanzeige {#widescreen-display}

Wenn Sie eines der folgenden Objekte in Workfront anzeigen, wird das gesamte Browserfenster automatisch ausgefüllt:

* Projekte
* Aufgaben
* Probleme
* Berichte
* Dashboards
* Kalender

Vor dieser Änderung befanden sich zwei weiße Seitenleisten auf beiden Seiten des angezeigten Bereichs. Die Breitbildansicht passt sich nun dynamisch an die Breite des Bildschirms und des Browser-Fensters an.

## Spaltengröße ändern und in Berichten und Listen neu anordnen {#resize-and-reorder-columns-in-reports-and-lists}

Jetzt können Sie Spalten in einem Bericht oder einer Liste neu anordnen und die Größe ändern, ohne den Bericht bearbeiten zu müssen. (Diese Funktion wurde mit der Einstellung der Umgebung für frühzeitigen Zugriff Anfang dieses Jahres entfernt. Sie wird jetzt wieder eingeführt.)

Diese Funktion steht nicht für Dashboard-Listen oder -Berichte zur Verfügung, da diese Listen in einer neuen Datenrasterstruktur neu gestaltet wurden. Für alle anderen Listen ist diese Funktion in dieser Version aktiviert.

Weitere Informationen zum Ändern der Größe und Neuanordnen von Spalten finden Sie unter [Spaltenbreite und -reihenfolge ändern](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

## Option &quot;Benutzerdefinierte Daten löschen&quot;beim Kopieren von Aufgaben und Problemen {#clear-custom-data-option-when-copying-tasks-and-issues}

Beim Kopieren einer Aufgabe oder eines Problems können Sie jetzt eine Option zum Löschen benutzerdefinierter Daten auswählen. Wenn Sie die benutzerdefinierten Daten einer Aufgabe oder eines Problems löschen möchten, wird das Formular in das neue Element kopiert, die benutzerdefinierten Daten im Formular jedoch nicht. Das Löschen von benutzerdefinierten Daten wirkt sich auch auf die benutzerdefinierten Formulare aus, die an die Dokumente angehängt sind, oder auf die benutzerdefinierten Formulare, die an die Ausgaben für die Aufgabe angehängt sind.

Vor dieser Änderung wurden die benutzerdefinierten Daten, die in einem benutzerdefinierten Formular enthalten waren, auch beim Kopieren der Aufgabe oder des Problems in das neue Element kopiert. 

Weitere Informationen zum Kopieren von Aufgaben finden Sie unter [Aufgaben kopieren und duplizieren](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Weitere Informationen zu Kopierproblemen finden Sie unter [Kopierprobleme](../../../../manage-work/issues/manage-issues/copy-issues.md).

## Erstellen eines Projekts direkt aus einer Vorlage {#create-a-project-directly-from-a-template}

Sie können jetzt ein Projekt aus einer Vorlage auf Vorlagenebene erstellen.

Vor dieser Änderung können Sie ein Projekt aus einer Vorlage nur auf der Registerkarte &quot;Projekte&quot;im Projektbereich von Workfront erstellen, indem Sie die Option **Neues Projekt aus Vorlage** verwenden.

Weitere Informationen zum Erstellen eines Projekts aus einer Vorlage finden Sie unter [Erstellen eines Projekts mit einer Vorlage](../../../../manage-work/projects/create-projects/create-project-from-template.md).

## Verhindern, dass Aufgaben und Probleme gelöscht werden, wenn Stunden protokolliert werden {#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged}

Sie können Workfront jetzt so konfigurieren, dass das Löschen von Aufgaben und Problemen, bei denen Stunden protokolliert wurden, entweder zugelassen oder verhindert wird.

Vor dieser Änderung wurden beim Löschen einer Aufgabe oder eines Problems, bei dem Stunden protokolliert wurden, die Stunden entweder mit der Aufgabe oder dem Problem gelöscht oder entsprechend Ihren Voreinstellungen für das Arbeitsblatt und die Stunden in das Projekt verschoben.

Weitere Informationen zum Löschen von Aufgaben finden Sie unter [Aufgaben löschen](../../../../manage-work/tasks/manage-tasks/delete-tasks.md).

Weitere Informationen zum Löschen von Problemen finden Sie unter [Löschprobleme](../../../../manage-work/issues/manage-issues/delete-issues.md).

Weitere Informationen zum Aktivieren der Systemeinstellung für Aufgaben- und Problemlöschungen finden Sie unter [Systemweite Aufgaben- und Ausgabevoreinstellungen konfigurieren](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Entfernung der Einstellung &quot;Frühzeitiger Zugriff&quot;aus dem Einrichtungsbereich {#removal-of-the-early-access-setting-from-the-setup-area}

Wir entfernen die Einstellung, die es Workfront-Administratoren ermöglichte, Benutzer für die Teilnahme an der Umgebung für frühzeitigen Zugriff zu registrieren. Diese Funktion wird seit Ende 2016 nicht mehr unterstützt. Wir haben 2017 keine neuen Funktionen für Early Access veröffentlicht und alle Funktionen, die in dieser Umgebung noch vorhanden waren, wurden in die Produktion verschoben.

Vor dieser Änderung konnten Workfront-Administratoren Benutzer weiterhin zur Umgebung für frühzeitigen Zugriff hinzufügen, es gab jedoch keine neuen Funktionen für den Zugriff.

## Änderung der Standard-E-Mail-Adresse in Workfront {#workfront-default-email-address-change}

Die Standard-E-Mail-Adresse für ausgehende Workfront-E-Mails wurde von [noreply@attask.com](mailto:noreply@attask.com) in [noreply@my.workfront.com](mailto:noreply@workfront.com) geändert.

Wenn Sie derzeit aus Workfront gesendete E-Mails filtern, müssen Sie Ihren Filter so ändern, dass er die neue Standardadresse widerspiegelt. 

Die Änderung der Standardadresse hat keine Auswirkungen auf konfigurierte Workfront-E-Mail-Adressen. 

Weitere Informationen finden Sie unter .

## In-App-Benachrichtigung für angemeldete Objekte {#in-app-notification-for-subscribed-objects}

Wenn ein Benutzer einen Kommentar zu Projekten, Aufgaben und Problemen abgibt, für die Sie angemeldet sind, erhalten Sie jetzt eine In-App-Benachrichtigung. Weitere Informationen zu In-App-Abonnement-Benachrichtigungen finden Sie unter [Anzeigen und Verwalten von In-App-Benachrichtigungen](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

Je nach den Funktionen, die Ihr Workfront-Administrator aktiviert hat, können Sie auch E-Mail-Benachrichtigungen für abonnierte Elemente erhalten. Sie können sich einfach von einem Artikel über einen Link in einer Anmelde-E-Mail abmelden, wie in [Adobe Workfront-Benachrichtigungen](../../../../workfront-basics/using-notifications/wf-notifications.md) beschrieben.

Vor dieser Änderung haben Sie immer eine E-Mail-Benachrichtigung für abonnierte Artikel erhalten und es gab keine Option, eine In-App-Benachrichtigung zu erhalten.

Sie können zwar die Abonnement-E-Mail deaktivieren, aber In-App-Benachrichtigungen für abonnierte Elemente können nicht deaktiviert werden. Weitere Informationen finden Sie unter [Konfigurieren von Ereignisbenachrichtigungen für alle Benutzer im System](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Weitere Informationen zum Abonnieren von Elementen finden Sie unter [Artikel in Adobe Workfront abonnieren](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md).

## @Tagging derzeit nicht in der Vorschauumgebung verfügbar {#tagging-currently-not-available-in-the-preview-environment}

Wenn wir daran arbeiten, die Funktion &quot;Rich-Text-Format&quot;in den Aktualisierungsstream zu übertragen, können Sie das Symbol &quot;@&quot;vorübergehend nicht verwenden, um andere Benutzer im Aktualisierungsstream für die folgenden Objekte in der Vorschauumgebung zu taggen:

* Projekt
* Aufgabe
* Problem
* Arbeitszeittabelle

Sie können andere weiterhin taggen, indem Sie auf das Symbol **Andere einschließen auf dieses Update** klicken.

Weitere Informationen finden Sie unter [Taggen anderer Benutzer bei Updates](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Einbeziehen von Informationen zur Benutzerzuordnung in den Nutzungsbericht in ein Projekt {#include-user-allocation-information-in-the-utilization-report-on-a-project}

>[!NOTE]
>
>Die Tools für die Ressourcenplanung wurden mit Version 23.1 eingestellt und aus Workfront entfernt. Weitere Informationen zum Planen von Ressourcen mit dem Lastenausgleich finden Sie unter [Übersicht über den Lastenausgleich](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Der Nutzungsbericht zu einem Projekt berücksichtigt nun, ob die geplanten Stunden für die Dauer einer Aufgabe neu zugewiesen wurden. Wenn die Benutzerzuordnung für Stunden geändert wurde (wie unter &quot;Verwalten von Benutzerzuweisungen in den Planungsbereichen&quot;beschrieben), können die Daten im Nutzungsbericht betroffen sein, wenn die im Nutzungsbericht ausgewählten Daten nur einen Teil einer Aufgabe enthalten.

Weitere Informationen finden Sie unter [Überblick über den Bericht &quot;Ressourcenauslastung&quot;](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).
