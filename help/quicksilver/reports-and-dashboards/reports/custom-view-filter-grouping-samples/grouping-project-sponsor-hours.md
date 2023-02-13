---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Gruppierung: Projektsponsor für Stunden'
description: Diese Stundengruppierung organisiert Stunden nach dem Sponsor des Projekts, in dem die Stunden protokolliert werden. Die standardmäßige ReportBuilder-Oberfläche für Stundengruppierungen enthält keine Zuordnung zum Feld Projektsponsor . Sie müssen die Benutzeroberfläche des Textmodus verwenden, um auf dieses Feld zuzugreifen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Gruppierung: Projektsponsor für Stunden

Diese Stundengruppierung organisiert Stunden nach dem Sponsor des Projekts, in dem die Stunden protokolliert werden. Die standardmäßige ReportBuilder-Oberfläche für Stundengruppierungen enthält keine Zuordnung zum Feld Projektsponsor . Sie müssen die Benutzeroberfläche des Textmodus verwenden, um auf dieses Feld zuzugreifen.

![hour_report_grouped_by_sponsor.png](assets/hour-report-grouped-by-sponsor-350x39.png)

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

## Gruppe nach Projekt-Sponsor für Stunden

So wenden Sie diese Gruppierung an:

1. Rufen Sie eine Liste der Stunden auf.
1. Aus dem **Gruppierung** Dropdown-Menü auswählen **Neue Gruppierung**.

1. Klicken **In den Textmodus wechseln**.
1. Entfernen Sie den Text im **Gruppieren Ihres Berichts** Bereich.

1. Ersetzen Sie den Text durch den folgenden Code:

   <pre>group.0.linkedname=project:sponsor:name<br>group.0.name=<br>group.0.valueField=project:sponsor:name<br>group.0.valueFormat=HTML<br>textmode=true<br></pre>

1. Klicken **Gruppierung speichern**.
