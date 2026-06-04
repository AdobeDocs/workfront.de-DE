---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Konfiguration der Optionen für OPTASK copyIssue
description: Eine Erläuterung der vom copyIssue-Endpunkt erwarteten ganzzahligen Werte.
author: Becky
feature: Workfront API
role: Developer
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
TQID: https://experienceleague.adobe.com/9cDJFoKl6zqpaAvqzpGqzflcbGZNrAWvEnUAFuqD-Rc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 122
ht-degree: 16%

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
