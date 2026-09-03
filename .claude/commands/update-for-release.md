---
name: update-for-release
description: ""
source-git-commit: 4c2305da7635694d9d7bc174b5837a0d57fb7ac0
workflow-type: tm+mt
source-wordcount: '2009'
ht-degree: 0%

---


# Aktualisierung für Version (Workfront)

Diese Fähigkeit führt Sie durch die Aktualisierung von Workfront-Hilfeartikeln für eine bevorstehende Funktionsveröffentlichung. Der Workflow ist das Gegenteil von `remove-preview-highlighting`: den Artikeln wird neues Verhalten hinzugefügt, als Vorschau markiert und (später bei GA) von dieser anderen Fähigkeit bereinigt.

## Umfang

Anwenden, wenn **alle** wahr sind:

1. Der Benutzer aktualisiert Workfront-Hilfeartikel für eine Funktion, die im Lieferumfang enthalten ist (normalerweise zuerst in der Vorschau).
2. Mit der Änderung wird ein neues Verhalten oder eine neue Benutzeroberfläche eingeführt, keine GA-Bereinigung. Verwenden Sie für die GA-Bereinigung **remove-preview-highlighting**.
3. Die Datei ist **kein** Versionshinweis. Verwenden Sie für Versionshinweise **release-notes-formatter**.
4. Der Nutzer hat Funktionskontext angegeben: mindestens eine Kurzbeschreibung und einen Screenshot; idealerweise eine PRD-URL (Adobe Wiki).

Wenn der Umfang unklar ist, bestätigen Sie dies, bevor Sie beginnen.

## Erforderlicher Workflow (menschlicher Workflow)

**Sie** Repository nicht massenweise. Jeweils einen Artikel verschieben. Fragen Sie nach jedem Artikel, ob Sie mit dem nächsten fortfahren möchten.

### &#x200B;1. Erfassen des Funktionskontexts

Bestätigen Sie mit dem Benutzer:

