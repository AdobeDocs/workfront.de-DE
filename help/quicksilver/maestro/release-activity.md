---
title: Adobe Maestro-Release-Aktivität
description: Adobe Maestro ist derzeit für ausgewählte Workfront-Kunden verfügbar. Lesen Sie diesen Artikel oft, um mehr über die Funktionen zu erfahren, die kürzlich für Adobe Maestro veröffentlicht wurden.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 53911aa3-74fd-4747-9008-f86a521ffba6
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '3730'
ht-degree: 0%

---

# Adobe Maestro-Release-Aktivität

{{maestro-important-intro}}

In diesem Artikel werden die Funktionen aufgelistet, die nach dem Start des geschlossenen Betaprogramms von Maestro am 22. Mai 2023 veröffentlicht wurden.

Die veröffentlichten Funktionen werden in der Reihenfolge ihrer Veröffentlichung aufgelistet, wobei die neuesten zuerst aufgeführt werden. Kunden, die am geschlossenen Betaprogramm von Maestro teilnehmen, können auf alle Funktionen in ihrer Produktionsumgebung zugreifen.

>[!IMPORTANT]
>
>Zwischen Mai 2023 und Dezember 2023 wurden alle Funktionen in diesem Artikel sowohl in der Vorschau- als auch in der Produktionsumgebung veröffentlicht. Die Maestro-Funktionen wurden seit Januar 2024 vorübergehend aus den Umgebungen für Vorschau und Sandbox entfernt. Alle nach diesem Datum veröffentlichten Funktionen sind derzeit in der Produktion verfügbar.

In diesem Artikel werden die Funktionen und Patches aufgelistet, die nach dem Start des geschlossenen Betaprogramms von Maestro am 22. Mai 2023 veröffentlicht wurden.

Die Funktionen werden wöchentlich veröffentlicht und in der Reihenfolge ihrer Veröffentlichung aufgelistet, wobei die neuesten zuerst aufgeführt werden. Kunden, die am geschlossenen Betaprogramm von Maestro teilnehmen, können auf alle Funktionen in ihrer Vorschau- und Produktionsumgebung zugreifen.

>[!IMPORTANT]
>
>Die in den folgenden Abschnitten referenzierte Dokumentation ist einige Zeit verfügbar, nachdem die Funktionen für die Produktion freigegeben wurden.


## Woche vom 29. Januar 2024

### Verbesserte Freigabe von Ansichten und Arbeitsbereichen

Produktion: 30. Januar 2024

Vorschau: zu bestimmen

Wir haben die Freigabe von Arbeitsbereichen und Ansichten mit den folgenden Verbesserungen verbessert:

* Um Klarheit darüber zu schaffen, was die einzelnen Berechtigungsebenen einem Benutzer ermöglichen, haben wir Details für jede Berechtigungsebene hinzugefügt, wenn wir einen Arbeitsbereich und eine Ansicht freigeben.

* Sie können jetzt einen Link in einen Arbeitsbereich kopieren oder ihn anzeigen und für andere freigeben. Benutzer müssen mindestens über Anzeigeberechtigungen für den Arbeitsbereich oder die Ansicht verfügen, um über den kopierten Link auf sie zugreifen zu können.

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Freigeben von Arbeitsbereichen](/help/quicksilver/maestro/access/share-workspaces.md)
* [Ansichten freigeben](/help/quicksilver/maestro/access/share-views.md)

### Miniaturansichten zu Datensätzen hinzufügen

Produktion: 1. Februar 2024

Vorschau: zu bestimmen

Sie können jetzt jedem Datensatz einzelne Miniaturansichten hinzufügen, um sie in einer Ansicht zu unterscheiden. In der Tabellenansicht können Sie Bilddateien hinzufügen, die Sie zuvor auf Ihrem Computer als Miniaturansichten gespeichert haben. Die Miniaturansichten können für jeden Datensatz eindeutig sein und sowohl in der Tabelle als auch in der Timeline-Ansicht der Datensatztypseite angezeigt werden.

Weitere Informationen finden Sie unter [Miniaturansichten zu Datensätzen hinzufügen](/help/quicksilver/maestro/records/add-thumbnails-to-records.md).

### Entfernen Sie verbundene Plattenkarten.

Produktion: 1. Februar 2024

Vorschau: zu bestimmen

Um Verwirrung zu vermeiden und Ihren Workflow zu vereinfachen, haben wir die Karten vom Typ Datensatz entfernt, die durch das Verbinden von Maestro-Datensätzen mit Objekten aus Drittanbieteranwendungen aus einem Arbeitsbereich erstellt wurden. <!---Now, when you connect Workfront objects with Maestro records, for example, you can navigate to Workfront to manage the linked objects. You can no longer find the read-only Workfront object record type page in Maestro. This simplifies the number of objects and places you manage information for your objects.  -->


