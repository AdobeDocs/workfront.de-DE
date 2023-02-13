---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Probleme mit Validierungsinformationen"
description: Die folgende Problemansicht zeigt den Genehmigungsprozess, den Schritt, die Namen der Genehmiger und den Status des Problems, bevor die Genehmigung erteilt wurde. Einige dieser Felder sind nicht über den Standard-Interface-Builder zugänglich.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4e123844-a0d6-474b-87fb-d30ed391ad07
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---

# Ansicht: Probleme mit Validierungsinformationen

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

## Anzeigen von Problemen mit Genehmigungsinformationen

1. Gehen Sie zu einer Liste von Problemen.
1. Aus dem **Ansicht** Dropdown-Menü auswählen **Neue Ansicht**.

1. Im **Spaltenvorschau** -Bereich, alle Spalten außer einer entfernen.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte und dann auf **In den Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im **Textmodus** und ersetzen Sie sie durch den folgenden Code:
   <pre style="font-style: normal;">column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.valueFormat=int<br>column.0.link.lookup=link.view<br>column.0.link.valueField=objCode<br>column.0.link.valueFormat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.gestreckch=40<br>column.0.valueField=name<br>column.0.valueFormat=HTML<br>column.0.width=220<br>column.1.descriptionkey=assignedto<br>column.1.linkedname=assignedTo<br>column.1.listsort=nested(assignedTo).string(name)<br>column.1.namekey=assignedto<br>column.1.querysort=assignedTo:name<br>column.1.shortview=true<br>column.1.gestreckch=0<br>column.1.valueField=assignedTo:name<br>column.1.valueFormat=HTML<br>column.1.width=150<br>column.2.descriptionkey=role<br>column.2.linkedname=role<br>column.2.listsort=nested(role).string(name)<br>column.2.namekey=role<br>column.2.querysort=role:name<br>column.2.shortview=false<br>column.2.gestreckch=25<br>column.2.valueField=role:name<br>column.2.valueFormat=HTML<br>column.2.width=150<br>column.3.description=Approval Process Name<br>column.3.linkedname=direct<br>column.3.listsort=string(name)<br>column.3.name=Approval Process Name<br>column.3.querysort=name<br>column.3.shortview=false<br>column.3.gestreckch=35<br>column.3.valueField=approvalProcess:name<br>column.3.valueFormat=HTML<br>column.3.width=220<br>column.4.description=Approval Step Name<br>column.4.linkedname=direct<br>column.4.listsort=string(name)<br>column.4.name=Approval Step Name<br>column.4.querysort=name<br>column.4.shortview=false<br>column.4.gestreckch=0<br>column.4.valueField=currentApprovalStep:name<br>column.4.valueFormat=HTML<br>column.4.width=220<br>column.5.description=Vorheriger Status<br>column.5.linkedname=direct<br>column.5.listsort=string(name)<br>column.5.name=Vorheriger Status<br>column.5.querysort=name<br>column.5.shortview=false<br>column.5.gestreckch=0<br>column.5.valueField=previousStatus<br>column.5.valueFormat=HTML<br>column.5.width=220<br>column.6.linkedname=direct<br>column.6.listsort=HTML(ApproversString)<br>column.6.namekey=Genehmiger.plural.abbr<br>column.6.querysort=approversString<br>column.6.shortview=false<br>column.6.gestreckch=0<br>column.6.valueField=approversString<br>column.6.valueFormat=HTML<br>column.6.viewalias=Approver.plural<br>column.6.width=200<br></pre>

1. Klicken **Ansicht speichern**.
