---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Probleme mit dem Firmennamen des Urhebers"
description: In dieser Problemansicht wird der Unternehmensname angezeigt, der mit dem Benutzer verknüpft ist, der das Problem gesendet hat.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e628f7cf-4a7b-4125-bea6-348c72477bd7
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# Anzeigen: Probleme mit dem Firmennamen des Originators

In dieser Problemansicht wird der Unternehmensname angezeigt, der mit dem Benutzer verknüpft ist, der das Problem gesendet hat.

![custom_view_for_issues_with_originator_company_name.png](assets/custom-view-for-issues-350x33.png)

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

## Anzeigen von Problemen mit dem Firmennamen des Originators

So wenden Sie diese Ansicht an:

1. Gehen Sie zu einer Liste von Problemen.
1. Wählen Sie aus dem Dropdownmenü **Ansicht** die Option **Neue Ansicht** aus.

1. Im Bereich **Spaltenvorschau** werden alle Spalten mit Ausnahme einer entfernt.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte und dann auf **In Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im Feld **Textmodus** finden, und ersetzen Sie ihn durch den folgenden Code:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.valueFormat=val<br>column.0.link.lookup=link.view<br>column.0.link.value=val(objCode){5)}column.0.listsort=string(name)<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.valueField=name<br>column.0.valueFormat=HTML<br>column.0.width=140<br>column.1.descriptionkey=originator<br>column 1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valueField=ownerID<br>column.1.link.linkproperty.0.valueFormat=int<br>column.1.link.lookup=link.view<br>column.1.link.valueField=owner:objCode<br>column 1.link.valueFormat=val<br>column.1.listsort=nested(owner).string(name)<br>column.1.namekey=originator.abbr<br>column.1.querysort=owner:name<br>column.1.valueField=owner:name<br>column.1.valueFormat=HTML<br>column.1.width=151<br>column.2.descriptionkey=entrydate<br>column.2.listsort=atDateAsAtDate(entryDate)<br>column.2.namekey=entrydate.abbr<br>column.2.querysort=entryDate<br>column 2.valueField=entryDate<br>column.2.valueFormat=atDate<br>column.2.width=75<br>column.3.descriptionkey=age<br>column.3.listsort=doubleAsDouble(age)<br>column.3.namekey=age<br>column.3.queryquery=age<br>column.3.valueField=howOld<br>column.3.valueFormat=val<br>column.3.width=80<br>column.4.viewalias=statusicons<br>column.4.displayName=Flags<br>column.4.linkedname=direct<br>column.4.name ey=statusicons<br>column.4.valueField=<br>column.4.valueFormat=HTML<br>column.4.querysort=<br>column.4.tile.name=component.issuestatusicons<br>column.4.tile.pdfcomponent=issueStatusIcons<br>column.4.delimiter <br>column.4.tile.template=/WEB-INF/jsp/lists/components/issueStatusIcons.jsp<br>column.5.description=Firmenname des Originators<br>column.5.link.linkproperty.0.name=ID<br>column.5.link.linkproperty.0.valueField=owner:companyID<br>column.5.link.link.0.valueformat=int<br>column.5.link.lookup=link.view<br>column.5.link.valueField=owner:company:objCode<br>column.5.link.valueFormat=val<br>column.5.listsort=nested(owner:company).string(name)<br>column.5.name=Originator Company<br>column.5.querysort=owner:company:name<br>column.5.valueField=owner:company:name<br>column.5.valueFormat=HTML<br>column.5.width=151<br></pre>

1. Klicken Sie auf **Ansicht speichern**.
