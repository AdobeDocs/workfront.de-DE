---
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 1%
---
# Copilot-Anweisungen für workfront.de

Dieses Repository enthält die Adobe Workfront-Dokumentation in englischer Sprache. Die Regeln
Die folgenden Angaben gelten für jede Anfrage in diesem Arbeitsbereich. Themenspezifische Standards live in
`.github/instructions/*.instructions.md` und beim Bearbeiten automatisch laden
Übereinstimmende Dateien.

## Suche nach möglichen Artikeln, bevor neue erstellt werden

Wenn neue Inhalte eingehen - ein Eingangsdokument, Kunden- oder PM-Feedback, eine
Slack/Transkript-Einfügen, Screenshots mit Hinweisen oder Support-Fragen - **nicht
Schlagen Sie vor, zuerst einen neuen Artikel zu erstellen.** Repo und Oberflächenkandidat durchsuchen
Vorhandene Artikel, in die der Inhalt passen könnte.

Erforderlicher Workflow:

1. **Lesen Sie zuerst den neuen Inhalt** um Thema, Zielgruppe (Admin vs. Ende) zu identifizieren
Benutzer) und die spezifischen Fakten oder Schritte, die sie hinzufügt.
2. **Suche nach `help/` mit** und Dateisuche. Suchen Sie nach
Artikel, die bereits dieselbe Funktion, denselben Bereich oder denselben Workflow abdecken.
3. **Gibt eine Rangliste** Kandidatenartikel zurück (normalerweise 3-7), jeweils mit:
   - Der Dateipfad (als klickbarer Link).
   - Ein einzeiliger Grund dafür, dass es sich um einen Kandidaten handelt (in welchen Bereich würde er einpassen) oder warum
     Es ist die engste Übereinstimmung).
   - Alle Einschränkungen (z. B. „Zielgruppenabweichung„): Dies ist die Aufnahme durch den Endbenutzer.
     Admin-Facing„).
4. **Fragen Sie, wo Sie sie** können, bevor Sie sie entwerfen oder bearbeiten. Frage formulieren
explizit, zum Beispiel: „In welche davon soll ich mich einarbeiten?“ oder „Ich möchte
in #2 einfügen, oder denken Sie, dass es einen eigenen Artikel braucht?“
5. **Nur einen neuen Artikel vorschlagen** wenn kein vorhandener Artikel angemessen passt, und
Erklären Sie, warum keiner der Kandidaten funktioniert.

Selbst wenn der Inhalt „offensichtlich“ zu einem bekannten Artikel gehört, wird trotzdem 2-3 angezeigt
Alternativen, damit die Platzierung bestätigt werden kann. Dadurch werden Beinahe-Duplikate und
Orte, an denen der Inhalt bereits teilweise abgedeckt wurde.

## Änderungen vor der Bearbeitung von Hilfeartikeln vorschlagen

Wenn Sie im Begriff sind, einen `.md` Hilfeartikel unter `help/` zu bearbeiten, **bearbeiten Sie die Datei nicht.
Noch.** Zeigen Sie zunächst an, was Sie ändern möchten, und warten Sie auf die explizite Genehmigung.

Für jede Datei, die Sie berühren möchten:

1. Benennen Sie die Datei (Pfad).
2. Zeigen Sie die vorgeschlagene Änderung als umgrenzten Diff/Snippet — alten und neuen Text —
mit genügend Kontext, um eindeutig zu sein.
3. Geben Sie den Grund kurz an (ein Satz).
4. Beenden Sie mit einer expliziten Aufgabe, z. B. „Diese Änderungen anwenden?“ oder „Ich möchte
Fortfahren?“

Nur nach ausdrücklicher Genehmigung („ja“, „gehen“, „anwenden“, „tun“ usw.) Solltest du
Rufen Sie die Bearbeitungswerkzeuge auf.

Dies gilt für **alle** Bearbeitung eines Hilfeartikels `.md` Tippfehler, Link-Fehlerbehebungen,
Austausch einzelner Wörter, Terminologiebereinigung, neue Abschnitte und Neuschreibungen. Nein
Ausnahmen, es sei denn, der/die Benutzende sagt explizit „Just Fix it“ oder „Don&#39;t ask, just
Bearbeiten“ in der gleichen Runde.

