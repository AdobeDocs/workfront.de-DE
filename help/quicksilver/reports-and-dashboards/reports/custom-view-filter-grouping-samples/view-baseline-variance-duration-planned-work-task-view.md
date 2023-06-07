---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Ansicht: Grundlinienvarianz für Dauer und geplante Arbeit in einer Aufgabenansicht'''
description: 'In dieser Ansicht wird Folgendes in einer Aufgabenansicht angezeigt: "EDIT ME".'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2a1eef9c-016c-4a04-acda-6070fcb0e23d
source-git-commit: 18f26f976a47af003817f2f82f8550bdfbc0ab90
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# Ansicht: Grundlinienvarianz für Dauer und geplante Arbeit in einer Aufgabenansicht

Diese Ansicht zeigt Folgendes in einer Aufgabenansicht an:

* Aufgabeninformationen mit Grundlinien-Aufgabeninformationen.
* Die Differenz zwischen der Dauer und der standardmäßigen Baseline-Dauer.
* Der Unterschied zwischen der geplanten und der standardmäßigen geplanten Arbeit in der Grundlinie.

>[!NOTE]
>
> Die in der folgenden Ansicht angezeigten Daten vergleichen die tatsächlichen Aufgabenwerte mit den Werten, die mit den Standardgrundaufgaben verknüpft sind.

 

![baseline_variance_in_a_task_view.png](assets/baseline-variance-in-a-task-view-350x38.png)

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

## Grundlegende Varianz für Dauer und geplante Arbeit in einer Aufgabenansicht anzeigen

1. Gehen Sie zu einer Liste von Aufgaben.
1. Im **Ansicht** Dropdown-Menü auswählen **Neue Ansicht**.

1. Entfernen Sie alle Spalten in der Ansicht, mit Ausnahme der ersten.
1. Klicken Sie bei ausgewählter Spalte auf **In den Textmodus wechseln**.
1. Kopieren Sie den unten stehenden Text und fügen Sie ihn in die erste Spalte der Ansicht ein:

   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.valueFormat=int<br>column.0.link.lookup=link.view<br>column.0.link.valueField=objCode<br>column.0.link.valueFormat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.gestreckch=100<br>column.0.valueField=name<br>column.0.valueFormat=HTML<br>column.0.width=150<br>column.0.displayName=Task Name<br>column.1.descriptionkey=duration<br>column.1.linkedname=direct<br>column.1.listsort=intAsInt(durationMinutes)<br>column.1.namekey=duration.abbr<br>column.1.querysort=durationMinutes<br>column.1.shortview=false<br>column.1.gestreckch=0<br>column.1.valueField=durationFieldLong<br>column.1.valueFormat=composite<br>column.1.viewalias=duration<br>column.1.width=100<br>column.1.displayName=Task Duration<br>column.2.descriptionkey=view.relatedcolumn<br>column.2.descriptionkeyargkey.0=defaultbaselinetask<br>column.2.descriptionkeyargkey.1=duration<br>column.2.linkedname=defaultBaselineTask<br>column.2.listsort=intAsInt(durationMinutes)<br>column.2.namekey=duration<br>column.2.namekeyargkey.0=defaultbaselinetask.abbr<br>column.2.namekeyargkey.1=duration.abbr<br>column.2.querysort=defaultBaselineTask:durationMinutes<br>column.2.shortview=false<br>column.2.gestreckch=0<br>column.2.valueField=defaultBaselineTask:durationFieldLong<br>column.2.valueFormat=composite<br>column.2.viewalias=defaultBaselineTask:duration<br>column.2.width=100<br>column.2.displayName=Dflt Baseline Task: Dur<br>column.2.durationunitfield=durationUnit.value<br>column.3.description=Duration Variance"column.3.linkedname=direct<br>column.3.listsort=intAsInt(durationMinutes)<br>column.3.name=Duration Variance<br>column.3.querysort=durationMinutes<br>column.3.shortview=false<br>column.3.gestreckch=0<br>column.3.valueExpression=CONCAT(SUB({duration},{defaultBaselineTask}.{duration})/480," Days")<br>column.3.valueFormat=HTML<br>column.3.viewalias=duration<br>column.3.width=100<br>column.3.displayName=Duration Variance<br>column.4.descriptionkey=workrequired<br>column.4.linkedname=direct<br>column.4.listsort=doubleAsDouble(workRequired)<br>column.4.namekey=workrequired.abbr<br>column.4.querysort=workRequired<br>column.4.shortview=false<br>column.4.gestreckch=0<br>column.4.valueField=workFieldLong<br>column.4.valueFormat=composite<br>column.4.viewalias=workrequired<br>column.4.width=100<br>column.4.displayName=Wrk Req<br>column.5.descriptionkey=view.relatedcolumn<br>column.5.descriptionkeyargkey.0=defaultbaselinetask<br>column.5.descriptionkeyargkey.1=workrequired<br>column.5.linkedname=defaultBaselineTask<br>column.5.listsort=doubleAsDouble(workRequired)<br>column.5.namekey=view.relatedcolumn<br>column.5.namekeyargkey.0=defaultbaselinetask.abbr<br>column.5.namekeyargkey.1=workrequired.abbr<br>column.5.querysort=defaultBaselineTask:workRequired<br>column.5.shortview=false<br>column.5.gestreckch=0<br>column.5.valueField=defaultBaselineTask:workFieldLong<br>column.5.valueFormat=composite<br>column.5.viewalias=defaultBaselineTask:workrequired<br>column.5.width=100<br>column.5.displayName=Dflt Baseline Task: Arbeitsfläche<br>column.6.descriptionkey=workrequired<br>column.6.linkedname=direct<br>column.6.listsort=doubleAsDouble(workRequired)<br>column.6.name=Effort Variance<br>column.6.querysort=workRequired<br>column.6.shortview=false<br>column.6.gestreckch=0<br>column.6.valueExpression=CONCAT(SUB({workRequired},{defaultBaselineTask}.{workRequired})/60," Hours")<br>column.6.valueFormat=HTML<br>column.6.viewalias=workrequired<br>column.6.width=100<br>column.6.displayName=Effort Variance</pre>

1. Klicken **Ansicht speichern**.