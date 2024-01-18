---
content-type: release-notes
keywords: notes,vierteljährlich,update
navigation-topic: product-releases
title: 21.1 Weitere Verbesserungen
description: Auf dieser Seite werden alle anderen Verbesserungen beschrieben, die mit Version 21.1 der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden in der Produktionsumgebung ab der Woche des 15. Februar 2021 verfügbar sein.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: aa6cfba2-d1df-4d7c-975b-2ae0e63b6d85
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 0%

---

# 21.1 Weitere Verbesserungen

Auf dieser Seite werden alle anderen Verbesserungen beschrieben, die mit Version 21.1 der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden in der Produktionsumgebung ab der Woche des 15. Februar 2021 verfügbar sein.

Eine Liste aller in Version 21.1 verfügbaren Änderungen finden Sie unter [Übersicht über die Version 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Aktualisierungen der Anforderungen an Ereignisabonnements

Wir aktualisieren die Soft-disable-Anforderungen für Fehler bei der Ereignisabonnement-Funktion. Zusätzlich zu den bestehenden Anforderungen wird die Option Ereignisabonnements jetzt deaktiviert, wenn sie innerhalb von 2000 Versuchen keinen erfolgreichen Versand erzielen. Damit soll die bestehende 70-%-Ausfallregel verschärft werden, die unter bestimmten Bedingungen zu übermäßigen Fehlschlägen führen kann.

Darüber hinaus werden wir ab Februar 2021 in den Anforderungen für die Deaktivierung von Daten hinzufügen.

Weitere Informationen zu den neuen Anforderungen für die Deaktivierung und Deaktivierung von Softbounces finden Sie unter [Häufig gestellte Fragen - Ereignisabos](../../../wf-api/general/event-subs-faq.md).

## Neue Teamfelder für den täglichen Digest verfügbar

Wir haben der E-Mail &quot;Action Needed Daily Digest&quot;Teamgenehmigung und Zuweisungsfelder hinzugefügt.

Weitere Informationen finden Sie unter [Benachrichtigungen: Erforderliche Aktion](../../../workfront-basics/using-notifications/notifications-action-needed.md).

## Ersetzen der POP-E-Mail-Option in Anforderungswarteschlangen

Wir ersetzen die POP-E-Mail-Option für Anforderungswarteschlangen durch ein neues Workfront-verwaltetes System. Sie können zwar weiterhin Anfragen per E-Mail senden, müssen aber stattdessen eine neue von Adobe Workfront verwaltete E-Mail-Adresse im Bereich &quot;Anforderungswarteschlange&quot;einrichten.

Diese Änderungen können in der Vorschau getestet werden.

E-Mail wird automatisch in allen Vorschauumgebungen deaktiviert. Informationen zum Aktivieren von E-Mails für Testzwecke finden Sie unter [Aktivieren des Versands von E-Mails aus der Vorschau-Sandbox-Umgebung](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

Weitere Informationen finden Sie unter [Benutzer können ein Problem per E-Mail an ein Anforderungswarteschlangenprojekt senden](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

Weitere Informationen darüber, warum wir diese Änderung vornehmen, finden Sie unter [Neues von Adobe Workfront verwaltetes System zum Ersetzen von POP-E-Mails für Anforderungswarteschlangen durch 21.1](../../../product-announcements/announcements/announcement-archive/pop-removal-request-queue.md).

Diese Funktion ist jetzt im [Warteschlangenverwaltung im neuen Workfront-Erlebnis](https://one.workfront.com/s/learningpath4/queue-management-MCYCJRWK36QZBP7PGMNDMSPRN3LE) Lernpfad auf Workfront One.

## Einschränken der Stundenbearbeitung in Timesheets

Um eine bessere Kontrolle über Timesheets und die Stundenbearbeitung zu ermöglichen, haben wir eine Einstellung hinzugefügt, mit der Sie die Stundenbearbeitung auf Timesheet-Inhaber und Systemadministratoren beschränken können.

Zuvor konnten Benutzer, für die die Option Timesheets &amp; Stunden in ihrer Zugriffsebene aktiviert war, Stunden auf einem beliebigen Zeitblatt bearbeiten.

Weitere Informationen finden Sie unter [Zeitblatt- und Stundenvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Verbesserte Filter und Ansichten im Bereich Timesheets

Beim Hinzufügen eines Projekts, einer Aufgabe oder eines Problems zu einem Timesheet wurden die folgenden Verbesserungen hinzugefügt:

* Filter: Wir haben Filter für Projekte und Probleme hinzugefügt. Klicken Sie auf Mehr Optionen , um diese Filter anzuzeigen. Zuvor waren nur Aufgaben mit Filterung verfügbar.
* Ansichten: Zur Suchseite wurden Ansichts- und Gruppierungsoptionen hinzugefügt.

Weitere Informationen finden Sie unter [Protokollzeit](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Ausblenden des Zeitverlaufsfeldes in Timesheets

Sie können jetzt die Zeitüberschreitungsbox ausblenden, um die Verwirrung der Benutzer zu verringern, wenn Sie Überstunden in Workfront nicht verfolgen. Sie können die Zeitüberschreitungsbox für ein einmalig verwendetes Zeitblatt oder im Timesheet-Profil ausblenden:

* Einmaliges Datenblatt: Wenn Sie die Überstunden-Box in einem einzelnen Zeitblatt ausblenden, wird sie nur für dieses Zeitblatt ausgeblendet. Weitere Informationen finden Sie unter [Erstellen eines Datenblatts für die einmalige Verwendung](../../../timesheets/create-and-manage-timesheets/create-tmshts.md).
* Datenblatt-Profil: Wenn Sie das Feld für die Überstunden im Timesheet-Profil ausblenden, wird für alle zukünftigen Timesheets, die für die diesem Profil zugewiesenen Benutzer erstellt werden, die Überstunden-Komponente nicht angezeigt. Weitere Informationen finden Sie unter [Erstellen, Bearbeiten und Zuweisen von Timesheet-Profilen](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Zuvor war es nicht möglich, die Zeitverlaufsbox auf Zeitleisten auszublenden.

## Erweitern oder Reduzieren von Elementen in der Breadcrumb-Navigation

Um die Anzeige des vollständigen Breadcrumb-Pfads zu vereinfachen, haben wir die Funktion zum Erweitern und Reduzieren hinzugefügt.

Jetzt werden alle abgeschnittenen Elemente vor dem Projekt mit dem Text &quot;mehr&quot;gruppiert. Beispielsweise gibt &quot;3 weitere&quot;an, dass es 3 Objekte gibt, die nicht angezeigt werden.

Zuvor mussten Sie auf die Auslassungspunkte klicken, um abgeschnittene Objekte in einem Dropdown-Menü anzuzeigen.

Um alle Elemente im Breadcrumb anzuzeigen, klicken Sie am Anfang des Breadcrumbs auf &quot;Mehr&quot;, um die Elemente zu erweitern. Nach der Erweiterung können Sie auf &quot;Weniger&quot;klicken, um die Elemente erneut zu reduzieren.

## Neues Erscheinungsbild für die Breadcrumb-Navigation

Damit Benutzer leichter erkennen können, wo sie sich in Workfront befinden, und einfacher zwischen Objekten navigieren können, haben wir die folgenden Verbesserungen an der Breadcrumb-Navigation vorgenommen:

* Jedes Element im Breadcrumb enthält jetzt eine Objektbeschriftung.
* Die aktuelle Seite ist jetzt im Breadcrumb enthalten und kursiv dargestellt.
* Die Tastaturnavigation und die Bildschirmlesehilfen-Navigation sind jetzt für die Breadcrumbs verfügbar.
* Weitere geringfügige Stiländerungen