Weitere Informationen finden Sie unter [Datensätze verbinden](/help/quicksilver/maestro/records/connect-records.md).

## Woche vom 22. Januar 2024

### Neuer Verlaufsabschnitt zeigt Systemaktivität für Maestro-Datensätze an

Produktion: 25. Januar 2024

Vorschau: zu bestimmen

Um die Auditing-Funktionen zu verbessern, haben wir einen neuen Abschnitt im rechten Bereich eines Datensatzes eingeführt, in dem Sie Änderungen an dem vom System aufgezeichneten Datensatz überprüfen können.

Maestro zeichnet die folgenden Informationen im neuen Abschnitt Verlauf auf:

* Alle Feldänderungen

* Die alten und neuen Werte der Felder, wenn sich die Werte ändern

* Der vollständige Name des Benutzers, der die Änderung vorgenommen hat

* Ein Datum und ein Zeitstempel für den Zeitpunkt der Änderung.

Weitere Informationen finden Sie unter [Übersicht über den Verlaufsabschnitt](/help/quicksilver/maestro/records/history-section-overview.md).

### Neue Bezeichnung für neuen Datensatz-Link

Produktion: 25. Januar 2024

Vorschau: zu bestimmen

Um bei der Erstellung von Datensätzen Konsistenz zu gewährleisten, haben wir den Link + Neu zur Erstellung von Datensätzen in &quot;+ Neuer Datensatz&quot; umbenannt.  Vor dieser Aktualisierung enthielt der Link den Namen des Datensatztyps. Der neue Link ist jetzt bei der Erstellung von Betriebs- und Taxonomiedatensätzen verfügbar. Weitere Informationen finden Sie unter [Datensätze erstellen](/help/quicksilver/maestro/records/create-records.md).

## Woche vom 8. Januar 2024

### Maestro-Funktionen werden aus der Vorschau- und Sandbox-Umgebung entfernt

Vorschau und Sandbox: 11. Januar 2024

Der Maestro-Bereich und alle Maestro-Funktionen wurden vorübergehend aus der Vorschau- und Sandbox-Umgebung entfernt. Maestro wird zu diesen Umgebungen zu einem späteren Zeitpunkt hinzugefügt, zu dem wir in den Versionshinweisen zu den Aktivitäten kommunizieren werden.

### Maestro-Berechtigungen für Arbeitsbereiche und Ansichten

Produktion: 11. Januar 2024

Vorschau: zu bestimmen

Sie können jetzt einen Arbeitsbereich oder eine Ansicht für Benutzer und Gruppen freigeben. Je nachdem, welche Informationen angezeigt oder bearbeitet werden sollen, können Sie ihre Berechtigungen auf verschiedene Ebenen festlegen.

Wenn Sie einen Arbeitsbereich freigeben, haben Benutzer Berechtigungen für die Datensatztypen, Datensätze und Felder in diesem Bereich.

Wenn Sie einen Arbeitsbereich freigeben, erhalten Benutzer keine Freigabeberechtigungen für die Ansichten, die mit den Datensatztypen des Arbeitsbereichs verknüpft sind. Sie müssen Ansichten separate Berechtigungen erteilen.

Im Folgenden finden Sie die Berechtigungsebenen für Maestro-Arbeitsbereiche:

* Ansicht: Benutzer können Arbeitsbereiche anzeigen, die für sie freigegeben sind. Außerdem können sie Datensatztypen und Datensätze aus dem freigegebenen Arbeitsbereich anzeigen.

* Beitragen: Benutzer können Datensätze in dem für sie freigegebenen Arbeitsbereich erstellen, bearbeiten oder löschen.  Sie können keine für sie freigegebenen Datensatztypen oder Arbeitsbereiche erstellen oder bearbeiten.

* Verwalten: Benutzer können Arbeitsbereiche, Datensatztypen, Datensätze und Felder in Arbeitsbereichen erstellen, bearbeiten und löschen, die für sie freigegeben sind.

Im Folgenden finden Sie die Berechtigungsstufen für Datensatzansichten:

* Ansicht: Benutzer können die Ansicht aus dem Dropdown-Menü Ansicht einer Seite vom Typ Datensatz auswählen.
* Verwalten: Benutzer können die Ansicht bearbeiten, freigeben und löschen.

