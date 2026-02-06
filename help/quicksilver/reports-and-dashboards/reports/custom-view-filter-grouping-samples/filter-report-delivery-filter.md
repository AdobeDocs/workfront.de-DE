---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Anzeigen von für den Versand geplanten Berichten'
description: Dieser Berichtsfilter zeigt alle Berichte an, die automatisch in Adobe Workfront bereitgestellt werden sollen. Dies empfiehlt sich am besten bei der Standardansicht.
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: 7b937384-80c9-4bc7-94be-5573cf86b35b
source-git-commit: be102fd5f490b12837a231774253c030973c1c4f
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 11%

---

# Filter: Anzeigen von für den Versand geplanten Berichten

<!--Audited: 10/2024-->

Dieser Berichtsfilter zeigt alle Berichte an, die automatisch in Adobe Workfront bereitgestellt werden sollen. Dies empfiehlt sich am besten bei der Standardansicht.

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

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filter für Berichtversand

So wenden Sie diesen Filter an:

1. Navigieren Sie zu einer Liste mit Berichten.

1. Wählen Sie **Dropdown** Menü „Filter“ die Option **Neuer Filter**.

1. Klicken **Wechseln Sie in den Textmodus**.

1. Kopieren Sie **Bereich Filterregeln für Ihren Bericht festlegen** folgenden Code und fügen Sie ihn ein:

   ```
    scheduledReportsOM:ID_Mod=notblank
   ```

1. Klicken Sie auf **Filter speichern**.
