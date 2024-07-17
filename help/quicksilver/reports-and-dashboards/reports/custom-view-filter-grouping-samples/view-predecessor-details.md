---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Details des Vorgängers"
description: Diese Aufgabenansicht zeigt Details zu den Vorgängern der Aufgaben, die eine Sammlungsansicht verwenden. In einer Sammlungsansicht können Sie Informationen zu Objekten anzeigen, die sich in einer Eins-zu-viele-Beziehung befinden. In diesem Fall kann jede Aufgabe (eine) mehrere Vorgänger (viele) haben. In der Ansicht werden der Name der Aufgaben sowie die Namen der Vorgänger, die Projektnamen der Vorgänger, die geplanten Abschlussdaten der Vorgänger und die Status der Vorgänger angezeigt.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Ansicht: Details des Vorgängers

Diese Aufgabenansicht zeigt Details zu den Vorgängern der Aufgaben, die eine Sammlungsansicht verwenden. In einer Sammlungsansicht können Sie Informationen zu Objekten anzeigen, die sich in einer Eins-zu-viele-Beziehung befinden. In diesem Fall kann jede Aufgabe (eine) mehrere Vorgänger (viele) haben. In der Ansicht werden der Name der Aufgaben sowie die Namen der Vorgänger, die Projektnamen der Vorgänger, die geplanten Abschlussdaten der Vorgänger und die Status der Vorgänger angezeigt.

Informationen zum Referenzieren von Sammlungen in Berichten finden Sie unter [Referenzieren von Sammlungen in einem Bericht](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

![predecessor_details_task_view.png](assets/predecessor-details-task-view-350x34.png)

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

## Anzeigen von Vorgängerdetails

1. Gehen Sie zu einer Liste von Aufgaben.
1. Wählen Sie aus dem Dropdownmenü **Ansicht** die Option **Neue Ansicht** aus.

1. Im Bereich **Spaltenvorschau** werden alle Spalten mit Ausnahme einer entfernt.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte und dann auf **In Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im Feld **Textmodus** finden, und ersetzen Sie ihn durch den folgenden Code:
   <pre>column.0.displayName=<br>column.0.linkedname=direct<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.valueField=name<br>column.0.valueFormat=HTML<br>column.1.displayName=Predecessors Numbers &amp; Names<br>column.1.listdelimiter= 7}column.1.listmethod=nested(predecessors).lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueExpression=CONCAT({predecessor}.<br><br>{taskNumber},' - ',{predecessor}.{name})<br>column.1.valueFormat=HTML<br>column.2.displayName=predecessors Projektnamen<br>column.2.listdelimiter=<br><br>column.2.listmethod=nested(predecessors).lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueExpression= 8.{predecessor}{project}.{name}<br>column.2.valueFormat=HTML<br>column.3.displayName=predecessorsAbschlussdatumswerte<br>column.3.listdelimiter=<br><br>column.3.listmethod=nested(predecessors).lists<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.valueAusdruck={predecessor}.{plannedCompletionDate}<br>column.3.valueFormat=HTML<br>column.4.displayName=predecessors status<br>column.4.listdelimiter=<br><br>column.4.listmethod=nested(predecessors).lists<br>column.4.textmode=true<br>column.4.type=iterate<br>column.4.value expression={predecessor} .{status}<br>column.4.valueFormat=HTML</pre>

1. Klicken Sie auf **Ansicht speichern**.
