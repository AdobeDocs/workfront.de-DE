---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Fehlermeldung im Kalender: „Dieser Kalender hat die Ansichtsrechte eines deaktivierten Benutzers.“'
description: Erfahren Sie mehr über die Fehlermeldung „Dieser Kalender hat die Ansichtsrechte eines deaktivierten Benutzers“.
author: Lisa
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Fehlermeldung im Kalender: „Dieser Kalender hat die Ansichtsrechte eines deaktivierten Benutzers.“

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan, Arbeit</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Kalenderberechtigungen</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

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
