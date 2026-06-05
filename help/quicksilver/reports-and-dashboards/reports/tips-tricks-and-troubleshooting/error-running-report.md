---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Fehlermeldung beim Ausführen eines Berichts: „Sie sind derzeit nicht angemeldet.“'
description: Erfahren Sie mehr über die Fehlermeldung „Sie sind derzeit nicht angemeldet“.
author: Courtney
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Vg-z-oXY25if70i5l2GBZad4iBj6hNRhu9LHE-6kCU8
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
source-wordcount: 215
ht-degree: 32%

---

# Fehlermeldung beim Ausführen eines Berichts: „Sie sind derzeit nicht angemeldet.“

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
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Problem

Beim Ausführen oder Anzeigen eines Berichts in einem Dashboard gibt der folgende Fehler zurück:\
*Versuchen Sie es erneut. Sie sind derzeit nicht angemeldet.*

Es werden keine Ergebnisse im Bericht angezeigt.

## Ursache

Der Bericht ist derzeit so eingestellt, dass er als deaktivierter Benutzer ausgeführt wird.

## Lösung

Sie müssen über Verwaltungsberechtigungen für den Bericht verfügen, um die Berichteinstellungen ändern zu können.\
So passen Sie den Bericht an und sehen die Ergebnisse:

1. Zum Bericht gehen.
1. Klicken Sie **Berichtsaktionen** > **Bearbeiten** > **Berichteinstellungen**.

1. Geben Sie den Namen eines aktiven Benutzers im Feld **Diesen Bericht ausführen mit den Zugriffsrechten von:** an.\
   ODER\
   Lassen Sie das Feld **Diesen Bericht mit den Zugriffsrechten von ausführen:** leer.

1. Klicken Sie auf **Fertig**.
1. Klicken Sie auf **Speichern + schließen**.\
   Der Fehler sollte beim Ausführen dieses Berichts nicht erneut angezeigt werden.
