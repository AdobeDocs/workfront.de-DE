---
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: Kanban-Übersicht
description: Lesen Sie diesen Artikel, um besser zu verstehen, wie das Kanban-Board funktioniert.
author: Lisa
feature: Agile
exl-id: d7daa6c1-dae2-4e5c-a765-6a6ebdfaa331
source-git-commit: a478e5355db33e076b321a6219442198901f3252
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---

# Kanban-Übersicht

In den folgenden Abschnitten erfahren Sie, wie die [!UICONTROL Kanban] Board-Funktionen:

## [!UICONTROL Kanban] Layout und Funktionen der Pinnwände

Die [!UICONTROL Kanban] Pinnwand besteht aus folgenden Elementen:

**Rückwärtsspalte**: Zeigt alle Aufgaben an, die sich derzeit im Rückstand befinden. Diese Spalte wird nicht standardmäßig angezeigt. Weitere Informationen zum Rückstand, einschließlich der Anzeige im [!UICONTROL Kanban] Pinnwand, siehe [Verwalten des agilen Rückprotokolls](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

**Meldungsstatus**: Gibt an, wie sich eine Geschichte entwickelt, basierend darauf, in welcher Statusspalte sich die Geschichte befindet.

Weitere Informationen finden Sie unter [Status von Meldungen auf der Seite [!UICONTROL Kanban] Pinnwand](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md).

Meldungsstatus können für das Projekt angepasst werden, indem die agile Ansicht geändert wird, wie im Abschnitt beschrieben [[!UICONTROL Erstellen oder Anpassen einer Agile-Ansicht]](../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in [Ansichten - Übersicht in [!DNL Adobe Workfront]](../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

>[!NOTE]
>
>Standardmäßig werden maximal fünfzig Karten auf der Kanban-Pinnwand angezeigt, Sie können aber auf **[!UICONTROL Mehr anzeigen]** um zusätzliche Karten anzuzeigen.

## Beziehung zwischen Unteraufgaben und Meldungen

Wenn eine Geschichte Unteraufgaben enthält, können Sie keine Informationen über die übergeordnete Meldung selbst aktualisieren (z. B. Punkte/Stunden oder Prozentsatz der Vollständigkeit). Außerdem können Sie die Geschichte nicht über die [!UICONTROL Kanban] -Pinnwand, um ihren Status zu aktualisieren. Stattdessen spiegeln sich alle Änderungen, die Sie an den Unteraufgaben der Geschichte vornehmen, in der Geschichte wider. Die kombinierten Story-Punkte oder -Stunden für alle Unteraufgaben bestimmen die Punkte oder Stunden der übergeordneten Story.

Wenn zum Beispiel eine Geschichte nur eine Unteraufgabe an 4 Punkten bewertet hat, hat die Geschichte selbst auch 4 Punkte. Wenn Sie den Wert des Unteraufgabepunkts auf 3 ändern, wird der Punktwert der übergeordneten Meldung auf 3 geändert. Wenn Sie eine weitere Unteraufgabe für denselben Artikel erstellen und den Punktwert für diese Unteraufgabe auf 4 setzen, wird der Punktwert für den Artikel auf 7 geändert, um den kombinierten Punktwert für beide Unteraufgaben widerzuspiegeln.

Dasselbe gilt für Unteraufgaben der zweiten Ebene (Unteraufgaben von Unteraufgaben). Wenn eine Unteraufgabe eine oder mehrere Unteraufgaben der zweiten Ebene enthält, wird die Unteraufgabe anhand der Unteraufgaben der zweiten Ebene berechnet.

## Unterstützte Funktionen

Sie können die folgenden Aktionen ausführen, wenn Sie die Kanban-Pinnwand verwenden:

* [Hinzufügen einer Unteraufgabe zu einem vorhandenen Artikel auf der [!UICONTROL Kanban] Pinnwand](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [Hinzufügen vorhandener Aufgaben oder Probleme zum [!UICONTROL Kanban] Pinnwand](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [Weisen Sie Benutzern einen Artikel zu der [!UICONTROL Kanban] Pinnwand](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [Hinzufügen von Geschichten und Problemen aus dem [!UICONTROL Kanban] Pinnwand](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [Löschen von Meldungen oder Problemen aus dem [!UICONTROL Kanban] Pinnwand](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [Bearbeiten von Storeninformationen](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [Filtern nach Benutzer auf der [!UICONTROL Kanban] Pinnwand](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [Verwalten Sie die Grenze für laufende Arbeiten (WIP) auf der [!UICONTROL Kanban] Pinnwand](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [Ordnen Sie Geschichten zu [!UICONTROL Kanban] Pinnwand](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [Status von Meldungen auf der Seite [!UICONTROL Kanban] Pinnwand](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [Verwenden Sie Flags für Meldungen auf [!UICONTROL Kanban] Pinnwand](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [Fügen Sie dem [!UICONTROL Kanban] Pinnwand](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)
