---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Fehlermeldung beim Ausführen eines Berichts: „Sie sind derzeit nicht angemeldet.“'
description: Erfahren Sie mehr über die Fehlermeldung „Sie sind derzeit nicht angemeldet“.
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 3%

---

# Fehlermeldung beim Ausführen eines Berichts: „Sie sind derzeit nicht angemeldet.“

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
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

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
   Oder\
   Lassen Sie das Feld **Diesen Bericht mit den Zugriffsrechten von ausführen:** leer.

1. Klicken Sie **Fertig**.
1. Klicken Sie auf **Speichern + schließen**.\
   Der Fehler sollte beim Ausführen dieses Berichts nicht erneut angezeigt werden.
