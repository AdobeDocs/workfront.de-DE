---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Fehlermeldung beim Ausführen eines Berichts: „Sie sind derzeit nicht angemeldet.“'
description: Erfahren Sie mehr über die Fehlermeldung „Sie sind derzeit nicht angemeldet“.
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 6%

---

# Fehlermeldung beim Ausführen eines Berichts: „Sie sind derzeit nicht angemeldet.“

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
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   Oder\
   Lassen Sie das Feld **Diesen Bericht mit den Zugriffsrechten von ausführen:** leer.

1. Klicken Sie auf **Fertig**.
1. Klicken Sie auf **Speichern + schließen**.\
   Der Fehler sollte beim Ausführen dieses Berichts nicht erneut angezeigt werden.
