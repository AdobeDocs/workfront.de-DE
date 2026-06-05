---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Fehlermeldung im Kalender: „Dieser Kalender hat die Ansichtsrechte eines deaktivierten Benutzers.“'
description: Erfahren Sie mehr über die Fehlermeldung „Dieser Kalender hat die Ansichtsrechte eines deaktivierten Benutzers“.
author: Courtney
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/3yxFjvj--T8taJ2xrLTIia6YamTCwZeueTFSI-bMg4o
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 258
ht-degree: 23%

---

# Fehlermeldung im Kalender: „Dieser Kalender hat die Ansichtsrechte eines deaktivierten Benutzers bzw. einer deaktivierten Benutzerin.“

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
     <p>Standard</p>
     <p>Work oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Kalenderberechtigungen</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Problem

Sie erhalten die folgende Fehlermeldung, wenn Sie auf einen Kalender zugreifen, der für Sie freigegeben wurde: 

*Dieser Kalender hat die Ansichtsrechte eines deaktivierten Benutzers. Bitten Sie einen Administrator, die Kalenderprivilegien zu korrigieren.*

## Ursache

Der Benutzer, der diesen Kalender erstellt hat (sein ursprünglicher Besitzer), ist ein Benutzer, der deaktiviert wurde. 

## Lösung

Sie können dies wie folgt beheben:

1. Kopieren Sie den Originalkalender. Wenn Sie einen Kalender kopieren, werden Sie zum Besitzer des Kalenders. Der kopierte Kalender sollte alle Informationen aus dem ursprünglichen Kalender anzeigen.\
   Weitere Informationen zum Kopieren eines Kalenders finden Sie unter [Kopieren eines Kalenderberichts](../../../reports-and-dashboards/reports/calendars/copy-a-calendar-report.md).

1. Geben Sie den kopierten Kalender für dieselben Benutzer frei wie den ursprünglichen Kalender. Alle Benutzer sollten dieselben Informationen im neuen Kalender sehen.
1. (Optional und bedingt) Wenn Sie berechtigt sind, den ursprünglichen Kalender zu verwalten, entfernen Sie alle anderen Benutzer, für die der Kalender freigegeben ist, aus dem Bereich Kalenderfreigabe . Dadurch wird die Verwirrung bei Benutzern beseitigt, die versuchen, den falschen Kalender anzuzeigen.
