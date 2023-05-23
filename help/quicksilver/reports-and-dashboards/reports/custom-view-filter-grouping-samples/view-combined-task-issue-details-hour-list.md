---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: kombinierte Aufgaben- und Problemdetails in einer Stundenliste"
description: In dieser Stundenansicht werden die Spalten "Aufgabe"und "Problemname"sowie die Spalten "Aufgabe"und "Problemplanstunden"mit dem sharecol -Tag kombiniert. Da ein Stundeneintrag nur einer Aufgabe oder einem Problem zugeordnet werden kann, können beide Objekte nicht gleichzeitig in derselben Spalte angezeigt werden. Jede Zeile der Ansicht enthält die Informationen aus einer Aufgabe oder einem Problem.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cf1137fd-c26a-4907-afe9-2373d3434631
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---

# Ansicht: kombinierte Aufgaben- und Problemdetails in der Stundenliste

In dieser Stundenansicht werden die Spalten &quot;Aufgabe&quot;und &quot;Problemname&quot;sowie die Spalten &quot;Aufgabe&quot;und &quot;Geplante Aufgaben&quot;mit der Funktion

```
sharecol
```

-Tag. Da ein Stundeneintrag nur einer Aufgabe oder einem Problem zugeordnet werden kann, können beide Objekte nicht gleichzeitig in derselben Spalte angezeigt werden. Jede Zeile der Ansicht enthält die Informationen aus einer Aufgabe oder einem Problem.

Weitere Informationen zum

```
sharecol
```

Tag, siehe [Ansicht: Zusammenführen von Informationen aus mehreren Spalten in einer gemeinsamen Spalte](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).\
![custom_view_hours_with_task_and_issue_information.png](assets/custom-view-hours-with-350x48.png)

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

## Anzeigen kombinierter Aufgaben- und Problemdetails in einer Stundenliste

So wenden Sie diese Ansicht an:

1. Rufen Sie eine Liste der Stunden auf.
1. Aus dem **Ansicht** Dropdown-Menü auswählen **Neue Ansicht**.

1. Im **Spaltenvorschau** -Bereich, alle Spalten außer einer entfernen.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte und dann auf **In den Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im **Textmodus** und ersetzen Sie sie durch den folgenden Code:
   <pre>column.1.querysort=project:name<br>column.1.shortview=false<br>column.1.gestreckch=0<br>column.1.valueField=project:name<br>column.1.valueFormat=HTML<br>column.1.width=100<br>column.2.description=Aufgabe oder Problem<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valueField=task:ID<br>column.2.link.linkproperty.0.valueFormat=int<br>column.2.link.lookup=link.view<br>column.2.link.valueField=task:objCode<br>column.2.link.valueFormat=val<br>column.2.linkedname=task<br>column.2.listsort=nested(task).string(name)<br>column.2.name=Aufgabe oder Problem<br>column.2.querysort=task:name<br>column.2.sharecol=true<br>column.2.shortview=false<br>column.2.gestreckch=0<br>column.2.valueField=task:name<br>column.2.valueFormat=HTML<br>column.2.width=100<br>column.3.descriptionkey=optask<br>column.3.link.linkproperty.0.name=ID<br>column.3.link.linkproperty.0.valueField=opTask:ID<br>column.3.link.linkproperty.0.valueFormat=int<br>column.3.link.lookup=link.view<br>column.3.link.valueField=opTask:objCode<br>column.3.link.valueFormat=val<br>column.3.linkedname=optask<br>column.3.listsort=nested(opTask).string(name)<br>column.3.namekey=opTask<br>column.3.querysort=opTask:name<br>column.3.shortview=false<br>column.3.gestreckch=0<br>column.3.valueField=opTask:name<br>column.3.valueFormat=HTML<br>column.3.width=1<br>column.4.valueField=task:work<br>column.4.sharecol=true<br>column.4.linkedname=task<br>column.4.valueFormat=doubleAsInt<br>column.4.namekey=view.relatedcolumn<br>column.4.querysort=task:work<br>column.4.textmode=true<br>column.4.namekeyargkey.0=task<br>column.4.namekeyargkey.1=work<br>column.4.displayName=Geplanter Aufwand<br>column.5.displayName=Geplanter Aufwand<br>column.5.viewalias=opTask:workrequired<br>column.5.linkedname=opTask<br>column.5.valueField=opTask:workRequired<br>column.5.valueFormat=composite<br>column.5.querysort=opTask:workRequired<br>column.5.namekeyargkey.0=opTask<br>column.5.namekeyargkey.1=workrequired<br>column.5.namekey=view.relatedcolumn<br>column.5.textmode=true<br>column.6.descriptionkey=hours<br>column.6.linkedname=direct<br>column.6.listsort=doubleAsDouble(hours)<br>column.6.namekey=hours.abbr<br>column.6.querysort=hours<br>column.6.shortview=false<br>column.6.gestreckch=0<br>column.6.valueField=hours<br>column.6.valueFormat=doubleAsString<br>column.6.width=75<br>column.7.descriptionkey=entrydate<br>column.7.linkedname=direct<br>column.7.listsort=atDateAsAtDate(entryDate)<br>column.7.namekey=entrydate.abbr<br>column.7.querysort=entryDate<br>column.7.shortview=false<br>column.7.gestreckch=0<br>column.7.valueField=entryDate<br>column.7.valueFormat=atDate<br>column.7.width=75<br>column.8.descriptionkey=description<br>column.8.linkedname=direct<br>column.8.listsort=string(description)<br>column.8.namekey=description.abbr<br>column.8.querysort=description<br>column.8.shortview=false<br>column.8.gestreckch=0<br>column.8.valueField=description<br>column.8.valueFormat=HTML<br>column.8.width=150</pre>

1. Klicken **Ansicht speichern**.
