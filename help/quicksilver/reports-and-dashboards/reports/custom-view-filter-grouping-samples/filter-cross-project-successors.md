---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Unvollständige projektübergreifende Nachfolger anzeigen'
description: Dieser Aufgabenfilter gibt unvollständige projektübergreifende Nachfolger zurück.
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: aea955b1-581a-4ce0-8634-863ba1083c05
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '151'
ht-degree: 33%

---

# Filter: Unvollständige projektübergreifende Nachfolger anzeigen

Dieser Aufgabenfilter gibt unvollständige projektübergreifende Nachfolger zurück.

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
   <p>Mitwirkender oder Anfrage zum Ändern eines Filters </p>
   <p>Standard oder Plan zum Ändern eines Berichts</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtern von projektübergreifenden Nachfolgern

So wenden Sie diesen Filter an:

1. Zu einer Aufgabenliste gehen.
1. Wählen Sie **Dropdown** Menü „Filter“ die Option **Neuer Filter**.

1. Klicken Sie **Textmodus**.
1. Fügen Sie im angezeigten Bereich den folgenden Code ein:
   <pre>percentComplete=100<br>percentComplete_Mod=ne<br>successMM:projectID=FIELD:projectID<br>succorsMM:projectID_Mod=ne</pre>

1. Klicken Sie **Übernehmen** > **Als neu speichern**.
