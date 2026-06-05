---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Daten aus freigegebenen Spalten werden in Dashboard-Berichten nicht angezeigt
description: Daten aus freigegebenen Spalten werden nicht angezeigt, wenn der Bericht in einem mehrspaltigen Dashboard-Layout platziert wird, jedoch in einem einspaltigen Layout. Zeilenumbrüche werden ebenfalls überschrieben.
author: Courtney
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/OEFlwkdPf98g4-rC1tzaTmmEwb5-BXHx-j8XGrRR8sE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 162
ht-degree: 12%

---

# Daten aus freigegebenen Spalten werden in Dashboard-Berichten nicht angezeigt

## Problem

Daten aus freigegebenen Spalten werden nicht angezeigt, wenn der Bericht in einem mehrspaltigen Dashboard-Layout platziert wird, jedoch in einem einspaltigen Layout. Zeilenumbrüche werden ebenfalls überschrieben.

## Ursache

Nur Spalten, die als markiert sind

```
shortview=true
```

werden in die Dashboard-Ansicht des Berichts aufgenommen, wenn für das Dashboard-Layout die Aufteilung links/rechts oder die Aufteilung links/mittel/rechts eingerichtet ist.

## Lösung

Rufen Sie die im Bericht verwendete Ansicht auf und öffnen Sie den Textmodus. (Weitere Informationen finden Sie unter [Bearbeiten einer Ansicht im Textmodus](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md).) Alle Spalten im Bericht, einschließlich der in einer freigegebenen/zusammengeführten Spalte, mit folgender Kennzeichnung versehen

```
shortview=true
```

. Die Berichtsspalten werden dann ordnungsgemäß im Dashboard angezeigt.
