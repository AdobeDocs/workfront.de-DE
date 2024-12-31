---
title: Verbesserungen für Administratoren im vierten Quartal 2023
description: Verbesserungen für Administratoren im vierten Quartal 2023
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7ed37978-b821-488e-9ca1-b81825255be3
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 0%

---

# Verbesserungen für Administratoren im vierten Quartal 2023

Auf dieser Seite werden alle Admin-Verbesserungen beschrieben, die mit der Version vom vierten Quartal 2023 in der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen wurden mit Version 23.10 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im vierten Quartal 2023 des Versionszyklus verfügbar sind, finden Sie unter [Versionsübersicht für das vierte Quartal 2023](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).

## Korrekturabzugs- und Dokumentenentscheidungen, die für ältere Lizenzmodellkunden verfügbar sind

Legacy-Kunden, die noch nicht zum neuen Adobe Workfront-Lizenzmodell gewechselt sind, können jetzt Daten mit der Anzahl der Korrekturabzugs-/Dokumentenentscheidungen pro Benutzerin bzw. Benutzer und Monat in einem einzigen Bericht sehen. Diese Daten sind verfügbar, wenn Sie einen Bericht zu Benutzerentscheidungen ausführen.

Weitere Informationen finden Sie unter [Objekte in Adobe Workfront verstehen](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) und [Anzahl der Korrekturabzugs- und Dokumentenentscheidungen für alle Benutzer anzeigen](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/view-number-of-decisions-for-users.md).

## Berechnete Felder in benutzerdefinierten Formularen können jetzt den Platzhalter $$USER verwenden

Der `$$USER` Platzhalter ist jetzt in berechneten benutzerdefinierten Feldern und externen Suchfeldern im neuen Formular-Designer verfügbar. Wenn Sie in einer Berechnung auf `$$USER` verweisen, wird die ID des aktuellen Benutzers hinzugefügt. Sie können den Platzhalter auch mit einem anderen Feld verwenden. `$$USER.{name}` würde beispielsweise den Namen des aktuellen Benutzers hinzufügen.

Weitere Informationen zu berechneten Feldern finden Sie unter [Hinzufügen berechneter Felder mit dem Formular-Designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## Hinzufügen von Wertoptionen aus einer externen API zu einem benutzerdefinierten Formular

Ein neuer Feldtyp, **Externe Suche**, ist jetzt im Designer für benutzerdefinierte Formulare verfügbar. Wenn Daten in einem externen System gespeichert sind, können Sie mit diesem Feldtyp Optionen aus einer externen API laden und basierend auf anderen Feldwerten im benutzerdefinierten Formular filtern.

Wenn das Formular zu einem Objekt hinzugefügt wird, erscheinen die von der API zurückgegebenen Werte in einem Dropdown-Feld, und der Benutzer kann einen auswählen.

>[!NOTE]
>
>Der neue Feldtyp **Externe Suche** ist im Legacy-Formular-Builder nicht verfügbar.

Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
