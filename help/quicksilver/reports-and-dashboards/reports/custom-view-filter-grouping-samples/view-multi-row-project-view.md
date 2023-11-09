---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: mehrzeilige Projektansicht"
description: Erfahren Sie mehr über die mehrzeilige Projektansicht in Berichten.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 3c6028c0-2c9f-4f86-aa6c-bf089844bac8
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---

# Ansicht: mehrzeilige Projektansicht

In dieser Projektansicht haben Sie folgende Möglichkeiten:

* Zeigen Sie Projektinformationen im mehrzeiligen Format an.\
  Die Ansicht verwendet die

  ```
  sharecol=true
  ```

  -Tag, um mehrere Felder unter derselben Spaltenüberschrift zu kombinieren. Weitere Informationen zu diesem Tag finden Sie unter [Ansicht: Zusammenführen von Informationen aus mehreren Spalten in einer gemeinsamen Spalte](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

* Verwenden Sie eine Platzhalterspalte, die ein HTML-Zeilenumbruch-Tag (

  ```
  <br>
  ```

  ), um beispielsweise zu erzwingen, dass die Beschreibung unter dem Projektnamen angezeigt wird.
* Zeigen Sie den Projektinhaber in Klammern nach dem Projektnamen an.
* Zeigen Sie den Projektnamen als Link zum Projekt an.

![](assets/project-multi-row-stacked-view-350x219.png)

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

## Erstellen einer mehrzeiligen Projektansicht

1. Erstellen Sie eine neue Projektansicht. Weitere Informationen zum Erstellen einer neuen Ansicht finden Sie unter [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
1. Löschen Sie beim Erstellen der Ansicht alle Spalten außer einer.
1. Wählen Sie die verbleibende Spalte aus und klicken Sie auf **In den Textmodus wechseln**.
1. Kopieren Sie den Textmodus und fügen Sie ihn in die Spalte ein:
   <pre>column.0.linkedname=direct<br>column.0.link.valueFormat=val<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.valueFormat=int<br>column.0.link.valueField=objCode<br>column.0.link.lookup=link.view<br>column.0.sharecol=true<br>column.0.descriptionkey=name<br>column.0.width=150<br>column.0.querysort=name<br>column.0.valueField=name<br>column.0.name=Projektname / Manager / Beschreibung<br>column.0.shortview=false<br>column.0.gestreckch=100<br>column.0.textmode=true<br>column.0.listsort=string(name)<br>column.0.valueFormat=HTML<br>column.1.valueExpression=CONCAT(",{owner}.{name},")")<br>column.1.listsort=nested(owner).string(name)<br>column.1.width=1<br>column.1.linkedname=direct<br>column.1.querysort=owner:name<br>column.1.textmode=true<br>column.1.shortview=false<br>column.1.gestreckch=0<br>column.1.valueFormat=HTML<br>column.1.sharecol=true<br>column.2.width=1<br>column.2.value=<br><br>column.2.shortview=false<br>column.2.sharecol=true<br>column.2.gestreckch=0<br>column.2.textmode=true<br>column.2.valueFormat=HTML<br>column.3.styledef.style=font-color:#ccc;<br>column.3.descriptionkey=description<br>column.3.linkedname=direct<br>column.3.valueField=description<br>column.3.listsort=string(description)<br>column.3.querysort=description<br>column.3.namekey=description.abbr<br>column.3.textmode=true<br>column.3.sharecol=true<br>column.3.gestreckch=0<br>column.3.shortview=false<br>column.3.valueFormat=HTML<br>column.3.width=1<br>column.4.shortview=false<br>column.4.value=<br><br>column.4.sharecol=true<br>column.4.width=1<br>column.4.textmode=true<br>column.4.valueFormat=HTML\<br>column.4.gestreckch=0<br>column.5.name=Geplante Datumswerte/Dauer<br>column.5.width=150<br>column.5.querysort=scheduledStartDate<br>column.5.sharecol=true<br>column.5.gestreckch=0<br>column.5.textmode=true<br>column.5.shortview=false<br>column.5.linkedname=direct<br>column.5.listsort=atDateAsAtDate(scheduledStartDate)<br>column.5.valueField=scheduledStartDate<br>column.5.valueFormat=atDate<br>column.6.sharecol=true<br>column.6.gestreckch=0<br>column.6.width=1<br>column.6.textmode=true<br>column.6.value=-<br>column.6.valueFormat=HTML<br>column.6.shortview=false<br>column.7.namekey=plannedcomplete.date.abbr<br>column.7.width=1<br>column.7.sharecol=true<br>column.7.shortview=false<br>column.7.gestreckch=0<br>column.7.listsort=atDateAsAtDate(scheduledCompletionDate)<br>column.7.linkedname=direct<br>column.7.descriptionkey=plannedcompleteDate<br>column.7.textmode=true<br>column.7.querysort=scheduledCompletionDate<br>column.7.valueFormat=atDate<br>column.7.valueField=scheduledCompletionDate<br>column.8.value=<br><br>column.8.width=1<br>column.8.textmode=true<br>column.8.sharecol=true<br>column.8.valueFormat=HTML<br>column.8.gestreckch=0<br>column.9.textmode=true<br>column.9.listsort=intAsInt(durationMinutes)<br>column.9.gestreckch=0<br>column.9.valueField=durationFieldLong<br>column.9.descriptionkey=duration<br>column.9.viewalias=duration<br>column.9.querysort=durationMinutes<br>column.9.sharecol=true<br>column.9.width=100<br>column.9.shortview=false<br>column.9.namekey=duration.abbr<br>column.9.linkedname=direct<br>column.9.valueFormat=composite<br>column.10.textmode=true<br>column.10.gestreckch=0</pre>

1. Klicks **Ansicht speichern**.
