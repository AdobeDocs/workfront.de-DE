---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Anzeigen von Programm- und Portfolio-Informationen in einer Aufgabenansicht"
description: Diese Aufgabenansicht zeigt das Programm und das Portfolio an, die mit dem Aufgabenprojekt verknüpft sind. Diese Informationen sind in ReportBuilder beim Erstellen einer Aufgabenansicht nicht verfügbar. Diese Informationen sind nur im Textmodus verfügbar.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cdd5a1e9-3cbf-4951-b803-fca544b2519a
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Anzeigen: Anzeigen von Programm- und Portfolio-Informationen in einer Aufgabenansicht

Diese Aufgabenansicht zeigt das Programm und das Portfolio an, die mit dem Aufgabenprojekt verknüpft sind. Diese Informationen sind in ReportBuilder beim Erstellen einer Aufgabenansicht nicht verfügbar. Diese Informationen sind nur im Textmodus verfügbar.

Die Ansicht enthält auch Links zum Projekt, Programm und Portfolio aus einer Aufgabenliste.

![](assets/view--program-and-portfolio-350x116.png)

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

## Anzeigen von Programm- und Portfolio-Informationen in einer Aufgabenansicht

So wenden Sie diese Ansicht auf eine Aufgabenliste an:

1. Gehen Sie zu einer Liste von Aufgaben.
1. Wählen Sie aus dem Dropdownmenü **Ansicht** die Option **Neue Ansicht** aus.

1. Im Bereich **Spaltenvorschau** werden alle Spalten mit Ausnahme einer entfernt.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte und dann auf **In Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im Feld **Textmodus** finden, und ersetzen Sie ihn durch den folgenden Code:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.valueFormat=int<br>column.0.link.lookup=link.view<br>column.0.link.valueField=objCode<br>column.0.link.valueFormat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.extending=10<br>column.0.valueField=name<br>column.0.valueFormat=HTML<br>column.0.width=150<br>column.1.descriptionkey=project<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valueField=project:ID{1 8}column.1.link.linkproperty.0.valueFormat=int<br>column.1.link.lookup=link.view<br>column.1.link.valueField=project:objCode<br>column.1.link.valueFormat=val<br>column.1.linkedname=project<br>column.1.liststed=nested (project).string(name)<br>column.1.namekey=project<br>column.1.querysort=project:name<br>column.1.shortview=false<br>column.1.gestreckch=0<br>column.1.valueField=project:name<br>column.1.valueFormat=HTML<br>column.1.width=150<br>column.2.descriptionkey=program<br>column.2.displayName=Program<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valueField=project:program:ID<br>column.2.link.property.0.0.value.valueFormat=int<br>column.2.link.lookup=link.view<br>column.2.link.valueField=project:program:objCode<br>column.2.link.valueFormat=val<br>column.2.linkedname=project<br>column.2.listsort=nested(project:program).string name)<br>column.2.namekey=project<br>column.2.querysort=project:program:name<br>column.2.shortview=false<br>column.2.gestreckch=0<br>column.2.valueField=project:program:name<br>column.2.valueFormat=HTML{5 1}column.2.width=150<br>column.3.descriptionkey=portfolio<br>column.3.displayName=Portfolio<br>column.3.link.linkproperty.0.name=ID<br>column.3.link.linkproperty.0.valueField=project:portfolio:ID<br>link.3.link.link.link property.0.valueFormat=int<br>column.3.link.lookup=link.view<br>column.3.link.valueField=project:portfolio:objCode<br>column.3.link.valueFormat=val<br>column.3.linkedname=project<br>column.3.listsort=nested(project:) .string(name)<br>column.3.namekey=project<br>column.3.querysort=project:portfolio:name<br>column.3.shortview=false<br>column.3.gestreckch=0<br>column.3.valueField=project:portfolio:name<br>column.3.valueFormat=HTML<br>column.3.width=150 <br><br></pre>

1. Klicken Sie auf **Ansicht speichern**.
