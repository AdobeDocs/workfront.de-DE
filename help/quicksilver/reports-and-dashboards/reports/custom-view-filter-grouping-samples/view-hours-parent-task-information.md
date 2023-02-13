---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Ansicht: Stunden mit Informationen zu übergeordneten Aufgaben'''
description: Diese Stundenansicht zeigt den Namen der Aufgabe, in der die Stunden protokolliert wurden, sowie den Namen der übergeordneten Aufgabe an.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c24555fc-3bae-451b-8a44-28a8158199d1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# Ansicht: Stunden mit Informationen zu übergeordneten Aufgaben

Diese Stundenansicht zeigt den Namen der Aufgabe, in der die Stunden protokolliert wurden, sowie den Namen der übergeordneten Aufgabe an.

![custom_hour_view_with_task_and_parent_task_info.png](assets/custom-hour-view-with-task-and-parent-task-info-350x55.png)

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

## Anzeigen von Stunden mit Informationen zu übergeordneten Aufgaben

1. Rufen Sie eine Liste der Stunden auf.
1. Aus dem **Ansicht** Dropdown-Menü auswählen **Neue Ansicht**.

1. Im **Spaltenvorschau** -Bereich, alle Spalten außer einer entfernen.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte und dann auf **In den Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im **Textmodus** und ersetzen Sie sie durch den folgenden Code:
   <pre>column.0.aggregator.displayFormat=doubleAsString<br>column.0.aggregator.function=SUM<br>column.0.aggregator.namekey=hours<br>column.0.aggregator.valueField=hours<br>column.0.aggregator.valueFormat=doubleAsDouble<br>column.0.descriptionkey=hours<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.valueFormat=int<br>column.0.link.lookup=link.view<br>column.0.link.valueField=objCode<br>column.0.link.valueFormat=val<br>column.0.linkedname=direct<br>column.0.listsort=doubleAsDouble(hours)<br>column.0.namekey=hours.abbr<br>column.0.querysort=hours<br>column.0.shortview=false<br>column.0.gestreckch=100<br>column.0.valueField=hours<br>column.0.valueFormat=doubleAsString<br>column.0.width=150<br>column.1.descriptionkey=task<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valueField=task:ID<br>column.1.link.linkproperty.0.valueFormat=int<br>column.1.link.lookup=link.view<br>column.1.link.valueField=task:objCode<br>column.1.link.valueFormat=val<br>column.1.linkedname=task<br>column.1.listsort=nested(task).string(name)<br>column.1.namekey=task<br>column.1.querysort=task:name<br>column.1.shortview=false<br>column.1.gestreckch=0<br>column.1.valueField=task:name<br>column.1.valueFormat=HTML<br>column.1.width=150<br>column.2.description=Parent Task Name<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valueField=task:parent:ID<br>column.2.link.linkproperty.0.valueFormat=int<br>column.2.link.lookup=link.view<br>column.2.link.valueField=task:objCode<br>column.2.link.valueFormat=val<br>column.2.linkedname=task<br>column.2.listsort=nested(task:parent).string(name)<br>column.2.name=Übergeordneter Aufgabenname<br>column.2.querysort=task:parent:name<br>column.2.shortview=false<br>column.2.gestreckch=0<br>column.2.valueField=task:parent:name<br>column.2.valueFormat=HTML<br>column.2.width=150</pre>

1. Klicken **Ansicht speichern**.
