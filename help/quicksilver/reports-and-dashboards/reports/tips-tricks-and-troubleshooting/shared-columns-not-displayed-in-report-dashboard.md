---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Daten aus freigegebenen Spalten werden in Dashboard-Berichten nicht angezeigt
description: Daten aus freigegebenen Spalten werden nicht angezeigt, wenn der Bericht in einem mehrspaltigen Dashboard-Layout platziert wird, aber sie werden in einem einspaltigen Layout angezeigt. Zeilenumbrüche werden ebenfalls überschrieben.
author: Courtney
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 12%

---

# Daten aus freigegebenen Spalten werden in Dashboard-Berichten nicht angezeigt

## Problem

Daten aus freigegebenen Spalten werden nicht angezeigt, wenn der Bericht in einem mehrspaltigen Dashboard-Layout platziert wird, aber sie werden in einem einspaltigen Layout angezeigt. Zeilenumbrüche werden ebenfalls überschrieben.

## Ursache

Nur Spalten, die als

```
shortview=true
```

in der Dashboard-Ansicht des Berichts enthalten sind, wenn das Dashboard-Layout die Aufteilung nach links/rechts oder die Aufteilung nach links/Mitte/rechts eingerichtet hat.

## Lösung

Greifen Sie auf die im Bericht verwendete Ansicht zu und öffnen Sie den Textmodus. (Weitere Informationen finden Sie unter [Ansicht mit Textmodus bearbeiten](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md).) Beschriften Sie alle Spalten im Bericht, einschließlich der in einer freigegebenen/zusammengeführten Spalte verwendeten Spalten, mit

```
shortview=true
```

. Die Berichtsspalten werden dann im Dashboard korrekt angezeigt.