- **Was hat sich geändert** (1-2 Sätze Zusammenfassung des neuen Verhaltens oder Benutzeroberfläche).
- **Screenshot(s** der neuen Benutzeroberfläche. Falls vorhanden, speichern Sie unter dem `assets/` des Zielartikels mit einem beschreibenden Dateinamen für Kebab-Fälle (z. B. `add-custom-message.png`). Falls nicht angegeben, fragen Sie, ob auf einen gewartet werden soll, oder fahren Sie mit einer Platzhalterreferenz fort.
- **PRD URL** (Adobe Wiki), falls verfügbar. Rufen Sie sie mit dem `user-Adobe Wiki Confluence` MCP-Tool `get_wiki_content` ab. Lesen Sie es, um Verhalten zu finden, das der Benutzer in der Benutzeroberfläche nicht sehen kann: Nebeneffekte von Benachrichtigungen, was passiert, wenn etwas später bearbeitet oder hinzugefügt wird, nicht angezeigte Zeichenbeschränkungen, Berechtigungen usw.
- **Verfügbarkeit**: Nur Vorschau, Vorschau + Schnellfreigabe oder bereits allgemein verfügbar. Dies steuert die Snippet-Auswahl in Schritt 3.
- **Explizite**: Alle Artikel, die der Benutzer überspringen möchte (z. B. „diese Funktion ist nicht in Vorlagen enthalten„).

### &#x200B;2. Betroffene Artikel inventarisieren

Durchsuchen Sie das Repository mit den Keywords des Funktionsbereichs (z. B. `approval workflow`, `document approval`, die spezifische Feldbezeichnung). Erstellen einer Kandidatenliste:

- Artikel mit Anleitungen in der entsprechenden `help/quicksilver/.../`.
- Übersichtsartikel und FAQs, die den Funktionsbereich erwähnen.
- **Ausschließen** `product-announcements/` (in den Versionshinweisen wird eine andere Fähigkeit verwendet).
- **Ausschließen** Inhaltsverzeichnis-/Indexseiten, bei denen nur der Link-Text zu einem anderen Artikel erwähnt wird.
- **Ausschließen** Artikel, die der Benutzer in Schritt 1 überspringen wollte.

Zeigen Sie dem Benutzer die Kandidatenliste an. Fragen Sie, welche aktualisiert und welche übersprungen werden sollen. Querverweis `help/quicksilver/TOC.md`, wenn ein gleichrangiger Artikel fehlt.

### &#x200B;3. Auswahl des Vorschau-Snippets

`help/_includes/snippets.md` lesen und nach Verfügbarkeit auswählen:

| Verfügbarkeit | Snippet |
| --- | --- |
| Nur Vorschau - hervorgehobener Inhalt ist neu in einem Artikel mit ansonsten allgemeiner Verfügbarkeit | `{{highlighted-preview}}` |
| Nur Vorschau - der gesamte Artikel ist neu | `{{highlighted-preview-article-level}}` |
| Vorschau + Schnellfreigabe-Kunden, allgemein | `{{preview-fast-release-general}}` |

Wenn für das aktuelle Quartal bereits ein versionsspezifisches Snippet vorhanden ist, sollten Sie dieses dem generischen Snippet vorziehen. Bestätigen Sie die Auswahl mit dem Benutzer, bevor Sie sie anwenden.

### &#x200B;4. Pro Artikel - zuerst anzeigen, nach OK bearbeiten

Für jeden Artikel in der vom Benutzer bestätigten Liste:

1. **Lies die Datei.**

2. **Bestimmen des Hervorhebungsmusters.** Fragen Sie den Benutzer, der zu diesem Artikel passt (die Antwort kann je nach Artikel unterschiedlich sein):

   - **Duplizierung pro Abschnitt**: Hängen Sie `in Production` an die vorhandene Abschnittsüberschrift an. Fügen Sie einen neuen Abschnitt hinzu, an den `in Preview` angehängt und der in `<div class="preview"> ... </div>` eingeschlossen ist. Verwenden Sie , wenn das neue Verhalten das Verfahren selbst bedeutsam ändert - zusätzliche oder neu angeordnete Schritte, ein neues Bild oder eine andere Schrittbeschreibung. Typisch für Anleitungen.
   - **Duplizierung pro Zeile**: Für eine tabellenbasierte Feldbeschreibung, bei der sich nur eine Zeile ändert und der Rest der Tabelle/Prozedur unverändert bleibt, lassen Sie die vorhandene Zeile byte für byte unverändert und fügen Sie direkt danach eine neue `<tr class="preview">` hinzu. Weben Sie keine neuen Sätze in die ursprüngliche Zeile. Siehe „Duplizierung pro Zeile“ unter Inhaltsregeln für die genauen Konventionen.
   - **Einzelzeilenumbruch**: Fügen Sie den neuen Satz/die neuen Sätze inline innerhalb des vorhandenen Abschnitts ein, umschlossen in `<span class="preview"> ... </span>`. Verwenden Sie diese Option, wenn es sich beim Hinzufügen um ein oder zwei Sätze handelt, die natürlich in einen vorhandenen Absatz oder eine häufig gestellte Frage passen (keine Tabellenzeile, sondern Duplizierung pro Zeile für diese Sätze).
   - **Gemischt**: Einige Abschnitte im selben Artikel verwenden unterschiedliche Muster für unterschiedliche Inhalte. Diese Option wird angezeigt, wenn im Artikel prozedurale Tabellen, Abschnitte im FAQ-Stil und einfache Absätze kombiniert werden.

3. **Der Ausschnitt** unmittelbar nach der Überschrift H1 mit einer Leerzeile über und unter eine eigene Zeile setzen. Das Snippet befindet **vor** Einführungsabsatz.

4. **Sammeln Sie neue Details in „immer einschließen“ vs. „zur Überprüfung bereit“.** Dies ist der wichtigste Schritt.

   - **Immer einschließen** (automatisch anwenden, keine Eingabeaufforderung): unsichtbare Verhaltensweisen, die der Benutzer bei der Interaktion mit der Benutzeroberfläche nicht beobachten kann. Beispiele:
     - Nebeneffekte (z. B. „wenn Sie diese Einstellung ändern, wird die E-Mail erneut an alle Teilnehmer gesendet„)
     - Verhalten bei anderen Objekten oder späteren Ereignissen
     - Voraussetzungen und Berechtigungen
     - Beschränkungen werden nicht in der Benutzeroberfläche angezeigt
     - Alles, was Benutzende nur von der PRD, den Dokumenten oder dem Produkt-Team lernen können
   - **Zur Überprüfung bereitstellen** (Benutzenden mit `AskQuestion` als Mehrfachauswahl präsentieren): Fakten, die Benutzende bei Verwendung der Funktion auf dem Bildschirm sehen können. Beispiele:
     - Ein Zeichenzähler, den die Benutzeroberfläche bereits anzeigt (z. B. `0 / 500`)
     - Der standardmäßige erweiterte/reduzierte Status eines Felds
     - Standardmäßiger ausgewählter Status eines sichtbaren Kontrollkästchens
     - Beschriftungen der Schaltfläche neben dem Feld
     - Validierungsnachrichten, die inline angezeigt werden

   Geben Sie für jedes „Zur Überprüfung bereitstehende“ Element eine Ein-Satz-Begründung an („Hilft Anfängern, eine längere Nachricht zu planen“, „Hilft Benutzern, die sie in späteren Phasen nicht sehen, zu wissen, um sie zu erweitern„). Nur die Elemente einbeziehen, die der Benutzer auswählt. Das Standardprinzip lautet: „Wenn der Benutzer die Aufgabe auf dem Bildschirm sehen kann, muss sie nicht neu formuliert werden“ - aber der Benutzer erhält den endgültigen Aufruf.

   **Wenn Sie die tatsächlichen Sätze**, wenden Sie für jeden Behälter `~/.cursor/skills/writing-quality/SKILL.md` Sprach- und Tonregeln an, während Sie schreiben - eine einfache Feld-/Verhaltensbeschreibung, keinen Changelog-Eintrag („wurde entfernt“, „wurde hinzugefügt„) und stellen Sie keine unveränderte Anweisung erneut her, nur um eine Vorschau-Anmerkung anzufügen. Zeichnen Sie es beim ersten Mal richtig, anstatt den Ton in einem späteren Durchgang zu fixieren.

5. **Erfüllen Sie den Entwurf, bevor Sie** Text anzeigen. Dies ist ein Sicherheitsnetz, nicht das erste Mal, dass diese Regeln gelten - fangen Sie alles, was bei Schritt 4 verpasst wurde (Redundanz, Ton, Sprachabweichung mit den umgebenden Zeilen).

6. **Änderungen vorschlagen.** Vor-/Nach-Ausschnitten (oder einer fokussierten Beschreibung im Diff-Stil) für den Artikel anzeigen, die Folgendes behandeln: Platzierung von Ausschnitten, Umbenennungen von Überschriften, neue In-Preview-Inhalte und wo sie sich befinden, Screenshot-Referenz und etwaige Inline-`class="preview"`-Umbrüche.

7. **Warten Sie auf die explizite Genehmigung** („okay“, „Apply“, „yes„), bevor Sie die Datei schreiben.

8. **validate.** Führen Sie nach dem Schreiben die `ReadLints` für die Datei aus und melden Sie etwaige Probleme. Lesen Sie den geänderten Abschnitt erneut, um die Struktur zu bestätigen.

### &#x200B;5. Nach jedem Artikel

Frage, ob zum nächsten Artikel übergegangen werden soll, ob der aktuelle Artikel gestoppt, übersprungen oder erneut aufgerufen werden soll.

### &#x200B;6. Ende der Sitzung - Versionshinweise kopieren/einfügen

Wenn der Benutzer die Sitzung beendet (sagt „Done“, „Das war&#39;s“, „Stopp“ oder lehnt es ab, zum nächsten Artikel fortzufahren), fragen Sie:

> „Möchten Sie einen Eintrag mit Versionshinweisen zum Kopieren/Einfügen für die Seite mit der Verbesserung?“

Wenn ja, generieren Sie einen Entwurfseintrag mit dem Funktionskontext aus Schritt 1 und dem in dieser Sitzung aktualisierten primären Hilfeartikel. **Schreiben Sie sie nicht in eine Datei** — geben Sie sie nur als Text zum Kopieren/Einfügen an.

Formatieren Sie den Eintrag so, dass er zur Seitenstruktur des Produktbereichs der Qualifikation **Versionshinweise-Formatierer** passt:

```markdown
## {Feature name}

>[!NOTE]
>
>Preview: {date or TBD}
>Production fast release: {date or TBD}
>Production for everyone: {date or TBD}

{1–3 sentences describing what changed and why it helps users. Lead with the benefit, not the UI action.}

For more information, see [{Primary article title}](/help/quicksilver/{path-to-article}.md).
```

Regeln:

- Verwenden Sie `TBD` für alle noch nicht bekannten Datumsangaben. Fragen Sie den Benutzer, ob er über die Datumsangaben verfügt.
- Der Funktionsname ist die Groß-/Kleinschreibung des Satzes (wobei nur das erste Wort und die Eigennamen großgeschrieben werden).
- Die Beschreibung sollte sich auf das konzentrieren, was Benutzende jetzt tun können, und nicht auf die Implementierungsdetails.
- Link zum spezifischsten aktualisierten Artikel mit Anleitungen, keine Übersichtsseite.
- Wenn alle Datumsangaben unbekannt sind und der/die Benutzende keine Platzhalter verwenden möchte, `>[!NOTE]` Sie einen Datumsblock nicht ein. Lassen Sie ihn weg und beachten Sie, dass er später hinzugefügt werden muss.

## Inhaltsregeln

### Überschriften

- Hängen Sie genau **`in Production`** an vorhandene Abschnittsüberschriften an, die als Referenz auf der Produktionsseite beibehalten werden.
- Hängen Sie genau **`in Preview`** an neue Abschnittsüberschriften an.
- Behalten Sie den Rest der Überschrift in Großbuchstaben bei (pro `writing-quality`).

### Vorschau von Wrappers

- **Section-level**: in `<div class="preview"> ... </div>` einschließen. Platzieren Sie öffnende und schließende Tags in eigenen Zeilen mit einer leeren Zeile über und unter jedem Tag, sodass Markdown-Überschriften und -Listen innerhalb weiterhin gerendert werden.
- **Inline (Satzebene)**: Betätigen Sie den `<span class="preview"> ... </span>` innerhalb des vorhandenen Absatzes, der Tabellenzelle oder der FAQ-Antwort.
- Verschachteln Sie niemals einen `<span class="preview">` in einem `<div class="preview">`.

### Duplizierung pro Zeile

Für eine tabellenbasierte Feldbeschreibung, bei der sich nur das *Verhalten* des Felds ändert (nicht die umgebende Prozedur):

- Lassen Sie die vorhandene `<tr>` vollständig unverändert - sie steht nun für das aktuelle/Produktionsverhalten. Spleißt nie neue Sätze oder spannt sich nicht darin ein.
- Fügen Sie direkt danach eine neue Zeile hinzu:

  ```html
  <tr class="preview">
  <td><span class="preview"><strong>{new label} in preview</strong></span></td>
  <td><span class="preview">{self-contained description}</span></td>
  </tr>
  ```

- **Beschriftung**: Verwenden Sie nicht nur die ursprüngliche Feldbeschriftung und fügen Sie `(in Preview)` an. Schreiben Sie eine kurze, natürliche Beschriftung für die neue Funktion selbst (z. B. ursprüngliche Beschriftung „Namen oder E-Mails hinzufügen“ → neue Beschriftung „Personen oder Teams hinzufügen„) und hängen Sie dann `in preview` ohne Klammern an: „Personen oder Teams in der Vorschau hinzufügen“.
- **Beschreibung**: Schreiben Sie eine neue 1-3 Satz Beschreibung nur des neuen Verhaltens, in der vorhandenen Stimme des Artikels. Verwenden Sie die Sätze der ursprünglichen Zeile nicht wieder als Grundlage und fügen Sie Ergänzungen hinzu - die neue Zeile muss als vollständige, eigenständige Beschreibung gelesen werden.
- **Ergänzende Anmerkungen**: Hängen Sie mit einem `<br>` Zeilenumbruch an, gefolgt von `Note:` auf der nächsten Zeile, innerhalb derselben `<span class="preview">` — verschachteln Sie keine `<p>Note: ...</p>`. Da die neue Zeile eigenständig ist, sollten Sie hier alle noch relevanten Fakten aus der Anmerkung der ursprünglichen Zeile kurz neu angeben, anstatt anzunehmen, dass der Leser sie auch gesehen hat (z. B. eine Einschränkung im erweiterten Modus „jeweils eine offene Phase“, die gleichermaßen für die neue Zeile gilt).
- **Mehrere Varianten**: Wenn dasselbe Feld in mehr als einer Prozedur im selben Artikel aktualisiert wird (Standard vs. Erweitert, Legacy vs. ESM usw.) und das zugrunde liegende Verhalten tatsächlich unterschiedlich ist (z. B. behält Legacy einen Opt-in-Standardwert bei, während ESM immer erweitert wird), schreiben Sie jede Zeile so, dass sie dem tatsächlichen Verhalten dieser Variante entspricht. Kopieren Sie nicht den Text einer Variante in die Zeile einer anderen.

### Platzierung von Snippets

- Die Ausschnittlinie verläuft unmittelbar nach der H1, wobei oben und unten eine Leerzeile angezeigt wird.
- Snippet befindet **vor** dem Einführungsabsatz, dem `>[!IMPORTANT]` Callout und allen Zugriffsanforderungsblöcken.
- Ein Ausschnitt pro Artikel.

### Screenshots

- Speichern Sie neue Screenshots im `assets/`-Ordner des Artikels mit einem beschreibenden Dateinamen für Kebab-Fälle.
- Verweisen Sie im neuen Abschnitt In-Preview auf den neuen Screenshot. Wenn der Screenshot eines produktionsinternen Abschnitts die Funktion nicht mehr korrekt widerspiegelt, lassen Sie sie an Ort und Stelle - sie stellt dennoch das Produktionsverhalten bis zur allgemeinen Verfügbarkeit dar.
- Erstellen Sie keine Screenshot-Dateinamen; wenn noch kein Screenshot bereitgestellt wurde, fragen Sie den Benutzer.
- **Platzhalter für einen noch nicht vorhandenen Screenshot**: Wenn der/die Benutzende fortfahren möchte, ohne auf das Asset zu warten, fügen Sie einen HTML-Kommentar direkt nach der vorhandenen (Produktions-) Screenshot-Referenz hinzu und verwenden Sie diesen Dateinamen wieder mit einem `-v2` Suffix:

  ```html
  <!--
  preview screen![{same alt text}](assets/{existing-filename}-v2.png)
  -->
  ```

  Tauschen Sie die echte Referenz ein (und heben Sie die Auskommentierung auf), sobald der Screenshot bereitgestellt wurde.

### Hinweise und Tipps

- Maximal eine `>[!NOTE]` (oder `>[!TIP]`, `>[!IMPORTANT]`, `>[!WARNING]`) pro Abschnitt. Wenn der vorhandene Abschnitt bereits über eine Anmerkung verfügt, kombinieren Sie verwandte neue Inhalte in derselben Anmerkung als Aufzählungsliste, anstatt sie zu stapeln.

### Was nicht tun

- Artikel unter `product-announcements/` nicht bearbeiten.
- Führen Sie keine Massenbearbeitung durch, sondern wählen Sie jeweils nur einen Artikel mit expliziter Genehmigung aus.
- Schließen Sie keine Tatsachen der beobachtbaren Benutzeroberfläche ein, ohne sie zuerst dem Benutzer zu zeigen.
- Ändern Sie keine Inhalte in `<!-- ... -->` HTML-Kommentaren, es sei denn, der/die Benutzende sagt ausdrücklich dazu.
- Ändern Sie keine `author:` oder nicht verwandten Frontend-Felder.

## Qualitätsprüfungen vor der Präsentation von Bearbeitungen

Führen Sie diese vollständige Checkliste für **jeden** Artikel in der Sitzung aus - einschließlich sekundärer Artikel, bei denen Sie „nur eine Aufzählungszeichen hinzufügen“, nicht nur den ersten/primären.

- Das Snippet erscheint einmal in einer eigenen Zeile nach dem H1, mit Leerzeilen über und unter.
- Vorhandene Abschnittsüberschriften enden mit `in Production`.
- Neue Abschnittsüberschriften enden mit `in Preview` und der Abschnitt befindet sich innerhalb von `<div class="preview">`.
- Inline-Ergänzungen befinden sich in `<span class="preview">`.
- Duplikate pro Zeile: Das ursprüngliche `<tr>` ist byte-für-byte unverändert; das neue `<tr class="preview">` enthält beide Zellen in `<span class="preview">` umschlossen; die Beschriftung ist eine neue kurze Beschriftung + Kleinbuchstaben „in der Vorschau“ (nicht die ursprüngliche Beschriftung + „(in der Vorschau)„); jede zusätzliche Anmerkung verwendet `<br>` + `Note:` inline, keine verschachtelte `<p>`.
- Wenn dasselbe Feld in mehr als einer Prozedurvariante angezeigt wird (Standard/Erweitert, Legacy/ESM), entspricht der Wortlaut jeder neuen Zeile dem tatsächlichen Verhalten dieser Variante, anstatt von einer anderen Variante kopiert zu werden.
- Die neue mit einer Vorschau markierte Prosa liest sich wie ein einfaches Feld/eine Verhaltensbeschreibung, kein Änderungsprotokolleintrag und ändert nicht redundant eine unveränderte Anweisung.
- `ReadLints` ist in der bearbeiteten Datei sauber.
- Der Artikel wird in beiden Zuständen korrekt gelesen (mit ein- und ausgeblendetem Vorschauinhalt).

## Referenzen

- Workfront-Dokumentationsstil: Siehe die Kenntnisse **Schreibqualität** bei `~/.cursor/skills/writing-quality/SKILL.md`.
- Snippet-Katalog: `help/_includes/snippets.md` im Dokumentations-Repository.
- GA-Bereinigung (inverser Workflow): Siehe die Qualifikation **Entfernen-Vorschau-Hervorhebung** unter `.cursor/skills/remove-preview-highlighting/SKILL.md`.
- Adobe Wiki MCP für PRDs: `user-Adobe Wiki Confluence`, Tool `get_wiki_content`.
