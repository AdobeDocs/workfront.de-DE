---
mode: agent
description: Entfernen Sie den Dokumentationsrahmen „Nur Vorschau“ von Workfront für allgemeine Verfügbarkeit - Textbausteinfragmente in der Vorschau, class=„preview“-HTML und parallele In-Preview- und In-Production-Schritte oder -Abschnitte im Vergleich.
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 1%
---

# Hervorhebung für Vorschau entfernen

Diesen Workflow nur ausführen, wenn ich Sie auffordere, die „Hervorhebung der Vorschau entfernen“ (oder die
Mit der gleichen Absicht). Es konvertiert Anleitungen/Referenzen mit Vorschau-Tags von Courtney-Autoren
Themen in GA-fähige Inhalte umbenannt.

## Umfang

Nur anwenden, wenn **alle** wahr sind:

1. Ich habe diesen Workflow aufgerufen.
2. Der Dateipfad enthält **nicht** `product-announcements` (ganz ausschließen)
Baumstruktur: Versionshinweise, Betas, Ankündigungen).
3. Die Datei wird unten nicht unter **Ausgeschlossene Pfade** aufgeführt.
4. Die Frontend-`author:`-Zeile enthält **`Courtney`** (als alleiniger oder Co-Autor).
5. Der Artikel weist mindestens eine der folgenden Eigenschaften auf:
   - Vorschau-Umgebungssprache in Textprosa- oder echten Snippet-Absätzen
     („hervorgehobene Informationen“, „Vorschau-Umgebung“, „noch nicht allgemein)
     Available“, Fast-Release Notes) — **keine Übereinstimmung** Link-Text allein auf einem
     Inhaltsverzeichnis-/Indexseite;
   - Jedes HTML-Element mit `class="preview"` (`<span>`, `<div>`, `<p>`, `<li>`…)
   - Eine Vorschau-Snippet-Variable wie `{{highlighted-preview}}` oder
     `{{highlighted-preview-article-level}}`.

Wenn der Umfang unklar ist, bestätigen Sie ihn vor der Bearbeitung.

**Inhaltsverzeichnis/Indexseiten - immer überspringen** wenn der einzige Vorschautext in einer
Der Anzeigetext des Markdown-Links verweist auf einen anderen Artikel, und die Datei enthält keinen
`class="preview"`, keine Snippet-Variablen und kein Vorschau-Textbaustein in Prosa
Außerhalb von Links.

### Ausgeschlossene Pfade

Inventarisieren oder bearbeiten Sie diese nie, es sei denn, ich überschreibe explizit:

- `help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/send-to-aem.md`
- `help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-manage-reports.md`

## Erforderlicher Workflow (menschlicher Workflow)

Keine Massenbearbeitung ohne Genehmigung durchführen.

1. **Inventar** - Erstellen einer sortierten Liste von im Umfang enthaltenen Pfaden (`help/`). weglassen
   `product-announcements`, ausgeschlossene Pfade und reine Inhaltsverzeichnisangaben.
2. **Start** - Fragen Sie, ob mit dem ersten Artikel (oder einem Pfad-I-Namen) begonnen werden soll.
3. **Pro Artikel — zuerst anzeigen, nach OK bearbeiten** — Datei lesen, Änderungen vorschlagen als
Vor/nach Ausschnitten oder fokussiertem Diff, dann auf explizite Genehmigung warten.
4. **Nach jeder Datei** - Fragen Sie, ob Sie zur nächsten (oder STOP/SKIP) wechseln möchten.

## Inhaltsregeln (Vorschauinhalt wird zum Dokument)

Ziel: Das Verhalten für die Vorschau dokumentieren, „in Produktion“ veraltet lassen
Verzweigungen erstellen und dann Beschriftungen und Wrapper entfernen, die nur für die Vorschau gelten.

- **Parallele Schritte**: Entfernen des Schritts „In Produktion“; „In Vorschau“ beibehalten
den Inhalt des Schritts, ihn jedoch neu formulieren, sodass er nicht vorschauspezifisch ist. Nummerierung korrigieren. If
Keine klare Parallele, stoppen und fragen, welcher Block beibehalten werden soll.
- **Parallele Abschnitte**: Entfernen des Abschnitts „Produktionsumgebung“, Ersetzen
mit dem Inhalt des Vorschaubereichs, neutralisieren Sie dann den Vorschautext und entfernen Sie ihn
  `class="preview"`.
- **Hinweise zu Snippets und Top-of-Article**: Entfernen Sie den Textbaustein „Nur Vorschau“ und
Sätze, deren einziger Zweck die Verfügbarkeit einer Vorschau ist.
- **`class="preview"`**: Anfangs- und End-Tags entfernen, inneren Inhalt beibehalten.
Listen-/Tabellenstruktur beibehalten; fehlerhafte Listen oder fehlerhafte Leerzeichen beheben.
- **Auskommentierte Abschnitte (`<!-- … -->`)**: Ändern Sie sie nur, wenn ich sie explizit
Sag es. Wenn der Vorschauinhalt nur in Kommentaren angezeigt wird, rufen Sie ihn auf und stellen Sie Fragen.
Standard: Kommentare bleiben unverändert.

## Nicht

- Auf `product-announcements` oder ausgeschlossenen Pfaden ausführen.
- Automatisch auskommentierte Blöcke bearbeiten.
- „Vorschau“ entfernen, wenn es sich um einen Produktnamen in einem anderen Kontext (z. B. Vorschau) handelt
Sandbox-Umgebung) - Fragen Sie nach, wenn Sie sich nicht sicher sind.
- Ändern Sie die `author:` oder nicht verwandte Schriftart.
- Überspringen Sie den Schritt Anzeigen → Genehmigen .

## Qualitätsprüfungen vor der Präsentation von Bearbeitungen

- Keine weiteren `class="preview"` im vereinbarten Umfang.
- Keine verwaisten doppelten Überschriften oder fehlerhaften Schrittnummern.
- Einführung liest sich korrekt für GA (nicht „nur in der Vorschau“ für ausgelieferte Funktionen).
