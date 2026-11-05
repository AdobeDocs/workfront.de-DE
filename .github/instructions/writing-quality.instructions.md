---
description: Technische Schreibstandards von Workfront für Hilfeartikel. wendet das Workfront-Stil-Handbuch für Dokumentationen und die Grundsätze zur Entwicklung technischer Qualitätsinformationen (DQTI) an.
applyTo: "help/**/*.md"
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 1%
---

# Schreibqualität

Wenden Sie diese Standards an, wenn Sie einen Hilfeartikel bearbeiten, überprüfen oder schreiben.
Bewahren Sie die Absicht und technische Genauigkeit des Autors auf. Für die vollständige
Interpunktion, Terminologie, Großschreibung und Verfahrensreferenz, Lesen
[.cursor/skills/writing-quality/reference.md](../../.cursor/skills/writing-quality/reference.md).

Wenden **diese** nicht auf Versionshinweise unter an.
`help/quicksilver/product-announcements/product-releases/` - Verwenden Sie die
Anweisungen für release-notes-formatter.

## Stimme und Standpunkt

- Verwenden Sie **zweite Person** („Sie können…„) beim Adressieren des Lesers.
- Benutze Kontraktionen für einen Gesprächston (nicht, nicht, nicht, es ist, sie sind).
- Verwenden Sie „Wir empfehlen“ für Best Practices - nicht „Es wird empfohlen“ oder „Sie sollten“.
- Wenn Sie für eine Benutzergruppe schreiben, verweisen Sie auf andere Rollen in der dritten Person.
- Benutze nie geschlechtsspezifische Pronomina - strukturiere den Satz um oder verwende „sie“.
- Kein Schrägstrich für Auswahlmöglichkeiten - verwenden Sie „oder“ („er oder sie“ oder nicht „er/sie„).

## Klarheit (DQTI)

- Eine Idee pro Satz; Sätze unter ~25 Wörtern halten, wo möglich.
- Führen Sie mit der Aktion oder dem Ergebnis, nicht mit dem Hintergrundkontext.
- Verwenden Sie das einfachste Wort („Verwenden“ nicht „Verwenden“, „Starten“ nicht „Initiieren„).
- Nominalisierungen vermeiden („Erstellen“ statt „Erstellen von„).
- Verwenden Sie eine spezifische, konkrete Sprache - vermeiden Sie vage Begriffe („mehrere“, „verschiedene„).
- Vermeiden Sie doppelte Negative.

## Konkretheit und Aufgabenorientierung (DQTI)

- Verwenden Sie spezifische Beispiele mit realistischen Werten, benennen Sie exakte UI-Elemente und -Felder.
- Konzentrieren Sie sich darauf, was der Benutzer tun **, nicht darauf, was das System *ist*.
- Lead-Prozeduren mit Verben des Typs „Aufgabe erstellen“, „Benachrichtigungen konfigurieren“
- Geben Sie genügend Kontext zum Handeln, aber nicht mehr.
- Fügen Sie einen Link zu einer ausführlichen Hilfe hinzu („Weitere Informationen finden Sie [ „Artikel].„).

## Großschreibung

- **Überschriften**: Der Satz ist immer „Aufgabe erstellen“, nicht „Aufgabe erstellen“.
- **Workfront-Begriffe**: Wird nur großgeschrieben, wenn direkt auf ein Benutzeroberflächenelement verwiesen wird.
  - Direkt: „Füllen Sie das Feld Geplantes Abschlussdatum aus.“
  - Indirekt: „Jede Aufgabe muss ein geplantes Abschlussdatum haben.“
  - Tipp: Wenn Sie „das“ oder „a“ vor den Begriff stellen können, wird er in der Regel in Kleinbuchstaben geschrieben.
- **Schaltflächen**: Folgen Sie der Groß-/Kleinschreibung der Benutzeroberfläche; Schaltflächen mit nur Großbuchstaben werden zu Satzbuchstaben.
- **Roles**: „Systemadministrator“ für die Rolle in der Benutzeroberfläche; &quot;Workfront
Administrator“ für die Person an.

## Überschriften

- Imperative Befehle in Satzbuchstaben, aufgabenbasiert („Zugriffsebenen konfigurieren„).
- Übersichtsartikel enden mit „Overview“ („Projects overview„).
- Unterteilen Sie lange Abschnitte in mehrere Überschriften mit klaren Unterzielen.

## Querverweise und Links

| Situation | Format |
|-----------|--------|
| Link nach der Angabe von Informationen | „Weitere Informationen finden Sie unter [Artikelname].“ |
| Link ohne vorherige Info | „Weitere Informationen finden Sie unter [Artikelname].“ |
| Link zu einem Abschnitt in einem anderen Artikel | „Weitere Informationen finden Sie unter [Abschnittsname] in [Artikelname].“ |
| Link zu einem Abschnitt im selben Artikel | „Weitere Informationen finden Sie unter [Abschnittsname] in diesem Artikel.“ |

- In einem Absatz: inline. In einem Verfahrensschritt: In einer neuen Zeile nach dem Schritt.
- Mehrere Links: Verwenden Sie eine Aufzählungsliste.
- Verwenden Sie „obere rechte Ecke“ / „obere linke Ecke“ für Bildschirmpositionen.

