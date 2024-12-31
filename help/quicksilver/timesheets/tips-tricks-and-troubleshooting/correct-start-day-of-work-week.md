---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Korrigieren Sie den Starttag der Arbeitswoche für Arbeitszeittabellen.
description: Der Starttag der Woche auf meiner Arbeitszeittabelle stimmt nicht mit dem Starttag der Woche überein, der auf meinem Arbeitszeittabellen-Profil konfiguriert ist.
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Korrigieren Sie den Starttag der Arbeitswoche für Arbeitszeittabellen.

## Problem

Der Starttag der Woche auf meiner Arbeitszeittabelle stimmt nicht mit dem Starttag der Woche überein, der auf meinem Arbeitszeittabellen-Profil konfiguriert ist (wie in [Erstellen, Bearbeiten und Zuweisen von Arbeitszeittabellen-Profilen](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md) beschrieben).

## Lösung

Der Starttag einer Arbeitszeittabelle in Adobe Workfront verwendet die Sprach- und Gebietsschemaeinstellungen in Ihrem Browser, um den Wochentag zu bestimmen. Aus diesem Grund müssen Sie die Sprach- und Gebietsschema-Einstellungen für Ihren Browser aktualisieren.

Wenn beispielsweise die Browser-Sprache auf Englisch und das Gebietsschema auf Vereinigte Staaten eingestellt ist, beginnt die Woche am Sonntag. Alternativ dazu ist für die Browser-Sprache Englisch und für das Gebietsschema Großbritannien festgelegt. Der Starttag ist Montag.

Diese Einstellung wirkt sich auch auf den Starttag der Woche in den Popup-Kalendern im gesamten System aus.

Die Gebietsschema-Änderung wirkt sich nicht auf den Starttag der Woche auf dem Ressourcenraster (oder der Ressourcenraster-Ansicht) aus. Die Woche beginnt immer am Sonntag.

Im Folgenden finden Sie Anweisungen zum Ändern von Sprach- und Gebietsschemaeinstellungen für verschiedene Browser, die von Workfront unterstützt werden.

* **Chrome:** Kopieren Sie den folgenden Link und fügen Sie ihn in Ihren Chrome-Browser ein: `chrome://settings/languages` gehen Sie dann zu „Sprachen“.
* **Firefox:**Kopieren Sie den folgenden Link und fügen Sie ihn in Ihren Firefox-Browser ein: `about:preferences#content` gehen Sie dann zu Sprachen.
* **IE 11:** Tools -> Internetoptionen -> Allgemein -> Sprachen
* **Safari:** Leider erlaubt Safari nicht, die Browser-Sprachen zu ändern, ohne gleichzeitig die Sprache Ihres Betriebssystems zu ändern. Wahrscheinlich ist es einfacher, einfach einen anderen Browser wie Chrome oder Firefox zu installieren.


