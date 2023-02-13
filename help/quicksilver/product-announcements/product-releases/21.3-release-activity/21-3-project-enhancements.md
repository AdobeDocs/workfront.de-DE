---
title: 21.3 Projektverbesserungen
description: 21.3 Projektverbesserungen
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 1df4ccdb-5b74-414c-a622-b0a5ed30a8c4
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 0%

---

# 21.3 Projektverbesserungen

Auf dieser Seite werden alle Projektverbesserungen beschrieben, die mit Version 21.3 der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen wurden in der Produktionsumgebung in der Woche vom 21. Juli 2021 bereitgestellt.

Eine Liste aller in Version 21.3 verfügbaren Änderungen finden Sie unter [21.3 Versionsübersicht](../../../product-announcements/product-releases/21.3-release-activity/21-3-release-overview.md).

## Verknüpfen einer Vorlage mit einer Gruppe

>[!NOTE]
>
>Diese Funktion ist nur im neuen Adobe Workfront-Erlebnis verfügbar.

Um Ihnen bei der Optimierung des Projekterstellungsprozesses zu helfen und Sie einfacher zu identifizieren und darüber zu berichten, welchen Gruppen welche Projektvorlagen gehören, haben wir die Möglichkeit hinzugefügt, einer Projektvorlage eine Gruppe zuzuweisen.

