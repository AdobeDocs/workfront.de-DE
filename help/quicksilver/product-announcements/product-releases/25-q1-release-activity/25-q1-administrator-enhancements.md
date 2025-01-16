---
title: Verbesserungen für Administratoren im ersten Quartal 2025
description: Verbesserungen für Administratoren im ersten Quartal 2025
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: fa24040d-0403-4799-b690-c3d172797115
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 0%

---

# Verbesserungen für Administratoren im ersten Quartal 2025

Auf dieser Seite werden alle Admin-Verbesserungen beschrieben, die mit der Version vom ersten Quartal 2025 in der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller zu diesem Zeitpunkt im ersten Quartal 2025 verfügbaren Änderungen finden Sie unter [Versionsübersicht 1. Quartal 2025](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md).

## Geschäftsregeln werden jetzt für mehr Objekte unterstützt

>[!NOTE]
>
>Vorschau-Version: 16. Januar 2025; Produktionsversion für alle Kunden: Mit Version 25.1 (Januar 2025)
>
>_Nur für Organisationen im Ultimate-Plan verfügbar._

Sie können jetzt Geschäftsregeln erstellen und Validierungen auf diese zusätzlichen Objekte anwenden: Firma, Iteration, Sonstige Ressourcenkategorie, Aufgabengebiet, Benutzer, Zuweisung, Ressourcenpool, Ausfallzeit, Dokument und Stunde.

Die folgenden Objekte wurden bereits für Geschäftsregeln unterstützt: Projekt, Aufgabe, Anfrage, Portfolio, Programm, Ausgabe, Rechnungsnachweis, Gruppe, Risiko und Tarifkarte.

Weitere Informationen finden Sie unter [Erstellen und Bearbeiten von Geschäftsregeln](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md).

## Objekte zwischen Umgebungen zur Förderung der Umgebung vergleichen

>[!NOTE]
>
>Vorschau-Version: 6. Januar 2025; Produktionsversion für alle Kunden: Mit Version 25.1 (Januar 2025)

Um die Bestimmung des Objekts, das in einem Umgebungs-Promotion-Paket enthalten sein soll, zu erleichtern, haben wir die Möglichkeit hinzugefügt, Objekte über Umgebungen hinweg zu vergleichen. Jetzt können Sie Objekttypen und Umgebungen auswählen. Workfront generiert eine Liste von Objekten dieses Typs, unabhängig davon, ob sie in der Zielumgebung vorhanden sind und ob dieses Objekt Unterschiede zwischen der Quellumgebung und der Zielumgebung aufweist. Sie können dann Objekte direkt aus dieser Liste zu einem Paket hinzufügen.

Wenn ein(e) Benutzende(r) zuvor Objekte zwischen Umgebungen vergleichen wollte, müssen diese Objekte manuell überprüft werden.

Weitere Informationen finden Sie unter [Objekte zwischen Umgebungen ](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-compare.md).

## Mehr Objekte für die Umgebungsförderung verfügbar

>[!NOTE]
>
>Vorschau-Version: 6. Januar 2025; Produktionsversion für alle Kunden: Mit Version 25.1 (Januar 2025)

Um die Funktionen der Umgebung-Promotion zu erweitern, haben wir weitere Objekte hinzugefügt. Jetzt können Sie die folgenden Objekte zu einem Umgebungs-Promotion-Paket hinzufügen:

* Speicherorte
* Tarifkarten
* Arbeitsaufträge

Zuvor waren diese Objekte nicht für die Umgebungs-Promotion verfügbar.

Weitere Informationen zu Objekten, die für die Umgebungs-Promotion verfügbar sind, finden Sie unter [Unterstützte Objekte für die ](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion)-Promotion“ im Artikel Übersicht über die Umgebungs-Promotion.

## Verschieben von Aufgaben bei protokollierten Stunden verhindern

>[!NOTE]
>
>Vorschau-Version: 19. Dezember 2024; Produktionsversion für alle Kunden: Mit Version 25.1 (16. Januar 2025)

