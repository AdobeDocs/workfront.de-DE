---
title: Übersicht über die Version im ersten Quartal 2027
description: Diese Seite enthält Informationen zur Funktionalität, die in der Version vom ersten Quartal 2027 enthalten ist. Diese Verbesserungen werden voraussichtlich im Lauf des Quartals in der Produktionsumgebung zur Verfügung gestellt.
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 18e1d35b98b8c1afc6f9c1b14dba73d160b7e420
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 30%
---

# Übersicht über die Version im ersten Quartal 2027

Diese Seite enthält Informationen zur Funktionalität, die in der für Januar 2027 geplanten Version vom ersten Quartal 2027 enthalten ist.

Die Verbesserungen auf dieser Seite sind in der Vorschauumgebung verfügbar. Diese Seite wird mit zusätzlichen Verbesserungen aktualisiert, sobald die Veröffentlichung im ersten Quartal 2027 der geplanten Produktionsversion nahekommt.

>[!IMPORTANT]
>
>
>Sofern nicht anders angegeben, sind monatliche und vierteljährliche Veröffentlichungen am Donnerstag der zweiten vollen Woche des Monats verfügbar.
>
>| Monatliche Veröffentlichung | Vierteljährliche Veröffentlichung |
>|----|----|
>| <ul><li>2026.11 (12. November 2026)</li><li>2026.12 (17. Dezember 2026)</li><li>2027.01 (21. Januar 2027)</li></ul> | <ul><li>2027.01 (21. Januar 2027)</li></ul> |
>
>Weitere Informationen zum Schnellveröffentlichungsprozess finden Sie unter [Aktivieren oder Deaktivieren des Schnellveröffentlichungsprozesses](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront-Verbesserungen

* [Verbesserungen bei Projekten](#project-enhancements)


### Verbesserungen bei Projekten

<table>
    <tbody>
        <tr>
            <td><strong>Funktion</strong>
            </td>
            <td><strong>Vorschau</strong></td>
            <td><strong>Schnellveröffentlichung</strong></td>
            <td><strong>Vierteljährlich</strong></td>
        </tr>
        <tr>
            <td>
                <p><a href="/help/quicksilver/product-announcements/product-releases/27-q1-release-activity/27-q1-projects.md">Threads an den Anfang der Aktualisierungen heften</a></p>
                <p>Sie können jetzt die wichtigsten Threads oben im Bereich Aktualisierungen an ein Projekt, eine Aufgabe, ein Problem oder eine Anfrage anheften, damit wichtige Informationen für Ihr Team sichtbar bleiben.</p>
            </td>
            <td><p>15. Oktober 2026</p></td>
            <td><p>12. November 2026</p></td>
            <td><p>21. Januar 2027</p></td>
        </tr>
    </tbody>
</table>

## Versionshinweise für andere Bereiche

* [Versionsaktivität von Adobe Workfront Fusion](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).
* [Adobe Workfront Planning-Versionsaktivität](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

Für folgende Elemente gibt es derzeit keine Updates in der Version:

* Szenarienplaner
* Korrekturabzug
* Ziele

## Ankündigungen

### Veraltete Felder für Abrechnung und Kostensatz in Aufgabengebiet-Listenansichten werden entfernt

Im Laufe der Zeit haben wir erweiterte Raten-Management-Funktionen und spezielle Aufgabengebiet-Erlebnisse eingeführt, die einen vollständigeren und skalierbareren Ansatz zur Pflege von Raten-Informationen bieten. Infolgedessen bewegt sich die Ratenverwaltung in Richtung dieser dedizierten Erlebnisse statt in Richtung listenbasierter Management-Workflows.

Mit der Version vom Januar 2027 sind die alten Felder **Abrechnung pro Stunde** und **Kosten pro Stunde** nicht mehr in der Workfront-API oder in Aufgabengebiet-Listenansichten verfügbar, einschließlich Filter-/Ansicht-/Gruppierungskonfigurationen (sowohl Direktverweise als auch berechnete Spalten im Textmodus).

Als Ersatz in Berichten können Sie den empfohlenen Textmodus-Code verwenden (verwenden Sie nach Bedarf `costRates` oder `billingRates`):

    &quot;
    displayName=Test
    listDelimiter=&lt;br>
    listMethod=nested(costRates).lists
    type=iterate
    valueExpression=CONCAT({startDate},“ - &quot;,{endDate},“: &quot;,{value})
    valueFormat=HTML
    &quot;

Verwenden Sie zum Verwalten und Überprüfen der Vorgangsrollensätze die dedizierten Tarifverwaltungserfahrungen:

* Greifen Sie direkt über die Seite „Aufgabengebiet“ > „Tarife“ auf die Tarife für Aufgabengebiete zu und verwalten Sie sie.
* Verwenden Sie Tarifberichte, um Tarifinformationen in allen Aufgabengebieten zu überprüfen, zu analysieren und in Berichten zu erfassen.

Zur Vorbereitung auf die Änderung ist keine Aktion erforderlich. Administratoren, die derzeit die Felder **Abrechnung pro Stunde** und **Kosten pro Stunde** in den Listenansichten für Aufgabengebiete anzeigen, sollten ihre Workflows jedoch so aktualisieren, dass sie die oben beschriebenen empfohlenen Tarifverwaltungserlebnisse verwenden.

Informationen zu den Vorgangsrollensätzen finden Sie unter [Erstellen und Verwalten von &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

<!--

### Workfront Maintenance Updates

For information about the maintenance updates made during the First Quarter 2027 release, see [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=de).

-->

### Updates für Schulungen

Erfahren Sie mehr über die neuesten Updates von Lernprogrammen, Lernpfaden, Videos und Handbüchern für jede Adobe Workfront-Produktversion. Weitere Informationen finden Sie im Abschnitt „Neue Funktionen“ der Seite [Workfront-Tutorials](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=de).
