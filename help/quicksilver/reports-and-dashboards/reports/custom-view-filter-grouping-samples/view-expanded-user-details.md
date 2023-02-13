---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: erweiterte Benutzerdetails"
description: In dieser Benutzeransicht werden Informationen zu Ihren Benutzern angezeigt. Neben ihrem Namen, ihren Zugriffsstufen und ihrem Unternehmen werden hier auch Listen ihrer Gruppen, Teams und Jobrollen angezeigt.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a978b43-4718-43fb-80b8-844b35e09d06
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# Ansicht: erweiterte Benutzerdetails

In dieser Benutzeransicht werden Informationen zu Ihren Benutzern angezeigt. Neben ihrem Namen, ihren Zugriffsstufen und ihrem Unternehmen werden hier auch Listen ihrer Gruppen, Teams und Jobrollen angezeigt.

![extended_user_view.png](assets/expanded-user-view-350x75.png)

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

## Anzeigen erweiterter Benutzerdetails

So wenden Sie diese Ansicht an:

1. Navigieren Sie zu einer Liste von Benutzern.
1. Aus dem **Ansicht** Dropdown-Menü auswählen **Neue Ansicht**.

1. Im **Spaltenvorschau** -Bereich, alle Spalten außer einer entfernen.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte und dann auf **In den Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im **Textmodus** und ersetzen Sie sie durch den folgenden Code:

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: extra tag here that adds extra spaces in Preview)
   </MadCap:conditionalText>
   -->

   <pre>column.0.descriptionkey=name <br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.valueFormat=int<br>column.0.link.lookup=link.view<br>column.0.link.valueField=objCode<br>column.0.link.valueFormat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.gestreckch=0<br>column.0.valueField=name<br>column.0.valueFormat=HTML<br>column.0.width=150<br>column.1.descriptionkey=accessLevel<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valueField=accessLevel:ID<br>column.1.link.linkproperty.0.valueFormat=int<br>column.1.link.lookup=link.view<br>column.1.link.valueField=accessLevel:objCode<br>column.1.link.valueFormat=val<br>column.1.linkedname=accessLevel<br>column.1.listsort=string(displayName)<br>column.1.namekey=accessLevel<br>column.1.querysort=name<br>column.1.shortview=false<br>column.1.gestreckch=0<br>column.1.valueField=accessLevel:displayName<br>column.1.valueFormat=HTML<br>column.1.viewalias=accessLevel:displayName<br>column.1.width=100<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valueField=ID<br>column.2.link.linkproperty.0.valueFormat=int<br>column.2.link.lookup=link.view<br>column.2.link.value=val(objCode)<br>column.2.listdelimiter=<br>column.2.listmethod=nested(userGroups).lists<br>column.2.namekey=group.plural<br>column.2.gestreckch=50<br>column.2.type=iterate<br>column.2.valueField=group:name<br>column.2.valueFormat=HTML<br>column.2.width=150<br>column.3.displayName=Teams<br>column.3.listdelimiter=<br>column.3.listmethod=nested(teams).lists<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.valueExpression={name}<br>column.3.valueFormat=HTML<br>column.4.link.linkproperty.0.name=ID<br>column.4.link.linkproperty.0.valueField=ID<br>column.4.link.linkproperty.0.valueFormat=int<br>column.4.link.lookup=link.view<br>column.4.link.value=val(objCode)<br>column.4.listdelimiter=<br>column.4.listmethod=nested(userRoles).lists<br>column.4.namekey=jobrole.plural<br>column.4.gestreckch=50<br>column.4.type=iterate<br>column.4.valueField=role:name<br>column.4.valueFormat=HTML<br>column.4.width=150<br>column.5.descriptionkey=company<br>column.5.link.linkproperty.0.name=ID<br>column.5.link.linkproperty.0.valueField=company:ID<br>column.5.link.linkproperty.0.valueFormat=int<br>column.5.link.lookup=link.view<br>column.5.link.valueField=company:objCode<br>column.5.link.valueFormat=val<br>column.5.linkedname=company<br>column.5.listsort=nested(company).string(name)<br>column.5.namekey=company<br>column.5.querysort=company:name<br>column.5.shortview=false<br>column.5.gestreckch=0<br>column.5.valueField=company:name<br>column.5.valueFormat=HTML<br>column.5.width=150</pre>

1. Klicken **Ansicht speichern**.