Weitere Informationen finden Sie unter [Zugriffsübersicht](/help/quicksilver/maestro/access/access-overview.md) und [Übersicht über die Freigabe von Berechtigungen in Adobe Maestro](../maestro/access/sharing-permissions-overview.md).

### Neuer Formelfeldtyp

Produktion: 11. Januar 2024

Vorschau: zu bestimmen

Jetzt können Sie einem Datensatztyp ein Feld vom Typ Formel hinzufügen.

Formelfelder generieren einen neuen Wert anhand vorhandener Werte aus anderen Feldern eines Datensatztyps und einer Funktion, die angibt, wie die vorhandenen Werte berechnet werden sollen.

In einer Formelberechnung können Sie keine Suchfelder aus verknüpften Datensatztypen verwenden. Diese Funktion ist zu einem späteren Zeitpunkt verfügbar.

Weitere Informationen finden Sie unter [Übersicht über Formelfelder](/help/quicksilver/maestro/fields/formula-fields.md).

### Aktionen zum Rückgängigmachen/Wiederholen bei der Verwaltung von Datensätzen in der Tabellenansicht

Produktion: 11. Januar 2024

Vorschau: zu bestimmen

Sie können Ihre Änderungen jetzt rückgängig machen oder wiederholen, wenn Sie die folgenden Aktionen in der Tabellenansicht ausführen:

* Daten kopieren/einfügen
* Datensatz bearbeiten
* Datensatz hinzufügen
* Datensatz löschen

Sie können die folgenden Tastenanschläge verwenden, um Aktionen rückgängig zu machen oder wiederherzustellen:

* Rückgängig: STRG/BEFEHL + Z
* Wiederholen: STRG/ BEFEHL + UMSCHALT + Z

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Datensätze bearbeiten](/help/quicksilver/maestro/records/edit-records.md)

* [Datensätze löschen](/help/quicksilver/maestro/records/delete-records.md)

* [Datensätze erstellen](/help/quicksilver/maestro/records/create-records.md)

## Woche vom 25. Dezember 2023

### Suchen in der Timeline-Ansicht

Vorschau und Produktion: 27. Dezember 2023

Sie können jetzt nach einem Keyword suchen, um schnell einen Datensatz in der Timeline-Ansicht zu finden. Sie können Suchbegriffe und Sonderzeichen aus allen auf dem Bildschirm sichtbaren Feldern verwenden, um einen Datensatz zu finden. Weitere Informationen finden Sie unter [Verwalten der Timeline-Ansicht](../maestro/views/manage-the-timeline-view.md).

## Woche vom 18. Dezember 2023

### Hinzufügen von Kommentaren zu Datensätzen über die Detailseite

Vorschau und Produktion für alle Kunden: 18. Dezember 2023

>[!NOTE]
>
>Die folgenden Funktionen werden in der Produktion mit der Version vom Januar 2024 verfügbar sein:
>
>* Nach Kommentaren suchen
>
>* Bilder kopieren und einfügen
>
>* Bilder per Drag &amp; Drop verschieben
>
>Weitere Informationen finden Sie unter [Übersicht über die Version des ersten Quartals 2024](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

Sie können jetzt mit anderen an einzelnen Datensätzen zusammenarbeiten, indem Sie Kommentare hinzufügen oder auf andere antworten, während Sie einen Datensatz auf der Detailseite anzeigen.

Das Kommentarerlebnis für Maestro-Datensätze entspricht dem neuen Kommentarerlebnis für Workfront-Objekte.

Weitere Informationen finden Sie unter [Verwalten von Datensatzkommentaren](/help/quicksilver/maestro/records/manage-record-comments.md).

### Maestro-Connector (Beta) für Adobe Workfront Fusion

Produktion: 21. Dezember 2023

>[!IMPORTANT]
>
>Ihr Unternehmen muss Adobe Workfront Fusion erwerben, um Verbindungen mit Maestro aufbauen zu können.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/get-started/workfront-fusion-overview.md).

Jetzt können Sie Adobe Workfront Fusion verwenden, um eine Verbindung zu Maestro herzustellen. Mit der neuen Adobe Maestro Fusion-Verbindung können Sie:

* Datensätze erstellen, lesen, aktualisieren und löschen

* Datensatzliste nach Datensatztyp abrufen

* Löschen oder Abrufen einer Liste von Datensatztypen

* Suchdatensätze

* API-Aufruf

* Trigger eines Szenarios bei einer Änderung in Maestro

Weitere Informationen finden Sie unter [Adobe Maestro-Module](/help/quicksilver/workfront-fusion/apps-and-their-modules/maestro-modules.md).

## Woche vom 11. Dezember 2023

