---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Aktuelle Projekte mit ausstehender Genehmigung anzeigen'
description: Der folgende Projektfilter zeigt Projekte mit dem Status Aktuell - Ausstehende Genehmigung an, wobei der angemeldete Benutzer entweder Projektsponsor oder Portfolio-Manager ist.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# Filter: Aktuelle Projekte mit ausstehender Genehmigung anzeigen

<!--Audited: 10/2024-->

Der folgende Projektfilter zeigt Projekte mit dem Status Aktuell - Ausstehende Genehmigung an, wobei der angemeldete Benutzer entweder Projektsponsor oder Portfolio-Manager ist.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkender zum Ändern eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filter ändern </p></li>
   <li><p>Planen der Änderung eines Berichts</p></li> </ul></td> 
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

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtern aktueller Projekte mit ausstehender Genehmigung

So wenden Sie diesen Filter an:

1. Zu einer Projektliste gehen.
1. Wählen Sie **Dropdown** Menü „Filter“ die Option **Neuer Filter**.

1. Klicken Sie **Textmodus**.
1. Kopieren Sie den folgenden Code in den angezeigten Bereich und fügen Sie ihn ein:
   <pre>status=CUR:A<br>sponsorID=$$USER.ID<br>OR:a:status=CUR:A<br>OR:a:portfolio:ownerID=$$USER.ID</pre>

1. Klicken Sie **Übernehmen** > **Als neu speichern**.
