---
title: Adobe Maestro-Release-Aktivität
description: Adobe Maestro ist derzeit für ausgewählte Workfront-Kunden verfügbar. Lesen Sie diesen Artikel oft, um mehr über die Funktionen zu erfahren, die kürzlich für Adobe Maestro veröffentlicht wurden.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 53911aa3-74fd-4747-9008-f86a521ffba6
source-git-commit: bccd29ce284ca247b51971369102b5992061afb0
workflow-type: tm+mt
source-wordcount: '2796'
ht-degree: 0%

---

# Adobe Maestro-Release-Aktivität

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Maestro, ein neues Angebot von Adobe Workfront.
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist. Sie müssen Workfront-Kunde sein, um Maestro-Funktionen verwenden zu können.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro/maestro-overview.md).

In diesem Artikel werden die Funktionen aufgelistet, die nach dem Start des geschlossenen Betaprogramms von Maestro am 22. Mai 2023 veröffentlicht wurden.

Die veröffentlichten Funktionen werden in der Reihenfolge ihrer Veröffentlichung aufgelistet, wobei die neuesten zuerst aufgeführt werden. Kunden, die am geschlossenen Betaprogramm von Maestro teilnehmen, können auf alle Funktionen in ihrer Vorschau- und Produktionsumgebung zugreifen.

>[!IMPORTANT]
>
>Die in den folgenden Abschnitten referenzierte Dokumentation ist einige Zeit verfügbar, nachdem die Funktionen für die Produktion freigegeben wurden.

In diesem Abschnitt werden die Funktionen und Patches aufgelistet, die nach dem Start des geschlossenen Betaprogramms von Maestro am 22. Mai 2023 veröffentlicht wurden.

Die Funktionen werden wöchentlich veröffentlicht und in der Reihenfolge ihrer Veröffentlichung aufgelistet, wobei die neuesten zuerst aufgeführt werden. Kunden, die am geschlossenen Betaprogramm von Maestro teilnehmen, können auf alle Funktionen in ihrer Vorschau- und Produktionsumgebung zugreifen.

<!--
## Week of November 27, 2023

### Maestro permissions for users and groups

Production: November 28, 2023

>[!IMPORTANT]
>
>This functionality is not yet available in Preview.

You can now share a workspace with users and groups. You can set their permissions to different levels, depending on what information they need to view or edit in a Maestro workspace. After you share permissions to a workspace, users have permissions to the record types, records, and fields in that space.

The following are the permissions levels for Maestro workspaces:  

* None: Users cannot access any workspaces in Maestro, even if the Maestro area is shared with them through a layout template. 

* View: Users can view workspaces that are shared with them. They can also view record types, and records from the shared workspace. 

* Contribute: Users can create, edit, or delete records in the workspace that is shared with them.  They cannot create or edit record types or workspaces ones shared with them.  

* Manage: Users can create, edit, and delete record types, records, and fields in workspaces that are shared with them. They cannot create workspaces.  

Only Workfront administrators can create, edit, or delete workspaces and all information associated with them.  

For more information, see [Grant access to Adobe Maestro](../maestro/access/grant-access.md) and [Overview of sharing permissions in Adobe Maestro](../maestro/access/sharing-permissions-overview.md). -->

## Woche vom 18. Dezember 2024

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

     >[!NOTE]
     >
     >Felder vom Typ Formel werden zu einem späteren Zeitpunkt veröffentlicht.

* Das primäre Feld einer Tabellenansicht wird immer gesperrt und kann nicht verschoben werden, es sei denn, Sie legen ein anderes Feld als primäres Feld fest.

* Sie können das Primärfeld in einer Spaltenüberschrift ändern, die nicht primär ist.

* Alle Tabellenansichten eines Datensatztyps haben dasselbe Primärfeld, das Sie auswählen.

Weitere Informationen finden Sie unter [Tabellenansicht verwalten](/help/quicksilver/maestro/views/manage-the-table-view.md).


### Maestro-Datensätze mit Adobe Experience Manager Assets verbinden

Vorschau: 14. Dezember 2023

Produktionsversion: geplant für den 15. Dezember 2023

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

Sie können jetzt nach einem Suchbegriff suchen, um schnell einen Datensatz in der Tabellenansicht zu finden. Sie können Suchbegriffe und Sonderzeichen in allen auf dem Bildschirm sichtbaren Feldern verwenden, um einen Datensatz zu finden. Weitere Informationen finden Sie unter [Tabellenansicht verwalten](../maestro/views/manage-the-table-view.md).

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
