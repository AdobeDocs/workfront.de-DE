---
title: 21.3 Projektverbesserungen
description: 21.3 Projektverbesserungen
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1df4ccdb-5b74-414c-a622-b0a5ed30a8c4
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1129'
ht-degree: 0%

---

# 21.3 Projektverbesserungen

Auf dieser Seite werden alle mit Version 21.3 vorgenommenen Projektverbesserungen in der Vorschau-Umgebung beschrieben. Diese Verbesserungen wurden in der Woche vom 21. Juli 2021 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller mit Version 21.3 verfügbaren Änderungen finden Sie unter Übersicht über Version [21.3](../../../product-announcements/product-releases/21.3-release-activity/21-3-release-overview.md).

## Zuordnen einer Vorlage zu einer Gruppe

>[!NOTE]
>
>Diese Funktion ist nur in der neuen Adobe Workfront-Version verfügbar.

Um den Prozess der Projekterstellung zu optimieren und Ihnen zu helfen, leichter zu identifizieren und Berichte dazu zu erstellen, welchen Gruppen welche Projektvorlagen gehören, haben wir die Möglichkeit hinzugefügt, einer Projektvorlage eine Gruppe zuzuweisen.

Wenn Sie einer Projektvorlage eine Gruppe zuweisen, werden alle aus der Vorlage erstellten Projekte automatisch mit der Gruppe der Vorlage verknüpft. Weitere Informationen finden Sie unter [Projektvorlagen bearbeiten](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Außerdem können Sie einen Gruppengenehmigungsprozess an eine Vorlage und ihre Vorlagenaufgaben anhängen, wenn die Vorlage mit Ihrer Gruppe verknüpft ist. Weitere Informationen finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit Arbeiten](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Einfachere Bearbeitung von Feldern im Abschnitt Details

>[!NOTE]
>
>Diese Funktion ist nur in der neuen Adobe Workfront-Version verfügbar.

Mit den folgenden Verbesserungen können Sie Informationen im Abschnitt Details eines beliebigen Objekts leichter bearbeiten:

* Ein grauer Umriss um ein Feld, wenn Sie den Mauszeiger darüber bewegen, zeigt an, dass es bearbeitbar ist.
* Sie können Felder bearbeiten, indem Sie einmal darauf klicken.

Vor dieser Verbesserung war nicht klar, welche Felder bearbeitbar waren, und Sie mussten doppelklicken, um ein Feld zu bearbeiten.

## Bei der Berechnung des Übergabedatums sollten projektübergreifende Vorgänger berücksichtigt werden

Mit einer neuen Verbesserung bei der Berechnung von Übergabeterminen für Aufgaben in Adobe Workfront werden nun die projektübergreifenden Abhängigkeiten berücksichtigt.

Zuvor wurden die Übergabedaten nur anhand der Vorgänger der Aufgabe aus demselben Projekt berechnet.

Um sicherzustellen, dass Sie immer über ein genaues Übergabedatum für eine Aufgabe mit einem projektübergreifenden Vorgänger verfügen, müssen Sie jetzt die Zeitleiste des Projekts der Nachfolgeaufgabe neu berechnen. Nach der Neuberechnung der Zeitleiste werden die Übergabedaten der Aufgabe unter Berücksichtigung der projektübergreifenden Abhängigkeiten der Aufgaben berechnet.

Weitere Informationen zu Übergabedaten finden Sie unter [Übersicht über das Übergabedatum einer Aufgabe](../../../manage-work/tasks/task-information/handoff-task-date.md).

## Hinzufügen vorhandener Stories und Probleme aus dem Scrum-Board

>[!NOTE]
>
>Diese Funktion ist nur in der neuen Adobe Workfront-Version verfügbar.

Sie können jetzt eine vorhandene Story oder ein vorhandenes Problem direkt über das Scrum-Board hinzufügen. Dies erleichtert das Hinzufügen vorhandener Stories zu Ihrer aktuellen Iteration, ohne zur Backlog-Seite gehen zu müssen.

Weitere Informationen finden Sie unter [Hinzufügen von Storys und Problemen vom Scrum-Board](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Hinzufügen neuer Stories und Probleme aus dem Scrum-Board

>[!NOTE]
>
>Diese Funktion ist nur in der neuen Adobe Workfront-Version verfügbar.

Sie können jetzt eine neue Story oder ein neues Problem direkt über das Scrum-Board erstellen. Dies erleichtert das schnelle Hinzufügen einer neuen Story zu Ihrer aktuellen Iteration.

Weitere Informationen finden Sie unter [Hinzufügen von Storys und Problemen vom Scrum-Board](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Story oder Problem aus dem Kanban-Board löschen

>[!NOTE]
>
>Diese Funktion ist nur in der neuen Adobe Workfront-Version verfügbar.

Sie können eine Story oder ein Problem jetzt direkt aus Ihrem Kanban-Board löschen, indem Sie auf das Mehr -Symbol auf einer Story oder Problemkarte klicken und Löschen auswählen. Wenn Sie eine Story oder ein Problem löschen, wird diese für 30 Tage in den Papierkorb verschoben und kann nur vom Systemadministrator wiederhergestellt werden.

Weitere Informationen finden Sie unter [Löschen von Storys oder Problemen vom Kanban-Board](../../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md).

## Aktualisierungen der Kopfzeile und des Story Boards von Agile-Karten

>[!NOTE]
>
>Diese Funktion ist nur in der neuen Adobe Workfront-Version verfügbar.

Auf Kanban- und Scrum-Boards sind jetzt die folgenden Verbesserungen verfügbar:

* Die Storykarten und Pinnwand-Spalten haben eine feste Breite, sodass sich die Kartengrößen nicht ändern, wenn Sie die Browser-Fenstergröße anpassen.
* Die Spalte Storys wurde in Übergeordnete Story umbenannt.
* Jede Karte weist oben einen Titel auf, um sie als übergeordnete Story, Unteraufgabe (mit einer übergeordneten Story verknüpft), Story (nicht mit einer übergeordneten Story verknüpft) oder Problem zu identifizieren.
* Die Spalten werden durch Hintergrundschattierungen visuell getrennt.

Weitere Informationen finden Sie unter [Übersicht über Iterationen](../../../agile/use-scrum-in-an-agile-team/iterations/iterations-overview.md).

## Voreinstellungen für Gruppenprojekte, Aufgaben und Probleme

Wie wir bereits kommuniziert haben, haben wir in den Phasen bis zum 24. Juni 2021 Anpassungen auf Gruppenebene für Projekt-, Aufgaben- und Problemeinstellungen eingeführt. Jetzt ist der Rollout abgeschlossen und sie stehen allen Kunden in der Produktionsumgebung zur Verfügung.

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Projektvoreinstellungen für eine Gruppe konfigurieren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
* [Konfigurieren der Voreinstellungen für Aufgaben und Probleme für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

## Zulassen, dass externe Benutzer ein Dokument genehmigen

>[!NOTE]
>
>Diese Funktion ist nur in der neuen Adobe Workfront-Version verfügbar.

Sie können jetzt externe E-Mail-Adressen verwenden, um in der neuen Workfront-Version genehmigende Personen einem Dokument zuzuweisen.

Zuvor konnten Sie in Workfront Classic nur externe Benutzer nach E-Mail-Adresse hinzufügen.

Weitere Informationen finden Sie unter [Dokumentgenehmigungen anfordern](../../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Exportieren von Informationen aus dem Abschnitt Details eines Portfolios oder Programms

>[!NOTE]
>
>Diese Funktion wurde am 20. Mai 2021 in der Vorschau-Umgebung veröffentlicht. Die Version wird am 3. Juni 2021 in der Produktionsumgebung veröffentlicht.

>[!NOTE]
>
>Diese Funktion ist nur in der neuen Adobe Workfront-Version verfügbar.

Sie können jetzt Informationen aus dem Abschnitt Details von Portfolios und Programmen in eine PDF-Datei exportieren. Vor dieser Verbesserung konnten Sie Informationen aus dem Abschnitt Details nur aus Projekten, Aufgaben und Problemen exportieren.

Informationen zum Exportieren von benutzerdefinierten Formularen aus einem Objekt finden Sie unter [Exportieren von benutzerdefinierten Formularen und Objektdetails](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## Zeitstempel für geplantes Abschlussdatum wurde in der Kopfzeile des Objekts hinzugefügt

>[!NOTE]
>
>Diese Funktion ist nur in der neuen Adobe Workfront-Version verfügbar.

Um den einfachen Zugriff, die Benutzerfreundlichkeit und die Genauigkeit zu erleichtern, haben wir die Option hinzugefügt, einen Zeitstempel im geplanten Abschlussdatum der Kopfzeile von Projekten, Aufgaben oder Problemen auszuwählen.

Vor dieser Verbesserung hat Workfront beim Aktualisieren des geplanten Abschlussdatums eines Objekts Mitternacht als Standardzeit ausgewählt. Jetzt können Sie die Zeit sowie das Abschlussdatum anpassen.

Weitere Informationen zu den Objektkopfzeilen in der neuen Workfront-Version finden Sie unter [Neue Objektkopfzeilen](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

## Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt, ohne es zu bearbeiten

>[!NOTE]
>
>Diese Funktion ist nur in der neuen Adobe Workfront-Version verfügbar.

Wir haben das Hinzufügen eines benutzerdefinierten Formulars, das ein anderer Benutzer ausfüllt oder das Sie später ausfüllen werden, zu einem Objekt erleichtert. Das Formular wechselt beim Hinzufügen nicht mehr automatisch in den Bearbeitungsmodus. Sie können das leere Formular einfach im -Objekt speichern.

Wenn Sie ein benutzerdefiniertes Formular zu einem Objekt hinzugefügt haben, wurde die Seite zuvor in den Bearbeitungsmodus versetzt, und Sie mussten alle erforderlichen Felder im Formular ausfüllen, bevor Sie es im -Objekt speichern konnten. Dies war umständlich, wenn das Formular von einem anderen Benutzer ausgefüllt werden sollte oder wenn Sie noch nicht wussten, was Sie in ein Pflichtfeld im Formular einfügen sollten.

Informationen zum Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt finden Sie unter [Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

