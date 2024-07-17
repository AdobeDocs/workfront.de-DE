---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 Verbesserungen bei der Ressourcenverwaltung
description: Auf dieser Seite werden alle Verbesserungen der Ressourcenverwaltung beschrieben, die mit Version 20.3 der Produktionsumgebung vorgenommen wurden. Diese Verbesserungen wurden in der Produktionsumgebung in der Woche vom 10. August 2020 bereitgestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a2c34117-e03c-4394-9b81-7c18433531d1
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 0%

---

# 20.3 Verbesserungen bei der Ressourcenverwaltung

Auf dieser Seite werden alle Verbesserungen der Ressourcenverwaltung beschrieben, die mit Version 20.3 der Produktionsumgebung vorgenommen wurden. Diese Verbesserungen wurden in der Produktionsumgebung in der Woche vom 10. August 2020 bereitgestellt.

Eine Liste aller in Version 20.3 verfügbaren Änderungen finden Sie unter [20.3 - Versionsübersicht](../../../product-announcements/product-releases/20.3-release-activity/20-3-release-overview.md).

## Einbeziehen von Stunden aus Problemen in den Bereich &quot;Zugewiesene Arbeit&quot;des Workload Balancer

Damit Sie ein vollständiges Bild aller Arbeitslasten Ihrer Personen erhalten, haben wir eine Einstellung eingeführt, mit der Sie Stunden aus Problemen im Bereich &quot;Zugewiesene Arbeit&quot;des Arbeitsladerausgleichs einbeziehen können.