Für Änderungen, die mehrere Artikel umfassen, gruppieren Sie die vorgeschlagenen Unterschiede nach Datei unter
Eine Antwort. Wenn der Satz groß ist, listen Sie zuerst die betroffenen Dateien mit einer einzeiligen Zusammenfassung auf
Danach werden jeweils Unterschiede in Batches angezeigt und vor jedem Batch bestätigt.

Dies blockiert **nicht** schreibgeschützte Forschung (grep, read) oder Entwurf/Untersuchung
Im Chat (keine Dateischreibvorgänge).

## Lücken intelligent schließen

Wenn die Absicht aus dem Kontext ersichtlich ist, verpflichten Sie sich zur Antwort auf die beste Vorgehensweise, anstatt
Präsentation der Optionsmenüs. Anwendung der Schreibstandards (siehe
`.github/instructions/writing-quality.instructions.md`) Proaktiv - nicht warten
Um daran erinnert zu werden, ihnen zu folgen. Ordnen Sie neuen Text dem des zugehörigen Artikels zu.
Überschriften, Terminologie und Struktur. Frag nur, wann eine echte Mehrdeutigkeit
Ändern Sie das Ergebnis.

## Git-Commit-Nachrichten

### Betreffzeile

- Ungefähr **50 Zeichen oder weniger**.
- Fassen Sie die Änderung in **Imperative Stimmung** zusammen („Hinzufügen…“, „Beheben…“, „Refaktorieren…„).

### Textkörper

- Lassen Sie eine leere Zeile nach dem Betreff vor dem Textkörper.
- Zeilenumbruch bei etwa **72 Zeichen**.
- Verwenden Sie **Erläuterung &quot;**&quot;. Jede Aufzählung muss genau mit beginnen.
Eines von:
  - **📖** — wenn die Änderung **fügt** etwas Neues hinzu: neue Dateien, neue Abschnitte, neue
    Funktionen, neue Kopfzeilen, neue Zeilen oder andere neue Inhalte.
  - **✏️** — wenn die Änderung **ändert** vorhandenes Werk: Änderungen an bestehenden Zeilen,
    Aktualisierungen vorhandener Abschnitte, Umgestaltungen oder Änderungen an aktuellen Inhalten.

Beispiel:

```
Add refresh token rotation to auth flow

- 📖 Add refresh_tokens table and Alembic migration for schema v3.
- ✏️ Update session middleware to rotate secrets and revoke old tokens.
```

## Pull-Anfragen

### Ableiten des Jira-Problems

- Leiten Sie die Jira-Problem-ID vom **aktuellen Git-Verzweigungsnamen“ ab** (z. B.
Segment Matching `FFENT-8796`).
- **Wenn der Zweigname eine Jira-ID enthält:** Sie diese ID im PR-Titel und Link.
Es ist in `# Context` → `## Jira`.
- **Wenn der Zweigname keine Jira-ID enthält:** Sie den Jira-Schlüssel aus dem PR
Titel. Schließen Sie weiterhin `## Jira` mit genau `No ticket` ein.

### PR-Titel

- **mit Jira ID:** `{type}/{JIRA-ID}- {short task description}`
  - Beispiel: `feat/FFENT-8001- Add validation for numVariations in OCAPI request`
- **Ohne Jira-ID:** `{type}- {short task description}`
  - Beispiel: `docs- Refresh Object Composite API changelog`

Übertragungstypen: **feat** (neue Funktion), **fix** (Fehlerbehebung), **refactor** (restructure
ohne Verhaltensänderung), **PERF** (Leistung), **Stil** (nur Formatierung),
**test** (tests), **docs** (nur Dokumentation, neue Inhalte), **build** (build/CI/
dependencies), **OPS** (Infrastruktur/Bereitstellung), **chore** (Verschiedenes).

### PR-Körper — erforderliche Abschnitte

- `# Summary` - kurzer Überblick über die Änderungen und die Gründe dafür.
- `# Changes` - nach Datei geordnet. Verwenden Sie für jede Datei, die berührt wurde, eine Überschrift der Ebene 2
mit dem Pfad in Backticks und dann Aufzählungspunkten.
- `# Context` — immer einen `## Jira` Unterabschnitt mit der verknüpften Anfrage einschließen oder
  `No ticket`.

```markdown
# Changes

## `path/to/file.ext`
* Concise bullet describing the change in that file.

# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```