## Fett- und Kursiv-Formatierung

- **Fett** anklickbare Aktionen und Benutzeroberflächenelemente **nur in Verfahrensschritten**.
- Keine fett gedruckten UI-Elemente, Dialogfeldnamen, Seitennamen, Symbolnamen oder Menüs
Namen außerhalb von Verfahrensschritten.
- Verwenden Sie *kursiv* für Text, den der Benutzer eingeben soll („Typ *my.workfront.com*…„).
- Verwenden Sie niemals Kursiv für die Hervorhebung - strukturieren Sie stattdessen den Satz um.

## Hinweise, Tipps und Warnungen

Sparsam benutzen - Überbeanspruchung macht sie unsichtbar.

- Maximal ein Hinweis/Tipp/Warnhinweis pro Abschnitt; stapeln Sie sie niemals.
- Verknüpfte Notizen zu einer Notiz mit Aufzählungsliste kombinieren.
- Verwenden Sie keine Notizen, um neue Funktionen anzukündigen - überarbeiten Sie stattdessen den Artikeltext.

| Typ | Zweck |
|------|---------|
| `>[!NOTE]` | Informationen, die nicht zum Absatz passen; Versionierung/Kompatibilität |
| `>[!TIP]` | Nice-to-have Vorschläge, die dem Benutzer das Leben erleichtern |
| `>[!IMPORTANT]` | Wichtige Informationen für den Schritt oder das Verfahren |
| `>[!WARNING]` | Benutzer auf möglichen Datenverlust hinweisen |

## Vorgänge

- Verwenden Sie Befehlsüberschriften des Typs „Imperative“. Einführungen nur bei Bedarf.
- Bevorzugtes Intro-Format: Infinitivsatz + Doppelpunkt („So erstellen Sie ein temporäres
Kennwort:„).
- Für einstufige Vorgänge wird weiterhin eine nummerierte Liste verwendet.
- Verwenden Sie „type“ oder „select“ - vermeiden Sie vage Wörter wie „set“ oder „specified“.
- Bedingte Schritte: „(Bedingt) Wenn Sie Mitglied mehrerer Teams sind,
Wählen Sie …“. Optionale Schritte: „(Optional) Um ein Emoji hinzuzufügen, klicken Sie auf …“.
- Beschreiben Sie die Systemantwort, bevor oder unmittelbar danach.
- Mehrere Methoden: Dokumentieren Sie zunächst den einfachsten Weg und verwenden Sie dann „Oder“.
- Menü-/Registerkartennavigation: „Klicken Sie auf **E** > **Benachrichtigungen**&quot; (fett gedruckte Namen, nicht
Klammern; Leerzeichen um Klammern). Keine Klammern für Hauptmenü verwenden
Navigation - Verwenden Sie das Hauptmenü-Snippet.

## Interpunktions-Kurzanleitung

| Regel | Beispiel |
|------|---------|
| Oxford-Komma immer | „Motiv, Mittel und Chance“ |
| Komma vor „then“ in Prozeduren | „Klicken Sie auf Setup und dann auf Schnittstelle.“ |
| Komma nach Jahr in einer Datummitte | „Die Ausgabe vom 2. Januar 2016…“ |
| Kein Komma, nur für Monat und Jahr | „Januar 2016“ |
| Doppelpunkt vor einer Liste, Kleinbuchstaben nach | „Wählen Sie eine der folgenden Optionen aus: Option A“ |
| Kein Doppelpunkt nach den Verfahrensüberschriften | „Aufgabe erstellen“ |
| Em stricht sparsam | Strukturieren Sie den Satz nach Möglichkeit um |
| Punkte in Dateierweiterungen | „PDF-Datei hochladen“ |

## Organisation (DQTI)

- Logische Struktur mit progressiver Offenlegung (Übersicht → Details → Referenz).
- Ein Thema pro Abschnitt; Verwenden von Listen für mehr als 3 parallele Elemente.
- Listenelemente und deren Einführung grammatisch parallel halten.
- Verwenden Sie Tabellen für strukturierte Vergleiche oder Feldbeschreibungen.
- Vermeiden Sie Textwandabsätze - unterteilen Sie sie in verdauliche Abschnitte.

## Validierungs-Checkliste

- [ ] Zweite Person im Ganzen, Kontraktionen verwendet.
- [ ] Groß-/Kleinschreibung aller Überschriften.
- [ ] Workfront-Begriffe werden korrekt großgeschrieben (direkte oder indirekte Referenz).
- [ Fett nur bei anklickbaren Aktionen innerhalb von Verfahrensschritten ].
- [ ] Querverweise verwenden das Standardformat .
- [ ] Anmerkungen/Tipps/Warnungen nicht gestapelt, maximal eine pro Abschnitt.
- [ ] Oxford-Komma wird konsequent verwendet.
- [ ] Verfahrensschritte verwenden bestimmte Verben (Typ, Auswahl, Klick).
- [ ] Bedingte/optionale Schritte, die korrekt gekennzeichnet sind.
- [ ] Keine Geschlechtspronomen.
- [ ] Sätze sind klar, konkret und aufgabenorientiert, die Parallelstruktur gilt.