### Primärfeld in Tabellenansicht eines Datensatztyps aktualisieren

Vorschau und Produktion: 14. Dezember 2023

Jetzt können Sie das Feld auswählen, das in der ersten Spalte einer Maestro-Tabellenansicht angezeigt werden soll. Dieses Feld wird jetzt als primäres Feld bezeichnet.

Vor dieser Verbesserung wurde das Feld Name eines Datensatzes immer in der ersten Spalte der Tabellenansicht angezeigt und es konnte nicht an einer anderen Position platziert werden.

Beachten Sie bei dieser Verbesserung Folgendes:

* Die Spalte &quot;Name&quot;oder das Feld ist standardmäßig weiterhin die erste Spalte einer Tabelle.

* Sie können jedes Feld der folgenden Typen als primäres Feld auswählen und das Feld Name in der ersten Spalte ersetzen:

   * Einzeiliger Text

   * Zahl

   * Formel

* Das primäre Feld einer Tabellenansicht wird immer gesperrt und kann nicht verschoben werden, es sei denn, Sie legen ein anderes Feld als primäres Feld fest.

* Sie können das Primärfeld in einer Spaltenüberschrift ändern, die nicht primär ist.

* Alle Tabellenansichten eines Datensatztyps haben dasselbe Primärfeld, das Sie auswählen.

Weitere Informationen finden Sie unter [Tabellenansicht verwalten](/help/quicksilver/maestro/views/manage-the-table-view.md).


### Maestro-Datensätze mit Adobe Experience Manager Assets verbinden

Vorschau: 14. Dezember 2023

Produktionsversion: 21. Dezember 2023

>[!IMPORTANT]
>
>Die Workfront-Instanz Ihres Unternehmens muss mit der Adobe Business Platform oder der Adobe Admin Console integriert sein, um Maestro-Datensätze mit Adobe Experience Manager Assets verbinden zu können.
>
>Wenn Sie Fragen zum Einstieg in die Adobe Admin Console haben, lesen Sie den Abschnitt [Häufig gestellte Fragen zu Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).


Sie können jetzt eine Verbindung zwischen Maestro-Datensatztypen und Adobe Experience Manager Assets herstellen.

Nachdem Sie die Verbindung hergestellt haben, ist mit diesem Update die folgende Funktion verfügbar:

* Sie können Experience Manager-Assets und -Ordner mit einem Maestro-Datensatz aus einem bestimmten Repository in Experience Manager Assets verknüpfen, auf das sie Zugriff haben. In diesem Prozess können Sie Asset-Felder mit Maestro-Feldern verbinden.

* Maestro-Benutzer können den Namen der verbundenen Assets sowie die Werte der verbundenen Felder in Maestro anzeigen

<!--removed per PM, for now: 
* An Experience Manager Assets record type is automatically created in Maestro after you establish the connection. Connected assets are visible in the Maestro table and timeline views of this new record type.  
-->

* Sie können im Feld &quot;Verbundener Datensatz&quot;in der Tabellenansicht des Maestro-Datensatzes auf den Asset-Namen klicken und ein Popup-Fenster mit der Asset-Miniaturansicht und mehreren Schlüsselfeldern anzeigen. Im Popup-Fenster können Sie in Experience Manager zum Asset-Viewer navigieren und alle Details dazu anzeigen.

Weitere Informationen finden Sie unter [Datensatztypen verbinden](/help/quicksilver/maestro/architecture/connect-record-types.md).

## Woche vom 4. Dezember 2023

### Kopieren Sie Informationen aus einem Feld in ein anderes und fügen Sie sie in der Maestro-Tabellenansicht für die Felder vom Typ Personen und verknüpfte Datensätze ein.

Vorschau und Produktion: 5. Dezember 2023

Sie können jetzt Informationen aus einem Feld in ein anderes Feld desselben Typs in einer Tabellenansicht vom Typ Maestro-Datensatz kopieren und einfügen. Diese Funktion wird jetzt für die folgenden Feldtypen unterstützt:

* Personen
* Verknüpfte Datensatzfelder

Beachten Sie Folgendes:

* Das Kopieren und Einfügen von Feldwerten von einem Feld in ein anderes wird für Felder unterstützt, die mehrere Werte anzeigen.

* Es ist nicht möglich, Informationen aus anderen Quellen als einem Maestro-Feld des gleichen Typs zu kopieren wie das Feld, in das Sie die Informationen einfügen.

* Es ist nicht möglich, Feldwerte für Felder zu kopieren und einzufügen, die im Detailbereich eines Datensatzes angezeigt werden.

