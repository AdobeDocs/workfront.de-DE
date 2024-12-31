---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Anzeigen von für den Versand geplanten Berichten'
description: Dieser Berichtsfilter zeigt alle Berichte an, die automatisch in Adobe Workfront bereitgestellt werden sollen. Dies empfiehlt sich am besten bei der Standardansicht.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7b937384-80c9-4bc7-94be-5573cf86b35b
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 1%

---

# Filter: Anzeigen von für den Versand geplanten Berichten

<!--Audited: 10/2024-->

Dieser Berichtsfilter zeigt alle Berichte an, die automatisch in Adobe Workfront bereitgestellt werden sollen. Dies empfiehlt sich am besten bei der Standardansicht.

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

## Filter für Berichtversand

So wenden Sie diesen Filter an:

1. Navigieren Sie zu einer Liste mit Berichten.
1. Wählen Sie **Dropdown** Menü „Filter“ die Option **Neuer Filter**.

1. Klicken **Wechseln Sie in den Textmodus**.
1. Kopieren Sie **Bereich Filterregeln für Ihren Bericht festlegen** folgenden Code und fügen Sie ihn ein: `scheduledReportID=0<br>scheduledReportID_Mod=notnull`
1. Klicken Sie auf **Filter speichern**.
