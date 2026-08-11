---
name: clean-el-traffic-csv
description: Bereinigt einen unformatierten CSV-Export von Experience League/Adobe Analytics-Traffic nach unten zu Seiten, die nur Workfront sind, sortiert nach Seitenansichten. Verwenden Sie diese Option, wenn der/die Benutzende eine CSV-Datei für den Seiten-Traffic von Experience League bereitstellt (Spalten wie „Seiten-URL generisch“, „Unique Visitors“, „Besuche“, „Seitenansichten„) und bittet, sie zu bereinigen, zu filtern oder zu verarbeiten, oder die Tabelle „Dokumentation-Tracking“ / „Am häufigsten angezeigte Artikel“ erwähnt.
source-git-commit: e22d43e9962b2b00793577fd14ac00587e8a2a6d
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---


# Experience League-Traffic-CSV bereinigen

Wandelt einen unformatierten Adobe Analytics-Freiformtabellen-Export des Experience League-Seiten-Traffics in eine saubere, Workfront-basierte, deduplizierte CSV-Datei um, die nach Seitenansichten sortiert ist, überschreibt die Originaldatei und speichert außerdem eine datierte Kopie auf dem Desktop.

## Formen eingeben

Die Eingabe kann eine von zwei Formen sein:

1. **Rohexport** - beginnt mit Metadaten-Kommentarzeilen (`#===`, `# Freeform`, `# Report suite: ...`, `"# Date: <range>"` usw.), gefolgt von einer hierarchischen Aufschlüsselungstabelle (z. B. `Solution (v2)` → `workfront` → `Page URL Generic (v33)` → einzelnen URL-Zeilen). Die `Page URL Generic (v33)` der wörtlichen Zelle (oder eine ähnliche `Page URL Generic ...`) wird in der zweiten Spalte teilweise nach unten angezeigt.
2. **CSV bereits bereinigen** - Die erste Zeile ist bereits eine einfache Kopfzeile wie `Page URL Generic (v33),Unique Visitors,Visits,Page Views`, ohne Metadatenzeilen oder zusätzliche führende Spalten.

Ermitteln Sie vor dem Start, welches Shape Sie haben: Wenn Zeile 1 eine einfache Kopfzeile ist, die mit Form 2 übereinstimmt, fahren Sie direkt mit Schritt 2 fort (es ist kein Datumsbereich verfügbar, also überspringen Sie auch Schritt 7, es sei denn, der Benutzer gibt einen separaten Datumsbereich an).

## Workflow

### Schritt 0: Erfassen Sie den Datumsbereich (nur Rohexport, bevor Sie etwas löschen)

Finden Sie die Metadatenzeile in der Nähe der oberen übereinstimmenden `# Date: <range>` (z. B. `"# Date: Jul 1, 2026 - Jul 31, 2026"`). `<range>` (z. B. `Jul 1, 2026 - Jul 31, 2026`) - wird später in Schritt 7 benötigt. Tun Sie dies, bevor Zeilen gelöscht werden.

### Schritt 1: Entfernen des Rohexports aus einer einfachen Tabelle (nur Rohexport)

1. Suchen Sie die Zeile, die die `Page URL Generic (...)` enthält (sie befindet sich im Standardexport in der zweiten Spalte).
2. Löschen Sie jede Zeile oberhalb dieser Zeile, einschließlich der Metadaten-Kommentarzeilen und der Zwischensummenzeilen `Solution (v2)`/`workfront`.
3. Löschen Sie alle Spalten links von der `Page URL Generic` Zelle (im Standardexport ist dies nur Spalte A).
4. Ersetzen Sie in derselben Zeile (jetzt in der Kopfzeile) die numerischen Zwischensummenwerte rechts neben `Page URL Generic (...)` durch die literalen Kopfzeilen, in der folgenden Reihenfolge: `Unique Visitors`, `Visits`, `Page Views`. Lassen Sie die `Page URL Generic (...)` Zelle unverändert.

Ergebnis: eine einfache CSV mit `Page URL Generic (v33),Unique Visitors,Visits,Page Views`, gefolgt von einer Zeile pro URL.

### Schritt 2: Nur Workfront-Zeilen beibehalten

Überprüfen Sie für jede Datenzeile, ob die URL die literale Teilzeichenfolge `/workfront/` (Schrägstrich auf beiden Seiten) enthält. Gebietsschema-Präfix spielt keine Rolle (`/en/`, `/zh-hans/` usw. - alle bleiben so lange erhalten, wie das Produktsegment übereinstimmt).