Weitere Informationen finden Sie unter [Datensätze bearbeiten](../maestro/records/edit-records.md).

Informationen zu verknüpften Feldern finden Sie unter [Datensatztypen verbinden](../maestro/architecture/connect-record-types.md).

## Woche vom 27. November 2023

### Kopieren und Einfügen von Informationen aus einem Feld in ein anderes in der Maestro-Tabellenansicht

Vorschau und Produktion: 28. November 2023

Sie können jetzt Informationen aus einem Feld in ein anderes Feld desselben Typs in einer Tabellenansicht vom Typ Maestro-Datensatz kopieren und einfügen.

Beachten Sie Folgendes:

* Es ist nicht möglich, Informationen aus anderen Quellen als einem Maestro-Feld des gleichen Typs zu kopieren wie das Feld, in das Sie die Informationen einfügen.

* Es ist nicht möglich, Feldwerte für Felder zu kopieren und einzufügen, die im Detailbereich eines Datensatzes angezeigt werden.

* Für die folgenden Feldtypen können Sie keine Feldwerte kopieren und einfügen:

   * Personen

   * Systemfelder

   * Verknüpfte Felder, die durch das Verbinden von Datensätzen erstellt wurden

Weitere Informationen finden Sie unter [Datensätze bearbeiten](../maestro/records/edit-records.md).

## Woche vom 6. November 2023

### Gruppierung für die Tabellenansicht

Vorschau und Produktion: 7. November 2023

Sie können Datensätze nun in der Tabellenansicht einer Seite vom Typ Datensatz gruppieren. Sie können in der Maestro-Oberfläche nach drei eindeutigen Feldern gruppieren <!--checking into this for now: and by four fields when using the API-->.

Weitere Informationen finden Sie unter [Tabellenansicht verwalten](../maestro/views/manage-the-table-view.md).

## Woche vom 30. Oktober 2023

### Neue Feldtypen für Benutzer und Datumsfelder zum Erfassen, wer einen Datensatz erstellt oder zuletzt geändert hat oder zu welchem Datum

Vorschau und Produktion: 30. Oktober 2023

Wir haben die folgenden Feldtypen für Maestro-Datensätze eingeführt:

* Erstellt von

* Erstellungsdatum

* Zuletzt geändert von

* Zuletzt geändert am

Die Feldwerte der aus diesen Feldtypen erstellten Felder sind schreibgeschützt und erfassen den Namen des Benutzers, der einen Datensatz erstellt oder zuletzt geändert hat, oder das Datum, an dem der Datensatz erstellt oder zuletzt geändert wurde.

Weitere Informationen finden Sie unter [Felder erstellen](../maestro/fields/create-fields.md).

### Navigieren zu Workfront-Objekten aus einem Maestro-Datensatz

Vorschau und Produktion: 31. Oktober 2023

Sie können die Workfront-Objektseiten jetzt aus den folgenden Bereichen in Maestro öffnen:

* Die schreibgeschützte verknüpfte Tabellenansicht der Workfront-Objektdatensätze

* Die Seite mit den Details zum schreibgeschützten Workfront-Objektdatensatz

Weitere Informationen finden Sie unter [Datensätze verbinden](../maestro/records/connect-records.md).

### Verbesserte Navigation in der Tabellenansicht

Vorschau und Produktion: 2. November 2023

Wir haben die Navigation in der Tabellenansicht einer Seite vom Typ Datensatz verbessert.

Im Folgenden finden Sie einige Verbesserungen:

* Navigieren Sie mithilfe der Tabulatortaste auf der Tastatur durch die Spalten und Zeilen der Tabelle.

* Fügen Sie an jeder Spaltenposition einen neuen Datensatz hinzu. Vor dieser Verbesserung können Sie einen Datensatz nur aus der ersten Spalte hinzufügen.

* Verwenden Sie die Tastenkombination Umschalt + Eingabetaste , um einen neuen Datensatz (oder eine neue Zeile) zur Tabelle hinzuzufügen.

Weitere Informationen finden Sie unter [Datensätze erstellen](../maestro/records/connect-records.md).

## Woche vom 16. Oktober 2023

### Neuer Benutzerfeldtyp

Vorschau und Produktion: 16. Oktober 2023

Sie können jetzt ein Feld vom Typ Personen zu Maestro-Datensatztypen hinzufügen. Sie können Felder vom Typ Personen verwenden, um vorhandene Benutzer einem Datensatz zuzuordnen. Weitere Informationen finden Sie unter [Felder erstellen](../maestro/fields/create-fields.md).

### Rich-Text-Format für Absatzfelder

Vorschau und Produktion: 16. Oktober 2023

