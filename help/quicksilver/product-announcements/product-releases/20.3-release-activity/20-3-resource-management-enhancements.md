---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 Verbesserungen beim Ressourcenmanagement
description: Auf dieser Seite werden alle Verbesserungen des Ressourcen-Managements beschrieben, die mit der Version 20.3 in der Produktionsumgebung vorgenommen wurden. Diese Verbesserungen wurden in der Woche vom 10. August 2020 in der Produktionsumgebung verfügbar gemacht.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a2c34117-e03c-4394-9b81-7c18433531d1
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 0%

---

# 20.3 Verbesserungen beim Ressourcenmanagement

Auf dieser Seite werden alle Verbesserungen des Ressourcen-Managements beschrieben, die mit der Version 20.3 in der Produktionsumgebung vorgenommen wurden. Diese Verbesserungen wurden in der Woche vom 10. August 2020 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller mit Version 20.3 verfügbaren Änderungen finden Sie unter [20.3 - Versionsübersicht](../../../product-announcements/product-releases/20.3-release-activity/20-3-release-overview.md).

## Stunden aus Problemen in den Bereich Zugewiesene Arbeit des Workload-Balancer einbeziehen

Damit Sie sich ein vollständiges Bild von der Arbeitslast aller Ihrer Mitarbeiter machen können, haben wir eine Einstellung eingeführt, mit der Sie Stunden aus Problemen in den Bereich Zugewiesene Arbeit des Workload-Balancer einbeziehen können.

