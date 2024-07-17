---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Gruppierung: Projekt-Sponsor für Stunden"
description: Diese Stundengruppierung organisiert Stunden nach dem Sponsor des Projekts, in dem die Stunden protokolliert werden. Die standardmäßige ReportBuilder-Oberfläche für Stundengruppierungen enthält keine Zuordnung zum Feld Projektsponsor . Sie müssen die Benutzeroberfläche des Textmodus verwenden, um auf dieses Feld zuzugreifen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# Gruppierung: Projekt-Sponsor für Stunden

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
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Anforderung zur Änderung einer Gruppierung </p>
   <p>Berichtänderung planen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um eine Gruppierung zu ändern</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Gruppe nach Projekt-Sponsor für Stunden

So wenden Sie diese Gruppierung an:

1. Rufen Sie eine Liste der Stunden auf.
1. Wählen Sie aus dem Dropdownmenü **Gruppierung** die Option **Neue Gruppierung** aus.

1. Klicken Sie auf **Wechseln zum Textmodus**.
1. Entfernen Sie den Text im Bereich **Gruppieren Sie Ihren Bericht** .

1. Ersetzen Sie den Text durch den folgenden Code:
   <pre>group.0.linkedname=project:sponsor:name<br>group.0.name=<br>group.0.valueField=project:sponsor:name<br>group.0.valueFormat=HTML<br>textmode=true<br></pre>

1. Klicken Sie auf **Gruppierung speichern**.
