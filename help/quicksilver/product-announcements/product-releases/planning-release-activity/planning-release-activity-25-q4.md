---
content-type: release-notes
title: Versionsaktivität für Adobe Workfront Planning im vierten Quartal 2025
description: Dies ist die Veröffentlichungsaktivität für das Adobe Workfront Planning-Produkt im vierten Quartal 2025.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 4e1761f9-bf73-4355-925a-9136f2787a3f
source-git-commit: c7c958b09caf7e15f128a729f6b327f6c3fa21e8
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 0%

---

# Versionsaktivität für Adobe Workfront Planning im vierten Quartal 2025

In diesem Artikel werden die Funktionen beschrieben, die in Workfront Planning im vierten Quartal 2025 veröffentlicht werden.

<!--keep the sentence below for all future quarterly release pages-->

Eine Liste aller für Adobe Workfront Planning veröffentlichten Funktionen finden Sie unter [Adobe Workfront Planning Release-Aktivität: Artikelindex](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).



## Neue kombinierte Statusspalte in der Liste Einheitliche Anfrage

>[!NOTE]
>
>* Vorschau: 28. August 2025
>* Produktions-Schnellveröffentlichung: 11. September 2025
>* Produktion für alle Kunden: 16. Oktober 2025

Um das einheitliche Anfrageerlebnis zu vereinfachen, zeigt die Spalte Status jetzt sowohl den Anfragestatus als auch den Genehmigungsstatus an, je nachdem, was für eine bestimmte Anfrage gilt.

Weitere Informationen zum Erstellen von Anfragen finden Sie unter:

* Für Workfront: [Anfragen erstellen und senden](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)
* Für Workfront Planning: [Senden von Adobe Workfront Planning-Anfragen zum Erstellen von Datensätzen](/help/quicksilver/planning/requests/submit-requests.md)

## Neue Beschränkungen für Formelfelder

>[!NOTE]
>
>* Vorschau: 28. August 2025
>* Produktions-Schnellveröffentlichung: 11. September 2025
>* Produktion für alle Kunden: 16. Oktober 2025

Für Formelfelder wurden die folgenden Beschränkungen festgelegt:

* Pro Datensatztyp sind maximal 20 Formelfelder zulässig
* Für einen Formelausdruck gibt es eine Beschränkung von 50.000 Zeichen

Weitere Informationen finden Sie unter [Übersicht über Formelfelder](/help/quicksilver/planning/fields/formula-fields.md).

## Fehler anzeigen, wenn Formelwerte nicht aufgelöst werden können

>[!NOTE]
>
>* Vorschau: 28. August 2025
>* Produktions-Schnellveröffentlichung: 11. September 2025
>* Produktion für alle Kunden: 16. Oktober 2025

Um anzugeben, dass beim Beheben eines Formelfelds ein Problem auftritt, wird das Feld jetzt als &quot;#ERROR!“ angezeigt. in einem der folgenden Fälle:

* Wenn ein in einer Formel verwendetes Feld gelöscht wird.

* Wenn ein in einem aggregierten Suchfeld verwendetes Feld als #ERROR! angezeigt wird.

* Wenn ein Formelwert nicht im ausgewählten Format angezeigt werden kann.

Weitere Informationen finden Sie unter [Übersicht über Formelfelder](/help/quicksilver/planning/fields/formula-fields.md).

## Neue Ausdrücke zu Formelfeldern in Planning hinzugefügt

>[!NOTE]
>
>Vorschau: 7. August 2025
>>Produktion für alle :August, 2025
>>[!BADGE Aus dem Zeitplan]{type=Neutral}

Wir haben neue Ausdrücke mit der folgenden Verwendung zu Formelfeldern in Workfront Planning und zu berechneten benutzerdefinierten Feldern in Workfront hinzugefügt:

* **REMOVEACCENTS(Zeichenfolge)**: Entfernt diakritische Zeichen aus allen Zeichen mit Akzenten in der Eingabezeichenfolge.
* **REPLACEPATTERN (Zeichenfolge, Muster, Ersatzzeichenfolge)**: Ersetzt die Übereinstimmungen des angegebenen Musters durch die Ersatzzeichenfolge.
* **PASCAL(Zeichenfolge)**: Konvertiert die Eingabezeichenfolge in PascalCase, indem der erste Buchstabe eines jeden Worts großgeschrieben und alle Leerzeichen entfernt werden.

Weitere Informationen finden Sie unter [Übersicht über berechnete Datenausdrücke](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

## Hinzufügen der Schaltflächen „Maximieren“ und „Minimieren“ zum Erstellungsfenster des Formelfelds

>[!NOTE]
>
>Vorschau: 31. Juli 2025
>>Produktion für alle Kunden: 31. Juli 2025
>>[!BADGE Aus dem Zeitplan]{type=Neutral}

Es wurde eine Schaltfläche Maximieren hinzugefügt, um das Feld Formel beim Erstellen oder Bearbeiten des Felds in einer Datensatztabellen-Ansicht zu vergrößern. Darüber hinaus wurde im neuen vergrößerten Fenster eine Schaltfläche Minimieren hinzugefügt, um zum Feld Felderstellung zurückzukehren.

Weitere Informationen finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).

## Die Seite „Verbundene Datensätze“ ist jetzt im Vorschaubereich eines Datensatzes verfügbar

>[!NOTE]
>
>* Vorschau: 31. Juli 2025
>* Produktions-Schnellveröffentlichung: 14. August 2025
>* Produktion für alle Kunden: 16. Oktober 2025

Wir haben jetzt erreicht, dass das Erlebnis auf der Seite „Verbundene Datensätze“ im Vorschaufeld mit dem auf der Seite im Bereich „Details“ eines Datensatzes übereinstimmt.

Vor dieser Verbesserung war das Anzeigen verbundener Datensätze auf einer Seite mit verbundenen Datensätzen nur auf der vollständigen Seite des Bereichs Details eines Datensatzes möglich.

Weitere Informationen finden Sie unter [Seitenlayout für Einträge verwalten](/help/quicksilver/planning/records/manage-the-record-page.md).

<!--## Updates to Requesting experience 

>[!NOTE]
>
>* Preview: July 31, 2025
>* Production fast release: August 14, 2025
>* Production for all customers: October 16, 2025

To create a better user experience when making requests in Workfront and Workfront Planning, we've updated the requesting experience. Now you can:

* View Workfront and Workfront Planning requests in a single list.
* Filter submitted requests based on criteria you specify.
* Search for and select Workfront request queues and Workfront Planning forms in a consolidated experience.
* Hide and reorder columns in the submitted requests list.

This update also features changes to the look and feel of the page.

Previously, Workfront and Workfront Planning requests were on separate tabs, and filters were not customizable.

For more information on creating requests see:

* For Workfront: [Create and submit requests](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)
* For Workfront Planning: [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md) -->

## Erstellen von Datensätzen in der Zeitleisten-Ansicht

>[!NOTE]
>
>Vorschau: 24. Juli 2025
>>Produktions-Schnellveröffentlichung: 14. August 2025
>>Produktion für alle Kunden: 16. Oktober 2025

Sie können jetzt Datensätze in der Zeitleisten -Ansicht eines Datensatztyps erstellen, indem Sie an einer beliebigen Stelle in der Zeitleiste doppelklicken.

Sie können den Datumsbereich Ihres Datensatzes auswählen oder die Seite des Datensatzes öffnen, um alle Details zu bearbeiten.

Vor dieser Verbesserung konnten Sie neue Datensätze nur mithilfe der Schaltfläche Neuer Datensatz oder inline in der Tabellenansicht hinzufügen.

Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).