Weitere Informationen zum Arbeiten mit dem Workload Balancer finden Sie unter [Navigieren im Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Anpassen von Zuweisungen für arbeitsfreie Tage im Workload Balancer

Mit dem Workload-Balancer können Sie Zuweisungen für Ihre Ressourcen für arbeitsfreie Tage anpassen.

Informationen zum Verwalten von Zuweisungen im Workload Balancer finden Sie unter [Verwalten von Benutzerzuweisungen im Workload Balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Im Workload Balancer verfügbare Variablenfilter

Um Ihr Erlebnis zu verbessern und Ihnen mehr Flexibilität beim Austausch von Informationen zu bieten, haben wir jetzt Variablenfilter für den Workload Balancer implementiert. Die folgenden Filter wurden zum Workload-Balancer hinzugefügt:

* „Ich“ (beim Filtern nach Benutzern)
* „Meine Primäre Rolle“ (beim Filtern nach Rollen)
* „Mein Home-Team“ oder „Alle meine Teams“ (beim Filtern nach Teams).

Diese Filter ersetzen die Platzhalterfiltervariablen $$USER.ID, $$USER.roleID, $$USER.homeTeamID und $$USER.teamIDs

Wenn Sie einen dieser Filter anwenden und dann den Workload-Balancer freigeben oder in einem Dashboard platzieren, sehen alle anderen Benutzer ihre eigenen Informationen.

Informationen zum Anwenden von Filtern auf den Workload Balancer finden Sie unter [Filtern von Informationen im Workload Balancer](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Neue Sortierung für Projekte im Workload Balancer

Workload Balancer sortiert die Projekte nun nach dem frühesten geplanten Startdatum und nach dem neuesten geplanten Abschlussdatum der Aufgaben im Projekt, die während des vom Benutzer auf dem Bildschirm angezeigten Zeitraums auftreten. So können Sie die Arbeit in einer hierarchischen Struktur organisieren, sodass Sie die Arbeit für einen Tag leichter identifizieren können.

Weitere Informationen zum Anzeigen von Projekten und Arbeitselementen im Workload Balancer finden Sie unter [Navigieren im Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Anzeigen des tatsächlichen Arbeitsfortschritts im Workload Balancer

Um Ihnen einen genauen Überblick über den Fortschritt Ihrer Arbeitslast zu geben, haben wir im Workload Balancer eine neue Einstellung eingeführt, die den zeitlichen Ablauf von Aufgaben und Problemen entsprechend ihrem voraussichtlichen Datum anzeigt. Sie können die Einstellung Voraussichtliche Termine anzeigen aktivieren, um die voraussichtliche Zeitleiste des Arbeitselements zusätzlich zur geplanten Zeitleiste anzuzeigen.

Mit dieser Verbesserung wird außerdem angezeigt, dass zugewiesene Stunden aus den verbleibenden Tagen durchgestrichen werden, wenn eine Aufgabe oder ein Problem vor dem geplanten Abschlussdatum abgeschlossen wird. Dies bedeutet, dass diese Stunden nicht auf die Gesamtzuweisung des Benutzers angerechnet werden.

Informationen zum Navigieren im Workload Balancer und Aktivieren der Einstellungen finden Sie unter [Navigieren im Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Workload Balancer-Funktionen, die zuvor mit Version 20.2 als veröffentlicht kommuniziert wurden

* [Anpassen der täglichen und wöchentlichen Zuordnung im Workload Balancer](#adjust-daily-and-weekly-allocation-in-the-workload-balancer)
* [Aktualisieren der geplanten Stunden für die Aufgabe im Workload Balancer](#update-task-planned-hours-in-the-workload-balancer)
* [Eine bequemere Methode zur Aktualisierung von Zuweisungen im Workload Balancer](#a-more-convenient-way-to-update-allocations-in-the-workload-balancer)

### Tägliche und wöchentliche Zuordnung im Workload Balancer anpassen {#adjust-daily-and-weekly-allocation-in-the-workload-balancer}

Um ein Burnout Ihrer Ressourcen zu vermeiden, können Sie jetzt die tägliche und wöchentliche Zuordnung Ihrer Benutzer für die Arbeit mit dem Workload Balancer anpassen.

Vor dieser Verbesserung war dies nur mit den Tools für die Ressourcenplanung möglich.

Informationen zum Verwalten von Zuweisungen im Workload Balancer finden Sie unter [Verwalten von Benutzerzuweisungen im Workload Balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

**In diesen Umgebungen verfügbar:**

* Adobe Workfront Classic
* Das neue Adobe Workfront-Erlebnis

### Geplante Stunden für Aufgaben im Workload Balancer aktualisieren {#update-task-planned-hours-in-the-workload-balancer}

>[!NOTE]
>
>Diese Verbesserung wird kurz nach der Veröffentlichung von Version 2020.2 in der Produktion verfügbar sein.

Eine neue Option im Bereich Ressourcen-Management der Zugriffsebene ermöglicht es Benutzenden mit diesem Zugriff jetzt, die geplanten Stunden über den Workload Balancer zu bearbeiten. Wenn Sie Zuweisungen im Workload Balancer anpassen, muss die Gesamtzahl der täglichen Zuweisungen nicht mit der Anzahl der geplanten Stunden der Aufgaben übereinstimmen. Nachdem Sie die Zuteilungen gespeichert haben, wird die Summe der Zuteilungsstunden zu den geplanten Stunden der Aufgabe. Dies ist nur für Aufgaben mit dem Typ Einfache Dauer möglich.

Informationen zum Verwalten von Zuweisungen im Workload Balancer finden Sie unter [Verwalten von Benutzerzuweisungen im Workload Balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Informationen zum Gewähren des Zugriffs auf die Ressourcenverwaltung finden Sie unter [Zugriff auf die Ressourcenverwaltung gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

### Eine bequemere Methode zur Aktualisierung von Zuweisungen im Workload Balancer {#a-more-convenient-way-to-update-allocations-in-the-workload-balancer}

Um die Zuordnung von Benutzenden zu einem Arbeitselement im Workload Balancer zu verwalten, können Sie jetzt auf das Arbeitselement doppelklicken. Sie können auch weiterhin die Menüoption Zuordnungen bearbeiten verwenden. Außerdem müssen Sie die Anzeige von Zuordnungen nicht mehr aktivieren, um sie aktualisieren zu können.

Informationen zum Verwalten von Zuweisungen im Workload Balancer finden Sie unter [Verwalten von Benutzerzuweisungen im Workload Balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).
