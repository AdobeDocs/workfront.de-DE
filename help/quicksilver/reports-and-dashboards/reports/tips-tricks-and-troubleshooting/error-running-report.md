---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '"Fehlermeldung beim Ausführen eines Berichts: "Sie sind derzeit nicht angemeldet."'
description: Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel - BEARBEITEN SIE MICH - durchzuführen.
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 4%

---

# Fehlermeldung beim Ausführen eines Berichts: &quot;Sie sind derzeit nicht angemeldet.&quot;

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
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Problem

Wenn ein Bericht ausgeführt oder in einem Dashboard angezeigt wird, gibt der folgende Fehler zurück:\
*Versuchen Sie es erneut. Sie sind zurzeit nicht angemeldet.*

Im Bericht werden keine Ergebnisse angezeigt.

## Ursache

Der Bericht wird derzeit als deaktivierter Benutzer ausgeführt.

## Lösung

Sie müssen über Verwaltungsberechtigungen für den Bericht verfügen, um die Berichtseinstellungen ändern zu können.\
So passen Sie den Bericht an und sehen die Ergebnisse:

1. Gehen Sie zum Bericht.
1. Klicken **Berichtaktionen** > **Bearbeiten** > **Berichtseinstellungen**.

1. Geben Sie den Namen eines aktiven Benutzers im **Führen Sie diesen Bericht mit den Zugriffsrechten von aus:** -Feld.\
   Oder\
   Lassen Sie die **Führen Sie diesen Bericht mit den Zugriffsrechten von aus:** Feld leer.

1. Klicken **Fertig**.
1. Klicken **Speichern und schließen**.\
   Der Fehler sollte bei der Ausführung dieses Berichts nicht erneut angezeigt werden.
