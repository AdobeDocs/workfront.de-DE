---
title: Verbesserungen für Administratoren im vierten Quartal 2026
description: Verbesserungen für Administratoren im vierten Quartal 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 1dd8ab20d11b2b4471308ac5402b31e20359a04c
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 1%

---

# Verbesserungen für Administratoren im vierten Quartal 2026

Auf dieser Seite werden Admin-Verbesserungen beschrieben, die mit der Version vom vierten Quartal 2026 in der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im vierten Quartal 2026 des Versionszyklus verfügbar sind, finden Sie unter [Versionsübersicht für das vierte Quartal 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

## Gruppenadministratoren können Geschäftsprofile verwalten

>[!NOTE]
>
>Vorschau: 30. Juli 2026>Produktions-Schnellversion: 13. August 2026>Produktion für alle: 15. Oktober 2026

Gruppenadministratoren können jetzt Geschäftsprofile für die von ihnen verwalteten Gruppen erstellen, bearbeiten und löschen, ohne dass sie Systemadministratorzugriff benötigen. Dadurch erhalten Unternehmen mehr Flexibilität, die Verwaltung von Geschäftsprofilen auf Gruppenebene zu delegieren.

Weitere Informationen finden Sie unter [Geschäftsprofile anzeigen und verwalten](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-business-profiles.md).

## Unterstützung von Layout-Vorlagen für Ansichten in erweiterten Listen

>[!NOTE]
>
>Vorschau: 30. Juli 2026>Produktions-Schnellversion: 13. August 2026>Produktion für alle: 15. Oktober 2026

Ansichten für erweiterte Listen werden jetzt auf Systemebene über eine Layout-Vorlage unterstützt. Sie können vorhandene Systemansichten ausblenden, eine bestimmte Ansicht als Standardansicht zuweisen und eine benutzerdefinierte Ansicht zur Liste der Systemansichten hinzufügen.

Beispiele für erweiterte Listen in der Layout-Vorlage sind **Alle** und **Erweiterte Zuweisungen**. Eine erweiterte Liste enthält die Beschriftung „Neues Erlebnis“ neben den Ansichten.

Weitere Informationen finden Sie [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Massenbearbeitung von externen Suchfeldern

>[!NOTE]
>
>Vorschau: 30. Juli 2026>Produktions-Schnellversion: 13. August 2026>Produktion für alle: 15. Oktober 2026

Dialogfelder für die Massenbearbeitung ermöglichen jetzt die Bearbeitung von externen Suchfeldern. Dies war bisher nicht möglich.

In Situationen, in denen ein Suchfeld von einem anderen Suchfeld abhängig ist, kann das Feld mit der Abhängigkeit nur dann stapelweise bearbeitet werden, wenn das erste Feld für alle Objekte, die bearbeitet werden, identisch ist.

Eine Liste von Ländern hängt beispielsweise von der für eine Region getroffenen Auswahl ab. Wenn bei einem Projekt Asien die Region und bei einem anderen Europa die Region ist und Sie beide Projekte stapelweise bearbeiten, ist das Feld Land nicht verfügbar, da die Regionen nicht übereinstimmen. Wenn die Region für beide Projekte identisch sein soll, können Sie auch ein Land für beide Projekte auswählen.

Informationen zu externen Suchfeldern finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-external-lookup-fields).

## Unterstützte erweiterte Logik in der Vorschau des benutzerdefinierten Formular-Designers

>[!NOTE]
>
>Vorschau: 30. Juli 2026>Produktions-Schnellversion: 13. August 2026>Produktion für alle: 15. Oktober 2026

Der Vorschaumodus des benutzerdefinierten Formular-Designers unterstützt jetzt erweiterte Logikoptionen einschließlich erweiterter Anzeigelogik, Standardwertlogik, Validierungslogik, Formatierungslogik und Bearbeitbarkeitslogik. Sie können die Logikformeln in der Formularvorschau testen und sie im Logik-Builder nach Bedarf anpassen. Sie können auch ein Testobjekt auswählen (Projekt, Aufgabe, Problem usw.), , um eine Vorschau des Formulars mit echten kontextuellen Daten anzuzeigen.

Zuvor wurden im Vorschaumodus nur die grundlegenden Optionen für die Anzeige und zum Überspringen der Logik unterstützt.

Beachten Sie, dass diese Logiktypen nur für Organisationen mit den Workflow-Prime- oder Ultimate-Paketen verfügbar sind: erweiterte Anzeige, Standardwert, bedingte Formatierung und Bearbeitbarkeit.

Weitere Informationen finden Sie unter [Hinzufügen von Logikregeln zu benutzerdefinierten Formularen und Feldern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md) und [Organisieren und Vorschau eines Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).

## Änderungsverfolgung zur einheitlichen Überprüfung und Genehmigung

>[!NOTE]
>
>Vorschau: 30. Juli 2026>Produktions-Schnellversion: 13. August 2026>Produktion für alle: 15. Oktober 2026

Die Seite „Änderungsverlauf“ in Workfront erfasst jetzt Aktivitäten in einheitlichen Prüfungs- und Genehmigungs-Workflows und bietet Admins einen vollständigen Governance-Trail für Prüfungs- und Dokumentenlebenszyklus-Ereignisse.

Genehmigungs-, Staging- und Teilnehmeraktionen werden jetzt verfolgt. Diese Maßnahmen können Folgendes umfassen:

* Treffen einer Genehmigungsentscheidung im Frame.io-Viewer
* Erstellen oder Löschen einer Genehmigung
* Aktualisieren eines Dokuments, z. B. Umbenennen, Verschieben oder Löschen

Jeder Eintrag enthält die getrackten Standardfelder: Datum und Uhrzeit, Vorgang, Benutzername (oder „systemgeneriert„) und Objektname. MCP-Aktivitäten werden erfasst, einschließlich der LLM (wie Claude), die die Aktualisierung vorgenommen hat. Frame.io-Viewer-Kommentare sind nicht enthalten.

Weitere Informationen finden Sie unter [Anzeigen und Verwalten des &#x200B;](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).
