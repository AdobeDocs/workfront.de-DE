---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Gruppierung: Projekte nach dem Eingangsdatum"
description: Bei dieser benutzerdefinierten Projektgruppierung können Sie Projekte anzeigen, die nach ihren Datumswerten für die Einsendung gruppiert sind.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 511faad5-b5bd-4e2d-8daa-3fcde49a502c
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 0%

---

# Gruppierung: Projekte nach dem Datum der Einsendung

Bei dieser benutzerdefinierten Projektgruppierung können Sie Projekte anzeigen, die nach ihren Datumswerten für die Einsendung gruppiert sind.

Jede Gruppierung zeigt Projekte mit einem Einstiegsdatum in:

* Die letzten 30 Tage
* 30-60 Tage
* 60 Tage oder älter

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

## Gruppieren von Projekten nach Entrypdatum

So wenden Sie diese Gruppierung an:

1. Wechseln Sie zu einem vorhandenen Projektbericht oder erstellen Sie einen neuen Projektbericht.\
   Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Aus dem **Gruppierung** Registerkarte, klicken Sie auf **Gruppierung hinzufügen**.

1. Klicken **In den Textmodus wechseln**.
1. Entfernen Sie den Text im **Gruppieren Ihres Berichts** Bereich.
1. Ersetzen Sie den Text durch den folgenden Code:

   ```
   group.0.linkedname=direct<br>
   ```

   ```
   group.0.name=Project Entry<br>
   ```

   ```
   group.0.valueexpression=IF(ABS(DATEDIFF({entryDate},$$TODAY))<=30,"Last 30 Days",IF(ABS(DATEDIFF({entryDate},$$TODAY))>30&&ABS(DATEDIFF({entryDate},$$TODAY))<=60,"30-60 Days","Older than 60 days"))<br>
   ```

   ```
   group.0.valueformat=atDateAsMonthString<br>
   ```

   ```
   textmode=true
   ```

1. Klicken **Speichern und schließen**.
