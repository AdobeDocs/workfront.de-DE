---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Probleme mit Genehmigungsinformationen"
description: Die folgende Problemansicht zeigt den Genehmigungsprozess, den Schritt, die Namen der Genehmiger und den Status des Problems, bevor die Genehmigung erteilt wurde. Einige dieser Felder sind nicht über den Standard-Interface-Builder zugänglich.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4e123844-a0d6-474b-87fb-d30ed391ad07
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Anzeigen: Probleme mit Genehmigungsinformationen

Die folgende Problemansicht zeigt den Genehmigungsprozess, den Schritt, die Namen der Genehmiger und den Status des Problems, bevor die Genehmigung erteilt wurde. Einige dieser Felder sind nicht über den Standard-Interface-Builder zugänglich.

![custom_issue_view_with_approval_info.png](assets/custom-issue-view-with-approval-info-350x46.png)

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

## Anzeigen von Problemen mit Genehmigungsinformationen

1. Gehen Sie zu einer Liste von Problemen.
1. Wählen Sie aus dem Dropdownmenü **Ansicht** die Option **Neue Ansicht** aus.

1. Im Bereich **Spaltenvorschau** werden alle Spalten mit Ausnahme einer entfernt.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte und dann auf **In Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im Feld **Textmodus** finden, und ersetzen Sie ihn durch den folgenden Code:
   <pre style="font-style: normal;">column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.valueFormat=int<br>column.0.link.lookup=link.view<br>column.0.link.valueField=objCode<br>column.0.link.valueFormat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.gestreckch=40<br>column 0.valueField=name<br>column.0.valueFormat=HTML<br>column.0.width=220<br>column.1.descriptionkey=assignedto<br>column.1.linkedname=assignedTo<br>column.1.listsort=nested(assignedTo).string(name){1 8}column.1.namekey=assignedto<br>column.1.querysort=assignedTo:name<br>column.1.shortview=true<br>column.1.gestreckch=0<br>column.1.valueField=assignedTo:name<br>column.1.valueFormat=HTML<br>column.1.width=150<br>column.2.descriptionkey=role<br>column.2.linkedname=role<br>column.2.listsort=nested(role).string(name)<br>column.2.namekey=role<br>column.2.querysort=role:name<br>column.2.view=false<br>column.2.gestreckch=25<br>column.2.valueField=role:name<br>column.2.valueFormat=HTML<br>column.2.width=150<br>column.3.description=Approval Process Name<br>column.3.linkedname=direct<br>column.3.listsort=string(name)<br>column.3.name=Approval Process Name<br>column.3.querysort=name<br>column.3.shortview=false<br>column.3.gestreckch=35<br>column.3.valueField=approvalProcess:name<br>column.3.valueFormat=HTML{4 4}column.3.width=220<br>column.4.description=Approval Step Name<br>column.4.linkedname=direct<br>column.4.listsort=string(name)<br>column.4.name=Approval Step Name<br>column.4.querysort=name<br>column.4.shortview=false{5 1}column.4.gestreckch=0<br>column.4.valueField=currentApprovalStep:name<br>column.4.valueFormat=HTML<br>column.4.width=220<br>column.5.description=Previous Status<br>column.5.linkedname=direct<br>column.5.list sort=string(name)<br>column.5.name=Previous Status<br>column.5.querysort=name<br>column.5.shortview=false<br>column.5.gestreckch=0<br>column.5.valueField=previousStatus<br>column.5.valueFormat=HTML<br>column.5 width=220<br>column.6.linkedname=direct<br>column.6.listsort=HTML(approversString)<br>column.6.namekey=Genehmiger.plural.abbr<br>column.6.querysort=GenehmigersString<br>column.6.shortview=false<br>column 6.gestreckch=0<br>column.6.valueField=approversString<br>column.6.valueFormat=HTML<br>column.6.viewalias=Genehmiger.plural<br>column.6.width=200<br><br><br><br></pre>

1. Klicken Sie auf **Ansicht speichern**.
