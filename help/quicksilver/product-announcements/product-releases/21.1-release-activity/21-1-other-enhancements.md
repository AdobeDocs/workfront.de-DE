---
content-type: release-notes
keywords: Anmerkungen,vierteljährlich,aktualisieren
navigation-topic: product-releases
title: 21.1 Weitere Verbesserungen
description: Auf dieser Seite werden alle anderen Verbesserungen beschrieben, die mit Version 21.1 an der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden in der Woche vom 15. Februar 2021 in der Produktionsumgebung verfügbar gemacht.
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

Auf dieser Seite werden alle anderen Verbesserungen beschrieben, die mit Version 21.1 an der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden in der Woche vom 15. Februar 2021 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller mit Version 21.1 verfügbaren Änderungen finden Sie unter Übersicht über Version [21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Aktualisierungen der Fehleranforderungen für Ereignisabonnements

Die Anforderungen für die Soft-Deaktivierung von Ereignisabonnementfehlern werden aktualisiert. Zusätzlich zu den bestehenden Anforderungen werden Ereignisabonnements jetzt vorläufig deaktiviert, wenn sie nicht innerhalb von 2000 Versuchen einen erfolgreichen Versand erreichen. Damit soll die bestehende 70 %-Regel für Fehlschläge gestärkt werden, die unter bestimmten Bedingungen zu übermäßig vielen Fehlern führen kann.

Darüber hinaus werden ab Februar 2021 auch die Anforderungen für die harte Deaktivierung hinzugefügt.

Weitere Informationen zu den neuen Anforderungen für Soft-Disabled und Hard-Disable finden Sie unter [FAQs - Ereignisabonnements](../../../wf-api/general/event-subs-faq.md).

## Neue Team-Felder für die tägliche Zusammenfassung verfügbar

Wir haben die Felder Team-Genehmigung und Zuweisungen zur E-Mail „Tägliche Auswahl der Aktion erforderlich“ hinzugefügt.

Weitere Informationen finden Sie unter [Benachrichtigungen: Aktion erforderlich](../../../workfront-basics/using-notifications/notifications-action-needed.md).

## POP-E-Mail-Option in Anfrage-Warteschlangen ersetzen

Wir ersetzen die POP-E-Mail-Option für Anfrage-Warteschlangen durch ein neues Workfront-verwaltetes System. Sie können Anfragen weiterhin per E-Mail senden, müssen jedoch stattdessen eine neue von Adobe Workfront verwaltete E-Mail-Adresse im Bereich Anfrage-Warteschlange einrichten.

Diese Änderungen können in der Vorschau getestet werden.

E-Mail wird in allen Vorschauumgebungen automatisch deaktiviert. Informationen zum Aktivieren von E-Mails für Testzwecke finden Sie unter [Aktivieren des E-Mail-Versands aus der Sandbox-Vorschau-Umgebung](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

Weitere Informationen finden Sie unter [Benutzer können ein Problem per E-Mail an ein Anfrage-Warteschlangenprojekt senden](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

Weitere Informationen dazu, warum wir diese Änderung vornehmen, finden Sie unter [Neues verwaltetes Adobe Workfront-System, um POP-E-Mails für Anfrage-Warteschlangen durch 21.1 zu ](../../../product-announcements/announcements/announcement-archive/pop-removal-request-queue.md).

Diese Funktion ist jetzt im Lernpfad [Warteschlangenverwaltung im neuen Workfront-Erlebnis](https://one.workfront.com/s/learningpath4/queue-management-MCYCJRWK36QZBP7PGMNDMSPRN3LE) auf Workfront One enthalten.

## Stundenbearbeitung auf Arbeitszeittabellen beschränken

Um mehr Kontrolle über Arbeitszeittabellen und die Stundenbearbeitung zu erhalten, haben wir eine Einstellung hinzugefügt, mit der Sie die Bearbeitung von Arbeitszeittabellen auf Arbeitszeittabellen-Besitzer und Systemadministratoren beschränken können.

Zuvor konnten Benutzende, bei denen die Option Arbeitszeittabellen und Stunden in ihrer Zugriffsebene aktiviert war, Stunden in jeder Arbeitszeittabelle bearbeiten.

Weitere Informationen finden Sie unter [Arbeitszeittabelle und Stundenvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Verbesserte Filter und Ansichten im Arbeitszeittabellen-Bereich

Wir haben die folgenden Verbesserungen hinzugefügt, wenn Sie ein Projekt, eine Aufgabe oder ein Problem zu einer Arbeitszeittabelle hinzufügen:

* Filter: Wir haben Filter für Projekte und Probleme hinzugefügt. Klicken Sie auf Weitere Optionen , um diese Filter anzuzeigen. Zuvor waren nur für Aufgaben Filter verfügbar.
* Ansichten: Auf der Suchseite wurden Ansicht- und Gruppierungsoptionen hinzugefügt.

Weitere Informationen finden Sie unter [Zeit erfassen](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Überstundenfeld in Arbeitszeittabellen ausblenden

Sie können jetzt das Feld „Überstunden“ ausblenden, um Benutzerverwirrung zu stillen, wenn Sie die Überstunden in Workfront nicht verfolgen. Sie können das Überstundenfeld für eine Arbeitszeittabelle zur einmaligen Verwendung oder im Arbeitszeittabellen-Profil ausblenden:

* Arbeitszeittabelle zur einmaligen Verwendung: Wenn Sie das Feld „Überstunden“ in einer einzelnen Arbeitszeittabelle ausblenden, wird es nur für diese Arbeitszeittabelle ausgeblendet. Weitere Informationen finden Sie [Erstellen einer Arbeitszeittabelle zur einmaligen Verwendung](../../../timesheets/create-and-manage-timesheets/create-tmshts.md).
* Arbeitszeittabellen-Profil: Wenn Sie das Feld „Überstunden“ im Arbeitszeittabellen-Profil ausblenden, wird das Feld „Überstunden“ für alle zukünftigen Arbeitszeittabellen, die für den/die diesem Profil zugewiesenen Benutzer erstellt wurden, nicht angezeigt. Weitere Informationen finden Sie unter [Erstellen, Bearbeiten und Zuweisen von Arbeitszeittabellen-Profilen](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Zuvor konnten Sie das Feld „Überstunden“ auf Arbeitszeittabellen nicht ausblenden.

## Ein- oder Ausblenden von Elementen in der Breadcrumb-Navigation

Um die Anzeige des vollständigen Breadcrumb-Pfads zu vereinfachen, haben wir Funktionen zum Erweitern und Reduzieren hinzugefügt.

Jetzt werden alle abgeschnittenen Elemente vor dem Projekt mit dem Text „more“ gruppiert. „3 More“ zeigt beispielsweise an, dass drei Objekte nicht angezeigt werden.

Zuvor mussten Sie auf die Auslassungszeichen klicken, um abgeschnittene Objekte in einem Dropdown-Menü anzuzeigen.

Um alle Elemente im Breadcrumb anzuzeigen, klicken Sie auf „Mehr“ am Anfang des Breadcrumbs, um die Elemente zu erweitern. Nach dem Erweitern können Sie auf „Weniger“ klicken, um die Elemente erneut auszublenden.

## Neues Erscheinungsbild für die Breadcrumb-Navigation

Damit Benutzende besser erkennen können, wo sie sich in Workfront befinden, und einfacher zwischen Objekten navigieren können, haben wir die folgenden Verbesserungen bei der Breadcrumb-Navigation vorgenommen:

* Jedes Element im Breadcrumb enthält jetzt eine Objektbeschriftung.
* Die aktuelle Seite ist jetzt im Breadcrumb enthalten und wird kursiv angezeigt.
* Für die Breadcrumbs sind jetzt die Tastaturnavigation und die Navigation durch die Sprachausgabe verfügbar.
* Zusätzliche kleinere Stiländerungen