Da das Verschieben von Aufgaben oder Problemen, bei denen Stunden protokolliert wurden, manchmal Probleme mit der Compliance oder der Prüfung verursachen kann, haben wir im Bereich „Setup“ unter „Voreinstellungen für Aufgaben und Probleme“ eine Voreinstellung hinzugefügt, mit der Sie verhindern können, dass Benutzer Aufgaben und Probleme verschieben, wenn Stunden darauf protokolliert wurden. Vor dieser Verbesserung konnten Benutzer Aufgaben und Probleme in andere Projekte verschieben, selbst wenn Stunden daran protokolliert wurden.

Weitere Informationen finden Sie [Konfigurieren von systemweiten Aufgaben- und Problemvoreinstellungen](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Voreinstellung zur Verwendung von Projekt- oder Benutzerzeitplänen für Aufgaben mit einfacher Zuweisung

>[!NOTE]
>
>Vorschau-Version: 21. November 2024; Produktion für die schnelle Veröffentlichung: Mit der Version 24.12 (12. Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (16. Januar 2025)

Als System- oder Gruppenadministrator haben Sie jetzt eine neue Einstellung, um anzugeben, ob Workfront den Zeitplan des Projekts oder des Benutzers verwenden soll, um den Zeitplan des Projekts zu berechnen, wenn Sie einer Aufgabe einen Benutzer zuweisen und sowohl das Projekt als auch der Benutzer einem Zeitplan zugeordnet sind. Vor dieser Verbesserung gab es diese Einstellung für Zuweisungen für mehrere Benutzer. Die Einstellung ist jetzt für Zuweisungen von einzelnen Benutzern zu Aufgaben verfügbar.

Weitere Informationen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Geschäftsregeln unterstützen jetzt Hyperlinks

>[!NOTE]
>
>Vorschau-Version: 21. November 2024; Produktion für die schnelle Veröffentlichung: Mit der Version 24.12 (12. Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (16. Januar 2025)

Sie können jetzt Hyperlinks in die benutzerdefinierte Fehlermeldung einer Geschäftsregel einfügen, um Benutzende dabei zu unterstützen, ihre Aktion innerhalb der Beschränkung der Regel zu ändern. Die statische URL könnte eine Verknüpfung zu Dokumentationen oder anderen Seiten aufweisen, die für den Benutzer hilfreich wären.

Weitere Informationen finden Sie [Erstellen und Bearbeiten von Geschäftsregeln](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md).

## Filtern von Feldern mit nativer automatischer Textvervollständigung ist jetzt verfügbar

>[!NOTE]
>
>Vorschau-Version: 21. November 2024; Produktion für die schnelle Veröffentlichung: Mit der Version 24.12 (12. Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (16. Januar 2025)

Wenn Sie einem benutzerdefinierten Formular einen nativen Feldverweis hinzufügen und es auf ein Feld mit automatischer Textvervollständigung verweist (z. B. Portfolio, Unternehmen oder Inhaber), ist jetzt eine Filteroption verfügbar. Mit dem Filter können Sie die Objekte einschränken, die Benutzerinnen und Benutzer bei der Verwendung des Felds auswählen können. Dieser benutzerdefinierte Filter funktioniert genauso wie ein Filter für ein benutzerdefiniertes Feld mit automatischer Textvervollständigung, wobei der Textmodus zum Definieren des Filters verwendet wird.

Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Symbol „Verschieben nach“ zu benutzerdefinierten Feldern hinzugefügt

>[!NOTE]
>
>Vorschau-Version: 29. Oktober 2024; Produktion für die schnelle Veröffentlichung: Mit der Version 24.11 (14. November 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (16. Januar 2025)

Wenn ein benutzerdefiniertes Formular mehrere Abschnitte mit vielen Feldern enthält, kann es schwierig sein, ein Feld durch Ziehen und Ablegen von einem Abschnitt in einen anderen zu verschieben. Zu jedem Feld wurde das Symbol „Verschieben nach“ hinzugefügt, über das Sie den Bereich auswählen können, in dem das Feld platziert werden soll.

Weitere Informationen finden Sie unter [Organisieren und Vorschau eines Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).
