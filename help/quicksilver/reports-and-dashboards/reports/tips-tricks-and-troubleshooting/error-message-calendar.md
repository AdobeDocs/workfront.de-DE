---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: "Fehlermeldung im Kalender: 'Dieser Kalender hat die Anzeigerechte eines deaktivierten Benutzers.'"
description: Erfahren Sie mehr über die Fehlermeldung "Dieser Kalender hat die Anzeigerechte eines deaktivierten Benutzers".
author: Lisa
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 6%

---

# Fehlermeldung im Kalender: &quot;Dieser Kalender hat die Anzeigerechte eines deaktivierten Benutzers.&quot;

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
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Kalender verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Problem

Beim Zugriff auf einen für Sie freigegebenen Kalender erhalten Sie die folgende Fehlermeldung: 

*Dieser Kalender hat die Anzeigerechte eines deaktivierten Benutzers. Bitten Sie einen Administrator, die Kalenderprivilegien zu ändern.*

## Ursache

Der Benutzer, der diesen Kalender erstellt hat (sein ursprünglicher Eigentümer), ist ein Benutzer, der deaktiviert wurde. 

## Lösung

Sie können dies wie folgt beheben:

1. Kopieren Sie den Originalkalender. Wenn Sie einen Kalender kopieren, werden Sie zum Eigentümer des Kalenders. Der kopierte Kalender sollte alle Informationen aus dem Originalkalender enthalten.\
   Weitere Informationen zum Kopieren eines Kalenders finden Sie unter [Kalenderberichte kopieren](../../../reports-and-dashboards/reports/calendars/copy-a-calendar-report.md).

1. Geben Sie den kopierten Kalender für dieselben Benutzer wie den ursprünglichen Kalender frei. Alle Benutzer sollten dieselben Informationen im neuen Kalender sehen.
1. (Optional und bedingt) Wenn Sie berechtigt sind, den ursprünglichen Kalender zu verwalten, entfernen Sie alle anderen Benutzer, für die der Kalender freigegeben ist, aus dem Bereich &quot;Freigabe im Kalender&quot;. Dadurch wird die Verwirrung der Benutzer beseitigt, die versuchen, den falschen Kalender anzuzeigen.