Für Absatzfelder wurden Steuerelemente im Rich-Text-Format hinzugefügt. Sie können Absatzfelder mit Rich Text formatieren, entweder in der Tabellenansicht eines Datensatztyps oder auf der Detailseite eines Datensatzes. Weitere Informationen finden Sie unter [Datensätze bearbeiten](../maestro/records/edit-records.md).


### Farbkodierung für die Timeline-Ansicht aufzeichnen und gruppieren

Vorschau und Produktion: 19. Oktober 2023

Sie können jetzt die Datensatzleisten und die Gruppierungen in der Timeline-Ansicht farbcodieren.

Im Folgenden finden Sie Optionen für die Farben, die Sie in der Timeline-Ansicht für Datensatzbalken und -gruppierungen anzeigen möchten:

* Die Gruppierungen können die folgenden Farben aufweisen:

   * Grau (Standard)

   * Die Farbe des Felds, nach dem Sie eine Gruppierung vornehmen

* Balken können die folgenden Farben aufweisen:

   * Die Farbe des Datensatztyps

   * Die Farbe eines ausgewählten Felds

   * Die Farbe der Gruppierung

   * Keine Farbe (Standard)

Beim Abgleich von Farben mit einem bestimmten Feld können Sie nur Felder mit farbcodierten Optionen auswählen.

Weitere Informationen finden Sie unter [Verwalten der Timeline-Ansicht](../maestro/views/manage-the-timeline-view.md).

## Woche vom 9. Oktober 2023

### In Tabellenansicht suchen

Vorschau und Produktion: 9. Oktober 2023

Sie können jetzt nach einem Suchbegriff suchen, um schnell einen Datensatz in der Tabellenansicht zu finden. Sie können Suchbegriffe und Sonderzeichen aus allen auf dem Bildschirm sichtbaren Feldern verwenden, um einen Datensatz zu finden. Weitere Informationen finden Sie unter [Tabellenansicht verwalten](../maestro/views/manage-the-table-view.md).

## Woche vom 18. September 2023

### Zeilen neu anordnen

Vorschau und Produktion: 20. September 2023

Sie können jetzt eine oder mehrere Zeilen (oder Datensätze) in der Tabellenansicht einer Datensatztypseite neu anordnen. Weitere Informationen finden Sie unter [Tabellenansicht verwalten](../maestro/views/manage-the-table-view.md).

## Woche vom 4. September 2023

### Verbinden von Maestro-Datensätzen mit Workfront-Unternehmen und -Gruppen

Vorschau und Produktion: 5. September 2023

Sie können jetzt einen Maestro-Datensatz mit Workfront-Unternehmen und -Gruppen verbinden. Sie müssen zunächst eine Verbindung zwischen einem Maestro-Record-Typ und den Workfront-Unternehmen und -Gruppen-Objekttypen herstellen. Anschließend können Sie einen einzelnen Maestro-Datensatz des ausgewählten Datensatztyps mit einzelnen Workfront-Unternehmen und -Gruppen verbinden.

Beachten Sie Folgendes:

* Sie müssen für jeden Workspace eine Verbindung zwischen den Maestro-Datensatztypen und den Workfront-Objektarten &quot;Unternehmen&quot;und &quot;Gruppe&quot;herstellen.

* Es ist nicht möglich, Taxonomie-Datensatztypen mit Workfront-Objekttypen zu verbinden.

* Sie können mehrere Maestro-Datensätze mit demselben Unternehmen oder derselben Workfront-Gruppe sowie mehrere Unternehmen oder Gruppen mit demselben Maestro-Datensatz verbinden.

* Sie können keine Firmen oder Gruppen in Maestro bearbeiten. Alle in Workfront durchgeführten Unternehmens- oder Gruppenänderungen werden in Maestro bei der Überprüfung der mit Maestro verknüpften Datensätze angezeigt.

  Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Datensatztypen verbinden](../maestro/architecture/connect-record-types.md)
   * [Datensätze verbinden](../maestro/records/connect-records.md)

### URL-Unterstützung für einzeilige Textfelder

Vorschau und Produktion: 7. September 2023

Für eine bessere Sichtbarkeit beim Arbeiten mit Links in der Tabellenansicht wurde Unterstützung für URLs in einzeiligen Textfeldern hinzugefügt. Durch die Verwendung von URLs zu anderen Websites oder externen Laufwerken beim Aktualisieren eines einzeiligen Textfelds werden diese jetzt als Links identifiziert und Sie können in der Tabelle auf sie klicken. Vor dieser Verbesserung wurden Links als Text angezeigt.

