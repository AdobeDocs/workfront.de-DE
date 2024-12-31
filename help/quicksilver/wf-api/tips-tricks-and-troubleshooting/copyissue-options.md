---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Konfiguration der Optionen für OPTASK copyIssue
description: Eine Erläuterung der vom copyIssue-Endpunkt erwarteten ganzzahligen Werte.
author: Becky
feature: Workfront API
role: Developer
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 4%

---

# Konfiguration der Optionen für OPTASK copyIssue


Eine der Eigenschaften für einen copyIssue-API-Aufruf ist ein Feld namens `options`. Dieses Feld erwartet eine Ganzzahl.

Um eine der folgenden Optionen einzuschließen, geben Sie die entsprechende Ganzzahl ein. Um mehr als eine Option einzubeziehen, geben Sie die Summe der übereinstimmenden Ganzzahlen ein.

| Option | Wert* |
|---|---|
| Zuweisungen löschen | 2 |
| Fortschritt löschen | 4 |
| Dokumente löschen | 128 |
| Aktualisierungen löschen | 65536 |
| Berechtigungen löschen | 524288 |
| Benutzerdefinierte Daten löschen | 1048576 |

*Alle Werte sind Potenzen von 2.

Beispiele:

* Um den Fortschritt beim Kopieren des Problems zu löschen, geben Sie den `options` Wert `4` ein.

* Um sowohl den Fortschritt als auch die Dokumente zu löschen, geben Sie den `options` Wert `132` ein.

  Fortschritt löschen = 4

  Dokumente löschen = 128

  4 + 128 = 132
