---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2 Projektverbesserungen
description: Auf dieser Seite werden alle Projektverbesserungen beschrieben, die mit Version 2020.2 der Produktionsumgebung vorgenommen wurden. Diese Verbesserungen wurden in der Produktionsumgebung in der Woche vom 11. Mai 2020 bereitgestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 150bc838-d6a5-445a-af77-62c4ed74dd1b
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 0%

---

# 2020.2 Projektverbesserungen

Auf dieser Seite werden alle Projektverbesserungen beschrieben, die mit Version 2020.2 der Produktionsumgebung vorgenommen wurden. Diese Verbesserungen wurden in der Produktionsumgebung in der Woche vom 11. Mai 2020 bereitgestellt.

Eine Liste aller Änderungen, die mit Version 2020.2 verfügbar sind, finden Sie unter [Versionsübersicht 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Für Workfront-Administratoren: Neue Notfallsicherung, wenn der Projektstatus für neue Projekte ausgeblendet oder entsperrt wird

Unter Einrichtung konfigurieren Sie eine Voreinstellung, um sicherzustellen, dass jedes neue Projekt beim Erstellen des Projekts einen bestimmten Status hat. Dies ist wichtig, da ein Projekt immer einen Status benötigt, um in Workfront ordnungsgemäß funktionieren zu können, selbst wenn das Projekt neu ist.

Um sicherzustellen, dass neue Projekte immer einen Status haben, selbst wenn ein Administrator den für neue Projekte konfigurierten Status ausblendet oder entsperrt, weist das System allen neuen Projekten jetzt den ersten Status in der Liste Status zu, bis Sie den neuen Status für neue Projekte erneut konfigurieren.

Weitere Informationen zum Festlegen der Voreinstellung für den Status aller neuen Projekte finden Sie unter [Systemweite Projektanvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (oder, wenn Sie Adobe Workfront Classic verwenden, finden Sie unter [Festlegen von Projektanvoreinstellungen](https://one.workfront.com/s/article/Setting-Project-Preferences-1883392298)).

**In diesen Umgebungen verfügbar:**

* Adobe Workfront Classic
* Die neue Adobe Workfront-Erfahrung

## Für Workfront-Administratoren: Verbessertes Design in den Projekteinstellungen

Die Erfahrung mit dem Festlegen von Projektvoreinstellungen ist jetzt intuitiver und einfacher zu verwenden:

* Titel sind größer als Optionsbeschriftungen, sodass Sie schneller finden können, wonach Sie suchen.
* Trennlinien und zusätzliche Leerräume trennen jeden Abschnitt, damit Sie sich leichter auf Ihre Aufgaben konzentrieren können.
* Wenn Sie eine ungültige Zahl für eine Option wie &quot;Typische Stunden pro Arbeitstag&quot;eingeben, wird sofort eine Warnmeldung angezeigt, anstatt nach dem Klicken auf &quot;Speichern&quot;angezeigt zu werden.
* Optionsbeschriftungen stimmen mit dem entsprechenden Schnittstellentext an anderer Stelle in Workfront überein, z. B. im Detailbereich und in Berichten.

Weitere Informationen zum Bereich &quot;Projektvoreinstellungen&quot;finden Sie unter [Konfigurieren von systemweiten Projektvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (bzw. bei Verwendung von Adobe Workfront Classic finden Sie unter [Festlegen von Projektvoreinstellungen](https://one.workfront.com/s/article/Setting-Project-Preferences-1883392298)).

**In diesen Umgebungen verfügbar:**

* Adobe Workfront Classic
* Die neue Adobe Workfront-Erfahrung

## Ausgewählter Filter, Ansicht und Gruppierung, die in Berichtlisten beibehalten werden

Jetzt wird der letzte Filter, die Ansicht oder die Gruppierung ausgewählt, die auf einen bestimmten Bericht angewendet werden, selbst wenn sich der Benutzer bei Workfront ab- und wieder anmeldet.

Nachdem ein Benutzer zuvor einen Filter, eine Ansicht oder eine Gruppierung auf eine Berichtsliste angewendet und dann von dieser Seite weg navigiert hat, wurde der Standardfilter, die Ansicht oder die Gruppierung angezeigt, wenn der Benutzer das nächste Mal zu diesem Bericht navigierte.

**In diesen Umgebungen verfügbar:**

* Die neue Adobe Workfront-Erfahrung
* Adobe Workfront Classic

## Durch Verschieben und Kopieren von Aufgaben in ein anderes Projekt wird die Aufgabenbegrenzung beibehalten, wenn Aufgaben in die Zeitleiste des Projekts passen.

Die Verarbeitung der datumsspezifischen Aufgabenbegrenzung einer Aufgabe durch Workfront wurde verbessert, wenn Sie die Aufgabe kopieren oder in ein anderes Projekt verschieben. Beispiele für datumsspezifische Aufgabenbeschränkungen sind Muss am , Muss abgeschlossen werden, Feste Datumswerte, Start nicht später als usw.

Wenn Sie beispielsweise eine Aufgabe mit der Einschränkung Must Start On in ein anderes Projekt verschieben oder kopieren, dessen geplantes Startdatum vor dem Startdatum der Aufgabe liegt, behält die Aufgabe die Beschränkung bei, nachdem sie kopiert oder verschoben wurde. Wenn Sie eine Aufgabe mit der Beschränkung Must Start On in ein Projekt verschieben oder kopieren, dessen geplantes Startdatum nach dem Startdatum der Aufgabe liegt, ändert sich die Aufgabenbegrenzung in Sofort wie möglich.

Vor dieser Änderung ändert sich die Aufgabenbegrenzung immer in So bald wie möglich.

Informationen zum Verschieben von Aufgaben finden Sie unter [Verschieben von Aufgaben](../../../manage-work/tasks/manage-tasks/move-tasks.md) (oder bei Verwendung von Adobe Workfront Classic finden Sie unter [Verschieben von Aufgaben](https://one.workfront.com/s/article/Moving-Tasks-2081996259)).

Weitere Informationen zum Kopieren von Aufgaben finden Sie unter [Kopieren und Duplizieren von Aufgaben](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) (bzw. bei Verwendung von Adobe Workfront Classic finden Sie unter [Aufgaben kopieren und duplizieren](https://one.workfront.com/s/article/Copy-and-Duplicate-Tasks-218695605)).

Einen Überblick über alle Aufgabenbeschränkungen finden Sie unter [Übersicht über Aufgabenbegrenzungen](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) (oder wenn Sie Adobe Workfront Classic verwenden, finden Sie unter [Übersicht über Aufgabenbegrenzungen](https://one.workfront.com/s/article/Task-Constraint-Overview-453396848)).

**In diesen Umgebungen verfügbar:**

* Adobe Workfront Classic
* Die neue Adobe Workfront-Erfahrung

## Verhindern von Datenverlust beim Vornehmen von Änderungen auf der Registerkarte Details oder in einer Aufgabenliste

Um beim manuellen Speichern von Änderungen Datenverlust zu vermeiden, wenn Sie Informationen auf der Detailseite eines Objekts oder von Aufgaben in einer Aufgabenliste auf Projektebene aktualisieren, wird jetzt eine Warnmeldung angezeigt, die Sie darüber informiert, dass nicht gespeicherte Änderungen vorliegen, bevor Sie versuchen, Informationen in der Kopfzeile zu bearbeiten. Die einzigen Aktionen, die vor dem Speichern der Änderungen zulässig sind, sind das Abonnieren oder Hinzufügen des Objekts zu Ihren Favoriten.

Informationen zum Bearbeiten von Aufgaben in einer Liste finden Sie unter [Aufgaben in einer Liste bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)

**In diesen Umgebungen verfügbar:**

* Die neue Adobe Workfront-Erfahrung

