---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Filter: Anzeigen von Versandberichten"'
description: Dieser Berichtsfilter zeigt alle Berichte an, deren Bereitstellung in Adobe Workfront geplant ist. Es wird am besten mit der Standardansicht verwendet.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7b937384-80c9-4bc7-94be-5573cf86b35b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 0%

---

# Filter: Anzeige der für die Bereitstellung geplanten Berichte

Dieser Berichtsfilter zeigt alle Berichte an, deren Bereitstellung in Adobe Workfront geplant ist. Es wird am besten mit der Standardansicht verwendet.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Filter für Berichtbereitstellung

So wenden Sie diesen Filter an:

1. Gehen Sie zu einer Liste von Berichten.
1. Aus dem **Filter** Dropdown-Menü auswählen **Neuer Filter**.

1. Klicken **In den Textmodus wechseln**.
1. Im **Festlegen von Filterregeln für Ihren Bericht** -Bereich, kopieren Sie den folgenden Code und fügen Sie ihn ein:

   ```
   scheduledReportID=0<br>scheduledReportID_Mod=notnull
   ```

1. Klicken **Filter speichern**.
