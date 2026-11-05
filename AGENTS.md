---
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%
---
# AGENTS.md

Agentenanleitung für das Repository **workfront.de** (Adobe Workfront Englisch
Dokumentation). Diese Datei verweist auf die kanonischen Anweisungen, sodass jeder Agent —
Unabhängig davon, welche Konventionsdatei sie liest — befolgt dieselben Regeln.

## Kanonische Befehlsdateien

- **Repo-weite Regeln**: [.github/copilot-instructions.md](.github/copilot-instructions.md)
— Suche nach Bewerbern/Artikeln, offer-before-edit, commit-message und PR-Format,
und „Lücken intelligent schließen.“
- **Schreibstandards** (gilt automatisch für `help/**/*.md`):
  [.github/instructions/writing-quality.instructions.](.github/instructions/writing-quality.instructions.md),
mit allen Details in
  [.cursor/skills/writing-quality/reference.md](.cursor/skills/writing-quality/reference.md).
- **Versionshinweise** (gilt automatisch für `product-announcements/product-releases/**`):
  [.github/instructions/release-notes-formatter.instructions.](.github/instructions/release-notes-formatter.instructions.md).
- **Bereinigung in der Vorschau-Hervorhebung** (On-Demand-Workflow):
  [.github/prompts/remove-preview-highlighting.prompt.](.github/prompts/remove-preview-highlighting.prompt.md).

## Nicht übertragbare Verhaltensweisen

1. **Finden Sie mögliche Artikel, bevor Sie neue erstellen.** Wenn neue Inhalte eingehen
Suchen Sie in nach einer Rangliste vorhandener Artikel, die `help/` passen könnten, und öffnen Sie sie.
Fragen Sie dann, wohin es gehört, bevor Sie es entwerfen.
2. **Änderungen vorschlagen, bevor Hilfe `.md` Artikel bearbeitet wird.** Vorgeschlagene anzeigen
Diff und warten auf die explizite Genehmigung. Die einzige Ausnahme ist, wenn ich sage „nur reparieren
Es“ oder „Nicht fragen, nur bearbeiten“ in der gleichen Reihe. Schreibgeschützte Forschung und In-Chat
Die Formulierungen sind immer in Ordnung.
3. **Lücken intelligent schließen.** Wenn die Absicht klar ist, verpflichten Sie sich zur
Best-Practice-Antwort und Übereinstimmung mit den Überschriften des zugehörigen Artikels,
Terminologie und Struktur statt der Darstellung von Optionsmenüs.
4. **Wenden Sie die Schreibstandards proaktiv** jede `help/` Bearbeitung an - warten Sie nicht
Zur Erinnerung.

## Konventionen für Bestätigung und Veröffentlichung

Die vollständige Version finden [&#128279;](.github/copilot-instructions.md) unter .github/copilot-instructions.md
Commit-Nachrichtenformat (unbedingter Betreff ≤ ~50 Zeichen; 📖 für Ergänzungen, ✏️ für
Änderungen) und PR-Struktur (Jira-ID aus dem Zweignamen; `# Summary`,
`# Changes` nach Datei, `# Context` → `## Jira`).