- Löschen Sie die Zeile, wenn die URL **nicht** `/workfront/` als Pfadsegment enthält. Dadurch werden andere Produkte wie `workfront-fusion`, `workfront-learn`, `proofhqpapi` usw. entfernt. (Eine Unterzeichenfolge wie `tutorials-workfront` **nicht** zählen. Die Übereinstimmung muss der exakte `/workfront/` des Segments sein.)
- Andernfalls bleibt die Zeile unverändert.

### Schritt 3: URL kürzen

Suchen Sie für jede überlebende Zeile `/using` in der URL und behalten Sie nur den Teil von (einschließlich) der `/` bei, die ihr folgt, wobei alles vor und einschließlich `/using` verworfen wird.

Beispiel: `https://experienceleague.adobe.com/de/docs/workfront/using/home` → `/home`

Wenn `/using` nicht in der URL einer Workfront-Zeile gefunden wird, lassen Sie diese URL unverändert und kennzeichnen Sie sie für den Benutzer, anstatt zu raten.

### Schritt 4: Entfernen von Fragment-/Abfragesuffixen

Wenn die gekürzte URL einen `#` oder `?` enthält, löschen Sie dieses Zeichen und alles, was danach steht.

Beispiel: `/manage-scenarios/restore-a-scenario-version#compare-scenario-versions` → `/manage-scenarios/restore-a-scenario-version`

### Schritt 5: Duplikate zusammenführen

Nach dem Zuschneiden können mehrere Zeilen nun dieselbe URL teilen (z. B. zwei verschiedene Gebietsschema-Zeilen, die auf denselben Pfad reduzieren). Alle Zeilen mit einer identischen URL in einer Zeile kombinieren, `Unique Visitors`, `Visits` und `Page Views` unabhängig voneinander summieren.

Beispiel: `/home,2,2,3` und `/home,5,6,7` → `/home,7,8,10`

### Schritt 6: Nach Seitenansichten sortieren

Sortieren Sie alle Datenzeilen nach absteigender `Page Views` (zuerst die größte). Die Kopfzeile bleibt oben über den sortierten Daten unverändert.

### Schritt 7: Hinzufügen der Datumsbereichszeile (nur Rohexport, wenn in Schritt 0 erfasst)

Entfernen Sie vor dem Einfügen alle Kommas aus dem erfassten Datumsbereich (z. B. `Jul 1, 2026 - Jul 31, 2026` → `Jul 1 2026 - Jul 31 2026`) - der Rohbereich enthält Kommas, die andernfalls als CSV-Spaltentrennzeichen in dieser Zeile fehlinterpretiert würden.

Fügen Sie ganz oben über der Kopfzeile eine neue Zeile ein, die nur den durch Kommas getrennten Datumsbereich enthält.

Endgültige Zeilenreihenfolge: Datumsbereich → Kopfzeile → sortierten Datenzeilen.

### Schritt 8: Speichern

Überschreiben Sie die ursprüngliche Eingabedatei mit dem bereinigten Ergebnis.

### Schritt 9: Speichern einer datierten Kopie auf dem Desktop (nur Rohexport, wenn in Schritt 0 ein Datumsbereich erfasst wurde)

Erstellen Sie eine dateinamenssichere Version des Datumsbereichs: Entfernen Sie Kommas und ersetzen Sie alle `\ / : * ? " < > |` durch `-` (diese Zeichen sind in Windows-Dateinamen ungültig und könnten andernfalls je nach Exportgebietsschema/Format in einem Datumsbereich angezeigt werden).

Speichern Sie eine zusätzliche Kopie der bereinigten CSV-Datei (gleicher Inhalt wie Schritt 8) mit dem folgenden Namen auf dem Desktop des aktuellen Benutzers:

`Documentation tracking report <filename-safe date range>.csv`

Beispiel: Ein erfasster `Apr 1, 2026 - Apr 30, 2026` wird `Documentation tracking report Apr 1 2026 - Apr 30 2026.csv`.

Überspringen Sie diesen Schritt für eine bereits bereinigte CSV (Form 2), es sei denn, der Benutzer gibt einen separaten Datumsbereich an.

## Außerhalb des Geltungsbereichs

Das Posten oder Freigeben der bereinigten CSV (z. B. in Slack) ist ein separater, noch nicht definierter Schritt - versuchen Sie nicht, die Datei im Rahmen dieser Kenntnisse anzuhängen oder hochzuladen.

