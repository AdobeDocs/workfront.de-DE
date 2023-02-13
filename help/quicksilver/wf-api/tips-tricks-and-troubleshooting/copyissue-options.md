---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Optionskonfiguration für OPTASK copyIssue
description: Eine Erläuterung der vom copyIssue -Endpunkt erwarteten ganzzahligen Werte.
author: Becky
feature: Workfront API
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
source-git-commit: 93a67b3dbd59f188dad6b060ec93c3f137c981b2
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 6%

---

# Optionskonfiguration für OPTASK copyIssue


Eine der Eigenschaften für einen API-Aufruf &quot;copyIssue&quot;ist ein Feld namens `options`. Dieses Feld erwartet eine Ganzzahl.

Um eine der folgenden Optionen einzuschließen, geben Sie die entsprechende Ganzzahl ein. Um mehrere Optionen einzuschließen, geben Sie die Summe der entsprechenden Ganzzahlen an.

| option | value* |
|---|---|
| Zuweisungen löschen | 2 |
| Klare Fortschritte | 4 |
| Dokumente löschen | 128 |
| Clear Updates | 65536 |
| Berechtigungen löschen | 524288 |
| Benutzerdefinierte Daten löschen | 1048576 |

*Alle Werte sind Befugnisse von 2.

Beispiele:

* Um den Fortschritt beim Kopieren des Problems zu löschen, geben Sie eine `options` Wert von `4`.

* Geben Sie einen `options` Wert von `132`.

   Kleiner Fortschritt = 4

   Clear Documents = 128

   4 + 128 = 132
