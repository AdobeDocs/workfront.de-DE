---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Korrigieren Sie den Starttag der Arbeitswoche für Timesheets.
description: Der Wochentag auf meinem Timesheet stimmt nicht mit dem Wochentag überein, der in meinem Timesheet-Profil konfiguriert ist.
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Korrigieren Sie den Starttag der Arbeitswoche für Timesheets.

## Problem

Der Wochentag auf meinem Timesheet stimmt nicht mit dem Wochentag überein, der in meinem Timesheet-Profil konfiguriert ist (wie unter [Erstellen, Bearbeiten und Zuweisen von Zeitzeichenprofilen](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md) beschrieben).

## Lösung

Der Wochentag eines Zeitblatts in Adobe Workfront verwendet die Spracheinstellungen und Gebietsschemaeinstellungen Ihres Browsers, um den Wochentag zu bestimmen. Aus diesem Grund müssen Sie die Spracheinstellungen und Gebietsschemaeinstellungen für Ihren Browser aktualisieren.

Wenn beispielsweise die Browsersprache auf Englisch und das Gebietsschema auf &quot;USA&quot;gesetzt ist, beginnt die Woche am Sonntag. Alternativ dazu ist der Starttag für die Browsersprache &quot;Englisch&quot;und für das Gebietsschema &quot;Großbritannien&quot;Montag.

Diese Einstellung wirkt sich auch auf den Wochentag in den Popup-Kalendern im gesamten System aus.

Die Änderung des Gebietsschemas hat keine Auswirkungen auf den Wochentag im Ressourcenraster (oder in der Ressourcenrasteransicht). Die Woche beginnt immer am Sonntag.

Im Folgenden finden Sie Anweisungen zum Ändern der Sprache und Gebietsschemaeinstellungen für verschiedene Browser, die von Workfront unterstützt werden.

* **Chrome:** Kopieren Sie den folgenden Link und fügen Sie ihn in Ihren Chrome-Browser ein: `chrome://settings/languages` und gehen Sie dann zu &quot;Sprachen&quot;.
* **Firefox:**Kopieren Sie den folgenden Link und fügen Sie ihn in Ihren Firefox-Browser ein: `about:preferences#content` und gehen Sie dann zu Sprachen.
* **IE 11:** Tools -> Internetoptionen -> Allgemein -> Sprachen
* **Safari:** Leider erlaubt Safari nicht, die Sprache des Webbrowsers zu ändern, ohne auch die Sprache des gesamten Betriebssystems zu ändern. Es ist wahrscheinlich einfacher, einfach einen anderen Browser wie Chrome oder Firefox zu installieren.


