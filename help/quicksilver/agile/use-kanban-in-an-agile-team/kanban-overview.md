---
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: Kanban-Übersicht
description: Lesen Sie diesen Artikel, um besser zu verstehen, wie das Kanban-Board funktioniert.
author: Courtney
feature: Agile
exl-id: d7daa6c1-dae2-4e5c-a765-6a6ebdfaa331
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 1%

---

# Überblick über Kanban

<!-- Audited: 01/2024 -->

Mit den folgenden Abschnitten können Sie die Funktionen des [!UICONTROL Kanban]-Boards besser verstehen.

Eine Beschreibung der K[!UICONTROL anban]-Methodik finden Sie unter [Erstellen eines agilen Teams](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

Wenn Sie an der Migration von einem Agile-Team (Kanban[!UICONTROL -Board ] [!DNL Workfront][!UICONTROL  Boards] interessiert sind, finden Sie weitere Informationen unter [Migrieren eines Agile-Teams [!UICONTROL Kanban]-Cards zu [!DNL Workfront] Boards](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md).

## [!UICONTROL Kanban] Board-Layout und -Funktionen

Das [!UICONTROL Kanban]-Board besteht aus den folgenden Elementen:

**Rückstandsspalte** Zeigt alle Aufgaben an, die sich derzeit im Rückstand befinden. Diese Spalte wird nicht standardmäßig angezeigt. Weitere Informationen zum Rückstand, einschließlich seiner Anzeige auf dem Kanban[!UICONTROL Board, finden Sie ]Verwalten des [-Rückstands](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

**Story-Status**: Gibt an, wie eine Story voranschreitet, je nachdem, in welcher Statusspalte sich die Story befindet.

Weitere Informationen finden Sie unter [Aktualisieren des Status von Storys auf der [!UICONTROL Kanban]-](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md).

Textabschnittsstatus können für das Projekt angepasst werden, indem die agile Ansicht geändert wird, wie im Abschnitt [[!UICONTROL Erstellen oder Anpassen einer agilen Ansicht]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) in [Erstellen oder Bearbeiten von Ansichten in  [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) beschrieben.

>[!NOTE]
>
>Auf dem Kanban-Board werden standardmäßig maximal fünfzig Karten angezeigt. Sie können jedoch auf **[!UICONTROL Mehr anzeigen]** klicken, um weitere Karten anzuzeigen.

## Beziehung zwischen Teilaufgaben und Textabschnitten

Wenn ein Textabschnitt Unteraufgaben enthält, können Sie keine Informationen zum übergeordneten Textabschnitt selbst aktualisieren (z. B. Punkte/Stunden oder Prozent abgeschlossen). Außerdem können Sie die Story nicht über die Kanban-[!UICONTROL  verschieben] um ihren Status zu aktualisieren. Stattdessen werden alle Änderungen, die Sie an den Unteraufgaben der Story vornehmen, in der Story widergespiegelt. Die kombinierten Story-Punkte oder -Stunden für alle Teilaufgaben bestimmen die Punkte oder Stunden der übergeordneten Story.

Wenn beispielsweise eine Story nur eine Teilaufgabe mit 4 Punkten hat, hat die Story selbst auch 4 Punkte. Wenn Sie den Punktwert für die Teilaufgabe in 3 ändern, wird der Punktwert der übergeordneten Story in 3 geändert. Wenn Sie eine weitere Teilaufgabe für dieselbe Story erstellen und den Punktwert für diese Teilaufgabe auf 4 setzen, wird der Punktwert für die Story auf 7 geändert, um den kombinierten Punktwert für beide Teilaufgaben widerzuspiegeln.

Dieselbe Logik gilt für Teilaufgaben der zweiten Ebene (Teilaufgaben von Teilaufgaben). Wenn eine Unteraufgabe eine oder mehrere Unteraufgaben der zweiten Ebene aufweist, wird die Unteraufgabe basierend auf den Unteraufgaben der zweiten Ebene berechnet.

## Unterstützte Funktionen

Bei Verwendung des Kanban-Boards können Sie die folgenden Aktionen ausführen:

* [Hinzufügen einer Unteraufgabe zu einer vorhandenen Story auf dem Board [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [Bestehende Aufgaben oder Probleme zum [!UICONTROL Kanban]-Board hinzufügen](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [Benutzer einer Story auf dem Board [!UICONTROL Kanban] zuweisen](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [Hinzufügen von Storys und Problemen aus dem [!UICONTROL Kanban]-Board](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [Storys oder Probleme aus dem Kanban[!UICONTROL Board ]](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [Bearbeiten von Story-Informationen](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [Nach Benutzer auf der [!UICONTROL Kanban]Pinnwand filtern](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [Verwalten Sie das Limit für laufende Arbeiten (Work In Progress, WIP) auf der [!UICONTROL Kanban] Pinnwand](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [Storys auf dem Kanban[!UICONTROL Board neu ]](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [Status der Storys auf dem Kanban[!UICONTROL Board ] aktualisieren](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [Flags auf Storys auf dem Kanban[!UICONTROL Board ]](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [Fügen Sie den Rückstand zum [!UICONTROL Kanban]-Mainboard hinzu.](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)
