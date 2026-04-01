---
source-git-commit: b3148e5706abd75f2dd260f32507dedf8e259f57
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 1%

---
# Git-Commit-Nachrichten

Wenden Sie diese Regel immer an. Wenn Sie eine Git-Commit-Nachricht entwerfen oder generieren (z. B. im Commit-Feld des Source-Steuerelements oder wenn Sie im Agenten-Chat gefragt werden), verwenden Sie dieses Format.

## Betreffzeile (nur erste Zeile)

- Ungefähr **50 Zeichen oder weniger**.
- Fassen Sie die Änderung in **Imperative Stimmung** (z. B. „Hinzufügen…“, „Beheben…“, „Refaktorieren…„) zusammen.

## Leerzeile

Lassen Sie eine **Leerzeile** hinter dem Betreff vor dem Textkörper.

## Textkörper (detaillierte Beschreibung)

- Zeilenumbruch bei etwa **72 Zeichen** (einschließlich Aufzählungszeichen und Leerzeichen).
- Verwenden Sie **Erläuterung &quot;**&quot;. Jeder Aufzählungszeichen muss mit genau einem der folgenden Elemente beginnen:
   - **📖** - Wird verwendet, wenn die Änderung **etwas Neues**: neue Dateien, neue Abschnitte, neue Funktionen, neue Kopfzeilen, neue Zeilen oder andere neue Inhalte.
   - **✏️** - Wird verwendet, wenn die Änderung **ändert** vorhandenes Werk: Bearbeitungen an vorhandenen Zeilen, Aktualisierungen vorhandener Abschnitte, Umgestaltungen vorhandenen Codes oder Änderungen am aktuellen Inhalt.

Wenden Sie **📖** oder **✏️** auf jede einzelne Aufzählung an, damit klar ist, was eingeführt wurde und was geändert wurde.

## Vorlage

Füllen Sie die Platzhalter aus (lassen Sie in der endgültigen Nachricht keine spitzen Klammern):

```
<Summarize change(s) in around 50 characters or less>

<More detailed explanatory description of the change wrapped into about 72
characters with bullets. >
```

## Beispiel

```
Add refresh token rotation to auth flow

- 📖 Add refresh_tokens table and Alembic migration for schema v3.
- ✏️ Update session middleware to rotate secrets and revoke old tokens.
```
