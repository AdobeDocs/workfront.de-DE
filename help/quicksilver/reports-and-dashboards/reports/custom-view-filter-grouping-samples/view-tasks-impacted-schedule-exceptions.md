---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Von Zeitplanausnahmen betroffene Aufgaben"
description: In dieser Aufgabenansicht werden Aufgaben identifiziert, die aufgrund von Wochenenden, persönlicher Zeitüberschreitung oder anderen Zeitplanausnahmen zu spät abgeschlossen werden müssen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7d7c77fa-d9a7-4e91-8dae-ad3aaca6f1da
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 0%

---

# Ansicht: Von Zeitplanausnahmen betroffene Aufgaben

In dieser Aufgabenansicht werden Aufgaben identifiziert, die aufgrund von Wochenenden, persönlicher Zeitüberschreitung oder anderen Zeitplanausnahmen zu spät abgeschlossen werden müssen.

Diese Ansicht zeigt Folgendes an:

* Dauer von Aufgaben
* Geplante Start- und geplante Abschlussdaten der Aufgaben
* Die Dauer der Aufgaben in Abhängigkeit von der Anzahl der Tage zwischen dem geplanten Start- und dem geplanten Abschlussdatum der Aufgaben (Kalenderdauer)
* Die Nummer des Tages im Zeitplan des Projekts, an dem die Aufgabe beginnt (Startdatum des Kalenders)
* Die Wochentagsdauer der Aufgaben entsprechend der Anzahl der Wochentage zwischen dem geplanten Start- und dem geplanten Abschlussdatum der Aufgaben (Wochentagsdauer)
* Wenn die Wochentagsdauer die Dauer der Aufgaben überschreitet, was darauf hindeutet, dass die Dauer der Aufgaben Ausnahmetage umfasst, werden die Aufgaben als &quot;Ausnahme&quot;markiert.\
  ![tasks_with_calendar_failures.png](assets/tasks-with-calendar-exceptions-350x51.png)

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

## Anzeigen von Aufgaben, die von planmäßigen Ausnahmen betroffen sind

1. Gehen Sie zu einer Liste von Aufgaben.
1. Wählen Sie aus dem Dropdownmenü **Ansicht** die Option **Neue Ansicht** aus.

1. Im Bereich **Spaltenvorschau** werden alle Spalten mit Ausnahme einer entfernt.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte und dann auf **In Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im Feld **Textmodus** finden, und ersetzen Sie ihn durch den folgenden Code:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.valueFormat=int<br>column.0.link.lookup=link.view<br>column.0.link.valueField=objCode<br>column.0.link.valueFormat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.extending=10<br>column.0.valueField=name<br>column.0.valueFormat=HTML<br>column.0.width=150<br>column.1.descriptionkey=duration<br>column.1.linkedname=direct<br>column.1.listsort=intAsInt(durationMinutes)<br>column 1.namekey=duration.abbr<br>column.1.querysort=durationMinutes<br>column.1.shortview=false<br>column.1.gestreckch=0<br>column.1.valueField=durationFieldLong<br>column.1.valueFormat=connection<br>column.1.viewalias{duration 25}column.1.width=80<br>column.2.descriptionkey=plannedstartdate<br>column.2.linkedname=direct<br>column.2.listsort=atDateAsAtDate(scheduledStartDate)<br>column.2.namekey=plannedstartdate.abbr{3 0}column.2.querysort=scheduledStartDate<br>column.2.shortview=false<br>column.2.gestreckch=0<br>column.2.valueField=scheduledStartDate<br>column.2.valueFormat=atDate<br>column.2.width=80<br>column.3.descriptionkey=plannedcompleteDate<br>column.3.linkedname=direct<br>column.3.listsort=atDateAsAtDate(scheduledCompletionDate)<br>column.3.namekey=plannedcompleteDate.abbr<br>column.3.querysort=scheduledCompletionDate{4 1}column.3.shortview=false<br>column.3.gestreckch=0<br>column.3.valueField=scheduledCompletionDate<br>column.3.valueFormat=atDate<br>column.3.width=80<br>column.4.aggregator.displayFormat=int<br>column.4.aggregator.function=SUM<br>column.4.aggregator.namekey=id<br>column.4.aggregator.valueExpression=DATEDIFF({plannedCompletionDate},<br>{plannedStartDate})+1<br>column.4.aggregator.valueFormat=intAsInt<br>column.4.descriptionkey=id 55}column.4.linkedname=direct<br>column.4.listsort=intAsInt(ID)<br>column.4.name=Calendar Duration<br>column.4.querysort=ID<br>column.4.shortview=false<br>column.4.gestreckch=0<br>column.4.value expression=DATEDIFF({plannedCompletionDate},{plannedStartDate})+1<br>column.4.valueFormat=int<br>column.4.width=80<br>column.5.aggregator.displayFormat=int<br>column.5.aggregator.function=SUM<br>column.5.aggregator.name=id 9}column.5.aggregator.valueExpression=DATEDIFF({plannedStartDate},{project}.<br><br><br><br><br><br>{plannedStartDate})+0<br>column.5.aggregator.valueFormat=intAsInt<br>column.5.descriptionkey=id<br>column.5.linkedname=direct<br>column.5.listsort=intAsInt(ID)<br>column.5.name=Calendar Start Date<br>column.5.querysort=ID<br>column.5.shortview=false<br>column.5.gestreckch=0<br>column.5.valueExpression=DATEDIFF({plannedStartDate},{project}.{plannedStartDate})+0<br>column.5.valueFormat=int<br>column.5.width=80<br>column.6.aggregator.displayFormat=int<br>column.6.aggregator.function=SUM<br>column.6.aggregator.namekey=id<br>column.6.aggregator.valueExpression=WEEKDAYDIFF({plannedStartDate}, 8}{plannedCompletionDate})+0<br>column.6.aggregator.valueFormat=HTML<br>column.6.descriptionkey=id<br>column.6.linkedname=direct<br>column.6.listsort=intAsInt(ID)<br>column.6.name=Week Day Duration<br>column.6.querysort=ID<br>column.6.shortview=false<br>column.6.gestreckch=0<br>column.6.valueExpression=WEEKDAYDIFF({plannedStartDate},{plannedCompletionDate})+0<br>column.6.valueFormat=int<br>column.6.width=80<br>column.7.aggregator.displayFormat=int<br>column.7.aggregator.expression=IF((WEEKDAYDIFF({plannedStartDate},{plannedCompletionDate})&gt;({duration}/480),"Exception","")<br>column.7.aggregator.function=SUM<br>column.7.aggregator.name ekey=id<br>column.7.aggregator.valueFormat=HTML<br>column.7.linkedname=direct<br>column.7.listsort=intAsInt(ID)<br>column.7.name=Schedule<br>column.7.querysort=ID<br>column.7.shortview=false<br>column.7.gestreckch=0<br>column.7.valueExpression=IF((WEEKDAYDIFF({plannedStartDate},{plannedCompletionDate})&gt;({duration}/480),"Exception",")<br>column.7.valueFormat=HTML<br>column.7.width=80<br></pre>

1. Klicken Sie auf **Ansicht speichern**.
