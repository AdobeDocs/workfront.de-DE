---
title: Verbesserungen für Administratoren im vierten Quartal 2023
description: Verbesserungen für Administratoren im vierten Quartal 2023
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7ed37978-b821-488e-9ca1-b81825255be3
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# Verbesserungen für Administratoren im vierten Quartal 2023

Auf dieser Seite werden alle Administratorverbesserungen beschrieben, die mit der Version vom 4. Quartal 2023 in der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen wurden mit Version 23.10 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die an dieser Stelle im Versionszyklus des vierten Quartals 2023 verfügbar sind, finden Sie unter [Überblick über das vierte Quartal 2023](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).

## Testversand- und Dokumententscheidungen, die für ältere Lizenzmodellkunden verfügbar sind

Alte Kunden, die noch nicht zum neuen Adobe Workfront-Lizenzmodell übergegangen sind, können jetzt Daten mit der Anzahl der pro Benutzer pro Monat durchgeführten Testversand-/Dokumententscheidungen in einem einzigen Bericht anzeigen. Diese Daten sind verfügbar, wenn Sie einen Bericht Benutzerentscheidungen ausführen.

Weitere Informationen finden Sie unter [Objekte in Adobe Workfront verstehen](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) und [Anzahl der Testsendungen und Dokumententscheidungen für alle Benutzer anzeigen](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/view-number-of-decisions-for-users.md).

## Berechnete Felder in benutzerdefinierten Formularen können jetzt den Platzhalter $$USER verwenden

Der Platzhalter `$$USER` ist jetzt in berechneten benutzerdefinierten Feldern und externen Suchfeldern im neuen Formularentwickler verfügbar. Wenn Sie in einer Berechnung auf `$$USER` verweisen, wird die aktuelle Benutzer-ID hinzugefügt. Sie können den Platzhalter auch mit einem anderen Feld verwenden. Beispielsweise würde `$$USER.{name}` den Namen des aktuellen Benutzers hinzufügen.

Weitere Informationen zu berechneten Feldern finden Sie unter [Berechnete Felder mit dem Formularentwickler hinzufügen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## Hinzufügen von Wertoptionen aus einer externen API zu einem benutzerdefinierten Formular

Der neue Feldtyp **Externe Suche** ist jetzt im benutzerdefinierten Formularentwickler verfügbar. Wenn Daten in einem externen System gespeichert sind, können Sie mit diesem Feldtyp Optionen aus einer externen API laden und basierend auf anderen Feldwerten im benutzerdefinierten Formular filtern.

Wenn das Formular einem Objekt hinzugefügt wird, werden die von der API zurückgegebenen Werte in einem Dropdown-Feld angezeigt und der Benutzer kann einen Wert auswählen.

>[!NOTE]
>
>Der neue Feldtyp **Externe Suche** ist im alten Formular-Builder nicht verfügbar.

Weitere Informationen finden Sie unter [Entwerfen eines Formulars mit dem Formularentwickler](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
