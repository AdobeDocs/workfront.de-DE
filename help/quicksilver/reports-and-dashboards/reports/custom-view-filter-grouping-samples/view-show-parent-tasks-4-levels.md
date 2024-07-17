---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Zeigt übergeordnete Aufgaben bis zu 4 Ebenen tief an"
description: Diese Aufgabenansicht zeigt den Aufgabennamen in der ersten Spalte und (falls vorhanden) bis zu 4 übergeordnete Aufgaben in separaten Spalten in derselben Liste an.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 66b45d64-794d-4adc-b208-2ded0dc9c5dc
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 0%

---

# Ansicht: Übergeordnete Aufgaben bis zu 4 Ebenen tief anzeigen

Diese Aufgabenansicht zeigt den Aufgabennamen in der ersten Spalte und (falls vorhanden) bis zu 4 übergeordnete Aufgaben in separaten Spalten in derselben Liste an.

![parent_tasks_4_levels_deep.png](assets/parent-tasks-4-levels-deep-350x29.png)

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
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Übergeordnete Aufgaben bis zu 4 Ebenen tief anzeigen

1. Gehen Sie zu einer Liste von Aufgaben.
1. Wählen Sie aus dem Dropdownmenü **Ansicht** die Option **Neue Ansicht** aus.

1. Im Bereich **Spaltenvorschau** werden alle Spalten mit Ausnahme einer entfernt.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte und dann auf **In Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im Feld **Textmodus** finden, und ersetzen Sie ihn durch den folgenden Code:

   ```
   column.0.descriptionkey=name
   ```

   <pre>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.valueFormat=int<br>column.0.link.lookup=link.view<br>column.0.link.valueField=objCode<br>column.0.link.valueFormat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.valueField=name<br>column.0.valueFormat=HTML<br>column.0.width=150<br>column.1.descriptionkey=parent<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valueField=parent:ID<br>column.1.link.linkproperty.0.valueFormat=int<br>column.1.link.lookup=link.view<br>column.1.link.valueField=parent:objCode<br>column.1.link.valueFormat=val<br>column.1.linkedname=parent<br>column.1.listsort=nested(parent).string(name)<br>column.1.namekey=parent<br>column.1 ysort=parent:name<br>column.1.shortview=false<br>column.1.gestreckch=0<br>column.1.valueField=parent:name<br>column.1.valueFormat=HTML<br>column.1.width=150<br>column.2.description=Parent<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valueField=parent:parent:ID<br>column.2.link.linkproperty.0.valueFormat=int<br>column.2.link.lookup=link.view<br>column.2.link.valueField=parent:parent:objCode<br>column.2.link.valueFormat=val<br>column.2.linkedname=parent<br>column.2.listsort=nested(parent:parent).string(name)<br>column.2.name=Parent Parent<br>column.2.querysort=parent:parent:name<br>column.2.shortview=false<br>column.2.gestreckch=0<br>column.2.valueField=parent:parent:name<br>column.2.valueFormat=HTML<br>column.2.width=150<br>column.3.description=Parent Parent<br>column.3.link.property 0.name=ID<br>column.3.link.linkproperty.0.valueField=parent:parent:parent:ID<br>column.3.link.linkproperty.0.valueFormat=int<br>column.3.link.lookup=link.view<br>column.3.link.valueField=parent:parent:parent:objCode 57}column.3.link.valueFormat=val<br>column.3.linkedname=parent<br>column.3.listsort=nested(parent:parent:parent).string(name)<br>column.3.name=Parent Parent Parent<br>column.3.querysort=parent:parent:parent:name<br>column.3.shortview=false<br>column.3.gestreckch=0<br>column.3.valueField=parent:parent:parent:name<br>column.3.valueFormat=HTML<br>column.3.width=150<br>column.4.description=Parent Parent Parent<br>column.4.link.linkproperty.0.name=ID<br>column.4.link.linkproperty.0.valueField=parent:parent:parent:parent:ID<br>column.4.link.linkproperty.0.valueFormat=int<br>column.4.link.lookup=link.view<br>column.4.valueField=parent:parent:parent:parent:objCode<br>column.4.link.valueFormat=val<br>column.4.linkedname=parent<br>column.4.listsort=nested(parent:parent:parent:parent).string(name)<br>column.4.name=Parent Parent Parent<br>.4.querysort=parent:parent:parent:parent:name<br>column.4.shortview=false<br>column.4.gestreckch=100<br>column.4.valueField=parent:parent:parent:parent:name<br>column.4.valueFormat=HTML<br>column.4 width=150<br></pre>

1. Klicken Sie auf **Ansicht speichern**.

   Der Name der Aufgabe wird in der ersten Spalte angezeigt. Wenn die Aufgabe übergeordnete Elemente hat, werden in den restlichen Spalten bis zu 4 übergeordnete Elemente angezeigt.