## Woche vom 28. August 2023

### Menü für die Feldanzeige in der Symbolleiste &quot;Tabellenansicht&quot;

Vorschau und Produktion: 31. August 2023

Um die richtigen Informationen zu einem bestimmten Datensatz anzuzeigen, insbesondere wenn Sie die Ansicht für andere freigeben möchten, die einige, aber nicht alle Felder eines Datensatztyps sehen müssen, können Sie jetzt auswählen, welche Felder (oder Spalten) angezeigt werden sollen und welche in der Tabellenansicht ausgeblendet werden sollen.

Sie können einzelne Felder in jeder Kopfzeile der Feldspalten ein- oder ausblenden oder Sie können alle Felder des Datensatztyps über eine Einstellung in der Symbolleiste der Tabellenansicht verwalten.

Weitere Informationen finden Sie unter [Tabellenansicht verwalten](../maestro/views/manage-the-table-view.md).

## Woche vom 21. August 2023

### Verbinden von Maestro-Datensätzen mit Programmen und Portfolios

Vorschau und Produktion: 24. August 2023

Sie können jetzt einen Maestro-Datensatz mit Workfront-Programmen und -Portfolios verbinden. Sie müssen eine Verbindung zwischen einem Maestro-Record-Typ und einem Programm oder Portfolio erstellen, das bzw. das ein verbundenes Feld erstellt. Anschließend können Sie alle Maestro-Datensätze aus allen anderen Datensatztypen innerhalb desselben Arbeitsbereichs mit bestimmten Programmen und Portfolios verbinden, wodurch ein schreibgeschützter Workfront-Programm- oder Workfront-Portfolio-Datensatztyp im selben Arbeitsbereich erstellt wird. Beachten Sie Folgendes:

* Die Datensatztypen des Workfront-Connectors sind für jeden Arbeitsbereich eindeutig.
* Sie können mehrere Maestro-Datensätze mit demselben Workfront-Programm oder -Portfolio sowie mehrere Programme und Portfolios mit demselben Maestro-Datensatz verbinden.
* Sie können keine Programme und Portfolios in Maestro bearbeiten. Alle in Workfront durchgeführten Programm- und Portfolioänderungen werden in Maestro bei der Überprüfung der verknüpften Datensätze angezeigt.

### Neue Sortierfunktion für die Tabellenansicht

Vorschau und Produktion: 24. August 2023

Sie können Datensätze nun in der Tabellenansicht einer Seite vom Typ Datensatz sortieren.
Die folgenden Funktionen sind jetzt verfügbar:

* Sortierung auf Tabellenebene, wobei mehrere Felder gleichzeitig sortiert werden können.
* Sortierung auf Spalten- oder Feldebene, wo Sie einzelne Felder sortieren können.

### Verbesserungen an der Timeline-Ansicht: neues Erscheinungsbild für Gruppierungen und der Umschalter für Kompakt-/Standardansicht

Vorschau und Produktion: 24. August 2023

Die Timeline-Ansicht wurde folgendermaßen verbessert:

* Sie können die Timeline-Ansicht jetzt in den folgenden Modi anzeigen:

   * Standard: Zeigt Datensätze in separaten Zeilen an.
   * Kompakt: Zeigt die Datensätze an, deren Daten sich nicht in derselben Zeile überschneiden.

* Das Erscheinungsbild der Gruppierungslinien in der Timeline-Ansicht wurde geändert, sodass sie über der Timeline der darin enthaltenen Datensätze angezeigt werden. Vor dieser Verbesserung wurden die Gruppierungslinien über die gesamte Zeitleistenlänge hinweg angezeigt.

## Woche vom 14. August 2023

### Neuanordnen von Spalten in der Tabellenansicht

Sie können Spalten in der Maestro-Tabellenansicht jetzt neu anordnen. Beachten Sie bei der Neuanordnung von Spalten Folgendes:

* Das Feld Name ist immer das erste Feld in der Tabellenansicht einer Seite vom Typ Datensatz

* Sie können das Feld &quot;Name&quot;nicht an eine andere Position verschieben

* Das Feld Name ist eingefroren und nicht Teil des horizontalen Bildlaufs.

### Horizontaler Bildlauf für die Timeline-Ansicht

Sie können jetzt einen horizontalen Bildlauf in der Timeline-Ansicht eines Datensatztyps durchführen.

## Woche vom 7. August 2023

### Import von Datensatztypen aus einer Excel-Datei

Vorschau und Produktion: 10. August 2023

