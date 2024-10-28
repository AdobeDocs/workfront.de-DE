---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Gruppierung: Projekte nach Datum der Einreichung"
description: Bei dieser benutzerdefinierten Projektgruppierung können Sie Projekte anzeigen, die nach ihren Datumswerten für die Einsendung gruppiert sind.
author: Nolan
feature: Reports and Dashboards
exl-id: 511faad5-b5bd-4e2d-8daa-3fcde49a502c
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# Gruppierung: Projekte nach Datum der Einsendung

Bei dieser benutzerdefinierten Projektgruppierung können Sie Projekte anzeigen, die nach ihren Datumswerten für die Einsendung gruppiert sind.

Jede Gruppierung zeigt Projekte mit einem Einstiegsdatum in:

* Die letzten 30 Tage
* 30-60 Tage
* 60 Tage oder älter

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkende bei der Änderung eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filteranforderung </p></li>
   <li><p>Berichtänderung planen</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gruppieren von Projekten nach Entrypdatum

So wenden Sie diese Gruppierung an:

1. Wechseln Sie zu einem vorhandenen Projektbericht oder erstellen Sie einen neuen Projektbericht.\
   Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Klicken Sie auf **Berichtaktionen** > **Bearbeiten**.
1. Klicken Sie auf der Registerkarte **Gruppierung** auf **Gruppierung hinzufügen**.
1. Klicken Sie auf **Wechseln zum Textmodus**.
1. Entfernen Sie den Text im Bereich **Gruppieren nach** .
1. Ersetzen Sie den Text durch den folgenden Code:

   group.0.linkedname=direct
group.0.name=Project Entry
group.0.valueExpression=IF(ABS(DATEDIFF({entryDate},$$TODAY))&lt;=30,&quot;Last 30 Days&quot;,IF(ABS(DATEDIFF({entryDate},$$TODAY))>30&amp;&amp;ABS(DATEDIFF({entryDate},$$TODAY))&lt;=60,&quot;3 -60 Tage&quot;,&quot;älter als 60 Tage&quot;))
group.0.valueFormat=atDateAsMonthString
textmode=true

1. Klicken Sie auf **Fertig** > **Gruppierung speichern**.
1. (Optional) Aktualisieren Sie den Namen der Gruppierung und klicken Sie dann auf **Gruppierung speichern**.
