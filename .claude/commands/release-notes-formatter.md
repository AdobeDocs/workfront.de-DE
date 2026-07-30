---
name: release-notes-formatter
description: Formatieren und validieren Sie die Versionshinweise zu Workfront, um Konsistenz, korrekte Struktur und ordnungsgemäße Verknüpfung zu gewährleisten. Wird nur für Versionshinweise in Produktversionsverzeichnissen verwendet oder wenn der Benutzer Versionshinweise, Produktversionen oder vierteljährliche Versionen erwähnt. Gilt nicht für Artikel mit Anleitungen oder allgemeine Dokumentationen.
source-git-commit: fa39320af72acf6d2ceaf201480baf78a07ae76e
workflow-type: tm+mt
source-wordcount: '1729'
ht-degree: 2%

---


# Formatierung von Versionshinweisen

Formatiert und validiert Adobe Workfront-Versionshinweise im `help/quicksilver/product-announcements/product-releases/`.

## Seitentypen

Identifizieren Sie den Seitentyp anhand des Dateipfads und Inhalts:

| Seitentyp | Dateimuster | Vorlage |
|-----------|-------------|----------|
| **Übersicht** | `{YY}-q{N}-release-overview.md` | Siehe .claude/commands/_release-notes-formatter-reference.md#overview-page-template |
| **Produktbereich** | `{YY}-q{N}-{area}.md` | Siehe .claude/commands/_release-notes-formatter-reference.md#product-area-page-template |
| **Planung** | `planning-release-activity-{YY}-q{N}.md` | Ähnlich wie Produktbereich |
| **Look-and-Feel** | `look-and-feel-updates-{YY}-q{N}.md` | Siehe .claude/commands/_release-notes-formatter-reference.md#look-and-feel-page-template |

## Schritt 0: Quartal bestimmen (vor allen anderen Schritten)

