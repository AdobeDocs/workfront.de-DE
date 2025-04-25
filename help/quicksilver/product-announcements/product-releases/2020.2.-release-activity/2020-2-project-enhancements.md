---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: Projektverbesserungen in 2020.2
description: Auf dieser Seite werden alle mit der Version 2020.2 vorgenommenen Projektverbesserungen in der Produktionsumgebung beschrieben. Diese Verbesserungen wurden in der Woche vom 11. Mai 2020 in der Produktionsumgebung verfügbar gemacht.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 150bc838-d6a5-445a-af77-62c4ed74dd1b
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 0%

---

# Projektverbesserungen in 2020.2

Auf dieser Seite werden alle mit der Version 2020.2 vorgenommenen Projektverbesserungen in der Produktionsumgebung beschrieben. Diese Verbesserungen wurden in der Woche vom 11. Mai 2020 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller mit Version 2020.2 verfügbaren Änderungen finden Sie unter [Übersicht über die Version 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Für Workfront-Admins: Neuer Failsafe, wenn der Projektstatus für neue Projekte ausgeblendet oder entsperrt ist

Im Setup konfigurieren Sie eine Voreinstellung, um sicherzustellen, dass jedes neue Projekt beim Erstellen des Projekts einen bestimmten Status hat. Dies ist wichtig, da ein Projekt immer einen Status benötigt, um in Workfront ordnungsgemäß zu funktionieren, auch wenn das Projekt brandneu ist.

Um sicherzustellen, dass neue Projekte immer einen Status haben, auch wenn ein Administrator den für neue Projekte konfigurierten Status ausblendet oder entsperrt, weist das System jetzt allen neuen Projekten den ersten Status in der Statusliste zu, bis Sie den neuen Status für neue Projekte erneut konfigurieren.

Informationen zum Festlegen der Voreinstellung für den Status aller neuen Projekte finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (oder wenn Sie Adobe Workfront Classic verwenden, finden Sie [Festlegen von Projektvoreinstellungen](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

**In diesen Umgebungen verfügbar:**

* Adobe Workfront Classic
* Das neue Adobe Workfront-Erlebnis

## Für Workfront-Administratoren: Verbessertes Design in den Projektvoreinstellungen

Das Festlegen von Projektvoreinstellungen ist jetzt intuitiver und einfacher zu handhaben:

* Titel sind größer als Optionsbeschriftungen, sodass Sie schneller finden können, wonach Sie suchen.
* Trennlinien und zusätzlicher Leerraum trennen jeden Abschnitt, damit Sie sich leichter auf das konzentrieren können, was Sie tun.
* Wenn Sie eine ungültige Zahl für eine Option wie „Typische Stunden pro Arbeitstag“ eingeben, wird sofort eine Warnmeldung angezeigt, anstatt nach dem Klicken auf Speichern.
* Optionsbeschriftungen entsprechen dem entsprechenden Schnittstellentext an anderer Stelle in Workfront, z. B. im Detailbereich und in Berichten.

Informationen zum Bereich Projektvoreinstellungen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (oder wenn Sie Adobe Workfront Classic verwenden, finden Sie weitere Informationen [Festlegen von Projektvoreinstellungen](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

**In diesen Umgebungen verfügbar:**

* Adobe Workfront Classic
* Das neue Adobe Workfront-Erlebnis

## Ausgewählte Filter, Ansichten und Gruppierungen in Berichtslisten beibehalten

Jetzt wird der letzte auf einen bestimmten Bericht angewendete Filter, die letzte Ansicht oder die letzte Gruppierung ausgewählt, auch wenn sich der/die Benutzende ab- und wieder bei Workfront anmeldet.

Nachdem ein(e) Benutzende(r) einen Filter, eine Ansicht oder eine Gruppierung auf eine Berichtsliste angewendet und dann die Seite verlassen hat, wurde beim nächsten Navigieren zum selben Bericht der Standardfilter, die Standardansicht oder die Standardgruppierung angezeigt.

**In diesen Umgebungen verfügbar:**

* Das neue Adobe Workfront-Erlebnis
* Adobe Workfront Classic

## Beim Verschieben und Kopieren von Aufgaben in ein anderes Projekt bleibt die Aufgabenbeschränkung erhalten, wenn Aufgaben in die Zeitleiste des Projekts passen

Wir haben die Art und Weise verbessert, wie Workfront die datumsspezifische Aufgabenbeschränkung einer Aufgabe handhabt, wenn Sie die Aufgabe kopieren oder in ein anderes Projekt verschieben. Beispiele für datumsspezifische Aufgabenbeschränkungen sind „Muss am“, „Muss am“, „Festes Datum“, „Start nicht später als“ usw.

Wenn Sie z. B. einen Vorgang mit der Einschränkung Muss beginnen am in ein anderes Projekt verschieben oder kopieren, dessen geplantes Startdatum vor dem Startdatum des Vorgangs liegt, behält der Vorgang die Einschränkung bei, nachdem er kopiert oder verschoben wurde. Wenn Sie einen Vorgang mit der Einschränkung Muss beginnen bei in ein Projekt verschieben oder kopieren, dessen geplantes Startdatum nach dem Startdatum des Vorgangs liegt, ändert sich die Aufgabenbeschränkung in So bald wie möglich.

Vor dieser Änderung wird die Aufgabenbeschränkung immer auf „So bald wie möglich“ geändert.

Informationen zum Verschieben von Aufgaben finden Sie unter [Verschieben von Aufgaben](../../../manage-work/tasks/manage-tasks/move-tasks.md) (oder bei Verwendung von Adobe Workfront Classic unter [Verschieben von Aufgaben](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

Informationen zum Kopieren von Aufgaben finden Sie unter [Aufgaben kopieren und duplizieren](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) (bzw. bei Verwendung von Adobe Workfront Classic unter [Aufgaben kopieren und duplizieren](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

Eine Übersicht über alle Aufgabeneinschränkungen finden Sie unter [Übersicht über Aufgabeneinschränkungen](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) (bzw. bei Verwendung von Adobe Workfront Classic unter [Übersicht über Aufgabeneinschränkungen](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

**In diesen Umgebungen verfügbar:**

* Adobe Workfront Classic
* Das neue Adobe Workfront-Erlebnis

## Verhindern von Datenverlust bei Änderungen auf der Registerkarte „Details“ oder in einer Aufgabenliste

Um Datenverluste beim manuellen Speichern von Änderungen auf Projektebene beim Aktualisieren von Informationen auf der Detailseite eines Objekts oder von Aufgaben in einer Aufgabenliste zu vermeiden, wird jetzt eine Warnmeldung angezeigt, die Sie darüber informiert, dass Sie ungespeicherte Änderungen haben, bevor Sie versuchen, Informationen in der Kopfzeile zu bearbeiten. Die einzigen Aktionen, die vor dem Speichern der Änderungen zulässig sind, sind das Abonnieren oder Hinzufügen des -Objekts zu Ihren Favoriten.

Informationen zum Bearbeiten von Aufgaben in einer Liste finden Sie unter [Bearbeiten von Aufgaben in einer Liste](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)

**In diesen Umgebungen verfügbar:**

* Das neue Adobe Workfront-Erlebnis

