---
content-type: release-notes
keywords: notes,vierteljährlich,update
navigation-topic: product-releases
title: 21.1 Verbesserungen beim Projekt-Management
description: Auf dieser Seite werden alle Verbesserungen des Projekt-Managements beschrieben, die mit Version 21.1 der Vorschaufunktion vorgenommen wurden. Diese Verbesserungen werden in der Produktionsumgebung ab der Woche des 15. Februar 2021 verfügbar sein.
author: Luke
feature: Product Announcements
exl-id: 95e75a28-5ac2-4d1d-acc3-dbc0b295b28f
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '972'
ht-degree: 1%

---

# 21.1 Verbesserungen beim Projekt-Management

Auf dieser Seite werden alle Verbesserungen des Projekt-Managements beschrieben, die mit Version 21.1 der Vorschaufunktion vorgenommen wurden. Diese Verbesserungen werden in der Produktionsumgebung ab der Woche des 15. Februar 2021 verfügbar sein.

Eine Liste aller in Version 21.1 verfügbaren Änderungen finden Sie unter [Übersicht über die Version 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Export ist jetzt im Abschnitt Metriken eines Projekts verfügbar

Um den Status und Fortschritt eines Projekts einfacher freizugeben, können Sie jetzt das gesamte Dashboard im Abschnitt &quot;Metriken&quot;eines Projekts in eine PNG-Datei exportieren.

Weitere Informationen finden Sie unter [Übersicht über Projektmetriken](../../../manage-work/projects/manage-projects/project-metrics.md).

Diese Funktion ist jetzt im [Planen der Grundlagen für das neue Workfront-Erlebnis, Teil 3: Projekt verwalten](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-MCG6OJL724XRBLHBXEAKGAUZOJ6U) Lernpfad auf Workfront One.

## Aktualisierung des Prozentsatzes des Problems, das abgeschlossen ist, wenn das Projekt oder die Aufgabe aus der Problemaktualisierung konvertiert wurde

Wir haben die Funktionsweise des Prozentsatzes der Fehlerbehebung bei Problemen aktualisiert, die in Projekte oder Aufgaben konvertiert wurden. Wenn mit der neuen Funktion ein Problem in eine Aufgabe oder ein Projekt konvertiert wird, wird der Prozentsatz der Fertigstellung des Problems synchron mit dem Prozentsatz der Fertigstellung der aufgelösten Aufgabe oder des aufgelösten Projekts aktualisiert, wenn die Einstellung &quot;Automatisch Update Behebbarer Probleme bei Änderung des Status der aufgelösten Objektänderungen&quot;bei der Einrichtung aktiviert ist.

Informationen zu Konvertierungsproblemen finden Sie unter [Übersicht über das Auflösen und Auflösen von Objekten](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## Neue Liste gesendeter Anforderungen

Damit Sie Ihre gesendeten Anfragen einfacher und konsistenter verwalten können, haben wir die Abschnitte Gesendete Anfragen und Alle Anforderungen im Bereich Anforderungen entfernt und durch eine neue Liste ersetzt. Die Liste hat ein bekanntes Erscheinungsbild, das mit allen anderen Listen im System übereinstimmt, sodass Sie nach verschiedenen Kategorien gesendeter Anforderungen filtern und schnell nach einer Anforderung suchen können, die möglicherweise schwierig zu finden ist.

Informationen zum Auffinden gesendeter Anfragen finden Sie unter [Gesendete Anforderungen suchen](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

Diese Funktion ist jetzt im [Grundlagen für Mitwirkende am neuen Workfront-Erlebnis](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) Lernpfad auf Workfront One.

Diese Funktion ist jetzt im [Anforderungen im neuen Workfront-Erlebnis](https://one.workfront.com/s/learningpath3/core-team-requests-in-the-new-workfront-experience-MCHWSSDWRFC5EKXFBXTQ6MJNKE7E) Lernpfad auf Workfront One.

## Aus der Seite &quot;Neue Anforderung&quot;entfernte Felder

>[!NOTE]
>
>Aus Version entfernt.

Im Rahmen der Neugestaltung der Seite &quot;Neue Anforderung&quot;haben wir die Felder für neue Probleme aktualisiert, die im Abschnitt &quot;Warteschlangeneinrichtung&quot;eines Projekts eingerichtet wurden.

Die folgenden Felder für neue Probleme werden nur angezeigt, wenn ein Problem im Abschnitt Probleme des Projekts erstellt wird. Sie werden beim Senden eines Problems mit einer Anforderungswarteschlange im Anforderungsbereich nicht angezeigt:

* Schweregrad
* Geplante Stunden
* Geplantes Startdatum
* URL
* Zugewiesen an
* Aufgabengebiet
* Team

Wir haben die Felder &quot;Zugeordnet an&quot;, &quot;Auftragsrolle&quot;und &quot;Team&quot;durch das neue Feld &quot;Zuweisungen&quot;auf der Seite &quot;Neue Anforderung&quot;ersetzt, um effizient einen Benutzer, eine Jobrolle oder ein Team in einem gemeinsamen Feld festzulegen, während Sie eine neue Anforderung senden.

Informationen zum Definieren neuer Problemfelder für ein Projekt finden Sie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Neues Erlebnis beim Senden von Anforderungen im Bereich &quot;Anforderungen&quot;

>[!NOTE]
>
>Aus der Veröffentlichung entfernt; wird in der Vorschau verbleiben und mit Version 21.2 für die Produktion freigegeben.

Um die Konsistenz mit dem neuen Workfront-Erlebnis zu gewährleisten und die Effizienz beim Senden von Anforderungen zu steigern, haben wir das Feld &quot;Neue Anforderung&quot;im Bereich &quot;Anforderungen&quot;neu gestaltet. Im Folgenden finden Sie einige Verbesserungen:

* Eine konsistente Benutzeroberfläche mit dem Rest des neuen Workfront-Erlebnisses
* Der Bereich &quot;Neue Anforderungen&quot;wurde für ein einfacheres und intuitiveres Erlebnis entfernt.
* Eine neue, effizientere Methode zum Anhängen von Dokumenten an Ihre Anforderungen

Möglichkeit, einen Link zur Anforderungswarteschlange, Themengruppe oder Warteschlangenthema freizugeben, während Sie die Anforderung eingeben.

Informationen zum Senden von Anfragen finden Sie unter [Erstellen und Senden von Workfront-Anforderungen](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## Link in eine Anforderungswarteschlange freigeben, wenn eine Anforderung gesendet wird

>[!NOTE]
>
>Aus der Veröffentlichung entfernt; wird in der Vorschau verbleiben und mit Version 21.2 für die Produktion freigegeben.

Jetzt ist es möglich, einen Link zu einer Anforderungswarteschlange, einer Themengruppe oder einem Warteschlangenthema freizugeben.

Bevor Sie eine neue Anforderung senden, können Sie einen Link in die Anforderungswarteschlange, die Themengruppe oder das Warteschlangenthema der Anforderung kopieren und für andere Benutzer freigeben oder in ein Dashboard einbetten.

Informationen zum Teilen eines Links zu einer Anforderungswarteschlange beim Senden einer Anforderung finden Sie unter [Link in eine Anforderungswarteschlange freigeben](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## Suchen Sie nach einer Gruppe, die Sie einem Projekt zuweisen möchten, und zeigen Sie deren Details an.

Es ist jetzt einfacher sicherzustellen, dass Sie die richtige Gruppe identifizieren, wenn Sie einem Projekt eine Gruppe zuweisen. Bewegen Sie den Mauszeiger über den Namen einer Gruppe, die Sie im Feld Gruppe finden, und klicken Sie dann auf das Informationssymbol, das neben dem Namen angezeigt wird, um die QuickInfo Gruppendetails anzuzeigen.

Diese QuickInfo enthält die Hierarchie der Gruppen über der Gruppe (falls vorhanden) und die Administratoren der Gruppe.

Je nach den für die Gruppe konfigurierten Details können Sie auch den Business Leader und die Beschreibung der Gruppe sehen.

Mit diesen Informationen können Sie sicher sein, dass Sie die richtige Gruppe auswählen, die Sie dem Projekt zuweisen möchten.

Weitere Informationen finden Sie unter [Informationen im Bereich &quot;Projektübersicht&quot;verwalten](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

## Bericht zur neuen Benutzerdelegation

Bisher konnten Informationen zu Aufgaben, Themen und Projektgenehmigungen nur vom Delegierten in seinem Heimatbereich eingesehen werden. Damit andere Benutzer diese Informationen sehen können, können Benutzer planen jetzt den Bericht Benutzerdelegation erstellen, in dem Folgendes angegeben wird:

* Wer hat diese Genehmigungen an einen anderen Benutzer delegiert
* Welcher Benutzer wurde diese Genehmigungen zugewiesen?
* Beginn und Ende dieser Delegationen

Weitere Informationen finden Sie unter [Erstellen eines Berichts zur Benutzerdelegation](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md).