>[!IMPORTANT]
>
>Weisen Sie niemals eine Funktion einem Dokumentquartal zu, indem Sie Kalenderquartalsmathematik an seinem Vorschau- oder Produktionsdatum verwenden. Das Dokument-Quartal basiert auf der **monatlichen Version** in der die Funktion gemäß der internen Gruppierung des Veröffentlichungskalenders von Workfront bereitgestellt wird, die gegenüber dem Kalenderquartal versetzt ist - siehe die Tabelle [2026](#2026-release-calendar)Veröffentlichungskalender am Ende dieser Datei. Beispielsweise gehört eine Funktion mit dem Produktionsdatum 13. August 2026 in das `26-q4` des Dokumentquartals und nicht `26-q3`, da die monatliche Version vom August `26-q4` zugeordnet ist.
>
>Die Tabelle „Quartalszuordnung“ weiter unten (geschriebene Form/Monate) dient zum Schreiben von Quartalsnamen in Titel (z. B. „Drittes Quartal“ für Q3) - sie ist **nicht** ausreichend, um zu entscheiden, zu welchen Quartalsdateien eine Funktion gehört. Führen Sie vor dem Erstellen oder Bearbeiten einer Datei einen Abgleich mit der Tabelle des Veröffentlichungskalenders durch.
>
>Wenn das Produktionsdatum einer Funktion nicht in der Tabelle des Veröffentlichungskalenders angezeigt wird (z. B. wenn es außerhalb des Datumsbereichs der Tabelle liegt), bitten Sie den Benutzer um einen aktualisierten Kalender, anstatt ihn zu erraten.

## Formatierungs-Workflow

### Schritt 1: Validieren von FrontMatter

Erforderliche Felder für alle Versionshinweisseiten:

```yaml
---
title: <descriptive title>
description: <matches or summarizes the title>
author: <author name>
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: <existing UUID — never generate or change>
---
```

Regeln:
- `feature` muss genau `Product Announcements` sein
- `recommendations` muss genau `noDisplay, noCatalog` sein
- Nie einen `exl-id` erfinden - nur einbeziehen, wenn bereits einer existiert
- `draft: Probably` nicht zu echten Seiten hinzufügen (nur Vorlagen)

### Schritt 2: Struktur nach Seitentyp überprüfen

#### Produktbereichsseiten

1. **H1**: `{Written Quarter} {Area} enhancements`
   - Beispiel: `# Second Quarter 2026 Administrator enhancements`
   - Quartal muss ausgewiesen werden: „Erstes Quartal“, „Zweites Quartal“, „Drittes Quartal“, „Viertes Quartal“

2. **Einführungsabsatz**: Beschreibt den Bereich und Links zur Übersicht
   - Muss eine Verknüpfung zur Übersichtsdatei **richtigen Quartals** herstellen
   - Häufige Fehler: Verlinken auf das vorherige Quartal (z. B. `26-q1` statt `26-q2`)

3. **H2 pro Funktion**: Funktionstitel als Überschrift
   - **Neueste Funktionen zuerst** - Die neueste Versionshinweise müssen als erster H2 nach dem Einführungsabsatz angezeigt werden
   - Ältere Merkmale folgen in umgekehrter chronologischer Reihenfolge

4. **Callout-Block für Datum** nach jedem H2:

```markdown
>[!NOTE]
>
>Preview: {Month Day, Year}
>Production fast release: {Month Day, Year}
>Production for everyone: {Month Day, Year}
```

&#x200B;5. **Hauptteil**: Funktionsbeschreibung und dann Link zur Hilfedokumentation

#### Übersichtsseiten

1. **H1**: `{Written Quarter} release overview`

2. **Einführungsabsatz** mit geplantem Veröffentlichungsmonat

3. **`>[!IMPORTANT]`-Block** mit Tabelle mit Freigabezeitplan

4. **H2-`Adobe Workfront enhancements`** mit Aufzählung von Anker-Links:

```markdown
* [Administrator enhancements](#administrator-enhancements)
* [Document enhancements](#document-enhancements)
```

&#x200B;5. **H3 pro Produktbereich** mit HTML-Funktionstabelle (siehe .claude/commands/_release-notes-formatter-reference.md#overview-feature-table)
   - Innerhalb jeder Tabelle **Neueste Funktionen zuerst** - die neueste Zeile wird oben in der Tabelle angezeigt (nach der Kopfzeile)

&#x200B;6. **Nachfolgende Abschnitte** (H2): Versionshinweise für andere Bereiche, Desktop Proofing Viewer-Updates, Ankündigungen, API-Version, Wartungs-Updates, Schulungs-Updates

### Schritt 3: Validieren von Links

- **Übersichts-Link in Produktbereichsseiten**: Muss auf dasselbe Quartal verweisen
  - Richtig: `26-q2-release-activity/26-q2-release-overview.md`
  - Falsch: `26-q1-release-activity/26-q1-release-overview.md`
- **Links in der Übersicht verankern**: Muss mit den H3-IDs übereinstimmen (Kleinbuchstaben, Bindestriche)
- **Funktionsverknüpfungen in Übersichtstabellen**: Muss `class="MCXref xref" xrefformat="{para}"` verwenden
- **Hilfe-Dokumentlinks**: Muss mit `/help/quicksilver/` beginnen

### Schritt 4: Daten validieren

- Format: `{Month} {Day}, {Year}` (z. B. „12. März 2026„)
- `TBD` für unbekannte Daten verwenden
- Datumsangaben im Seitenblock `>[!NOTE]` Produktbereichs müssen mit der entsprechenden Übersichtstabellenzeile übereinstimmen
- Vorschaudaten sollten vor Produktionsdaten liegen

### Schritt 5: Allgemeine Fehlerbehebungen

Wenden Sie diese Korrekturen bei der Formatierung an:

| Problem | Korrigieren |
|-------|-----|
| Falscher Übersichtslink für Quartal | Aktualisierung entsprechend dem eigenen Quartal der Datei |
| Fehlender `>[!NOTE]` | Block nach H2-Funktionsüberschrift hinzufügen |
| Inkonsistentes Datumsformat | Standardisieren auf `Month Day, Year` |
| Fehlende leere Zeile vor `>[!NOTE]` | Leere Zeile hinzufügen |
| Zusätzliche Leerzeichen in Legendenlinien | Nachfolgende Leerzeichen kürzen |
| HTML in den Produktbereichsseiten | Als Markdown beibehalten (HTML dient nur zur Tabellenübersicht) |
| Fehlende `exl-id` | Lassen Sie es weg - erzeugen Sie keine |

### Schritt 6: Inhaltsverzeichnis aktualisieren

Wenn Sie eine **neue** Versionshinweisseite (Übersicht oder Produktbereich) erstellen, fügen Sie sie in derselben Änderung zu `help/quicksilver/TOC.md` hinzu. Eine Seite, die nicht im Inhaltsverzeichnis enthalten ist, wird nicht in der veröffentlichten Navigation angezeigt, selbst wenn die Links in der Übersichtstabelle darauf verweisen.

Wo sie hinzugefügt werden soll:

- Das Inhaltsverzeichnis hat einen Abschnitt pro Quartal unter einer Überschrift wie `* 2026 Q3 Release {#release-26-q3}`. Wenn die Überschrift für das Quartal noch nicht vorhanden ist (erste Seite eines neuen Quartals), fügen Sie sie über dem vorherigen Quartal hinzu, sodass das neueste Quartal oben ist.
- Listen Sie unter der Überschrift „Quartal“ die Seiten in dieser Reihenfolge auf:
  1. **Übersicht** zuerst (`Third Quarter 2026 release overview`).
  2. **Produktbereichsseiten** alphabetisch nach Bereichsnamen (Administrator, Dokumente, Unternehmensvorgänge, Projekte, Berichterstellung, Anforderung).
  3. **Weitere Verbesserungen** zuletzt (immer nach den alphabetischen Produktbereichen).

Jeder Inhaltsverzeichniseintrag ist ein Markdown-Link unter Verwendung des Seitentitels und des absoluten Repository-Pfads:

```markdown
      * [Third Quarter 2026 Documents enhancements](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-documents.md)
```

Einzug (sechs Leerzeichen) an die umgebenden Einträge anpassen. Verwenden Sie die Seite H1 wörtlich als Link-Text - z. B. `Documents enhancements`, `Requesting enhancements` (nicht `Requests`) -, damit die Inhaltsverzeichniskennzeichnungen mit früheren Quartalen übereinstimmen.

Häufige Fehler, die zu vermeiden sind:

- Erstellen einer Produktbereichsseite ohne Hinzufügen zum Inhaltsverzeichnis
- Link zur Übersicht eines anderen Quartals von der neuen Produktbereichsseite (Schritt 3).
- Einfügen der Seiten eines neuen Quartals unter der Überschrift des vorherigen Quartals.

### Schritt 7: Startseite aktualisieren

Wenn Sie eine **Übersichtsseite eines neuen Quartals** erstellen (d. h. dies ist die erste Seite eines neuen Quartals, nicht nur eine neue Produktbereichsseite, die zu einem vorhandenen Quartal hinzugefügt wird), aktualisieren Sie `help/quicksilver/home.md` in derselben Änderung:

- Ersetzen Sie im Abschnitt `>[!TAB Latest release]` den Link Versionsübersicht durch den Link Übersicht des neuen Quartals.
- Aktualisieren Sie auch in diesem Abschnitt den Link der Adobe Workfront Planning-Versionsaktivität , sodass er auf die Planungsdatei (`planning-release-activity-{YY}-q{N}.md`) des neuen Quartals verweist, falls eine vorhanden ist.
- Fügen Sie auf der Registerkarte `>[!TAB {YYYY} releases]` für das aktuelle Jahr den Link Überblick für das neue Quartal oben in der Liste hinzu, oberhalb des Eintrags für das vorherige Quartal.

Berühren Sie `home.md` nicht, wenn Sie nur eine Produktbereichsseite zu einem Quartal hinzufügen, in dem bereits eine Übersichtsseite aufgeführt ist.

Häufige Fehler, die zu vermeiden sind:

- Erstellen der Übersichtsseite eines neuen Quartals ohne Aktualisierung der Registerkarte „Neueste Version“ von `home.md` (es verweist weiterhin auf das alte Quartal).
- Es wird vergessen, das neue Quartal auch zur Registerkartenliste des aktuellen Jahres hinzuzufügen.

## Konventionen für die Dateibenennung

| Typ | Muster | Beispiel |
|------|---------|---------|
| Überblick | `{YY}-q{N}-release-overview.md` | `26-q2-release-overview.md` |
| Produktbereich | `{YY}-q{N}-{area-slug}.md` | `26-q2-admin-and-setup.md` |
| Verzeichnis | `{YY}-q{N}-release-activity/` | `26-q2-release-activity/` |

Standardflächen-Schnecken: `admin-and-setup`, `documents`, `projects`, `reports`, `requests`, `other`

## Quartalszuordnung

>[!NOTE]
>
>Diese Tabelle dient zum Schreiben von Quartalsnamen (z. B. in einen H1- oder Titel). Es wird NICHT bestimmt, zu welchen Quartalsdateien eine Funktion gehört — verwenden Sie dazu die unten stehende Tabelle [2026](#2026-release-calendar)Versionskalender“, da das Dokumentenquartal gegenüber dem Kalenderquartal versetzt ist.

| Quartal | Schriftform | Months |
|---------|-------------|--------|
| Q1 | Erstes Quartal | Jan-Mar |
| Q2 | Zweites Quartal | Apr-Jun |
| Q3 | Drittes Quartal | Jul-Sep |
| Q4 | viertes Quartal | Okt-Dez |

**Wichtig - das Dokumentenquartal, das in Dateinamen (`26-q3`, `26-q4` usw.) verwendet wird ist um einen Monat ab dieser Kalenderzuordnung versetzt.** Stattdessen folgt sie der Workfront-internen Gruppierung „Veröffentlichungskalender“, wobei jedes Dokumentenquartal = die beiden vorangehenden monatlichen Versionen + der vierteljährliche Veröffentlichungsmonat ist. Beispielsweise umfasst das Dokumentenquartal `26-q3` die monatlichen Versionen vom Mai/Juni/Juli 2026 (vierteljährliche Version `2026.07`) und das Dokumentenquartal `26-q4` die monatlichen Versionen vom August/September/Oktober 2026 (vierteljährliche Version `2026.10`). Überprüfen Sie immer den unten stehenden Veröffentlichungskalender (oder fragen Sie nach einem aktualisierten Kalender), bevor Sie das Quartal einer Datei basierend auf der Kalenderquartalstabelle oben annehmen.

## Versionskalender 2026

Source: „Monthly Release Calendar 2026“ (Adobe Corp Wiki, AWF Space — `wiki.corp.adobe.com`, Space Key AWF, Titel: „2026 Monthly Release Calendar„). WebFetch kann diese Seite nicht erreichen (erfordert Adobe SSO). Bitten Sie den Benutzer, eine aktualisierte PDF/Tabelle einzufügen, wenn Datumsangaben erforderlich sind, die über das hier erfasste hinausgehen.

| Monat der Veröffentlichung | Abschließende Vorschau | Produktion | Monatliche Version | Vierteljährliche Veröffentlichung | Dokumentquartal |
|---|---|---|---|---|---|
| November 2025 | &#x200B;30. Oktober 2025 | &#x200B;13. November 2025 | 2025.11 | 2026.01 | &#x200B;26. Quartal 1 |
| Dez. 2025 | &#x200B;27. November 2025 | &#x200B;11. Dezember 2025 | 2025.12 | 2026.01 | &#x200B;26. Quartal 1 |
| Januar 2026 | &#x200B;23. Dezember 2025 | &#x200B;15. Januar 2026 | 2026.01 | 2026.01 | &#x200B;26. Quartal 1 |
| Februar 2026 | &#x200B;29. Januar 2026 | &#x200B;12. Februar 2026 | 2026.02 | 2026.04 | &#x200B;26. Quartal 2 |
| März 2026 | &#x200B;26. Februar 2026 | &#x200B;12. März 2026 | 2026.03 | 2026.04 | &#x200B;26. Quartal 2 |
| Apr 2026 | 02-Apr-2026 | &#x200B;16. April 2026 | 2026.04 | 2026.04 | &#x200B;26. Quartal 2 |
| Mai 2026 | &#x200B;30. April 2026 | &#x200B;14. Mai 2026 | 2026.05 | 2026.07 | &#x200B;26. Quartal 3 |
| Juni 2026 | &#x200B;28. Mai 2026 | &#x200B;11. Juni 2026 | 2026.06 | 2026.07 | &#x200B;26. Quartal 3 |
| Juli 2026 | &#x200B;07. Juli 2026 | &#x200B;16. Juli 2026 | 2026.07 | 2026.07 | &#x200B;26. Quartal 3 |
| Aug. 2026 | &#x200B;30. Juli 2026 | &#x200B;13. August 2026 | 2026.08 | 2026.10 | &#x200B;26. Quartal 4 |
| Sept. 2026 | 03-Sep-2026 | &#x200B;17. September 2026 | 2026.09 | 2026.10 | &#x200B;26. Quartal 4 |
| Oktober 2026 | 01-Okt-2026 | &#x200B;15. Oktober 2026 | 2026.10 | 2026.10 | &#x200B;26. Quartal 4 |
| November 2026 | &#x200B;29. Oktober 2026 | &#x200B;12. November 2026 | 2026.11 | 2027.01 | &#x200B;27. Quartal 1 |
| Dez. 2026 | &#x200B;26. November 2026 | &#x200B;10. Dezember 2026 | 2026.12 | 2027.01 | &#x200B;27. Quartal 1 |
| Januar 2027 | &#x200B;05. Januar 2027 | &#x200B;14. Januar 2027 | 2027.01 | 2027.01 | &#x200B;27. Quartal 1 |

Hinweise zur Verwendung dieser Tabelle:

- **Endgültige Vorschau** ist das letzte Datum, an dem Funktionen in der Vorschau für diese monatliche Version angezeigt werden können - verwenden Sie diese für das Aufzählungszeichen „Letztes Datum, an dem Funktionen in der Vorschau-Umgebung angezeigt werden können“ auf der Übersichtsseite (nur Viertelendmonat).
- **Production** ist das offizielle „Production-for-everyone“-Datum für diese monatliche Veröffentlichung.
- Für den Monat mit Quartalsende (der mit der Spalte für die vierteljährliche Veröffentlichung übereinstimmt) listet die Planungstabelle der Übersichtsseite die Version dieses Monats **zweimal** auf: einmal in der Spalte für die monatliche Veröffentlichung vom **einen Tag vor** dem Produktionsdatum (das Datum der schnellen Veröffentlichung) und einmal in der Spalte für die vierteljährliche Veröffentlichung vom tatsächlichen Produktionsdatum. Nicht-endgültige Monate in einem Quartal verwenden dasselbe Produktionsdatum sowohl in der monatlichen Auflistung als auch in den „Fast Release“-Referenzen - keine Anpassung erforderlich.
- Diese Tabelle läuft nur bis Januar 2027. Wenn spätere Termine benötigt werden, bitten Sie den Benutzer um einen aktualisierten Kalender, anstatt ihn zu erraten.

Die vierteljährliche Produktionsfreigabe erfolgt normalerweise am Donnerstag der zweiten vollen Woche des letzten Monats des Quartals.

## Validierungs-Checkliste

Überprüfen Sie beim Überprüfen einer Versionshinweisdatei Folgendes:

- [ ] Frontmatter enthält alle erforderlichen Felder mit korrekten Werten
- [ ] H1 entspricht dem Seitentyp-Format
- [ ] Link Überblick verweist auf das richtige Quartal
- [ ] Jede Funktion verfügt über einen `>[!NOTE]` Datumsblock (Produktbereichsseiten)
- [ ] Datumsformat ist konsistent (`Month Day, Year`)
- [ ] Funktionstabellen-Zeilen in der Übersicht stimmen mit dem Inhalt der Produktbereichsseite überein
- [ ] Keine fehlerhaften internen Links
- [ ] Anker-Links in der Übersicht stimmen mit den IDs im Abschnitt H3 überein
- [ ] Funktionen werden als „Newest-First“ sortiert (Produktbereichsseiten und Übersichtstabellen)
- [ ] Neue Versionshinweise werden in `help/quicksilver/TOC.md` unter dem richtigen Quartal aufgeführt, wobei die Übersicht zuerst und die Produktbereiche in alphabetischer Reihenfolge aufgeführt werden (Sonstige Letzte)
- [ ] Wenn die Übersichtsseite eines neuen Quartals erstellt wurde, verweisen `help/quicksilver/home.md` Registerkarte „Neueste Version“ und die Registerkarte des aktuellen Jahres darauf

## Weitere Ressourcen

- Vollständige HTML-Vorlagen und -Beispiele finden Sie unter .claude/commands/_release-notes-formatter-reference.md
