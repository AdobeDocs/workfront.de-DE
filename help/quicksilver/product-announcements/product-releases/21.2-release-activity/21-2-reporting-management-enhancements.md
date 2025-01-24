---
content-type: release-notes
keywords: Hinweise,vierteljährlich,Aktualisierung,Freigabe
navigation-topic: 2021-2-release-activity
title: 21. 2 Verbesserte Berichterstellung
description: Auf dieser Seite werden alle Berichtsverbesserungen beschrieben, die mit Version 21.2 an der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden in der Woche vom 10. Mai 2021 in der Produktionsumgebung verfügbar gemacht. Eine Liste aller mit Version 21.2 verfügbaren Änderungen finden Sie in der Übersicht über die Version 21.2.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1d5f76ef-bea7-4630-8051-454b0d109341
source-git-commit: 158af1f48fba264b98108b5f0a573b7904eb875e
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# 21. 2 Verbesserte Berichterstellung

Auf dieser Seite werden alle Berichtsverbesserungen beschrieben, die mit Version 21.2 an der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden in der Woche vom 10. Mai 2021 in der Produktionsumgebung verfügbar gemacht. Eine Liste aller mit Version 21.2 verfügbaren Änderungen finden Sie unter Übersicht über Version [21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Stundenbearbeitung in Projekten und Berichten einschränken

Um die Bearbeitung von Stunden in Projekt- und Stundenberichten auf der Registerkarte „Stunden“ zu steuern, haben wir eine Einstellung hinzugefügt, mit der Workfront-Admins die Bearbeitung von Stunden auf Stundeneigentümer und Systemadmins beschränken können.

Zuvor konnten Benutzende, deren Zugriffsebene Arbeitszeittabellen und Stunden aktiviert hatte, Stunden bearbeiten.

Weitere Informationen finden Sie unter [Arbeitszeittabelle und Stundenvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Neues Erscheinungsbild für das Feld „Arbeitsaufträge“ in aktualisierten Listen und Berichten

>[!NOTE]
>
>Diese Funktion ist nur in der neuen Adobe Workfront-Version verfügbar.

Um dem modernen Erscheinungsbild anderer Bereiche in der neuen Workfront-Version zu entsprechen, wurde der Stil für das Feld Arbeitsaufträge in aktualisierten Listen und Berichten geändert. Diese Neugestaltung umfasst:

* Ein abgerundeter Avatar für Benutzerprofilbilder, Aufgabengebiete und Teams
* Für Benutzer ohne Profilbilder werden Initialen angezeigt
* Ein neues Aufgabengebiet-Symbol
* Ein neues Personen -Symbol für erweiterte Zuweisungen
* Ein neues Symbol für eingeschränkten Zugriff
* Andere geringfügige Konstruktionsänderungen

Weitere Informationen zu Zuweisungen in Listen finden Sie unter [Aufgaben zuweisen](../../../manage-work/tasks/assign-tasks/assign-tasks.md) oder [Probleme zuweisen](../../../manage-work/issues/manage-issues/assign-issues.md).

![](assets/assignments-updates-350x193.png)

## Neues Erscheinungsbild für Felder mit automatischer Textvervollständigung in aktualisierten Listen und Berichten

>[!NOTE]
>
>Wurde am 20. Mai 2021 vorübergehend aus der Produktionsumgebung entfernt.

>[!NOTE]
>
>Diese Funktion ist nur in der neuen Adobe Workfront-Version verfügbar.

Um dem modernen Erscheinungsbild anderer Bereiche in der neuen Workfront-Version zu entsprechen, wurde der Stil für Felder mit automatischer Textvervollständigung in aktualisierten Listen und Berichten geändert. Zu diesen Änderungen gehören:

* Das Symbol für automatische Textvervollständigung wurde aus dem Feld entfernt.
* Wenn Sie auf ein Feld mit automatischer Textvervollständigung klicken, wird das Menü Vorschläge angezeigt, bevor Sie Text eingeben.
* Das Menü Vorschläge reagiert besser auf die Länge von Werten, und diese Werte werden jetzt am Ende abgeschnitten, wenn die Zeichenbeschränkung erreicht wird, anstatt in der Mitte des Werts.

Informationen zu aktualisierten Listen finden Sie im Abschnitt [Der Unterschied zwischen aktualisierten und alten Listen](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) im Artikel [Erste Schritte mit Listen in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

![](assets/typeahead-updates-350x336.png)

## Bericht zu Systemaktualisierungen

Der neue Journaleintragsbericht bietet eine bessere Überprüfbarkeit, da Sie zu Systemaktualisierungen weitergeleitet werden können, darunter:

* Statusänderungen in einem Projekt, einer Aufgabe oder einem Problem
* Gelöschte Aufgaben oder Probleme
* Werte in benutzerdefinierten Feldern
* Geplante Abschlussdaten
* Änderungen an Projektbesitzer

Sie können diesen Bericht beispielsweise so einrichten, dass die Aktivität rund um ein bestimmtes benutzerdefiniertes Feld angezeigt wird, einschließlich des Projekts für das benutzerdefinierte Feld, wann ein Wert eingegeben wurde, was dieser Wert war, wann das Feld aktualisiert wurde, was der vorherige Wert war, was der neu eingegebene Wert war, welche Benutzer diese Aktionen ausgeführt haben usw.

Zuvor konnten Sie Berichte zu Systemaktualisierungen nur über die Workfront-API erstellen.

Weitere Informationen zu diesem Bericht und dessen Verwendungszwecken finden Sie unter [Bericht über Aktualisierungen mit einem Journaleintragsbericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

