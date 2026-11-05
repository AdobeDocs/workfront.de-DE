---
description: Formatierungs- und Validierungsregeln für Adobe Workfront - Versionshinweise (Übersicht, Produktbereich, Planung und Erscheinungsbild).
applyTo: "help/quicksilver/product-announcements/product-releases/**/*.md"
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%
---

# Formatierer für Versionshinweise

Bei diesen Dateien **es sich um** Versionshinweise“, nicht um Anleitungsartikel. Wenden **nicht** die
Hier gelten allgemeine Standards für die Schreibqualität. Lesen Sie vor der Bearbeitung die vollständige Quelle von .
Wahrheit, die die Vorlagen und den Veröffentlichungskalender umfasst:

- [.cursor/skills/release-notes-formatter/SKILL.md](../../.cursor/skills/release-notes-formatter/SKILL.md)
- [.cursor/skills/release-notes-formatter/reference.md](../../.cursor/skills/release-notes-formatter/reference.md)

## Kritische Regel - Bestimmen Sie zuerst das Dokumentenquartal

&#x200B;> [!IMPORTANT]
> Nie eine Funktion einem Dokumentquartal zuweisen, wenn Kalenderquartalsmathematik verwendet wird
> Vorschau- oder Produktionsdatum Dokumentquartal basiert auf welcher (**)**
> Die Funktion wird gemäß der internen Gruppierung des Workfront-Veröffentlichungskalenders in ausgeliefert, die
> ist gegenüber dem Kalenderquartal versetzt. Beispiel: eine Funktion mit einer Produktionsumgebung
> Das Datum vom 13. August 2026 gehört in das `26-q4` des Dokumentenquartals, nicht `26-q3`. Immer
> Sehen Sie sich vorher die Tabelle mit dem Versionskalender 2026 in der Referenzdatei an
> Erstellen oder Bearbeiten von Dateien. Wenn ein Produktionsdatum außerhalb dieser Tabelle liegt,
> Nach einem aktualisierten Kalender fragen, anstatt zu raten.

## Wichtige Strukturregeln

- **Frontmatter**: `feature` muss genau `Product Announcements` sein;
  `recommendations` muss genau `noDisplay, noCatalog` sein. Erfinde nie ein Buch
  `exl-id` - Nur einbeziehen, wenn bereits eine vorhanden ist.
- **Neueste Funktionen zuerst**: Die neueste Versionshinweise sind die ersten H2 nach
Das Intro (Produktbereichsseiten) und die oberste Zeile jeder Funktionstabelle (Übersicht)
Seiten).
- **Übersichtslink**: Produktbereichsseiten müssen auf (**) verlinken**
Übersichtsdatei - Ein häufiger Fehler ist die Verknüpfung mit dem vorherigen Quartal.
- **Datumsbeschriftung**: Auf jede Funktion H2 folgt ein `>[!NOTE]` mit
Vorschau / Produktion Schnellveröffentlichung / Produktion für alle Termine, passend zu
Übersichtstabellenzeile. Datumsangaben als `Month Day, Year` formatieren; `TBD` verwenden, falls unbekannt.
- **Geschriebene Quartalsnamen** in H1s: „Erstes Quartal“, „Zweites Quartal“, „Drittes Quartal“
Quartal“, „Viertes Quartal“.

## Erforderliche begleitende Aktualisierungen beim Hinzufügen von Seiten

- **Neue Seite (alle)**: Fügen Sie sie bei derselben Änderung `help/quicksilver/TOC.md` hinzu.
(Übersicht zuerst, Produktbereichsseiten alphabetisch, andere Verbesserungen zuletzt).
- **Übersichtsseite des neuen Quartals**: auch `help/quicksilver/home.md` aktualisieren —
Aktualisieren Sie den Link auf der Registerkarte „Neueste Version“ und den Link zur Planungsaktivität und fügen Sie Folgendes hinzu
Das neue Quartal auf der Registerkarte für aktuelle Jahresversionen.

Die vollständigen Vorlagen finden Sie in den Dateien „SKILL.md“ und „reference.md“ oben.
Dateibenennungskonventionen, Linkformate und der vollständige Veröffentlichungskalender.
