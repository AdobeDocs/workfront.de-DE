---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ansicht: Details zum Vorgänger'
description: Diese Aufgabenansicht zeigt Details zu den Vorgängern der Aufgaben mithilfe einer Auflistungsansicht. In einer Auflistungsansicht können Sie Informationen zu Objekten anzeigen, die sich in einer 1:n-Beziehung befinden. In diesem Fall kann jede Aufgabe (eine) mehrere Vorgänger (viele) haben. In der Ansicht werden der Name der Vorgänge sowie die Namen der Vorgänger, die Projektnamen der Vorgänger, die geplanten Abschlussdaten der Vorgänger und der Status der Vorgänger angezeigt.
author: Courtney
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 14%

---

# Ansicht: Details zu Vorgängern

<!--Audited: 11/2024-->

Diese Aufgabenansicht zeigt Details zu den Vorgängern der Aufgaben mithilfe einer Auflistungsansicht. In einer Auflistungsansicht können Sie Informationen zu Objekten anzeigen, die sich in einer 1:n-Beziehung befinden. In diesem Fall kann jede Aufgabe (eine) mehrere Vorgänger (viele) haben. In der Ansicht werden der Name der Vorgänge sowie die Namen der Vorgänger, die Projektnamen der Vorgänger, die geplanten Abschlussdaten der Vorgänger und der Status der Vorgänger angezeigt.

Informationen zum Verweisen auf Auflistungen in Berichten finden Sie unter [Verweisen auf Auflistungen in einem Bericht](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

![predecessor_details_task_view.png](assets/predecessor-details-task-view-350x34.png)

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
   <p>Mitwirkender oder Anforderung zum Ändern einer Ansicht </p>
   <p>Standard oder Abo zum Ändern eines Berichts</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Bearbeitungszugriff auf Filter, Ansichten, Gruppierungen zum Ändern einer Ansicht</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Vorgängerdetails anzeigen

1. Wechseln Sie zu einer Liste von Aufgaben.
1. Wählen Sie im Dropdown-Menü **Ansicht** die Option **Neue Ansicht**.

1. Entfernen Sie im Bereich **Spaltenvorschau** alle Spalten mit Ausnahme einer Spalte.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte, und klicken Sie auf **In Textmodus wechseln** > **Textmodus bearbeiten**.
1. Entfernen Sie den Text, den Sie im Feld **Textmodus bearbeiten** finden, und ersetzen Sie ihn durch folgenden Code:

   ```
   column.0.displayname=
   column.0.linkedname=direct
   column.0.namekey=name
   column.0.querysort=name
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.1.displayname=Predecessors Numbers & Names
   column.1.listdelimiter=
   column.1.listmethod=nested(predecessors).lists
   column.1.textmode=true
   column.1.type=iterate
   column.1.valueexpression=CONCAT({predecessor}.{taskNumber},' - ',{predecessor}.{name})
   column.1.valueformat=HTML
   column.2.displayname=Predecessors Project Names
   column.2.listdelimiter=
   column.2.listmethod=nested(predecessors).lists
   column.2.textmode=true
   column.2.type=iterate
   column.2.valueexpression={predecessor}.{project}.{name}
   column.2.valueformat=HTML
   column.3.displayname=Predecessors Completion Dates
   column.3.listdelimiter=
   column.3.listmethod=nested(predecessors).lists
   column.3.textmode=true
   column.3.type=iterate
   column.3.valueexpression={predecessor}.{plannedCompletionDate}
   column.3.valueformat=HTML
   column.4.displayname=Predecessors Status
   column.4.listdelimiter=
   column.4.listmethod=nested(predecessors).lists
   column.4.textmode=true
   column.4.type=iterate
   column.4.valueexpression={predecessor}.{status}
   column.4.valueformat=HTML
   ```

1. Klicken Sie auf **Fertig** > **Ansicht speichern**.