## Implementierung (Rohexport)

Führen Sie für einen Rohexport die Schritte 0-8 mit diesem getesteten PowerShell-Skript aus, anstatt Zeilen manuell zu bearbeiten - dies ist schneller und weniger fehleranfällig für Dateien mit Hunderten von Zeilen. Ersetzen Sie `$path` durch den echten Dateipfad .

Überprüfen Sie vor der Ausführung, ob die Datei gesperrt ist (z. B. in Excel öffnen) - wenn `Set-Content` mit „von einem anderen Prozess verwendet wird“ fehlschlägt, bitten Sie den Benutzer, sie zu schließen, und führen Sie dann erneut aus.

```powershell
$path = "<full path to the CSV>"
$lines = Get-Content -Path $path -Encoding UTF8

# Step 0: capture the date range
$dateLine = $lines | Where-Object { $_ -match '# Date:\s*(.+?)"?\s*$' } | Select-Object -First 1
$null = $dateLine -match '# Date:\s*(.+?)"?\s*$'
$dateRange = $matches[1].Trim('"').Trim()

# Step 1: find the "Page URL Generic" row and strip everything above/left of it
$headerIdx = -1
for ($i = 0; $i -lt $lines.Count; $i++) {
    if ($lines[$i] -match 'Page URL Generic') { $headerIdx = $i; break }
}
$headerParts = $lines[$headerIdx].Split(',')
$urlHeaderLabel = $headerParts[1]
$newHeader = "$urlHeaderLabel,Unique Visitors,Visits,Page Views"

$dataLines = $lines[($headerIdx + 1)..($lines.Count - 1)] | Where-Object { $_.Trim() -ne '' }

$rows = @()
foreach ($line in $dataLines) {
    $comma1 = $line.IndexOf(',')
    $rest = $line.Substring($comma1 + 1)   # drop column(s) left of the URL
    $parts = $rest.Split(',')
    if ($parts.Count -ne 4) { continue }
    $url = $parts[0]
    $uv = [int]$parts[1]
    $vi = [int]$parts[2]
    $pv = [int]$parts[3]

    # Step 2: keep only /workfront/ rows
    if ($url -notmatch '/workfront/') { continue }

    # Step 3: trim to from "/using" onward
    $usingIdx = $url.IndexOf('/using')
    if ($usingIdx -lt 0) { continue }   # flag/report these separately if any occur
    $trimmed = $url.Substring($usingIdx + 6)   # 6 = length of "/using"

    # Step 4: strip # or ? suffix
    $hashIdx = $trimmed.IndexOfAny(@('#', '?'))
    if ($hashIdx -ge 0) { $trimmed = $trimmed.Substring(0, $hashIdx) }

    $rows += [PSCustomObject]@{ URL = $trimmed; UV = $uv; Visits = $vi; PV = $pv }
}

# Step 5: merge duplicates
$grouped = $rows | Group-Object URL | ForEach-Object {
    [PSCustomObject]@{
        URL    = $_.Name
        UV     = ($_.Group | Measure-Object UV -Sum).Sum
        Visits = ($_.Group | Measure-Object Visits -Sum).Sum
        PV     = ($_.Group | Measure-Object PV -Sum).Sum
    }
}

# Step 6: sort by Page Views descending
$sorted = $grouped | Sort-Object -Property PV -Descending

# Step 7 + 8: prepend date range (commas stripped) + header, then save
$dateRangeNoCommas = $dateRange -replace ',', ''
$outLines = @()
$outLines += $dateRangeNoCommas
$outLines += $newHeader
$outLines += $sorted | ForEach-Object { "$($_.URL),$($_.UV),$($_.Visits),$($_.PV)" }

Set-Content -Path $path -Value $outLines -Encoding UTF8

# Step 9: also save a dated copy to the Desktop
$safeDateRange = ($dateRange -replace ',', '') -replace '[\\/:*?"<>|]', '-'
$desktopPath = Join-Path ([Environment]::GetFolderPath('Desktop')) "Documentation tracking report $safeDateRange.csv"
Set-Content -Path $desktopPath -Value $outLines -Encoding UTF8
```

Bei einer bereits bereinigten CSV (Eingabe-Form 2) überspringen Sie die Kopfzeilenverschiebung, die Datumsbereichslogik und Schritt 9. Führen Sie einfach die Schritte 2-6 und 8 für die vorhandenen Kopfzeilen wie vorliegend aus.