Sie können jetzt eine Excel-Datei importieren, um in einem Arbeitsbereich Datensatztypen zu erstellen. Die Dateiblätter werden zu den Datensatztypen, und die Spalten der Datei werden zu ihren jeweiligen Feldern.

### Verbessertes Erlebnis beim Verbinden von Datensatztypen und Projekten

Vorschau und Produktion: 10. August 2023

Wir haben die Art und Weise verbessert, wie Sie Datensatztypen verbinden, einschließlich der Verbindung zu Workfront-Projekten. Im Rahmen dieser Verbesserung haben wir beim Hinzufügen eines Felds für einen Datensatztyp aus der Tabellenansicht folgende Änderungen vorgenommen:

* Das Feld Beziehungstyp wurde aus der Registerkarte &quot;Neues Feld&quot;entfernt.

* Fügen Sie eine Registerkarte &quot;Neue Verbindung&quot;hinzu, auf der Sie direkt den Datensatz oder den Objekttyp auswählen können, mit dem Sie eine Verbindung herstellen möchten, sodass kein Feld vom Typ Beziehung erforderlich ist.

## Woche vom 10. Juli 2023

### Erscheinungsbild eines Datensatztyps aktualisieren

Vorschau und Produktion: 13. Juli 2023

Sie können jetzt ein benutzerdefiniertes Symbol für einen Datensatztyp und eine benutzerdefinierte Farbe für das Symbol für den Datensatztyp auswählen.

### Neuer Feldtyp für Kontrollkästchen

Vorschau und Produktion: 13. Juli 2023

Sie können jetzt einen Kontrollkästchen-Feldtyp zu Maestro-Datensatztypen hinzufügen. Sie können ein Feld vom Typ Kontrollkästchen verwenden, um einem Datensatz eine einzige Kontrollkästchen-Option hinzuzufügen. Sie können dieses Feld verwenden, um ein bestimmtes Attribut oder einen bestimmten Status für diesen Datensatz anzugeben. Sie können sie beispielsweise als Markierung zum Tracking der Fertigstellung, Genehmigung oder eines anderen Binärattributs für jeden Datensatz verwenden.

## Woche vom 26. Juni 2023

### Schnelle Aktivierung des Kontextmenüs in einer Tabelle

Vorschau und Produktion: 28. Juni 2023

Wir haben die Aktivierung des Kontextmenüs ermöglicht, indem wir mit der rechten Maustaste auf eine beliebige Zeile eines Datensatzes klicken, wenn wir die Datensätze in der Tabellenansicht oder in einem Datensatztyp anzeigen. Sie können jetzt einen Link zur Detailseite des Datensatzes schnell anzeigen, löschen oder kopieren, wenn Sie das Kontextmenü von einer beliebigen Stelle in der Tabellenansicht eines Datensatztyps aus aufrufen. Vor dieser Verbesserung war das Kontextmenü nur über das Menü Mehr in der Spalte Name eines Datensatzes zugänglich.

## Woche vom 19. Juni 2023

### Namen von Datensatzfeldern sind eindeutig

Wir haben jetzt eine Anforderung eingeführt, dass die Feldnamen eines Maestro-Datensatztyps eindeutige Namen haben müssen. Felder, die zu verschiedenen Datensatztypen gehören, müssen keine eindeutigen Namen haben.

## Woche vom 5. Juni 2023

### Verbinden von Maestro-Datensätzen mit Workfront-Projekten

Vorschau und Produktion: 5. Juni 2023

Sie können jetzt einen Maestro-Datensatz mit Workfront-Projekten verbinden. Sie müssen einen Connector-Maestro-Record-Typ erstellen, um die Verbindung zwischen Maestro-Datensätzen und Workfront-Projekten herzustellen. Anschließend können Sie über das Feld Beziehung alle Maestro-Datensätze aus allen anderen Datensatztypen mit dem Connector-Datensatz verbinden. Beachten Sie Folgendes:

* Sie müssen für jeden Workspace über einen Connector-Record-Typ für Workfront verfügen.
* Sie können mehrere Maestro-Datensätze mit demselben Workfront-Projekt und mehrere Projekte mit demselben Maestro-Datensatz verbinden.
* Sie können keine Projekte in Maestro bearbeiten. Alle in Workfront durchgeführten Projektänderungen werden in Maestro bei der Überprüfung der verknüpften Datensätze angezeigt.

## Woche vom 29. Mai 2023

### Zweitdatumsanforderung für das Erstellen einer Timeline-Ansicht

Vorschau und Produktion: 31. Mai 2023

Sie müssen mindestens zwei Datumsfelder mit einem Datensatztyp verknüpfen, um eine Timeline-Ansicht zu erstellen.
