---
source-git-commit: 44629631cd2d99eadbed5fd81cf33458b13702af
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---
# Suche nach möglichen Artikeln, bevor neue erstellt werden

Wenn Courtney neue Inhalte einbindet - ein Eingangsdokument, Kunden- oder PM-Feedback, eine Slack-/Transkripteinfügung, Screenshots mit Notizen, Support-Fragen -, **schlagen Sie nicht vor, zuerst einen neuen Artikel zu erstellen.** Durchsuchen Sie das Repository und öffnen Sie die vorhandenen Artikel, in die der Inhalt passen könnte.

## Erforderlicher Workflow

1. **Lesen Sie zuerst den neuen Inhalt** um das Thema, die Zielgruppe (Administrator vs. Endbenutzer) und die spezifischen Fakten/Schritte, die hinzugefügt werden, zu identifizieren.
2. **`help/` nach Kandidaten suchen** mit grep und find. Suchen Sie nach Artikeln, die bereits dieselbe Funktion, denselben Bereich oder denselben Workflow abdecken.
3. **Gibt eine Rangliste** Kandidatenartikel zurück (normalerweise 3-7), jeweils mit:
   - Der Dateipfad (klickbarer Backtick-Pfad).
   - Ein einzeiliger Grund, warum es sich um einen Kandidaten handelt (in welchen Abschnitt es sich einfügen würde oder warum es die engste topische Übereinstimmung ist).
   - Alle Einschränkungen (z. B. „Zielgruppenabweichung - Endbenutzer, Aufnahme richtet sich an Administratoren„).
4. **Fragen Sie Courtney, wo Sie es hintun möchten** bevor Sie es entwerfen oder bearbeiten. Formulieren Sie die Frage explizit, z. B.: „In welche davon soll ich mich einarbeiten?“ oder „Soll ich es in #2 einfügen, oder braucht es einen eigenen Artikel?“
5. **Schlagen Sie nur einen neuen Artikel vor** wenn kein vorhandener Artikel angemessen passt, und erklären Sie, warum keiner der Kandidaten funktioniert.

Selbst wenn der Inhalt „offensichtlich“ in einen bekannten Artikel gehört, werden dennoch 2-3 Alternativen angezeigt, damit Courtney die Platzierung bestätigen kann. Dadurch werden Beinahe-Duplikate und Stellen erfasst, an denen der Inhalt bereits teilweise abgedeckt war.

---

# Änderungen vor der Bearbeitung von Hilfeartikeln vorschlagen

Wenn Sie im Begriff sind, einen `.md` Hilfeartikel unter `help/` zu bearbeiten, **bearbeiten Sie die Datei noch nicht**. Zeigen Sie zunächst an, was Sie ändern möchten, und warten Sie auf die explizite Genehmigung.

Für jede Datei, die Sie berühren möchten:

1. Benennen Sie die Datei (Pfad).
2. Zeigen Sie die vorgeschlagene Änderung als eingezäunten Diff/Snippet - alten und neuen Text - mit genügend Umgebungskontext, um eindeutig zu sein.
3. Geben Sie den Grund kurz an (1 Satz).
4. Beenden Sie mit einer expliziten Frage, z. B. „Werden diese Änderungen übernommen?“ oder „Soll ich fortfahren?“

Erst nachdem Courtney ja sagt (oder „los“, „bewerben“, „machen“ usw.) Sie sollten die Bearbeitungswerkzeuge aufrufen.

Dies gilt für **alle** Bearbeitungen eines Hilfeartikels `.md` Tippfehler, Link-Fehlerbehebungen, Austausch einzelner Wörter, Terminologiebereinigungen, neue Abschnitte und Neuschreibungen. Keine Ausnahme, es sei denn, Courtney sagt in derselben Runde explizit „nur reparieren“ oder „nicht fragen, nur bearbeiten“.

Für Änderungen, die mehrere Artikel umfassen: Gruppieren Sie die vorgeschlagenen Unterschiede nach Datei unter einer Antwort. Wenn der Satz groß ist, listen Sie die betroffenen Dateien zuerst mit jeweils einer 1-zeiligen Zusammenfassung auf, zeigen Sie dann Unterschiede in Batches an und bestätigen Sie sie vor jedem Batch.

