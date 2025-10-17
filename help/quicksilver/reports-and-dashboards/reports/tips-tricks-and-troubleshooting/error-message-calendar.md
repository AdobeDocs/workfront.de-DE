---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Fehlermeldung im Kalender: „Dieser Kalender hat die Ansichtsrechte eines deaktivierten Benutzers.“'
description: Erfahren Sie mehr über die Fehlermeldung „Dieser Kalender hat die Ansichtsrechte eines deaktivierten Benutzers“.
author: Jenny
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 1%

---

# Fehlermeldung im Kalender: „Dieser Kalender hat die Ansichtsrechte eines deaktivierten Benutzers.“

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
     <p>Arbeit oder höher</p>
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

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
