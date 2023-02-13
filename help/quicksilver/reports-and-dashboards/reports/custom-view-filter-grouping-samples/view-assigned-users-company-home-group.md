---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Unternehmen und Startseite des zugewiesenen Benutzers"
description: In dieser Aufgabenansicht werden das Unternehmen und die Home-Gruppe des Primären Eigentümers der Aufgabe angezeigt. Hierbei handelt es sich um Werte, die in der Standardoberfläche nicht verfügbar sind, aber über den Textmodus auf sie zugegriffen werden kann.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 818c1f3a-4e82-4dc3-af86-4f9dcf5c11a4
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Ansicht: Unternehmen und Startseite des zugewiesenen Benutzers

In dieser Aufgabenansicht werden das Unternehmen und die Home-Gruppe des Primären Eigentümers der Aufgabe angezeigt. Hierbei handelt es sich um Werte, die in der Standardoberfläche nicht verfügbar sind, aber über den Textmodus auf sie zugegriffen werden kann.

![](assets/view--assigned-user-s-company-and-home-group-350x80.png)

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

## Anzeigen des Unternehmens und der Startseite des zugewiesenen Benutzers

1. Gehen Sie zu einer Liste von Aufgaben.
1. Aus dem **Ansicht** Dropdown-Menü auswählen **Neue Ansicht**.

1. Im **Spaltenvorschau** -Bereich, alle Spalten außer einer entfernen.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte und dann auf **In den Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im **Textmodus** und ersetzen Sie sie durch den folgenden Code:
   <pre>column.0.descriptionkey=name<br> column.0.link.linkproperty.0.name=ID<br> column.0.link.linkproperty.0.valueField=ID<br> column.0.link.linkproperty.0.valueFormat=int<br> column.0.link.lookup=link.view<br> column.0.link.valueField=objCode<br> column.0.link.valueFormat=val<br> column.0.linkedname=direct<br> column.0.listsort=string(name)<br> column.0.namekey=name.abbr<br> column.0.querysort=name<br> column.0.shortview=false<br> column.0.gestreckch=100<br> column.0.valueField=name<br> column.0.valueFormat=HTML<br> column.0.width=150<br> column.1.descriptionkey=assignedto<br> column.1.link.linkproperty.0.name=ID<br> column.1.link.linkproperty.0.valueField=assignedTo:ID<br> column.1.link.linkproperty.0.valueFormat=int<br> column.1.link.lookup=link.view<br> column.1.link.valueField=assignedTo:objCode<br> column.1.link.valueFormat=val<br> column.1.linkedname=assignedTo<br> column.1.listsort=nested(assignedTo).string(name)<br> column.1.namekey=assignedto<br> column.1.querysort=assignedTo:name<br> column.1.shortview=false<br> column.1.gestreckch=0<br> column.1.valueField=assignedTo:name<br> column.1.valueFormat=HTML<br> column.1.width=150<br> column.2.description=Assigned To Company<br> column.2.displayName=Assigned To Company<br> column.2.linkedname=assignedTo:company<br> column.2.listsort=nested(assignedTo:company).string(name)<br> column.2.namekey=assignedto<br> column.2.querysort=assignedTo:company:name<br> column.2.shortview=false<br> column.2.gestreckch=0<br> column.2.valueField=assignedTo:company:name<br> column.2.valueFormat=HTML<br> column.2.width=150<br> column.3.description=Assigned To Home Group<br> column.3.displayName=Assigned To Home Group<br> column.3.linkedname=assignedTo:homeGroup<br> column.3.listsort=nested(assignedTo:homeGroup).string(name)<br> column.3.namekey=assignedto<br> column.3.querysort=assignedTo:homeGroup:name<br> column.3.shortview=false<br> column.3.gestreckch=0<br> column.3.valueField=assignedTo:homeGroup:name<br> column.3.valueFormat=HTML<br> column.3.width=150</pre>

1. Klicken **Änderungen speichern**.
