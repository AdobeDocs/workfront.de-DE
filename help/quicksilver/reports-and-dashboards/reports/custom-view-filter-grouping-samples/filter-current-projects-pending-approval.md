---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Aktuelle Projekte mit ausstehender Genehmigung anzeigen'
description: Der folgende Projektfilter zeigt Projekte mit dem Status Aktuell - Ausstehende Genehmigung an, wobei der angemeldete Benutzer entweder Projektsponsor oder Portfolio-Manager ist.
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/sPLW4-QHP5aXEd--UZVsS1WjY5-bJeyoOZ8mzYe7sww
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 192
ht-degree: 28%

---

# Filter: Aktuelle Projekte mit ausstehender Genehmigung anzeigen

<!--Audited: 10/2024-->

Der folgende Projektfilter zeigt Projekte mit dem Status Aktuell - Ausstehende Genehmigung an, wobei der angemeldete Benutzer entweder Projektsponsor oder Portfolio-Manager ist.

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

## Filtern aktueller Projekte mit ausstehender Genehmigung

So wenden Sie diesen Filter an:

1. Zu einer Projektliste gehen.
1. Wählen Sie **Dropdown** Menü „Filter“ die Option **Neuer Filter**.

1. Klicken Sie **Textmodus**.
1. Kopieren Sie den folgenden Code in den angezeigten Bereich und fügen Sie ihn ein:
   <pre>status=CUR:A<br>sponsorID=$$USER.ID<br>OR:a:status=CUR:A<br>OR:a:portfolio:ownerID=$$USER.ID</pre>

1. Klicken Sie **Übernehmen** > **Als neu speichern**.
