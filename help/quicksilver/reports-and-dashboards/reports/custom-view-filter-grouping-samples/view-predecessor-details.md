---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Anzeigen: Vorgängerdetails'
description: Diese Aufgabenansicht zeigt Details zu den Vorgängern der Aufgaben an, die eine Sammlungsansicht verwenden. In einer Sammlungsansicht können Sie Informationen zu Objekten anzeigen, die eine Eins-zu-viele-Beziehung aufweisen. In diesem Fall kann jede Aufgabe (eine) mehrere Vorgänger (viele) haben. In der Ansicht werden der Name der Aufgaben sowie die Namen der Vorgänger, die Projektnamen der Vorgänger, die geplanten Abschlussdaten der Vorgänger und der Status der Vorgänger angezeigt.
author: Nolan
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# Anzeigen: Vorgängerdetails

<!--Audited: 11/2024-->

Diese Aufgabenansicht zeigt Details zu den Vorgängern der Aufgaben an, die eine Sammlungsansicht verwenden. In einer Sammlungsansicht können Sie Informationen zu Objekten anzeigen, die eine Eins-zu-viele-Beziehung aufweisen. In diesem Fall kann jede Aufgabe (eine) mehrere Vorgänger (viele) haben. In der Ansicht werden der Name der Aufgaben sowie die Namen der Vorgänger, die Projektnamen der Vorgänger, die geplanten Abschlussdaten der Vorgänger und der Status der Vorgänger angezeigt.

Informationen zum Referenzieren von Sammlungen in Berichten finden Sie unter [Referenzieren von Sammlungen in einem Bericht](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

![PREDECESSOR_DETAILS_TASK_VIEW.png](assets/predecessor-details-task-view-350x34.png)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
   <p>Mitwirkender oder Anfrage zum Ändern einer Ansicht </p>
   <p>Standard oder Plan zum Ändern eines Berichts</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Anzeigen von Vorgängerdetails

1. Zu einer Aufgabenliste gehen.
1. Wählen Sie **Dropdown** Menü „Ansicht“ die Option **Neue Ansicht**.

1. Entfernen Sie **Bereich „Spaltenvorschau** alle Spalten mit Ausnahme einer Spalte.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte und dann auf **Wechseln in den Textmodus** > **Textmodus bearbeiten**.
1. Entfernen Sie den Text aus dem Feld **Textmodus bearbeiten** und ersetzen Sie ihn durch den folgenden Code:

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

1. Klicken Sie **Fertig** > **Ansicht speichern**.
