---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ansicht: Ist-Stunden über geplante Stunden in der gleichen Spalte einer Aufgabenansicht'
description: In dieser Aufgabenansicht wird die tatsächliche Anzahl der Stunden, die für eine Aufgabe erfasst wurden, über die für jede Aufgabe geplanten Stunden angezeigt.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1179283-dc2e-40d3-b8e0-4b1b79f83ad3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 1%

---

# Ansicht: Ist-Stunden über Soll-Stunden in derselben Spalte einer Aufgabenansicht

In dieser Aufgabenansicht wird die tatsächlich aufgezeichnete Anzahl von Stunden für eine Aufgabe über die für jede Aufgabe geplanten Stunden hinweg angezeigt.

![IST_vs_scheduled_in_task_report.png](assets/actual-vs-planned-in-task-report-350x58.png)

## Zugangsvoraussetzungen

Sie müssen über den folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo*</td> 
   <td> <p>Jegliche</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Anforderung zum Ändern einer Ansicht </p>
   <p>Planen des Änderns eines Berichts</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Bearbeiten des Zugriffs auf Berichte, Dashboards und Kalender, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen für Ihre Zugriffsebene festgelegt hat. Weitere Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern von benutzerdefinierten Zugriffsebenen</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Berechtigungen für Objekte</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Um herauszufinden, welchen Plan, Lizenztyp oder Zugriff Sie haben, wenden Sie sich an Ihren Workfront-Administrator.

## Anzeigen von Ist-Stunden über Soll-Stunden in einer Aufgabenansicht

So wenden Sie diese Ansicht an:

1. Wechseln Sie zu einer Liste von Aufgaben.
1. Wählen Sie aus dem Dropdownmenü **Ansicht** die Option **Neue Ansicht** aus.

1. Im Bereich **Spaltenvorschau** werden alle Spalten mit Ausnahme einer entfernt.
1. Klicken Sie auf die Überschrift der verbleibenden Spalte und dann auf **In den Textmodus** wechseln.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um den Text** zu bearbeiten.
1. Entfernen Sie den Text, den **Sie im Feld Textmodus** finden, und ersetzen Sie ihn durch den folgenden Code:
   <pre>column.0.descriptionkey=Name<br>Spalte.0.link.linkproperty.0.name=ID Spalte.0.link.linkproperty.0.valuefield=ID<br>Spalte.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direkte Spalte.0.listsort=string<br>(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=Name<br>column.0.shortview=false<br>column.0.stretch<br>=100<br>column.0.valuefield=Name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.viewalias=Zuweisungen<br>Spalte.1.displayname=<br>column.1.linkedname=direkte<br>Spalte.1.namekey=Zuweisungen<br>Spalte.1.valuefield=assignmentsListString<br>column.1.valueformat=HTML<br>column.1.tile.name=component.assignmentslist<br>column.2.displayname=Spalte Tatsächliche/ geplante Stunden.2.linkedname<br>=direkte<br>Spalte.2.namekey=actualworkrequired<br>column.2.querysort=actualWork<br>column.2.textmode=true<br>column.2.valueexpression=CONCAT({actualWorkRequired}/60,' / ',{workRequired}/60)<br>column.2.valuefield=actualWorkRequired<br>column.2.valueformat=zusammengesetzte<br>Spalte.2.viewalias=actualworkrequired<br>column.3.aggregator.function=SUMME<br>column.3.aggregator.valueexpression=SUB({actualWork}, {workRequired})<br>column.3.aggregator.valueformat=zusammengesetzte<br>Spalte.3.displayname=Stundenabweichung<br>column.3.linkedname=direkte<br>Spalte.3.textmode=true<br>column.3.valueexpression=SUB({actualWork}, {workRequired})/60<br>column.3.valueformat=customNumberAsString</pre>

1. Klicken Sie auf **Ansicht speichern**.
