---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Daten aus freigegebenen Spalten werden nicht in Dashboard-Berichten angezeigt
description: Daten aus freigegebenen Spalten werden nicht angezeigt, wenn der Bericht in einem Dashboard-Layout mit mehreren Spalten platziert wird, sondern in einem einzelnen Spaltenlayout. Zeilenumbrüche werden ebenfalls überschrieben.
author: Nolan
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---

# Daten aus freigegebenen Spalten werden nicht in Dashboard-Berichten angezeigt

## Problem

Daten aus freigegebenen Spalten werden nicht angezeigt, wenn der Bericht in einem Dashboard-Layout mit mehreren Spalten platziert wird, sondern in einem einzelnen Spaltenlayout. Zeilenumbrüche werden ebenfalls überschrieben.

## Ursache

Nur Spalten mit

```
shortview=true
```

werden in die Dashboard-Ansicht des Berichts aufgenommen, wenn das Dashboard-Layout die Rechts-/Links-Aufspaltung oder die Rechts-/Links-Aufspaltung aufweist.

## Lösung

Rufen Sie die im Bericht verwendete Ansicht auf und öffnen Sie den Textmodus. (Weitere Informationen finden Sie unter [Bearbeiten einer Ansicht im Textmodus](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md).) Beschriften Sie alle Spalten des Berichts, einschließlich der Spalten, die in einer gemeinsamen/zusammengeführten Spalte verwendet werden, mit

```
shortview=true
```

. Die Berichtsspalten werden dann korrekt im Dashboard angezeigt.
