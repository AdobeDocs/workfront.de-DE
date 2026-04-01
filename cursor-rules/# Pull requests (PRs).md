---
source-git-commit: b3148e5706abd75f2dd260f32507dedf8e259f57
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---
# Pull-Anforderungen (PRs)

Befolgen Sie diese Konventionen, wenn Sie einen Titel oder eine Beschreibung für eine Pull-Anfrage entwerfen oder überprüfen (z. B. in GitHub/GitLab oder wenn Sie im Agenten-Chat gefragt werden).

## Ableiten des Jira-Problems

- **Source der Wahrheit:** Leitet die Jira-Problem-ID vom **aktuellen Git-Verzweigungsnamen“ ab** z. B. einem Segment, das dem Projektschlüsselmuster entspricht, z. B. `FFENT-8796`).
- **Wenn der Zweigname eine Jira-ID enthält:** Verwenden Sie diese ID im PR-Titel (siehe unten) und verknüpfen Sie sie in `# Context` → `## Jira`.
- **Wenn der Zweigname keine Jira-ID enthält:** Behandeln Sie den PR als nicht mit einem Ticket verknüpft. **Lassen Sie** Jira-Schlüssel aus dem PR-Titel aus (erfinden Sie kein Ticket). Schließen Sie weiterhin `# Context` → `## Jira` mit dem Inhalt genau ein: `No ticket` (kein Link).

## PR-Titel

**Wenn der Zweigname eine Jira-Problem-ID enthält** schließen Sie **beide** ein:

1. Die **Jira-Problem-ID** (z. B. `FFENT-8001`).
2. Der **Commit-Typ** (siehe Liste unten), wobei dieses Muster verwendet wird:

`{type}/{JIRA-ID}- {short task description}`

Beispiel:

`feat/FFENT-8001- Add validation for numVariations in OCAPI request`

Verwenden Sie nach der ID eine knappe Beschreibung im Imperativ-Stil . Passen Sie das angezeigte Leerzeichen an: Typ, Schrägstrich, Jira-Schlüssel mit nachfolgendem Bindestrich, Leerzeichen, dann die Beschreibung.

**Wenn der Zweigname keine Jira-Problem-ID enthält** lassen Sie das Ticket im Titel weg und verwenden Sie:

`{type}- {short task description}`

Beispiel:

`docs- Refresh Object Composite API changelog`

### Akzeptable Commit-Typen (verwenden Sie genau diese Beschriftungen vor der `/`)

- **feat** - Fügt eine neue Funktion hinzu. Wenn ein neues Inhaltsverzeichniselement hinzugefügt oder die JIRA mit einer anderen `feat` Jira verbunden wird.
- **fix** - Behebt einen Fehler
- **refactor** - Schreibt/restrukturiert Code ohne Verhaltensänderung
- **PERF** - Verbessert die Leistung (Spezial-Refaktorierung)
- **style** — Nur Formatierung/Leerzeichen; keine Änderung der Bedeutung. Nur Bearbeitungen
- **Test** - Fügt Tests hinzu oder korrigiert sie
- **docs** - Neuer Inhalt hinzugefügt. Nur Dokumentation
- **build** - Build-Tools, CI, Abhängigkeiten, Projektversion usw.
- **OPS** - Infrastruktur, Bereitstellung, Sicherung, Wiederherstellung usw.
- **chore** — Verschiedenes (z. B. `.gitignore`)

## PR-Körper — erforderliche Abschnitte

Verwenden **genau diese Abschnitte der obersten Ebene** (Markdown-Überschriften):

### 1. `# Summary`

Kurzer Überblick über **Was** und **Warum** (geschäftliche oder technische Absicht).

### 2. `# Changes`

Organisieren nach **Datei**. Verwenden Sie für jede Datei, die Sie berührt haben, eine Überschrift der Stufe 2 mit dem Pfad in Backticks und dann Aufzählungspunkte zur Beschreibung der Bearbeitungen.

Format:

```markdown
# Changes

## `path/to/file.ext`
* Concise bullet describing the change in that file.

## `another/file.ts`
* Another bullet for that file.
```

### 3. `# Context`

Fügen Sie unter &quot;**&quot; immer** Unterabschnitt `# Context`Jira“ ein.

**Wenn der Verzweigungsname eine Jira-ID enthält:** Verwenden Sie einen anklickbaren Link zu dem Problem (leiten Sie den Schlüssel vom Verzweigungsnamen ab).

Format:

```markdown
# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

Ersetzen Sie den Schlüssel und die URL durch das eigentliche Ticket. Wenn mehrere Tickets gelten, listen Sie jedes in einer eigenen Zeile im selben Unterabschnitt auf.

**Wenn der Zweigname keine Jira-ID enthält:** Behalten Sie `## Jira` bei und verwenden Sie genau:

```markdown
# Context

## Jira
No ticket
```

## Beispiel (vollständige PR-Beschreibung)

```markdown
# Summary
Adds minimum and maximum constraints for numVariations in the Object Composite API v4 OpenAPI spec.

# Changes

## `static/object-composite-v4.json`
* numVariations in OCAPIRequest now includes minimum: 1 and maximum: 3 to align with the allowed range (number of variations to generate).

# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

## Beispiel (vollständige PR-Beschreibung, Verzweigung ohne Jira-ID)

**Titel:** `docs- Refresh Object Composite API changelog`

```markdown
# Summary
Refreshes the changelog for the Object Composite API.

# Changes

## `CHANGELOG.md`
* Documents the latest OCAPI v4 constraint updates.

# Context

## Jira
No ticket
```