Weitere Informationen zum Arbeiten mit dem Lastenausgleich finden Sie unter [Navigieren im Arbeitslastausgleich](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Anpassen der Zuordnungen für Nicht-Arbeitstage im Arbeitslastausgleich

Sie können mithilfe des Workload Balancer die Zuordnungen für Ihre Ressourcen für Nicht-Arbeitstage anpassen.

Informationen zum Verwalten von Zuordnungen im Arbeitslastausgleich finden Sie unter [Verwalten von Benutzerzuordnungen im Arbeitslastausgleich](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Variablenfilter im Lastenausgleich verfügbar

Um Ihr Erlebnis zu verbessern und Ihnen mehr Flexibilität beim Austausch von Informationen zu bieten, haben wir nun Variablenfilter für den Arbeitslastausgleich implementiert. Die folgenden Filter wurden zum Lastenausgleich hinzugefügt:

* &quot;Me&quot;(beim Filtern nach Benutzern)
* &quot;Meine Primäre Rolle&quot;(beim Filtern nach Rollen)
* &quot;My Home Team&quot; oder &quot;All My Teams&quot; (bei der Filterung nach Teams).

Diese Filter ersetzen die Platzhalterfiltervariablen von $$USER.ID, $$USER.roleID, $$USER.homeTeamID und $$USER.teamID.

Wenn Sie einen dieser Filter anwenden und dann den Lastenausgleich freigeben oder ihn in einem Dashboard platzieren, sehen alle anderen Benutzer ihre eigenen Informationen.

Weitere Informationen zum Anwenden von Filtern auf den Arbeitslastausgleich finden Sie unter [Filterinformationen im Arbeitslastausgleich](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Neue Sortierung für Projekte im Arbeitslastausgleich

Der Lastenausgleich sortiert die Projekte jetzt zunächst nach dem frühesten geplanten Startdatum und dann nach dem neuesten geplanten Abschlussdatum der Aufgaben im Projekt, die während des Zeitrahmens auftreten, den der Benutzer auf dem Bildschirm anzeigt. Auf diese Weise können Sie Arbeiten in einer baumähnlichen Hierarchie organisieren, mit der Sie die Arbeit für einen Tag leichter identifizieren können.

Weitere Informationen zum Anzeigen von Projekten und Arbeitselementen im Arbeitslastausgleich finden Sie unter [Navigieren im Arbeitslastausgleich](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Tatsächlichen Arbeitsfortschritt im Arbeitslastausgleich anzeigen

Um Ihnen einen genauen Überblick über den Fortschritt Ihrer Arbeitslast zu geben, haben wir eine neue Einstellung im Arbeitslastausgleich eingeführt, die den Zeitrahmen von Aufgaben und Problemen entsprechend den prognostizierten Daten anzeigt. Sie können die Einstellung Vorgeschlagene Daten anzeigen aktivieren, um die geplante Timeline des Arbeitselements zusätzlich zur geplanten Timeline anzuzeigen.

Mit dieser Verbesserung werden bei einer Aufgabe oder einem Problem, die vor dem geplanten Abschlussdatum abgeschlossen wurde, die zugewiesenen Stunden der verbleibenden Tage durchlaufen, um anzuzeigen, dass sie nicht mit der Gesamtzuordnung des Benutzers angerechnet werden.

Informationen zum Navigieren im Arbeitslastausgleich und Aktivieren von Einstellungen finden Sie unter [Navigieren im Arbeitslastausgleich](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Funktionen des Arbeitslastausgleichs, die zuvor mit Version 20.2 als veröffentlicht kommuniziert wurden

* [Passen Sie die tägliche und wöchentliche Zuordnung im Lastenausgleich an](#adjust-daily-and-weekly-allocation-in-the-workload-balancer)
* [Aktualisieren der geplanten Aufgaben im Arbeitslastausgleich](#update-task-planned-hours-in-the-workload-balancer)
* [Eine einfachere Möglichkeit, die Zuordnungen im Arbeitslastausgleich zu aktualisieren](#a-more-convenient-way-to-update-allocations-in-the-workload-balancer)

### Passen Sie die tägliche und wöchentliche Zuordnung im Lastenausgleich an. {#adjust-daily-and-weekly-allocation-in-the-workload-balancer}

Um das Ausbrechen Ihrer Ressourcen zu vermeiden, können Sie jetzt die tägliche und wöchentliche Zuordnung Ihrer Benutzer mithilfe des Workload Balancer anpassen, um zu funktionieren.

Vor dieser Verbesserung war dies nur mit den Tools für die Ressourcenplanung möglich.

Informationen zum Verwalten von Zuordnungen im Arbeitslastausgleich finden Sie unter [Verwalten von Benutzerzuordnungen im Arbeitslastausgleich](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

**In diesen Umgebungen verfügbar:**

* Adobe Workfront Classic
* Die neue Adobe Workfront-Erfahrung

### Aktualisieren der geplanten Stunden im Arbeitslastausgleich {#update-task-planned-hours-in-the-workload-balancer}

>[!NOTE]
>
>Diese Verbesserung ist in der Produktion bald nach der Version 2020.2 verfügbar.

Eine neue Option im Bereich Ressourcenverwaltung der Zugriffsebene ermöglicht es Benutzern mit diesem Zugriff nun, geplante Stunden über den Lastenausgleich zu bearbeiten. Wenn Sie die Zuordnungen im Arbeitslastausgleich anpassen, muss die Gesamtanzahl der täglichen Zuweisungen nicht mit der Anzahl der geplanten Stunden der Aufgaben übereinstimmen. Nachdem Sie Ihre Zuordnungen gespeichert haben, werden die gesamten Zuordnungszeiten zu den geplanten Stunden der Aufgabe. Dies ist nur bei Aufgaben mit einem einfachen Durationstyp möglich.

Informationen zum Verwalten von Zuordnungen im Arbeitslastausgleich finden Sie unter [Verwalten von Benutzerzuordnungen im Arbeitslastausgleich](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Informationen zur Gewährung des Zugriffs auf die Ressourcenverwaltung finden Sie unter [Gewähren des Zugriffs auf die Ressourcenverwaltung](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

### Eine einfachere Möglichkeit, die Zuordnungen im Arbeitslastausgleich zu aktualisieren {#a-more-convenient-way-to-update-allocations-in-the-workload-balancer}

Um die Zuordnung eines Benutzers zu einem Arbeitselement im Arbeitslastausgleich einfacher zu verwalten, können Sie jetzt auf das Arbeitselement doppelklicken. Sie können auch die vorhandene Menüoption Zuordnung bearbeiten verwenden. Darüber hinaus müssen Sie die Anzeige von Zuordnungen nicht mehr aktivieren, um sie aktualisieren zu können.

Informationen zum Verwalten von Zuordnungen im Arbeitslastausgleich finden Sie unter [Verwalten von Benutzerzuordnungen im Arbeitslastausgleich](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).