Wenn Sie einer Projektvorlage eine Gruppe zuweisen, werden alle aus der Vorlage erstellten Projekte automatisch der Gruppe der Vorlage zugeordnet. Weitere Informationen finden Sie unter [Bearbeiten von Projektvorlagen](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Sie können auch einen Gruppengenehmigungsprozess an eine Vorlage und ihre Vorlagenaufgaben anhängen, wenn die Vorlage Ihrer Gruppe zugeordnet ist. Weitere Informationen finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Einfachere Bearbeitung von Feldern im Abschnitt &quot;Details&quot;

>[!NOTE]
>
>Diese Funktion ist nur im neuen Adobe Workfront-Erlebnis verfügbar.

Mit den folgenden Verbesserungen können Sie Informationen im Abschnitt Details eines Objekts einfacher bearbeiten:

* Eine graue Umrisslinie um ein Feld, wenn der Mauszeiger darüber bewegt wird, zeigt an, dass es bearbeitbar ist.
* Sie können Felder durch einmaliges Klicken bearbeiten.

Vor dieser Verbesserung war nicht klar, welche Felder bearbeitbar waren und Sie mussten doppelklicken, um ein Feld zu bearbeiten.

## Bei der Berechnung der Übergabe-Daten sollten Sie projektübergreifende Vorfälle berücksichtigen

Mit einer neuen Verbesserung der Art und Weise, wie Adobe Workfront Übergabedaten für Aufgaben berechnet, werden die projektübergreifenden Abhängigkeiten nun berücksichtigt.

Zuvor wurden die Übergabe-Daten nur anhand der Vorgänger der Aufgabe desselben Projekts berechnet.

Um nun sicherzustellen, dass Sie immer ein genaues Übermittlungsdatum für eine Aufgabe mit einem projektübergreifenden Vorgänger haben, müssen Sie die Zeitleiste des Projekts der Nachfolgeaufgabe neu berechnen. Nach der Neuberechnung der Zeitleiste werden die Übergabedaten der Aufgabe unter Berücksichtigung der projektübergreifenden Abhängigkeiten der Aufgaben berechnet.

Weitere Informationen zu Übergabe-Daten finden Sie unter [Übersicht über das Datum der Aufgabenübergabe](../../../manage-work/tasks/task-information/handoff-task-date.md).

## Hinzufügen vorhandener Meldungen und Probleme aus der Scrum-Pinnwand

>[!NOTE]
>
>Diese Funktion ist nur im neuen Adobe Workfront-Erlebnis verfügbar.

Sie können jetzt eine vorhandene Meldung oder ein Problem direkt über das Scrum-Forum hinzufügen. Dies erleichtert das Hinzufügen vorhandener Meldungen zu Ihrer aktuellen Iteration, ohne zur Backlog-Seite wechseln zu müssen.

Weitere Informationen finden Sie unter [Hinzufügen von Meldungen und Problemen aus der Scrum-Pinnwand](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Hinzufügen neuer Meldungen und Probleme über das Scrum-Forum

>[!NOTE]
>
>Diese Funktion ist nur im neuen Adobe Workfront-Erlebnis verfügbar.

Sie können jetzt eine neue Meldung oder ein neues Problem direkt über das Scrum-Forum erstellen. Dies erleichtert das schnelle Hinzufügen einer neuen Geschichte zu Ihrer aktuellen Iteration.

Weitere Informationen finden Sie unter [Hinzufügen von Meldungen und Problemen aus der Scrum-Pinnwand](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Geschichte oder Ausgabe aus dem Kanban-Board löschen

>[!NOTE]
>
>Diese Funktion ist nur im neuen Adobe Workfront-Erlebnis verfügbar.

Sie können jetzt eine Geschichte oder ein Problem direkt aus Ihrem Kanban-Board löschen, indem Sie auf das Symbol Mehr auf einer Geschichte oder Ausgabekarte klicken und Löschen auswählen. Wenn Sie einen Artikel oder ein Problem löschen, wird er 30 Tage lang in den Papierkorb verschoben und kann nur vom Systemadministrator abgerufen werden.

Weitere Informationen finden Sie unter [Löschen von Geschichten oder Problemen aus dem Kanban-Board](../../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md).

## Aktualisierungen der Kartenkopfzeile und des Storyboards

>[!NOTE]
>
>Diese Funktion ist nur im neuen Adobe Workfront-Erlebnis verfügbar.

Auf Kanban- und Scrum-Pinnwänden sind jetzt die folgenden Verbesserungen verfügbar:

* Die Storykarten und Pinnwände haben eine feste Breite, sodass sich die Kartengrößen nicht ändern, wenn Sie die Größe des Browser-Fensters anpassen.
* Die Spalte &quot;Geschichten&quot;wurde in &quot;Übergeordnete Meldung&quot;umbenannt.
* Oben auf jeder Karte befindet sich eine Beschriftung, mit der sie als übergeordnete Meldung, Unteraufgabe (die mit einer übergeordneten Meldung verknüpft ist), Meldung (die nicht mit einer übergeordneten Meldung verknüpft ist) oder Problem identifiziert werden kann.
* Die Hintergrundschattierung trennt die Spalten visuell.

Weitere Informationen finden Sie unter [Iterationen - Übersicht](../../../agile/use-scrum-in-an-agile-team/iterations/iterations-overview.md).

## Voreinstellungen für Gruppenprojekte, Aufgaben und Probleme

Wie wir bereits zuvor kommuniziert haben, haben wir in Phasen bis zum 24. Juni 2021 Gruppenanpassungen für Projekt-, Aufgaben- und Problempräferenzen eingeführt. Jetzt ist der Rollout abgeschlossen und steht allen Kunden in der Produktion zur Verfügung.

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Konfigurieren von Projektvoreinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
* [Konfigurieren von Aufgaben- und Problemeinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

## Zulassen der Genehmigung eines Dokuments durch externe Benutzer

>[!NOTE]
>
>Diese Funktion ist nur im neuen Adobe Workfront-Erlebnis verfügbar.

Sie können jetzt externe E-Mail-Adressen verwenden, um Genehmiger im neuen Workfront-Erlebnis einem Dokument zuzuweisen.

Zuvor konnten externe Benutzer nur in Workfront Classic nach E-Mail-Adresse hinzugefügt werden.

Weitere Informationen finden Sie unter [Dokumentgenehmigungen anfordern](../../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Exportieren von Informationen aus dem Bereich Details eines Portfolios oder Programms

>[!NOTE]
>
>Diese Funktion wurde am 20. Mai 2021 in der Vorschau-Umgebung veröffentlicht. Es wird am 3. Juni 2021 in der Produktionsumgebung veröffentlicht.

>[!NOTE]
>
>Diese Funktion ist nur im neuen Adobe Workfront-Erlebnis verfügbar.

Sie können jetzt Informationen aus dem Bereich Details der Portfolios und Programme in eine PDF-Datei exportieren. Vor dieser Verbesserung konnten Sie Informationen aus dem Abschnitt Details nur aus Projekten, Aufgaben und Problemen exportieren.

Informationen zum Exportieren benutzerdefinierter Formulare aus einem Objekt finden Sie unter [Exportieren benutzerdefinierter Formulare und Objektdetails](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## Der Zeitstempel für das geplante Abschlussdatum wurde in der Kopfzeile des Objekts hinzugefügt.

>[!NOTE]
>
>Diese Funktion ist nur im neuen Adobe Workfront-Erlebnis verfügbar.

Um den Zugriff, die Einfachheit und die Genauigkeit zu erleichtern, haben wir die Option hinzugefügt, einen Zeitstempel im geplanten Abschlussdatum des Headers von Projekten, Aufgaben oder Problemen auszuwählen.

Vor dieser Verbesserung hat Workfront bei der Aktualisierung des geplanten Abschlussdatums eines Objekts Mitternacht als Standardzeit ausgewählt. Jetzt können Sie die Zeit sowie das Abschlussdatum anpassen.

Informationen zu den Objektüberschriften im neuen Workfront-Erlebnis finden Sie unter [Neue Objektüberschriften](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

## Benutzerdefiniertes Formular zu einem Objekt hinzufügen, ohne es zu bearbeiten

>[!NOTE]
>
>Diese Funktion ist nur im neuen Adobe Workfront-Erlebnis verfügbar.

Wir haben es einfacher gemacht, einem Objekt ein benutzerdefiniertes Formular hinzuzufügen, das jemand anderes ausfüllt oder das Sie später ausfüllen werden. Das Formular wird beim Hinzufügen nicht mehr automatisch in den Bearbeitungsmodus versetzt. Sie können das leere Formular einfach im Objekt speichern.

Wenn Sie zuvor ein benutzerdefiniertes Formular zu einem Objekt hinzugefügt haben, wurde die Seite in den Bearbeitungsmodus versetzt und Sie mussten alle erforderlichen Felder im Formular ausfüllen, bevor Sie es im Objekt speichern konnten. Dies war unpraktisch, wenn das Formular von einem anderen Benutzer ausgefüllt werden sollte oder Sie noch nicht wussten, was in ein erforderliches Feld eingegeben werden sollte.

Informationen zum Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt finden Sie unter [Benutzerdefiniertes Formular zu einem Objekt hinzufügen](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