Dies blockiert **nicht** die schreibgeschützte Recherche (grep, read) oder das Entwerfen/die Untersuchung in Chat (keine Dateischreibvorgänge).

---

# Git-Commit-Nachrichten

Folgen Sie beim Entwerfen oder Generieren einer Git-Commit-Nachricht diesem Format.

## Betreffzeile

- Ungefähr **50 Zeichen oder weniger**.
- Fassen Sie die Änderung in **Imperative Stimmung** (z. B. „Hinzufügen…“, „Beheben…“, „Refaktorieren…„) zusammen.

## Textkörper

- Lassen Sie eine leere Zeile nach dem Betreff vor dem Textkörper.
- Zeilenumbruch bei etwa **72 Zeichen**.
- Verwenden Sie **Erläuterung &quot;**&quot;. Jeder Aufzählungszeichen muss mit genau einem der folgenden Elemente beginnen:
   - **📖** - Wird verwendet, wenn die Änderung **etwas Neues**: neue Dateien, neue Abschnitte, neue Funktionen, neue Kopfzeilen, neue Zeilen oder andere neue Inhalte.
   - **✏️** - Wird verwendet, wenn die Änderung **ändert** Bestehendes Werk: Bearbeitungen an vorhandenen Zeilen, Aktualisierungen vorhandener Abschnitte, Umgestaltungen oder Änderungen am aktuellen Inhalt.

Beispiel:

```
Add refresh token rotation to auth flow

- 📖 Add refresh_tokens table and Alembic migration for schema v3.
- ✏️ Update session middleware to rotate secrets and revoke old tokens.
```

---

# Pull-Anforderungen (PRs)

## Ableiten des Jira-Problems

- Leiten Sie die Jira-Problem-ID vom **aktuellen Git-Verzweigungsnamen** ab (z. B. einem Segment-Matching-`FFENT-8796`).
- **Wenn der Zweigname eine Jira-ID enthält:** Verwenden Sie diese ID im PR-Titel und verknüpfen Sie sie in `# Context` → `## Jira`.
- **Wenn der Zweigname keine Jira-ID enthält:** Sie den Jira-Schlüssel aus dem PR-Titel aus. Schließen Sie weiterhin `## Jira` mit genau: `No ticket` ein.

## PR-Titel

**mit Jira ID:** `{type}/{JIRA-ID}- {short task description}`
Beispiel: `feat/FFENT-8001- Add validation for numVariations in OCAPI request`

**Ohne Jira-ID:** `{type}- {short task description}`
Beispiel: `docs- Refresh Object Composite API changelog`

### Commit-Typen

- **feat** - Fügt eine neue Funktion hinzu
- **fix** - Behebt einen Fehler
- **refactor** - Schreibt/restrukturiert Code ohne Verhaltensänderung
- **PERF** - Verbessert die Leistung
- **style** — Nur Formatierung/Leerzeichen; keine Änderung der Bedeutung
- **Test** - Fügt Tests hinzu oder korrigiert sie
- **docs** — Nur Dokumentation, neue Inhalte hinzugefügt
- **build** - Build-Tools, CI, Abhängigkeiten, Projektversion
- **OPS** - Infrastruktur, Bereitstellung, Sicherung, Wiederherstellung
- **chore** — Verschiedenes (z. B. `.gitignore`)

## PR-Körper — erforderliche Abschnitte

### `# Summary`
Kurzer Überblick darüber, was sich geändert hat und warum.

### `# Changes`
Organisiert nach Datei. Verwenden Sie für jede Datei, die Sie berührt haben, eine Überschrift der Stufe 2 mit dem Pfad in Backticks und dann Aufzählungspunkte.

```markdown
# Changes

## `path/to/file.ext`
* Concise bullet describing the change in that file.
```

### `# Context`
Fügen Sie immer einen `## Jira` Unterabschnitt hinzu.

```markdown
# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

Oder wenn kein Ticket vorliegt: `No ticket`
