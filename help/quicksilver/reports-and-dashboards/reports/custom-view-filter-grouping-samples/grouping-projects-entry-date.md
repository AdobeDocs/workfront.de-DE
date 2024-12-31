---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppierung: Projekte nach Eingabedatum'
description: In dieser benutzerdefinierten Projektgruppierung können Sie Projekte gruppiert nach ihren Werten für das Eingabedatum anzeigen.
author: Nolan
feature: Reports and Dashboards
exl-id: 511faad5-b5bd-4e2d-8daa-3fcde49a502c
source-git-commit: a6874c3a2dfda02b8a25f78056767d8c59c888e9
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Gruppierung: Projekte nach Eingabedatum

<!--Audited: 10/2024-->

In dieser benutzerdefinierten Projektgruppierung können Sie Projekte gruppiert nach ihren Werten für das Eingabedatum anzeigen.

Jede Gruppierung zeigt Projekte mit einem Eingabedatum in:

* Die letzten 30 Tage
* 30-60 Tage
* 60 Tage oder älter

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

## Projekte nach Eingabedatum gruppieren

Um diese Gruppierung anzuwenden:

1. Zu einem vorhandenen Projektbericht wechseln oder einen neuen Projektbericht erstellen.\
   Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Klicken Sie **Berichtsaktionen** > **Bearbeiten**.
1. Klicken Sie auf der **Gruppierung** auf **Gruppierung hinzufügen**.
1. Klicken Sie **In Textmodus wechseln**.
1. Entfernen Sie den Text im Bereich **Gruppieren nach**.
1. Ersetzen Sie den Text durch den folgenden Code:


   ```
   group.0.linkedname=direct
   group.0.name=Project Entry
   group.0.valueexpression=IF(ABS(DATEDIFF({entryDate},$$TODAY))<=30,"Last 30 Days",IF(ABS(DATEDIFF({entryDate},$$TODAY))>30&&ABS(DATEDIFF({entryDate},$$TODAY))<=60,"30-60 Days","Older than 60 days"))
   group.0.valueformat=atDateAsMonthString
   textmode=true
   ```

1. Klicken Sie **Fertig** > **Gruppierung speichern**.
1. (Optional) Aktualisieren Sie den Namen der Gruppierung und klicken Sie dann auf **Gruppierung speichern**.