## Option „Freigeben hinzufügen“ im Menü „Mehr“ einer Karte vom Typ „Datensatz“

>[!NOTE]
>
>Vorschau: 24. Juli 2025
>>Produktions-Schnellveröffentlichung: 14. August 2025
>>Produktion für alle Kunden: 16. Oktober 2025

Sie können jetzt einen Datensatztyp über das Menü Mehr der Karte Datensatztyp auf der Seite Arbeitsbereich freigeben. Vor dieser Verbesserung war die Option Freigeben nur auf der Seite „Datensatztyp“ verfügbar.

Weitere Informationen finden Sie [Datensatztypen freigeben](/help/quicksilver/planning/access/share-record-types.md).

## Alle Workfront Planning-Ansichten im Vollbildmodus anzeigen

>[!NOTE]
>
>Vorschau: 24. Juli 2025
>>Produktions-Schnellveröffentlichung: 14. August 2025
>>Produktion für alle Kunden: 16. Oktober 2025

Sie können jetzt alle Workfront Planning-Ansichten (Tabelle, Timeline und Kalender) im Vollbildmodus anzeigen. Die Ansichtsfunktion bleibt erhalten und Sie können die Ansicht auch im Vollbildmodus ändern.

Vor dieser Verbesserung gab es diese Funktion nicht.

Weitere Informationen finden Sie unter [Verwalten von Datensatzansichten](/help/quicksilver/planning/views/manage-record-views.md).

## Teams als genehmigende Personen in Planungsanfrageformularen hinzufügen

>[!NOTE]
>
>Vorschau: 22. Juli 2025
>>Produktion für die Schnellveröffentlichung: 14. August 2025
>>Produktion für alle Kunden: 16. Oktober 2025

Um den Genehmigungsprozess flexibler zu gestalten, haben wir die Möglichkeit hinzugefügt, Teams als genehmigende Personen in Planungsanfrageformularen hinzuzufügen. Jetzt können Sie beim Festlegen von Genehmigern Team-Namen eingeben und auswählen. Jedes Teammitglied kann eine Entscheidung treffen, die als Genehmigungsentscheidung für das gesamte Team gilt.

Zuvor konnten nur einzelne Benutzer als genehmigende Personen zugewiesen werden.

Weitere Informationen finden Sie unter [Hinzufügen einer Genehmigung zu einem Anfrageformular in Adobe Workfront Planning](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

## Neue Felder zum Anzeigen von Informationen zur Datensatzgenehmigung

>[!NOTE]
>
>Vorschau: 17. Juli 2025
>>Produktion für die Schnellveröffentlichung: 14. August 2025
>>Produktion für alle Kunden: 16. Oktober 2025

Wir führen die folgenden Felder ein, um Genehmigungsinformationen für Datensätze zu erfassen, die durch Senden einer Anfrage mit einer Genehmigung erstellt wurden:

* Genehmigt von
* Validierungsdatum

Weitere Informationen finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).

## Felder basierend auf angewendeten Gruppierungen automatisch ausfüllen

>[!NOTE]
>
>Vorschau: 10. Juli 2025
>>Produktions-Schnellveröffentlichung: 14. August 2025
>>Produktion für alle Kunden: 16. Oktober 2025


Wenn Sie nun auf eine Tabellenansicht Gruppierungen angewendet haben, werden beim Hinzufügen eines Datensatzes zur Tabelle automatisch die Felder ausgefüllt, die mit den Gruppierungen verknüpft sind, denen Sie den Datensatz hinzufügen.

Wenn mehrere Gruppierungen angewendet werden, füllt das System die mit allen Gruppierungen verknüpften Felder nur dann automatisch, wenn Sie den Datensatz am Ende der Liste innerhalb der letzten Gruppierungskriterien hinzufügen.

Vor dieser Verbesserung mussten Sie die mit Gruppierungen verknüpften Felder manuell aktualisieren.

Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).
