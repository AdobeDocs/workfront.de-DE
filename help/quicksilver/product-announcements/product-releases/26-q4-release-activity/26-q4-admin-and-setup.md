---
title: Verbesserungen für Administratoren im vierten Quartal 2026
description: Verbesserungen für Administratoren im vierten Quartal 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: db296d9043cb793e1af74bca38197de682f54cb8
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 1%

---

# Verbesserungen für Administratoren im vierten Quartal 2026

Auf dieser Seite werden Admin-Verbesserungen beschrieben, die mit der Version vom vierten Quartal 2026 in der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im vierten Quartal 2026 des Versionszyklus verfügbar sind, finden Sie unter [Versionsübersicht für das vierte Quartal 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

<!--

## Interface improvements to the Actions list

>[!NOTE]
>
>Preview: August 20, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

The Actions list in the Update Feeds section of the Setup area has an updated look and feel.

The following enhancements are included:

* We removed the Save and Cancel buttons.
* The Track column now appears in the last position.
* We removed the confirmation message that previously displayed when you saved changes in this area.

For information, see [Configure system updates](/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

-->

## Gruppenadministratoren können Geschäftsprofile verwalten

>[!NOTE]
>
>Vorschau: 30. Juli 2026
>Produktions-Schnellveröffentlichung: 13. August 2026
>Produktion für alle: 15. Oktober 2026

Gruppenadministratoren können jetzt Geschäftsprofile für die von ihnen verwalteten Gruppen erstellen, bearbeiten und löschen, ohne dass sie Systemadministratorzugriff benötigen. Dadurch erhalten Unternehmen mehr Flexibilität, die Verwaltung von Geschäftsprofilen auf Gruppenebene zu delegieren.

Weitere Informationen finden Sie unter [Geschäftsprofile anzeigen und verwalten](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-business-profiles.md).

## Unterstützung von Layout-Vorlagen für Ansichten in erweiterten Listen

>[!NOTE]
>
>Vorschau: 30. Juli 2026
>Produktions-Schnellveröffentlichung: 13. August 2026
>Produktion für alle: 15. Oktober 2026

Ansichten für erweiterte Listen werden jetzt auf Systemebene über eine Layout-Vorlage unterstützt. Sie können vorhandene Systemansichten ausblenden, eine bestimmte Ansicht als Standardansicht zuweisen und eine benutzerdefinierte Ansicht zur Liste der Systemansichten hinzufügen.

Beispiele für erweiterte Listen in der Layout-Vorlage sind **Alle** und **Erweiterte Zuweisungen**. Eine erweiterte Liste enthält die Beschriftung „Neues Erlebnis“ neben den Ansichten.

Weitere Informationen finden Sie [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Massenbearbeitung von externen Suchfeldern

>[!NOTE]
>
>Vorschau: 30. Juli 2026
>Produktions-Schnellveröffentlichung: 13. August 2026
>Produktion für alle: 15. Oktober 2026

Dialogfelder für die Massenbearbeitung ermöglichen jetzt die Bearbeitung von externen Suchfeldern. Dies war bisher nicht möglich.

In Situationen, in denen ein Suchfeld von einem anderen Suchfeld abhängig ist, kann das Feld mit der Abhängigkeit nur dann stapelweise bearbeitet werden, wenn das erste Feld für alle Objekte, die bearbeitet werden, identisch ist.

Eine Liste von Ländern hängt beispielsweise von der für eine Region getroffenen Auswahl ab. Wenn bei einem Projekt Asien die Region und bei einem anderen Europa die Region ist und Sie beide Projekte stapelweise bearbeiten, ist das Feld Land nicht verfügbar, da die Regionen nicht übereinstimmen. Wenn die Region für beide Projekte identisch sein soll, können Sie auch ein Land für beide Projekte auswählen.

Informationen zu externen Suchfeldern finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-external-lookup-fields).

## Unterstützte erweiterte Logik in der Vorschau des benutzerdefinierten Formular-Designers

>[!NOTE]
>
>Vorschau: 30. Juli 2026
>Produktions-Schnellveröffentlichung: 13. August 2026
>Produktion für alle: 15. Oktober 2026

Der Vorschaumodus des benutzerdefinierten Formular-Designers unterstützt jetzt erweiterte Logikoptionen einschließlich erweiterter Anzeigelogik, Standardwertlogik, Validierungslogik, Formatierungslogik und Bearbeitbarkeitslogik. Sie können die Logikformeln in der Formularvorschau testen und sie im Logik-Builder nach Bedarf anpassen. Sie können auch ein Testobjekt auswählen (Projekt, Aufgabe, Problem usw.), , um eine Vorschau des Formulars mit echten kontextuellen Daten anzuzeigen.

Zuvor wurden im Vorschaumodus nur die grundlegenden Optionen für die Anzeige und zum Überspringen der Logik unterstützt.

Beachten Sie, dass diese Logiktypen nur für Organisationen mit den Workflow-Prime- oder Ultimate-Paketen verfügbar sind: erweiterte Anzeige, Standardwert, bedingte Formatierung und Bearbeitbarkeit.

Weitere Informationen finden Sie unter [Hinzufügen von Logikregeln zu benutzerdefinierten Formularen und Feldern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md) und [Organisieren und Vorschau eines Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).

## Änderungsverfolgung zur einheitlichen Überprüfung und Genehmigung

>[!NOTE]
>
>Vorschau: 30. Juli 2026
>Produktions-Schnellveröffentlichung: 13. August 2026
>Produktion für alle: 15. Oktober 2026

Die Seite „Änderungsverlauf“ in Workfront erfasst jetzt Aktivitäten in einheitlichen Prüfungs- und Genehmigungs-Workflows und bietet Admins einen vollständigen Governance-Trail für Prüfungs- und Dokumentenlebenszyklus-Ereignisse.

Genehmigungs-, Staging- und Teilnehmeraktionen werden jetzt verfolgt. Diese Maßnahmen können Folgendes umfassen:

* Treffen einer Genehmigungsentscheidung im Frame.io-Viewer
* Erstellen oder Löschen einer Genehmigung
* Aktualisieren eines Dokuments, z. B. Umbenennen, Verschieben oder Löschen

Jeder Eintrag enthält die getrackten Standardfelder: Datum und Uhrzeit, Vorgang, Benutzername (oder „systemgeneriert„) und Objektname. MCP-Aktivitäten werden erfasst, einschließlich der LLM (wie Claude), die die Aktualisierung vorgenommen hat. Frame.io-Viewer-Kommentare sind nicht enthalten.

Weitere Informationen finden Sie unter [Anzeigen und Verwalten des &#x200B;](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md).

## Definieren eines benutzerdefinierten Programms als Landingpage in der Layout-Vorlage

>[!NOTE]
>
>Vorschau: 30. Juli 2026
>Produktions-Schnellveröffentlichung: 13. August 2026
>Produktion für alle: 15. Oktober 2026

Sie können jetzt ein benutzerdefiniertes Programm als Landingpage in einer Layout-Vorlage festlegen. Benutzerdefinierte Programme, die bereits zum Hauptmenü hinzugefügt wurden, können als Landingpage verwendet werden.

Benutzerdefinierte Programme müssen separat erstellt werden, bevor sie als Hauptmenü- oder Landingpage-Optionen verfügbar werden.

Weitere Informationen finden Sie unter [Anpassen der Landingpage mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md) und [Erstellen benutzerdefinierter Programme für Workfront mit Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

## Konfigurieren von getrackten Feldern im Änderungsverlauf

>[!NOTE]
>
>Vorschau: 30. Juli 2026
>Produktions-Schnellveröffentlichung: 13. August 2026
>Produktion für alle: 15. Oktober 2026

Sie können Felder hinzufügen, die Sie für einen bestimmten Objekttyp in Workfront verfolgen möchten. Wenn Benutzende Informationen in diesem Feld ändern, zeichnet das System Informationen über die Änderung als Eintrag im Änderungsverlauf auf.

Zuvor war der Konfigurationsbildschirm zum Definieren der verfolgten Felder schreibgeschützt.

Weitere Informationen finden Sie unter [Felder zum Nachverfolgen im Änderungsverlauf konfigurieren](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/configure-fields-in-change-history.md).

## Administrativer Zugriff auf den Änderungsverlauf zu Zugriffsebenen hinzugefügt

>[!NOTE]
>
>Vorschau: 30. Juli 2026
>Produktions-Schnellveröffentlichung: 13. August 2026
>Produktion für alle: 15. Oktober 2026

Auf der Zugriffsebene Standard können Sie jetzt festlegen, ob Benutzer mit dieser Zugriffsebene Zugriff auf die Liste „Änderungsverlauf“ haben sollen. Die **Änderungsverlauf** ist im Abschnitt **Administratorzugriff zulassen für** auf der Zugriffsebene verfügbar.

Weitere Informationen finden Sie unter [Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md) und [Anzeigen und Verwalten des Änderungsverlaufs](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md).


