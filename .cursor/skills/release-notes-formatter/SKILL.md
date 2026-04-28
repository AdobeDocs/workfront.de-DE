---
name: release-notes-formatter
description: Formatieren und validieren Sie die Versionshinweise zu Workfront, um Konsistenz, korrekte Struktur und ordnungsgemäße Verknüpfung zu gewährleisten. Wird nur für Versionshinweise in Produktversionsverzeichnissen verwendet oder wenn der Benutzer Versionshinweise, Produktversionen oder vierteljährliche Versionen erwähnt. Gilt nicht für Artikel mit Anleitungen oder allgemeine Dokumentationen.
source-git-commit: ec081e557ec48adcfcb3833bf11dcee91312ef4e
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 3%

---


# Formatierung von Versionshinweisen

Formatiert und validiert Adobe Workfront-Versionshinweise im `help/quicksilver/product-announcements/product-releases/`.

## Seitentypen

Identifizieren Sie den Seitentyp anhand des Dateipfads und Inhalts:

| Seitentyp | Dateimuster | Vorlage |
|-----------|-------------|----------|
| **Übersicht** | `{YY}-q{N}-release-overview.md` | [reference.md#overview](reference.md#overview-page-template) |
| **Produktbereich** | `{YY}-q{N}-{area}.md` | [reference.md#product-area](reference.md#product-area-page-template) |
| **Planung** | `planning-release-activity-{YY}-q{N}.md` | Ähnlich wie Produktbereich |
| **Look-and-Feel** | `look-and-feel-updates-{YY}-q{N}.md` | [reference.md#Look-and-Feel](reference.md#look-and-feel-page-template) |

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

5. **Hauptteil**: Funktionsbeschreibung und dann Link zur Hilfedokumentation

#### Übersichtsseiten

1. **H1**: `{Written Quarter} release overview`

2. **Einführungsabsatz** mit geplantem Veröffentlichungsmonat

3. **`>[!IMPORTANT]`-Block** mit Tabelle mit Freigabezeitplan

4. **H2-`Adobe Workfront enhancements`** mit Aufzählung von Anker-Links:

```markdown
* [Administrator enhancements](#administrator-enhancements)
* [Document enhancements](#document-enhancements)
```

5. **H3 pro Produktbereich** mit HTML-Funktionstabelle (siehe [reference.md](reference.md#overview-feature-table))
   - Innerhalb jeder Tabelle **Neueste Funktionen zuerst** - die neueste Zeile wird oben in der Tabelle angezeigt (nach der Kopfzeile)

6. **Nachfolgende Abschnitte** (H2): Versionshinweise für andere Bereiche, Desktop Proofing Viewer-Updates, Ankündigungen, API-Version, Wartungs-Updates, Schulungs-Updates

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

| Problem | Fehlerbehebung |
|-------|-----|
| Falscher Übersichtslink für Quartal | Aktualisierung entsprechend dem eigenen Quartal der Datei |
| Fehlender `>[!NOTE]` | Block nach H2-Funktionsüberschrift hinzufügen |
| Inkonsistentes Datumsformat | Standardisieren auf `Month Day, Year` |
| Fehlende leere Zeile vor `>[!NOTE]` | Leere Zeile hinzufügen |
| Zusätzliche Leerzeichen in Legendenlinien | Nachfolgende Leerzeichen kürzen |
| HTML in den Produktbereichsseiten | Als Markdown beibehalten (HTML dient nur zur Tabellenübersicht) |
| Fehlende `exl-id` | Lassen Sie es weg - erzeugen Sie keine |

## Konventionen für die Dateibenennung

| Typ | Muster | Beispiel |
|------|---------|---------|
| Überblick | `{YY}-q{N}-release-overview.md` | `26-q2-release-overview.md` |
| Produktbereich | `{YY}-q{N}-{area-slug}.md` | `26-q2-admin-and-setup.md` |
| Verzeichnis | `{YY}-q{N}-release-activity/` | `26-q2-release-activity/` |

Standardflächen-Schnecken: `admin-and-setup`, `documents`, `projects`, `reports`, `requests`, `other`

## Quartalszuordnung

| Quartal | Schriftform | Months |
|---------|-------------|--------|
| Q1 | Erstes Quartal | Jan-Mar |
| Q2 | Zweites Quartal | Apr-Jun |
| Q3 | Drittes Quartal | Jul-Sep |
| Q4 | viertes Quartal | Okt-Dez |

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

## Weitere Ressourcen

- Vollständige HTML-Vorlagen und -Beispiele finden Sie unter [reference.md](reference.md)
