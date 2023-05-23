---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Tatsächliche Stunden über geplante Stunden in derselben Spalte einer Aufgabenansicht"
description: In dieser Aufgabenansicht wird die tatsächlich aufgezeichnete Anzahl von Stunden für eine Aufgabe über die für jede Aufgabe geplanten Stunden hinweg angezeigt.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1179283-dc2e-40d3-b8e0-4b1b79f83ad3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Ansicht: Tatsächliche Stunden über geplante Stunden in derselben Spalte einer Aufgabenansicht

In dieser Aufgabenansicht wird die tatsächlich aufgezeichnete Anzahl von Stunden für eine Aufgabe über die für jede Aufgabe geplanten Stunden hinweg angezeigt.

![IST_vs_scheduled_in_task_report.png](assets/actual-vs-planned-in-task-report-350x58.png)

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
   <td> <p>Anforderung zum Ändern einer Ansicht </p>
   <p>Berichtänderung planen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Tatsächliche Stunden über geplante Stunden in einer Aufgabenansicht anzeigen

So wenden Sie diese Ansicht an:

1. Gehen Sie zu einer Liste von Aufgaben.
1. Aus dem **Ansicht** Dropdown-Menü auswählen **Neue Ansicht**.

1. Im **Spaltenvorschau** -Bereich, alle Spalten außer einer entfernen.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte und dann auf **In den Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im **Textmodus** und ersetzen Sie sie durch den folgenden Code:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.valueFormat=int<br>column.0.link.lookup=link.view<br>column.0.link.valueField=objCode<br>column.0.link.valueFormat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.gestreckch=100<br>column.0.valueField=name<br>column.0.valueFormat=HTML<br>column.0.width=150<br>column.1.viewalias=assignments<br>column.1.displayName=<br>column.1.linkedname=direct<br>column.1.namekey=assignments<br>column.1.valueField=assignmentsListString<br>column.1.valueFormat=HTML<br>column.1.tile.name=component.assignmentslist<br>column.2.displayName=Tatsächliche/geplante Stunden<br>column.2.linkedname=direct<br>column.2.namekey=actualworkrequired<br>column.2.querysort=ISTWork<br>column.2.textmode=true<br>column.2.valueExpression=CONCAT({ISTWorkRequired}/60,' / ',{workRequired}/60)<br>column.2.valueField=ISTWorkRequired<br>column.2.valueFormat=composite<br>column.2.viewalias=actualworkrequired<br>column.3.aggregator.function=SUM<br>column.3.aggregator.valueExpression=SUB({ISTWork}, {workRequired})<br>column.3.aggregator.valueFormat=composite<br>column.3.displayName=Hours Variation<br>column.3.linkedname=direct<br>column.3.textmode=true<br>column.3.valueExpression=SUB({ISTWork}, {workRequired})/60<br>column.3.valueFormat=customNumberAsString</pre>

1. Klicken **Ansicht speichern**.
